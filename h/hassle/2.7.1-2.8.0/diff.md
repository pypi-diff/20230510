# Comparing `tmp/hassle-2.7.1.tar.gz` & `tmp/hassle-2.8.0.tar.gz`

## Comparing `hassle-2.7.1.tar` & `hassle-2.8.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     2380 2020-02-02 00:00:00.000000 hassle-2.7.1/CHANGELOG.md
--rw-r--r--   0        0        0    33936 2020-02-02 00:00:00.000000 hassle-2.7.1/docs/hassle.html
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 hassle-2.7.1/docs/index.html
--rw-r--r--   0        0        0    42729 2020-02-02 00:00:00.000000 hassle-2.7.1/docs/search.js
--rw-r--r--   0        0        0    93051 2020-02-02 00:00:00.000000 hassle-2.7.1/docs/hassle/generate_tests.html
--rw-r--r--   0        0        0   122922 2020-02-02 00:00:00.000000 hassle-2.7.1/docs/hassle/hassle.html
--rw-r--r--   0        0        0   107599 2020-02-02 00:00:00.000000 hassle-2.7.1/docs/hassle/hassle_config.html
--rw-r--r--   0        0        0   112334 2020-02-02 00:00:00.000000 hassle-2.7.1/docs/hassle/hassle_utilities.html
--rw-r--r--   0        0        0   165006 2020-02-02 00:00:00.000000 hassle-2.7.1/docs/hassle/new_project.html
--rw-r--r--   0        0        0    52052 2020-02-02 00:00:00.000000 hassle-2.7.1/docs/hassle/run_tests.html
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 hassle-2.7.1/src/hassle/.gitignore_template
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 hassle-2.7.1/src/hassle/.vscode_template
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 hassle-2.7.1/src/hassle/README_template.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hassle-2.7.1/src/hassle/__init__.py
--rw-r--r--   0        0        0     4082 2020-02-02 00:00:00.000000 hassle-2.7.1/src/hassle/generate_tests.py
--rw-r--r--   0        0        0     7002 2020-02-02 00:00:00.000000 hassle-2.7.1/src/hassle/hassle.py
--rw-r--r--   0        0        0     5456 2020-02-02 00:00:00.000000 hassle-2.7.1/src/hassle/hassle_config.py
--rw-r--r--   0        0        0     5055 2020-02-02 00:00:00.000000 hassle-2.7.1/src/hassle/hassle_utilities.py
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 hassle-2.7.1/src/hassle/license_template.txt
--rw-r--r--   0        0        0     9175 2020-02-02 00:00:00.000000 hassle-2.7.1/src/hassle/new_project.py
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 hassle-2.7.1/src/hassle/pyproject_template.toml
--rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 hassle-2.7.1/src/hassle/run_tests.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 hassle-2.7.1/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 hassle-2.7.1/LICENSE.txt
--rw-r--r--   0        0        0    22059 2020-02-02 00:00:00.000000 hassle-2.7.1/README.md
--rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 hassle-2.7.1/pyproject.toml
--rw-r--r--   0        0        0    22508 2020-02-02 00:00:00.000000 hassle-2.7.1/PKG-INFO
+-rw-r--r--   0        0        0     2706 2020-02-02 00:00:00.000000 hassle-2.8.0/CHANGELOG.md
+-rw-r--r--   0        0        0    33936 2020-02-02 00:00:00.000000 hassle-2.8.0/docs/hassle.html
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 hassle-2.8.0/docs/index.html
+-rw-r--r--   0        0        0    44738 2020-02-02 00:00:00.000000 hassle-2.8.0/docs/search.js
+-rw-r--r--   0        0        0    93372 2020-02-02 00:00:00.000000 hassle-2.8.0/docs/hassle/generate_tests.html
+-rw-r--r--   0        0        0   134014 2020-02-02 00:00:00.000000 hassle-2.8.0/docs/hassle/hassle.html
+-rw-r--r--   0        0        0   107599 2020-02-02 00:00:00.000000 hassle-2.8.0/docs/hassle/hassle_config.html
+-rw-r--r--   0        0        0   116364 2020-02-02 00:00:00.000000 hassle-2.8.0/docs/hassle/hassle_utilities.html
+-rw-r--r--   0        0        0   165062 2020-02-02 00:00:00.000000 hassle-2.8.0/docs/hassle/new_project.html
+-rw-r--r--   0        0        0    53742 2020-02-02 00:00:00.000000 hassle-2.8.0/docs/hassle/run_tests.html
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 hassle-2.8.0/src/hassle/.gitignore_template
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 hassle-2.8.0/src/hassle/.vscode_template
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 hassle-2.8.0/src/hassle/README_template.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hassle-2.8.0/src/hassle/__init__.py
+-rw-r--r--   0        0        0     4156 2020-02-02 00:00:00.000000 hassle-2.8.0/src/hassle/generate_tests.py
+-rw-r--r--   0        0        0     7838 2020-02-02 00:00:00.000000 hassle-2.8.0/src/hassle/hassle.py
+-rw-r--r--   0        0        0     5456 2020-02-02 00:00:00.000000 hassle-2.8.0/src/hassle/hassle_config.py
+-rw-r--r--   0        0        0     5246 2020-02-02 00:00:00.000000 hassle-2.8.0/src/hassle/hassle_utilities.py
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 hassle-2.8.0/src/hassle/license_template.txt
+-rw-r--r--   0        0        0     9187 2020-02-02 00:00:00.000000 hassle-2.8.0/src/hassle/new_project.py
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 hassle-2.8.0/src/hassle/pyproject_template.toml
+-rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 hassle-2.8.0/src/hassle/run_tests.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 hassle-2.8.0/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 hassle-2.8.0/LICENSE.txt
+-rw-r--r--   0        0        0    22059 2020-02-02 00:00:00.000000 hassle-2.8.0/README.md
+-rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 hassle-2.8.0/pyproject.toml
+-rw-r--r--   0        0        0    22533 2020-02-02 00:00:00.000000 hassle-2.8.0/PKG-INFO
```

### Comparing `hassle-2.7.1/CHANGELOG.md` & `hassle-2.8.0/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,31 @@
 # Changelog
 
-## 2.7.0 (2023-04-28)
+## 2.7.1 (2023-05-02)
+
+#### Fixes
+
+* remove update_minimum_python_version from build process since vermin is incorrectly reporting min versions
+#### Refactorings
+
+* set requires-python to >=3.10 in pyproject_template
+#### Docs
+
+* modify doc string formatting
+
+
+## v2.7.0 (2023-04-28)
 
 #### Refactorings
 
 * add a pause to manually prune the changelog before committing the autoupdate
+#### Others
+
+* build v2.7.0
+* update changelog
 
 
 ## v2.6.0 (2023-04-15)
 
 #### Refactorings
 
 * return minimum py version as string
```

### Comparing `hassle-2.7.1/docs/hassle.html` & `hassle-2.8.0/docs/hassle.html`

 * *Files identical despite different names*

### Comparing `hassle-2.7.1/docs/search.js` & `hassle-2.8.0/docs/search.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -742,14 +742,22 @@
         "modulename": "hassle.hassle",
         "qualname": "get_args",
         "kind": "function",
         "doc": "<p></p>\n",
         "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"return-annotation\">) -> <span class=\"n\">argparse</span><span class=\"o\">.</span><span class=\"n\">Namespace</span>:</span></span>",
         "funcdef": "def"
     }, {
+        "fullname": "hassle.hassle.build",
+        "modulename": "hassle.hassle",
+        "qualname": "build",
+        "kind": "function",
+        "doc": "<p>Perform the build process.</p>\n\n<p>Steps:</p>\n\n<ul>\n<li>Run tests (unless <code>skip_tests</code> is <code>True</code>)</li>\n<li>Raise error and abandon build if tests fail</li>\n<li>Format source code with <code>Black</code></li>\n<li>Sort source code imports with <code>isort</code></li>\n<li>Update project dependencies in <code>pyproject.toml</code></li>\n<li>Generate docs</li>\n<li>Delete previous <code>dist</code> folder contents</li>\n<li>Invoke build module</li>\n</ul>\n",
+        "signature": "<span class=\"signature pdoc-code multiline\">(<span class=\"param\">\t<span class=\"n\">package_dir</span><span class=\"p\">:</span> <span class=\"n\">pathier</span><span class=\"o\">.</span><span class=\"n\">pathier</span><span class=\"o\">.</span><span class=\"n\">Pathier</span>,</span><span class=\"param\">\t<span class=\"n\">skip_tests</span><span class=\"p\">:</span> <span class=\"nb\">bool</span> <span class=\"o\">=</span> <span class=\"kc\">False</span>,</span><span class=\"param\">\t<span class=\"n\">overwrite_dependencies</span><span class=\"p\">:</span> <span class=\"nb\">bool</span> <span class=\"o\">=</span> <span class=\"kc\">False</span></span><span class=\"return-annotation\">):</span></span>",
+        "funcdef": "def"
+    }, {
         "fullname": "hassle.hassle.main",
         "modulename": "hassle.hassle",
         "qualname": "main",
         "kind": "function",
         "doc": "<p></p>\n",
         "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"n\">args</span><span class=\"p\">:</span> <span class=\"n\">argparse</span><span class=\"o\">.</span><span class=\"n\">Namespace</span> <span class=\"o\">=</span> <span class=\"kc\">None</span></span><span class=\"return-annotation\">):</span></span>",
         "funcdef": "def"
@@ -880,14 +888,22 @@
         "modulename": "hassle.hassle_utilities",
         "qualname": "tag_version",
         "kind": "function",
         "doc": "<p>Add a git tag corresponding\nto the version number in pyproject.toml.</p>\n",
         "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"n\">package_path</span><span class=\"p\">:</span> <span class=\"n\">pathier</span><span class=\"o\">.</span><span class=\"n\">pathier</span><span class=\"o\">.</span><span class=\"n\">Pathier</span></span><span class=\"return-annotation\">):</span></span>",
         "funcdef": "def"
     }, {
+        "fullname": "hassle.hassle_utilities.format_files",
+        "modulename": "hassle.hassle_utilities",
+        "qualname": "format_files",
+        "kind": "function",
+        "doc": "<p>Use <code>Black</code> to format file(s).</p>\n",
+        "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"n\">path</span><span class=\"p\">:</span> <span class=\"n\">pathier</span><span class=\"o\">.</span><span class=\"n\">pathier</span><span class=\"o\">.</span><span class=\"n\">Pathier</span></span><span class=\"return-annotation\">):</span></span>",
+        "funcdef": "def"
+    }, {
         "fullname": "hassle.new_project",
         "modulename": "hassle.new_project",
         "kind": "module",
         "doc": "<p></p>\n"
     }, {
         "fullname": "hassle.new_project.get_args",
         "modulename": "hassle.new_project",
@@ -990,16 +1006,16 @@
         "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"return-annotation\">) -> <span class=\"n\">argparse</span><span class=\"o\">.</span><span class=\"n\">Namespace</span>:</span></span>",
         "funcdef": "def"
     }, {
         "fullname": "hassle.run_tests.run_tests",
         "modulename": "hassle.run_tests",
         "qualname": "run_tests",
         "kind": "function",
-        "doc": "<p>Run tests with coverage and pytest.</p>\n",
-        "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"n\">package_path</span><span class=\"p\">:</span> <span class=\"n\">pathier</span><span class=\"o\">.</span><span class=\"n\">pathier</span><span class=\"o\">.</span><span class=\"n\">Pathier</span></span><span class=\"return-annotation\">):</span></span>",
+        "doc": "<p>Run tests with coverage and pytest.</p>\n\n<p>Returns True if all tests passed.</p>\n",
+        "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"n\">package_path</span><span class=\"p\">:</span> <span class=\"n\">pathier</span><span class=\"o\">.</span><span class=\"n\">pathier</span><span class=\"o\">.</span><span class=\"n\">Pathier</span></span><span class=\"return-annotation\">) -> <span class=\"nb\">bool</span>:</span></span>",
         "funcdef": "def"
     }, {
         "fullname": "hassle.run_tests.main",
         "modulename": "hassle.run_tests",
         "qualname": "main",
         "kind": "function",
         "doc": "<p></p>\n",
```

### Comparing `hassle-2.7.1/docs/hassle/generate_tests.html` & `hassle-2.8.0/docs/hassle/generate_tests.html`

 * *Files 0% similar despite different names*

```diff
@@ -63,138 +63,140 @@
 
                 
                         <input id="mod-generate_tests-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 
                         <label class="view-source-button" for="mod-generate_tests-view-source"><span>View Source</span></label>
 
                         <div class="pdoc-code codehilite"><pre><span></span><span id="L-1"><a href="#L-1"><span class="linenos">  1</span></a><span class="kn">import</span> <span class="nn">argparse</span>
-</span><span id="L-2"><a href="#L-2"><span class="linenos">  2</span></a><span class="kn">import</span> <span class="nn">os</span>
-</span><span id="L-3"><a href="#L-3"><span class="linenos">  3</span></a><span class="kn">import</span> <span class="nn">tokenize</span>
-</span><span id="L-4"><a href="#L-4"><span class="linenos">  4</span></a>
+</span><span id="L-2"><a href="#L-2"><span class="linenos">  2</span></a><span class="kn">import</span> <span class="nn">tokenize</span>
+</span><span id="L-3"><a href="#L-3"><span class="linenos">  3</span></a>
+</span><span id="L-4"><a href="#L-4"><span class="linenos">  4</span></a><span class="kn">import</span> <span class="nn">isort</span>
 </span><span id="L-5"><a href="#L-5"><span class="linenos">  5</span></a><span class="kn">from</span> <span class="nn">pathier</span> <span class="kn">import</span> <span class="n">Pathier</span>
 </span><span id="L-6"><a href="#L-6"><span class="linenos">  6</span></a>
-</span><span id="L-7"><a href="#L-7"><span class="linenos">  7</span></a><span class="n">root</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="vm">__file__</span><span class="p">)</span><span class="o">.</span><span class="n">parent</span>
+</span><span id="L-7"><a href="#L-7"><span class="linenos">  7</span></a><span class="kn">from</span> <span class="nn">hassle</span> <span class="kn">import</span> <span class="n">hassle_utilities</span>
 </span><span id="L-8"><a href="#L-8"><span class="linenos">  8</span></a>
-</span><span id="L-9"><a href="#L-9"><span class="linenos">  9</span></a>
-</span><span id="L-10"><a href="#L-10"><span class="linenos"> 10</span></a><span class="k">def</span> <span class="nf">get_args</span><span class="p">()</span> <span class="o">-&gt;</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span><span class="p">:</span>
-</span><span id="L-11"><a href="#L-11"><span class="linenos"> 11</span></a>    <span class="n">parser</span> <span class="o">=</span> <span class="n">argparse</span><span class="o">.</span><span class="n">ArgumentParser</span><span class="p">()</span>
-</span><span id="L-12"><a href="#L-12"><span class="linenos"> 12</span></a>
-</span><span id="L-13"><a href="#L-13"><span class="linenos"> 13</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="L-14"><a href="#L-14"><span class="linenos"> 14</span></a>        <span class="s2">&quot;paths&quot;</span><span class="p">,</span>
-</span><span id="L-15"><a href="#L-15"><span class="linenos"> 15</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
-</span><span id="L-16"><a href="#L-16"><span class="linenos"> 16</span></a>        <span class="n">default</span><span class="o">=</span><span class="s2">&quot;.&quot;</span><span class="p">,</span>
-</span><span id="L-17"><a href="#L-17"><span class="linenos"> 17</span></a>        <span class="n">nargs</span><span class="o">=</span><span class="s2">&quot;*&quot;</span><span class="p">,</span>
-</span><span id="L-18"><a href="#L-18"><span class="linenos"> 18</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; The name of the package or project to generate tests for,</span>
-</span><span id="L-19"><a href="#L-19"><span class="linenos"> 19</span></a><span class="s2">        assuming it&#39;s a subfolder of your current working directory.</span>
-</span><span id="L-20"><a href="#L-20"><span class="linenos"> 20</span></a><span class="s2">        Can also be a full path to the package. If nothing is given,</span>
-</span><span id="L-21"><a href="#L-21"><span class="linenos"> 21</span></a><span class="s2">        the current working directory will be used.</span>
-</span><span id="L-22"><a href="#L-22"><span class="linenos"> 22</span></a><span class="s2">        Can also be individual files.&quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="L-23"><a href="#L-23"><span class="linenos"> 23</span></a>    <span class="p">)</span>
-</span><span id="L-24"><a href="#L-24"><span class="linenos"> 24</span></a>
-</span><span id="L-25"><a href="#L-25"><span class="linenos"> 25</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="L-26"><a href="#L-26"><span class="linenos"> 26</span></a>        <span class="s2">&quot;-t&quot;</span><span class="p">,</span>
-</span><span id="L-27"><a href="#L-27"><span class="linenos"> 27</span></a>        <span class="s2">&quot;--tests_dir&quot;</span><span class="p">,</span>
-</span><span id="L-28"><a href="#L-28"><span class="linenos"> 28</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
-</span><span id="L-29"><a href="#L-29"><span class="linenos"> 29</span></a>        <span class="n">default</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span>
-</span><span id="L-30"><a href="#L-30"><span class="linenos"> 30</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; A specific tests directory path to write tests to.</span>
-</span><span id="L-31"><a href="#L-31"><span class="linenos"> 31</span></a><span class="s2">        When supplying individual files to paths arg, the default</span>
-</span><span id="L-32"><a href="#L-32"><span class="linenos"> 32</span></a><span class="s2">        behavior is to create a &#39;tests&#39; directory in the parent </span>
-</span><span id="L-33"><a href="#L-33"><span class="linenos"> 33</span></a><span class="s2">        directory of the specified file, resulting in multiple </span>
-</span><span id="L-34"><a href="#L-34"><span class="linenos"> 34</span></a><span class="s2">        &#39;tests&#39; directories being created if the files exist in</span>
-</span><span id="L-35"><a href="#L-35"><span class="linenos"> 35</span></a><span class="s2">        subdirectories. Supply a path to this arg to override</span>
-</span><span id="L-36"><a href="#L-36"><span class="linenos"> 36</span></a><span class="s2">        this behavior.&quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="L-37"><a href="#L-37"><span class="linenos"> 37</span></a>    <span class="p">)</span>
-</span><span id="L-38"><a href="#L-38"><span class="linenos"> 38</span></a>
-</span><span id="L-39"><a href="#L-39"><span class="linenos"> 39</span></a>    <span class="n">args</span> <span class="o">=</span> <span class="n">parser</span><span class="o">.</span><span class="n">parse_args</span><span class="p">()</span>
-</span><span id="L-40"><a href="#L-40"><span class="linenos"> 40</span></a>    <span class="k">return</span> <span class="n">args</span>
-</span><span id="L-41"><a href="#L-41"><span class="linenos"> 41</span></a>
-</span><span id="L-42"><a href="#L-42"><span class="linenos"> 42</span></a>
-</span><span id="L-43"><a href="#L-43"><span class="linenos"> 43</span></a><span class="k">def</span> <span class="nf">get_function_names</span><span class="p">(</span><span class="n">filepath</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]:</span>
-</span><span id="L-44"><a href="#L-44"><span class="linenos"> 44</span></a>    <span class="sd">&quot;&quot;&quot;Returns a list of function names from a .py file.&quot;&quot;&quot;</span>
-</span><span id="L-45"><a href="#L-45"><span class="linenos"> 45</span></a>    <span class="k">with</span> <span class="n">filepath</span><span class="o">.</span><span class="n">open</span><span class="p">(</span><span class="s2">&quot;r&quot;</span><span class="p">)</span> <span class="k">as</span> <span class="n">file</span><span class="p">:</span>
-</span><span id="L-46"><a href="#L-46"><span class="linenos"> 46</span></a>        <span class="n">tokens</span> <span class="o">=</span> <span class="nb">list</span><span class="p">(</span><span class="n">tokenize</span><span class="o">.</span><span class="n">generate_tokens</span><span class="p">(</span><span class="n">file</span><span class="o">.</span><span class="n">readline</span><span class="p">))</span>
-</span><span id="L-47"><a href="#L-47"><span class="linenos"> 47</span></a>    <span class="n">functions</span> <span class="o">=</span> <span class="p">[]</span>
-</span><span id="L-48"><a href="#L-48"><span class="linenos"> 48</span></a>    <span class="k">for</span> <span class="n">i</span><span class="p">,</span> <span class="n">token</span> <span class="ow">in</span> <span class="nb">enumerate</span><span class="p">(</span><span class="n">tokens</span><span class="p">):</span>
-</span><span id="L-49"><a href="#L-49"><span class="linenos"> 49</span></a>        <span class="c1"># If token.type is &quot;name&quot; and the preceeding token is &quot;def&quot;</span>
-</span><span id="L-50"><a href="#L-50"><span class="linenos"> 50</span></a>        <span class="k">if</span> <span class="p">(</span>
-</span><span id="L-51"><a href="#L-51"><span class="linenos"> 51</span></a>            <span class="n">token</span><span class="o">.</span><span class="n">type</span> <span class="o">==</span> <span class="mi">1</span>
-</span><span id="L-52"><a href="#L-52"><span class="linenos"> 52</span></a>            <span class="ow">and</span> <span class="n">tokens</span><span class="p">[</span><span class="n">i</span> <span class="o">-</span> <span class="mi">1</span><span class="p">]</span><span class="o">.</span><span class="n">type</span> <span class="o">==</span> <span class="mi">1</span>
-</span><span id="L-53"><a href="#L-53"><span class="linenos"> 53</span></a>            <span class="ow">and</span> <span class="n">tokens</span><span class="p">[</span><span class="n">i</span> <span class="o">-</span> <span class="mi">1</span><span class="p">]</span><span class="o">.</span><span class="n">string</span> <span class="o">==</span> <span class="s2">&quot;def&quot;</span>
-</span><span id="L-54"><a href="#L-54"><span class="linenos"> 54</span></a>        <span class="p">):</span>
-</span><span id="L-55"><a href="#L-55"><span class="linenos"> 55</span></a>            <span class="n">functions</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">token</span><span class="o">.</span><span class="n">string</span><span class="p">)</span>
-</span><span id="L-56"><a href="#L-56"><span class="linenos"> 56</span></a>    <span class="k">return</span> <span class="n">functions</span>
-</span><span id="L-57"><a href="#L-57"><span class="linenos"> 57</span></a>
-</span><span id="L-58"><a href="#L-58"><span class="linenos"> 58</span></a>
-</span><span id="L-59"><a href="#L-59"><span class="linenos"> 59</span></a><span class="k">def</span> <span class="nf">write_placeholders</span><span class="p">(</span>
-</span><span id="L-60"><a href="#L-60"><span class="linenos"> 60</span></a>    <span class="n">package_path</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">,</span>
-</span><span id="L-61"><a href="#L-61"><span class="linenos"> 61</span></a>    <span class="n">pyfile</span><span class="p">:</span> <span class="n">Pathier</span> <span class="o">|</span> <span class="nb">str</span><span class="p">,</span>
-</span><span id="L-62"><a href="#L-62"><span class="linenos"> 62</span></a>    <span class="n">functions</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">],</span>
-</span><span id="L-63"><a href="#L-63"><span class="linenos"> 63</span></a>    <span class="n">tests_dir</span><span class="p">:</span> <span class="n">Pathier</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="L-64"><a href="#L-64"><span class="linenos"> 64</span></a><span class="p">):</span>
-</span><span id="L-65"><a href="#L-65"><span class="linenos"> 65</span></a>    <span class="sd">&quot;&quot;&quot;Write placeholder functions to the</span>
-</span><span id="L-66"><a href="#L-66"><span class="linenos"> 66</span></a><span class="sd">    tests/test_{pyfile} file if they don&#39;t already exist.</span>
-</span><span id="L-67"><a href="#L-67"><span class="linenos"> 67</span></a><span class="sd">    The placeholder functions use the naming convention</span>
-</span><span id="L-68"><a href="#L-68"><span class="linenos"> 68</span></a><span class="sd">    test_{function_name}</span>
-</span><span id="L-69"><a href="#L-69"><span class="linenos"> 69</span></a>
-</span><span id="L-70"><a href="#L-70"><span class="linenos"> 70</span></a><span class="sd">    :param package_path: Path to the package.</span>
+</span><span id="L-9"><a href="#L-9"><span class="linenos">  9</span></a><span class="n">root</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="vm">__file__</span><span class="p">)</span><span class="o">.</span><span class="n">parent</span>
+</span><span id="L-10"><a href="#L-10"><span class="linenos"> 10</span></a>
+</span><span id="L-11"><a href="#L-11"><span class="linenos"> 11</span></a>
+</span><span id="L-12"><a href="#L-12"><span class="linenos"> 12</span></a><span class="k">def</span> <span class="nf">get_args</span><span class="p">()</span> <span class="o">-&gt;</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span><span class="p">:</span>
+</span><span id="L-13"><a href="#L-13"><span class="linenos"> 13</span></a>    <span class="n">parser</span> <span class="o">=</span> <span class="n">argparse</span><span class="o">.</span><span class="n">ArgumentParser</span><span class="p">()</span>
+</span><span id="L-14"><a href="#L-14"><span class="linenos"> 14</span></a>
+</span><span id="L-15"><a href="#L-15"><span class="linenos"> 15</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="L-16"><a href="#L-16"><span class="linenos"> 16</span></a>        <span class="s2">&quot;paths&quot;</span><span class="p">,</span>
+</span><span id="L-17"><a href="#L-17"><span class="linenos"> 17</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
+</span><span id="L-18"><a href="#L-18"><span class="linenos"> 18</span></a>        <span class="n">default</span><span class="o">=</span><span class="s2">&quot;.&quot;</span><span class="p">,</span>
+</span><span id="L-19"><a href="#L-19"><span class="linenos"> 19</span></a>        <span class="n">nargs</span><span class="o">=</span><span class="s2">&quot;*&quot;</span><span class="p">,</span>
+</span><span id="L-20"><a href="#L-20"><span class="linenos"> 20</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; The name of the package or project to generate tests for,</span>
+</span><span id="L-21"><a href="#L-21"><span class="linenos"> 21</span></a><span class="s2">        assuming it&#39;s a subfolder of your current working directory.</span>
+</span><span id="L-22"><a href="#L-22"><span class="linenos"> 22</span></a><span class="s2">        Can also be a full path to the package. If nothing is given,</span>
+</span><span id="L-23"><a href="#L-23"><span class="linenos"> 23</span></a><span class="s2">        the current working directory will be used.</span>
+</span><span id="L-24"><a href="#L-24"><span class="linenos"> 24</span></a><span class="s2">        Can also be individual files.&quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="L-25"><a href="#L-25"><span class="linenos"> 25</span></a>    <span class="p">)</span>
+</span><span id="L-26"><a href="#L-26"><span class="linenos"> 26</span></a>
+</span><span id="L-27"><a href="#L-27"><span class="linenos"> 27</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="L-28"><a href="#L-28"><span class="linenos"> 28</span></a>        <span class="s2">&quot;-t&quot;</span><span class="p">,</span>
+</span><span id="L-29"><a href="#L-29"><span class="linenos"> 29</span></a>        <span class="s2">&quot;--tests_dir&quot;</span><span class="p">,</span>
+</span><span id="L-30"><a href="#L-30"><span class="linenos"> 30</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
+</span><span id="L-31"><a href="#L-31"><span class="linenos"> 31</span></a>        <span class="n">default</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span>
+</span><span id="L-32"><a href="#L-32"><span class="linenos"> 32</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; A specific tests directory path to write tests to.</span>
+</span><span id="L-33"><a href="#L-33"><span class="linenos"> 33</span></a><span class="s2">        When supplying individual files to paths arg, the default</span>
+</span><span id="L-34"><a href="#L-34"><span class="linenos"> 34</span></a><span class="s2">        behavior is to create a &#39;tests&#39; directory in the parent </span>
+</span><span id="L-35"><a href="#L-35"><span class="linenos"> 35</span></a><span class="s2">        directory of the specified file, resulting in multiple </span>
+</span><span id="L-36"><a href="#L-36"><span class="linenos"> 36</span></a><span class="s2">        &#39;tests&#39; directories being created if the files exist in</span>
+</span><span id="L-37"><a href="#L-37"><span class="linenos"> 37</span></a><span class="s2">        subdirectories. Supply a path to this arg to override</span>
+</span><span id="L-38"><a href="#L-38"><span class="linenos"> 38</span></a><span class="s2">        this behavior.&quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="L-39"><a href="#L-39"><span class="linenos"> 39</span></a>    <span class="p">)</span>
+</span><span id="L-40"><a href="#L-40"><span class="linenos"> 40</span></a>
+</span><span id="L-41"><a href="#L-41"><span class="linenos"> 41</span></a>    <span class="n">args</span> <span class="o">=</span> <span class="n">parser</span><span class="o">.</span><span class="n">parse_args</span><span class="p">()</span>
+</span><span id="L-42"><a href="#L-42"><span class="linenos"> 42</span></a>    <span class="k">return</span> <span class="n">args</span>
+</span><span id="L-43"><a href="#L-43"><span class="linenos"> 43</span></a>
+</span><span id="L-44"><a href="#L-44"><span class="linenos"> 44</span></a>
+</span><span id="L-45"><a href="#L-45"><span class="linenos"> 45</span></a><span class="k">def</span> <span class="nf">get_function_names</span><span class="p">(</span><span class="n">filepath</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]:</span>
+</span><span id="L-46"><a href="#L-46"><span class="linenos"> 46</span></a>    <span class="sd">&quot;&quot;&quot;Returns a list of function names from a .py file.&quot;&quot;&quot;</span>
+</span><span id="L-47"><a href="#L-47"><span class="linenos"> 47</span></a>    <span class="k">with</span> <span class="n">filepath</span><span class="o">.</span><span class="n">open</span><span class="p">(</span><span class="s2">&quot;r&quot;</span><span class="p">)</span> <span class="k">as</span> <span class="n">file</span><span class="p">:</span>
+</span><span id="L-48"><a href="#L-48"><span class="linenos"> 48</span></a>        <span class="n">tokens</span> <span class="o">=</span> <span class="nb">list</span><span class="p">(</span><span class="n">tokenize</span><span class="o">.</span><span class="n">generate_tokens</span><span class="p">(</span><span class="n">file</span><span class="o">.</span><span class="n">readline</span><span class="p">))</span>
+</span><span id="L-49"><a href="#L-49"><span class="linenos"> 49</span></a>    <span class="n">functions</span> <span class="o">=</span> <span class="p">[]</span>
+</span><span id="L-50"><a href="#L-50"><span class="linenos"> 50</span></a>    <span class="k">for</span> <span class="n">i</span><span class="p">,</span> <span class="n">token</span> <span class="ow">in</span> <span class="nb">enumerate</span><span class="p">(</span><span class="n">tokens</span><span class="p">):</span>
+</span><span id="L-51"><a href="#L-51"><span class="linenos"> 51</span></a>        <span class="c1"># If token.type is &quot;name&quot; and the preceeding token is &quot;def&quot;</span>
+</span><span id="L-52"><a href="#L-52"><span class="linenos"> 52</span></a>        <span class="k">if</span> <span class="p">(</span>
+</span><span id="L-53"><a href="#L-53"><span class="linenos"> 53</span></a>            <span class="n">token</span><span class="o">.</span><span class="n">type</span> <span class="o">==</span> <span class="mi">1</span>
+</span><span id="L-54"><a href="#L-54"><span class="linenos"> 54</span></a>            <span class="ow">and</span> <span class="n">tokens</span><span class="p">[</span><span class="n">i</span> <span class="o">-</span> <span class="mi">1</span><span class="p">]</span><span class="o">.</span><span class="n">type</span> <span class="o">==</span> <span class="mi">1</span>
+</span><span id="L-55"><a href="#L-55"><span class="linenos"> 55</span></a>            <span class="ow">and</span> <span class="n">tokens</span><span class="p">[</span><span class="n">i</span> <span class="o">-</span> <span class="mi">1</span><span class="p">]</span><span class="o">.</span><span class="n">string</span> <span class="o">==</span> <span class="s2">&quot;def&quot;</span>
+</span><span id="L-56"><a href="#L-56"><span class="linenos"> 56</span></a>        <span class="p">):</span>
+</span><span id="L-57"><a href="#L-57"><span class="linenos"> 57</span></a>            <span class="n">functions</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">token</span><span class="o">.</span><span class="n">string</span><span class="p">)</span>
+</span><span id="L-58"><a href="#L-58"><span class="linenos"> 58</span></a>    <span class="k">return</span> <span class="n">functions</span>
+</span><span id="L-59"><a href="#L-59"><span class="linenos"> 59</span></a>
+</span><span id="L-60"><a href="#L-60"><span class="linenos"> 60</span></a>
+</span><span id="L-61"><a href="#L-61"><span class="linenos"> 61</span></a><span class="k">def</span> <span class="nf">write_placeholders</span><span class="p">(</span>
+</span><span id="L-62"><a href="#L-62"><span class="linenos"> 62</span></a>    <span class="n">package_path</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">,</span>
+</span><span id="L-63"><a href="#L-63"><span class="linenos"> 63</span></a>    <span class="n">pyfile</span><span class="p">:</span> <span class="n">Pathier</span> <span class="o">|</span> <span class="nb">str</span><span class="p">,</span>
+</span><span id="L-64"><a href="#L-64"><span class="linenos"> 64</span></a>    <span class="n">functions</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">],</span>
+</span><span id="L-65"><a href="#L-65"><span class="linenos"> 65</span></a>    <span class="n">tests_dir</span><span class="p">:</span> <span class="n">Pathier</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="L-66"><a href="#L-66"><span class="linenos"> 66</span></a><span class="p">):</span>
+</span><span id="L-67"><a href="#L-67"><span class="linenos"> 67</span></a>    <span class="sd">&quot;&quot;&quot;Write placeholder functions to the</span>
+</span><span id="L-68"><a href="#L-68"><span class="linenos"> 68</span></a><span class="sd">    tests/test_{pyfile} file if they don&#39;t already exist.</span>
+</span><span id="L-69"><a href="#L-69"><span class="linenos"> 69</span></a><span class="sd">    The placeholder functions use the naming convention</span>
+</span><span id="L-70"><a href="#L-70"><span class="linenos"> 70</span></a><span class="sd">    test_{function_name}</span>
 </span><span id="L-71"><a href="#L-71"><span class="linenos"> 71</span></a>
-</span><span id="L-72"><a href="#L-72"><span class="linenos"> 72</span></a><span class="sd">    :param pyfile: Path to the pyfile to write placeholders for.</span>
+</span><span id="L-72"><a href="#L-72"><span class="linenos"> 72</span></a><span class="sd">    :param package_path: Path to the package.</span>
 </span><span id="L-73"><a href="#L-73"><span class="linenos"> 73</span></a>
-</span><span id="L-74"><a href="#L-74"><span class="linenos"> 74</span></a><span class="sd">    :param functions: List of functions to generate</span>
-</span><span id="L-75"><a href="#L-75"><span class="linenos"> 75</span></a><span class="sd">    placehodlers for.&quot;&quot;&quot;</span>
-</span><span id="L-76"><a href="#L-76"><span class="linenos"> 76</span></a>    <span class="n">package_name</span> <span class="o">=</span> <span class="n">package_path</span><span class="o">.</span><span class="n">stem</span>
-</span><span id="L-77"><a href="#L-77"><span class="linenos"> 77</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">tests_dir</span><span class="p">:</span>
-</span><span id="L-78"><a href="#L-78"><span class="linenos"> 78</span></a>        <span class="n">tests_dir</span> <span class="o">=</span> <span class="n">package_path</span> <span class="o">/</span> <span class="s2">&quot;tests&quot;</span>
-</span><span id="L-79"><a href="#L-79"><span class="linenos"> 79</span></a>    <span class="n">tests_dir</span><span class="o">.</span><span class="n">mkdir</span><span class="p">()</span>
-</span><span id="L-80"><a href="#L-80"><span class="linenos"> 80</span></a>    <span class="n">pyfile</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="n">pyfile</span><span class="p">)</span>
-</span><span id="L-81"><a href="#L-81"><span class="linenos"> 81</span></a>    <span class="n">test_file</span> <span class="o">=</span> <span class="n">tests_dir</span> <span class="o">/</span> <span class="sa">f</span><span class="s2">&quot;test_</span><span class="si">{</span><span class="n">pyfile</span><span class="o">.</span><span class="n">name</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="L-82"><a href="#L-82"><span class="linenos"> 82</span></a>    <span class="c1"># Makes sure not to overwrite previously written tests</span>
-</span><span id="L-83"><a href="#L-83"><span class="linenos"> 83</span></a>    <span class="c1"># or additional imports.</span>
-</span><span id="L-84"><a href="#L-84"><span class="linenos"> 84</span></a>    <span class="k">if</span> <span class="n">test_file</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
-</span><span id="L-85"><a href="#L-85"><span class="linenos"> 85</span></a>        <span class="n">content</span> <span class="o">=</span> <span class="n">test_file</span><span class="o">.</span><span class="n">read_text</span><span class="p">()</span> <span class="o">+</span> <span class="s2">&quot;</span><span class="se">\n\n</span><span class="s2">&quot;</span>
-</span><span id="L-86"><a href="#L-86"><span class="linenos"> 86</span></a>    <span class="k">else</span><span class="p">:</span>
-</span><span id="L-87"><a href="#L-87"><span class="linenos"> 87</span></a>        <span class="n">content</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;import pytest</span><span class="se">\n</span><span class="s2">from </span><span class="si">{</span><span class="n">package_name</span><span class="si">}</span><span class="s2"> import </span><span class="si">{</span><span class="n">pyfile</span><span class="o">.</span><span class="n">stem</span><span class="si">}</span><span class="se">\n\n\n</span><span class="s2">&quot;</span>
-</span><span id="L-88"><a href="#L-88"><span class="linenos"> 88</span></a>    <span class="k">for</span> <span class="n">function</span> <span class="ow">in</span> <span class="n">functions</span><span class="p">:</span>
-</span><span id="L-89"><a href="#L-89"><span class="linenos"> 89</span></a>        <span class="n">test_function</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;def test_</span><span class="si">{</span><span class="n">function</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="L-90"><a href="#L-90"><span class="linenos"> 90</span></a>        <span class="k">if</span> <span class="n">test_function</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">content</span> <span class="ow">and</span> <span class="n">function</span> <span class="o">!=</span> <span class="s2">&quot;__init__&quot;</span><span class="p">:</span>
-</span><span id="L-91"><a href="#L-91"><span class="linenos"> 91</span></a>            <span class="n">content</span> <span class="o">+=</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">test_function</span><span class="si">}</span><span class="s2">():</span><span class="se">\n</span><span class="s2">    ...</span><span class="se">\n\n\n</span><span class="s2">&quot;</span>
-</span><span id="L-92"><a href="#L-92"><span class="linenos"> 92</span></a>    <span class="n">test_file</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span><span class="n">content</span><span class="p">)</span>
-</span><span id="L-93"><a href="#L-93"><span class="linenos"> 93</span></a>    <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;black </span><span class="si">{</span><span class="n">tests_dir</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="L-94"><a href="#L-94"><span class="linenos"> 94</span></a>    <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;isort </span><span class="si">{</span><span class="n">tests_dir</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="L-95"><a href="#L-95"><span class="linenos"> 95</span></a>
-</span><span id="L-96"><a href="#L-96"><span class="linenos"> 96</span></a>
-</span><span id="L-97"><a href="#L-97"><span class="linenos"> 97</span></a><span class="k">def</span> <span class="nf">generate_test_files</span><span class="p">(</span><span class="n">package_path</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">,</span> <span class="n">tests_dir</span><span class="p">:</span> <span class="n">Pathier</span> <span class="o">=</span> <span class="kc">None</span><span class="p">):</span>
-</span><span id="L-98"><a href="#L-98"><span class="linenos"> 98</span></a>    <span class="sd">&quot;&quot;&quot;Generate test files for all .py files in &#39;src&#39;</span>
-</span><span id="L-99"><a href="#L-99"><span class="linenos"> 99</span></a><span class="sd">    directory of &#39;package_path&#39;.&quot;&quot;&quot;</span>
-</span><span id="L-100"><a href="#L-100"><span class="linenos">100</span></a>    <span class="n">pyfiles</span> <span class="o">=</span> <span class="p">[</span>
-</span><span id="L-101"><a href="#L-101"><span class="linenos">101</span></a>        <span class="n">file</span>
-</span><span id="L-102"><a href="#L-102"><span class="linenos">102</span></a>        <span class="k">for</span> <span class="n">file</span> <span class="ow">in</span> <span class="p">(</span><span class="n">package_path</span> <span class="o">/</span> <span class="s2">&quot;src&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">rglob</span><span class="p">(</span><span class="s2">&quot;*.py&quot;</span><span class="p">)</span>
-</span><span id="L-103"><a href="#L-103"><span class="linenos">103</span></a>        <span class="k">if</span> <span class="n">file</span><span class="o">.</span><span class="n">name</span> <span class="o">!=</span> <span class="s2">&quot;__init__.py&quot;</span>
-</span><span id="L-104"><a href="#L-104"><span class="linenos">104</span></a>    <span class="p">]</span>
-</span><span id="L-105"><a href="#L-105"><span class="linenos">105</span></a>    <span class="k">for</span> <span class="n">pyfile</span> <span class="ow">in</span> <span class="n">pyfiles</span><span class="p">:</span>
-</span><span id="L-106"><a href="#L-106"><span class="linenos">106</span></a>        <span class="n">write_placeholders</span><span class="p">(</span><span class="n">package_path</span><span class="p">,</span> <span class="n">pyfile</span><span class="p">,</span> <span class="n">get_function_names</span><span class="p">(</span><span class="n">pyfile</span><span class="p">),</span> <span class="n">tests_dir</span><span class="p">)</span>
-</span><span id="L-107"><a href="#L-107"><span class="linenos">107</span></a>
-</span><span id="L-108"><a href="#L-108"><span class="linenos">108</span></a>
-</span><span id="L-109"><a href="#L-109"><span class="linenos">109</span></a><span class="k">def</span> <span class="nf">main</span><span class="p">(</span><span class="n">args</span><span class="p">:</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span> <span class="o">=</span> <span class="kc">None</span><span class="p">):</span>
-</span><span id="L-110"><a href="#L-110"><span class="linenos">110</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="p">:</span>
-</span><span id="L-111"><a href="#L-111"><span class="linenos">111</span></a>        <span class="n">args</span> <span class="o">=</span> <span class="n">get_args</span><span class="p">()</span>
-</span><span id="L-112"><a href="#L-112"><span class="linenos">112</span></a>    <span class="n">args</span><span class="o">.</span><span class="n">paths</span> <span class="o">=</span> <span class="p">[</span><span class="n">Pathier</span><span class="p">(</span><span class="n">path</span><span class="p">)</span><span class="o">.</span><span class="n">resolve</span><span class="p">()</span> <span class="k">for</span> <span class="n">path</span> <span class="ow">in</span> <span class="n">args</span><span class="o">.</span><span class="n">paths</span><span class="p">]</span>
-</span><span id="L-113"><a href="#L-113"><span class="linenos">113</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">tests_dir</span><span class="p">:</span>
-</span><span id="L-114"><a href="#L-114"><span class="linenos">114</span></a>        <span class="n">args</span><span class="o">.</span><span class="n">tests_dir</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">tests_dir</span><span class="p">)</span><span class="o">.</span><span class="n">resolve</span><span class="p">()</span>
-</span><span id="L-115"><a href="#L-115"><span class="linenos">115</span></a>    <span class="k">for</span> <span class="n">path</span> <span class="ow">in</span> <span class="n">args</span><span class="o">.</span><span class="n">paths</span><span class="p">:</span>
-</span><span id="L-116"><a href="#L-116"><span class="linenos">116</span></a>        <span class="k">if</span> <span class="n">path</span><span class="o">.</span><span class="n">is_dir</span><span class="p">():</span>
-</span><span id="L-117"><a href="#L-117"><span class="linenos">117</span></a>            <span class="n">generate_test_files</span><span class="p">(</span><span class="n">path</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">tests_dir</span><span class="p">)</span>
-</span><span id="L-118"><a href="#L-118"><span class="linenos">118</span></a>        <span class="k">elif</span> <span class="n">path</span><span class="o">.</span><span class="n">is_file</span><span class="p">():</span>
-</span><span id="L-119"><a href="#L-119"><span class="linenos">119</span></a>            <span class="n">write_placeholders</span><span class="p">(</span>
-</span><span id="L-120"><a href="#L-120"><span class="linenos">120</span></a>                <span class="n">path</span><span class="o">.</span><span class="n">parent</span><span class="p">,</span> <span class="n">path</span><span class="p">,</span> <span class="n">get_function_names</span><span class="p">(</span><span class="n">path</span><span class="p">),</span> <span class="n">args</span><span class="o">.</span><span class="n">tests_dir</span>
-</span><span id="L-121"><a href="#L-121"><span class="linenos">121</span></a>            <span class="p">)</span>
-</span><span id="L-122"><a href="#L-122"><span class="linenos">122</span></a>
-</span><span id="L-123"><a href="#L-123"><span class="linenos">123</span></a>
-</span><span id="L-124"><a href="#L-124"><span class="linenos">124</span></a><span class="k">if</span> <span class="vm">__name__</span> <span class="o">==</span> <span class="s2">&quot;__main__&quot;</span><span class="p">:</span>
-</span><span id="L-125"><a href="#L-125"><span class="linenos">125</span></a>    <span class="n">main</span><span class="p">(</span><span class="n">get_args</span><span class="p">())</span>
+</span><span id="L-74"><a href="#L-74"><span class="linenos"> 74</span></a><span class="sd">    :param pyfile: Path to the pyfile to write placeholders for.</span>
+</span><span id="L-75"><a href="#L-75"><span class="linenos"> 75</span></a>
+</span><span id="L-76"><a href="#L-76"><span class="linenos"> 76</span></a><span class="sd">    :param functions: List of functions to generate</span>
+</span><span id="L-77"><a href="#L-77"><span class="linenos"> 77</span></a><span class="sd">    placehodlers for.&quot;&quot;&quot;</span>
+</span><span id="L-78"><a href="#L-78"><span class="linenos"> 78</span></a>    <span class="n">package_name</span> <span class="o">=</span> <span class="n">package_path</span><span class="o">.</span><span class="n">stem</span>
+</span><span id="L-79"><a href="#L-79"><span class="linenos"> 79</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">tests_dir</span><span class="p">:</span>
+</span><span id="L-80"><a href="#L-80"><span class="linenos"> 80</span></a>        <span class="n">tests_dir</span> <span class="o">=</span> <span class="n">package_path</span> <span class="o">/</span> <span class="s2">&quot;tests&quot;</span>
+</span><span id="L-81"><a href="#L-81"><span class="linenos"> 81</span></a>    <span class="n">tests_dir</span><span class="o">.</span><span class="n">mkdir</span><span class="p">()</span>
+</span><span id="L-82"><a href="#L-82"><span class="linenos"> 82</span></a>    <span class="n">pyfile</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="n">pyfile</span><span class="p">)</span>
+</span><span id="L-83"><a href="#L-83"><span class="linenos"> 83</span></a>    <span class="n">test_file</span> <span class="o">=</span> <span class="n">tests_dir</span> <span class="o">/</span> <span class="sa">f</span><span class="s2">&quot;test_</span><span class="si">{</span><span class="n">pyfile</span><span class="o">.</span><span class="n">name</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="L-84"><a href="#L-84"><span class="linenos"> 84</span></a>    <span class="c1"># Makes sure not to overwrite previously written tests</span>
+</span><span id="L-85"><a href="#L-85"><span class="linenos"> 85</span></a>    <span class="c1"># or additional imports.</span>
+</span><span id="L-86"><a href="#L-86"><span class="linenos"> 86</span></a>    <span class="k">if</span> <span class="n">test_file</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
+</span><span id="L-87"><a href="#L-87"><span class="linenos"> 87</span></a>        <span class="n">content</span> <span class="o">=</span> <span class="n">test_file</span><span class="o">.</span><span class="n">read_text</span><span class="p">()</span> <span class="o">+</span> <span class="s2">&quot;</span><span class="se">\n\n</span><span class="s2">&quot;</span>
+</span><span id="L-88"><a href="#L-88"><span class="linenos"> 88</span></a>    <span class="k">else</span><span class="p">:</span>
+</span><span id="L-89"><a href="#L-89"><span class="linenos"> 89</span></a>        <span class="n">content</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;import pytest</span><span class="se">\n</span><span class="s2">from </span><span class="si">{</span><span class="n">package_name</span><span class="si">}</span><span class="s2"> import </span><span class="si">{</span><span class="n">pyfile</span><span class="o">.</span><span class="n">stem</span><span class="si">}</span><span class="se">\n\n\n</span><span class="s2">&quot;</span>
+</span><span id="L-90"><a href="#L-90"><span class="linenos"> 90</span></a>    <span class="k">for</span> <span class="n">function</span> <span class="ow">in</span> <span class="n">functions</span><span class="p">:</span>
+</span><span id="L-91"><a href="#L-91"><span class="linenos"> 91</span></a>        <span class="n">test_function</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;def test_</span><span class="si">{</span><span class="n">function</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="L-92"><a href="#L-92"><span class="linenos"> 92</span></a>        <span class="k">if</span> <span class="n">test_function</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">content</span> <span class="ow">and</span> <span class="n">function</span> <span class="o">!=</span> <span class="s2">&quot;__init__&quot;</span><span class="p">:</span>
+</span><span id="L-93"><a href="#L-93"><span class="linenos"> 93</span></a>            <span class="n">content</span> <span class="o">+=</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">test_function</span><span class="si">}</span><span class="s2">():</span><span class="se">\n</span><span class="s2">    ...</span><span class="se">\n\n\n</span><span class="s2">&quot;</span>
+</span><span id="L-94"><a href="#L-94"><span class="linenos"> 94</span></a>    <span class="n">test_file</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span><span class="n">content</span><span class="p">)</span>
+</span><span id="L-95"><a href="#L-95"><span class="linenos"> 95</span></a>    <span class="n">hassle_utilities</span><span class="o">.</span><span class="n">format_files</span><span class="p">(</span><span class="n">tests_dir</span><span class="p">)</span>
+</span><span id="L-96"><a href="#L-96"><span class="linenos"> 96</span></a>    <span class="p">[</span><span class="n">isort</span><span class="o">.</span><span class="n">file</span><span class="p">(</span><span class="n">path</span><span class="p">)</span> <span class="k">for</span> <span class="n">path</span> <span class="ow">in</span> <span class="n">tests_dir</span><span class="o">.</span><span class="n">rglob</span><span class="p">(</span><span class="s2">&quot;*.py&quot;</span><span class="p">)]</span>
+</span><span id="L-97"><a href="#L-97"><span class="linenos"> 97</span></a>
+</span><span id="L-98"><a href="#L-98"><span class="linenos"> 98</span></a>
+</span><span id="L-99"><a href="#L-99"><span class="linenos"> 99</span></a><span class="k">def</span> <span class="nf">generate_test_files</span><span class="p">(</span><span class="n">package_path</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">,</span> <span class="n">tests_dir</span><span class="p">:</span> <span class="n">Pathier</span> <span class="o">=</span> <span class="kc">None</span><span class="p">):</span>
+</span><span id="L-100"><a href="#L-100"><span class="linenos">100</span></a>    <span class="sd">&quot;&quot;&quot;Generate test files for all .py files in &#39;src&#39;</span>
+</span><span id="L-101"><a href="#L-101"><span class="linenos">101</span></a><span class="sd">    directory of &#39;package_path&#39;.&quot;&quot;&quot;</span>
+</span><span id="L-102"><a href="#L-102"><span class="linenos">102</span></a>    <span class="n">pyfiles</span> <span class="o">=</span> <span class="p">[</span>
+</span><span id="L-103"><a href="#L-103"><span class="linenos">103</span></a>        <span class="n">file</span>
+</span><span id="L-104"><a href="#L-104"><span class="linenos">104</span></a>        <span class="k">for</span> <span class="n">file</span> <span class="ow">in</span> <span class="p">(</span><span class="n">package_path</span> <span class="o">/</span> <span class="s2">&quot;src&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">rglob</span><span class="p">(</span><span class="s2">&quot;*.py&quot;</span><span class="p">)</span>
+</span><span id="L-105"><a href="#L-105"><span class="linenos">105</span></a>        <span class="k">if</span> <span class="n">file</span><span class="o">.</span><span class="n">name</span> <span class="o">!=</span> <span class="s2">&quot;__init__.py&quot;</span>
+</span><span id="L-106"><a href="#L-106"><span class="linenos">106</span></a>    <span class="p">]</span>
+</span><span id="L-107"><a href="#L-107"><span class="linenos">107</span></a>    <span class="k">for</span> <span class="n">pyfile</span> <span class="ow">in</span> <span class="n">pyfiles</span><span class="p">:</span>
+</span><span id="L-108"><a href="#L-108"><span class="linenos">108</span></a>        <span class="n">write_placeholders</span><span class="p">(</span><span class="n">package_path</span><span class="p">,</span> <span class="n">pyfile</span><span class="p">,</span> <span class="n">get_function_names</span><span class="p">(</span><span class="n">pyfile</span><span class="p">),</span> <span class="n">tests_dir</span><span class="p">)</span>
+</span><span id="L-109"><a href="#L-109"><span class="linenos">109</span></a>
+</span><span id="L-110"><a href="#L-110"><span class="linenos">110</span></a>
+</span><span id="L-111"><a href="#L-111"><span class="linenos">111</span></a><span class="k">def</span> <span class="nf">main</span><span class="p">(</span><span class="n">args</span><span class="p">:</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span> <span class="o">=</span> <span class="kc">None</span><span class="p">):</span>
+</span><span id="L-112"><a href="#L-112"><span class="linenos">112</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="p">:</span>
+</span><span id="L-113"><a href="#L-113"><span class="linenos">113</span></a>        <span class="n">args</span> <span class="o">=</span> <span class="n">get_args</span><span class="p">()</span>
+</span><span id="L-114"><a href="#L-114"><span class="linenos">114</span></a>    <span class="n">args</span><span class="o">.</span><span class="n">paths</span> <span class="o">=</span> <span class="p">[</span><span class="n">Pathier</span><span class="p">(</span><span class="n">path</span><span class="p">)</span><span class="o">.</span><span class="n">resolve</span><span class="p">()</span> <span class="k">for</span> <span class="n">path</span> <span class="ow">in</span> <span class="n">args</span><span class="o">.</span><span class="n">paths</span><span class="p">]</span>
+</span><span id="L-115"><a href="#L-115"><span class="linenos">115</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">tests_dir</span><span class="p">:</span>
+</span><span id="L-116"><a href="#L-116"><span class="linenos">116</span></a>        <span class="n">args</span><span class="o">.</span><span class="n">tests_dir</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">tests_dir</span><span class="p">)</span><span class="o">.</span><span class="n">resolve</span><span class="p">()</span>
+</span><span id="L-117"><a href="#L-117"><span class="linenos">117</span></a>    <span class="k">for</span> <span class="n">path</span> <span class="ow">in</span> <span class="n">args</span><span class="o">.</span><span class="n">paths</span><span class="p">:</span>
+</span><span id="L-118"><a href="#L-118"><span class="linenos">118</span></a>        <span class="k">if</span> <span class="n">path</span><span class="o">.</span><span class="n">is_dir</span><span class="p">():</span>
+</span><span id="L-119"><a href="#L-119"><span class="linenos">119</span></a>            <span class="n">generate_test_files</span><span class="p">(</span><span class="n">path</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">tests_dir</span><span class="p">)</span>
+</span><span id="L-120"><a href="#L-120"><span class="linenos">120</span></a>        <span class="k">elif</span> <span class="n">path</span><span class="o">.</span><span class="n">is_file</span><span class="p">():</span>
+</span><span id="L-121"><a href="#L-121"><span class="linenos">121</span></a>            <span class="n">write_placeholders</span><span class="p">(</span>
+</span><span id="L-122"><a href="#L-122"><span class="linenos">122</span></a>                <span class="n">path</span><span class="o">.</span><span class="n">parent</span><span class="p">,</span> <span class="n">path</span><span class="p">,</span> <span class="n">get_function_names</span><span class="p">(</span><span class="n">path</span><span class="p">),</span> <span class="n">args</span><span class="o">.</span><span class="n">tests_dir</span>
+</span><span id="L-123"><a href="#L-123"><span class="linenos">123</span></a>            <span class="p">)</span>
+</span><span id="L-124"><a href="#L-124"><span class="linenos">124</span></a>
+</span><span id="L-125"><a href="#L-125"><span class="linenos">125</span></a>
+</span><span id="L-126"><a href="#L-126"><span class="linenos">126</span></a><span class="k">if</span> <span class="vm">__name__</span> <span class="o">==</span> <span class="s2">&quot;__main__&quot;</span><span class="p">:</span>
+</span><span id="L-127"><a href="#L-127"><span class="linenos">127</span></a>    <span class="n">main</span><span class="p">(</span><span class="n">get_args</span><span class="p">())</span>
 </span></pre></div>
 
 
             </section>
                 <section id="get_args">
                             <input id="get_args-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
@@ -202,45 +204,45 @@
         <span class="def">def</span>
         <span class="name">get_args</span><span class="signature pdoc-code condensed">(<span class="return-annotation">) -> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span>:</span></span>
 
                 <label class="view-source-button" for="get_args-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#get_args"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="get_args-11"><a href="#get_args-11"><span class="linenos">11</span></a><span class="k">def</span> <span class="nf">get_args</span><span class="p">()</span> <span class="o">-&gt;</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span><span class="p">:</span>
-</span><span id="get_args-12"><a href="#get_args-12"><span class="linenos">12</span></a>    <span class="n">parser</span> <span class="o">=</span> <span class="n">argparse</span><span class="o">.</span><span class="n">ArgumentParser</span><span class="p">()</span>
-</span><span id="get_args-13"><a href="#get_args-13"><span class="linenos">13</span></a>
-</span><span id="get_args-14"><a href="#get_args-14"><span class="linenos">14</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="get_args-15"><a href="#get_args-15"><span class="linenos">15</span></a>        <span class="s2">&quot;paths&quot;</span><span class="p">,</span>
-</span><span id="get_args-16"><a href="#get_args-16"><span class="linenos">16</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
-</span><span id="get_args-17"><a href="#get_args-17"><span class="linenos">17</span></a>        <span class="n">default</span><span class="o">=</span><span class="s2">&quot;.&quot;</span><span class="p">,</span>
-</span><span id="get_args-18"><a href="#get_args-18"><span class="linenos">18</span></a>        <span class="n">nargs</span><span class="o">=</span><span class="s2">&quot;*&quot;</span><span class="p">,</span>
-</span><span id="get_args-19"><a href="#get_args-19"><span class="linenos">19</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; The name of the package or project to generate tests for,</span>
-</span><span id="get_args-20"><a href="#get_args-20"><span class="linenos">20</span></a><span class="s2">        assuming it&#39;s a subfolder of your current working directory.</span>
-</span><span id="get_args-21"><a href="#get_args-21"><span class="linenos">21</span></a><span class="s2">        Can also be a full path to the package. If nothing is given,</span>
-</span><span id="get_args-22"><a href="#get_args-22"><span class="linenos">22</span></a><span class="s2">        the current working directory will be used.</span>
-</span><span id="get_args-23"><a href="#get_args-23"><span class="linenos">23</span></a><span class="s2">        Can also be individual files.&quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="get_args-24"><a href="#get_args-24"><span class="linenos">24</span></a>    <span class="p">)</span>
-</span><span id="get_args-25"><a href="#get_args-25"><span class="linenos">25</span></a>
-</span><span id="get_args-26"><a href="#get_args-26"><span class="linenos">26</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="get_args-27"><a href="#get_args-27"><span class="linenos">27</span></a>        <span class="s2">&quot;-t&quot;</span><span class="p">,</span>
-</span><span id="get_args-28"><a href="#get_args-28"><span class="linenos">28</span></a>        <span class="s2">&quot;--tests_dir&quot;</span><span class="p">,</span>
-</span><span id="get_args-29"><a href="#get_args-29"><span class="linenos">29</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
-</span><span id="get_args-30"><a href="#get_args-30"><span class="linenos">30</span></a>        <span class="n">default</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span>
-</span><span id="get_args-31"><a href="#get_args-31"><span class="linenos">31</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; A specific tests directory path to write tests to.</span>
-</span><span id="get_args-32"><a href="#get_args-32"><span class="linenos">32</span></a><span class="s2">        When supplying individual files to paths arg, the default</span>
-</span><span id="get_args-33"><a href="#get_args-33"><span class="linenos">33</span></a><span class="s2">        behavior is to create a &#39;tests&#39; directory in the parent </span>
-</span><span id="get_args-34"><a href="#get_args-34"><span class="linenos">34</span></a><span class="s2">        directory of the specified file, resulting in multiple </span>
-</span><span id="get_args-35"><a href="#get_args-35"><span class="linenos">35</span></a><span class="s2">        &#39;tests&#39; directories being created if the files exist in</span>
-</span><span id="get_args-36"><a href="#get_args-36"><span class="linenos">36</span></a><span class="s2">        subdirectories. Supply a path to this arg to override</span>
-</span><span id="get_args-37"><a href="#get_args-37"><span class="linenos">37</span></a><span class="s2">        this behavior.&quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="get_args-38"><a href="#get_args-38"><span class="linenos">38</span></a>    <span class="p">)</span>
-</span><span id="get_args-39"><a href="#get_args-39"><span class="linenos">39</span></a>
-</span><span id="get_args-40"><a href="#get_args-40"><span class="linenos">40</span></a>    <span class="n">args</span> <span class="o">=</span> <span class="n">parser</span><span class="o">.</span><span class="n">parse_args</span><span class="p">()</span>
-</span><span id="get_args-41"><a href="#get_args-41"><span class="linenos">41</span></a>    <span class="k">return</span> <span class="n">args</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="get_args-13"><a href="#get_args-13"><span class="linenos">13</span></a><span class="k">def</span> <span class="nf">get_args</span><span class="p">()</span> <span class="o">-&gt;</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span><span class="p">:</span>
+</span><span id="get_args-14"><a href="#get_args-14"><span class="linenos">14</span></a>    <span class="n">parser</span> <span class="o">=</span> <span class="n">argparse</span><span class="o">.</span><span class="n">ArgumentParser</span><span class="p">()</span>
+</span><span id="get_args-15"><a href="#get_args-15"><span class="linenos">15</span></a>
+</span><span id="get_args-16"><a href="#get_args-16"><span class="linenos">16</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="get_args-17"><a href="#get_args-17"><span class="linenos">17</span></a>        <span class="s2">&quot;paths&quot;</span><span class="p">,</span>
+</span><span id="get_args-18"><a href="#get_args-18"><span class="linenos">18</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
+</span><span id="get_args-19"><a href="#get_args-19"><span class="linenos">19</span></a>        <span class="n">default</span><span class="o">=</span><span class="s2">&quot;.&quot;</span><span class="p">,</span>
+</span><span id="get_args-20"><a href="#get_args-20"><span class="linenos">20</span></a>        <span class="n">nargs</span><span class="o">=</span><span class="s2">&quot;*&quot;</span><span class="p">,</span>
+</span><span id="get_args-21"><a href="#get_args-21"><span class="linenos">21</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; The name of the package or project to generate tests for,</span>
+</span><span id="get_args-22"><a href="#get_args-22"><span class="linenos">22</span></a><span class="s2">        assuming it&#39;s a subfolder of your current working directory.</span>
+</span><span id="get_args-23"><a href="#get_args-23"><span class="linenos">23</span></a><span class="s2">        Can also be a full path to the package. If nothing is given,</span>
+</span><span id="get_args-24"><a href="#get_args-24"><span class="linenos">24</span></a><span class="s2">        the current working directory will be used.</span>
+</span><span id="get_args-25"><a href="#get_args-25"><span class="linenos">25</span></a><span class="s2">        Can also be individual files.&quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="get_args-26"><a href="#get_args-26"><span class="linenos">26</span></a>    <span class="p">)</span>
+</span><span id="get_args-27"><a href="#get_args-27"><span class="linenos">27</span></a>
+</span><span id="get_args-28"><a href="#get_args-28"><span class="linenos">28</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="get_args-29"><a href="#get_args-29"><span class="linenos">29</span></a>        <span class="s2">&quot;-t&quot;</span><span class="p">,</span>
+</span><span id="get_args-30"><a href="#get_args-30"><span class="linenos">30</span></a>        <span class="s2">&quot;--tests_dir&quot;</span><span class="p">,</span>
+</span><span id="get_args-31"><a href="#get_args-31"><span class="linenos">31</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
+</span><span id="get_args-32"><a href="#get_args-32"><span class="linenos">32</span></a>        <span class="n">default</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span>
+</span><span id="get_args-33"><a href="#get_args-33"><span class="linenos">33</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; A specific tests directory path to write tests to.</span>
+</span><span id="get_args-34"><a href="#get_args-34"><span class="linenos">34</span></a><span class="s2">        When supplying individual files to paths arg, the default</span>
+</span><span id="get_args-35"><a href="#get_args-35"><span class="linenos">35</span></a><span class="s2">        behavior is to create a &#39;tests&#39; directory in the parent </span>
+</span><span id="get_args-36"><a href="#get_args-36"><span class="linenos">36</span></a><span class="s2">        directory of the specified file, resulting in multiple </span>
+</span><span id="get_args-37"><a href="#get_args-37"><span class="linenos">37</span></a><span class="s2">        &#39;tests&#39; directories being created if the files exist in</span>
+</span><span id="get_args-38"><a href="#get_args-38"><span class="linenos">38</span></a><span class="s2">        subdirectories. Supply a path to this arg to override</span>
+</span><span id="get_args-39"><a href="#get_args-39"><span class="linenos">39</span></a><span class="s2">        this behavior.&quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="get_args-40"><a href="#get_args-40"><span class="linenos">40</span></a>    <span class="p">)</span>
+</span><span id="get_args-41"><a href="#get_args-41"><span class="linenos">41</span></a>
+</span><span id="get_args-42"><a href="#get_args-42"><span class="linenos">42</span></a>    <span class="n">args</span> <span class="o">=</span> <span class="n">parser</span><span class="o">.</span><span class="n">parse_args</span><span class="p">()</span>
+</span><span id="get_args-43"><a href="#get_args-43"><span class="linenos">43</span></a>    <span class="k">return</span> <span class="n">args</span>
 </span></pre></div>
 
 
     
 
                 </section>
                 <section id="get_function_names">
@@ -250,28 +252,28 @@
         <span class="def">def</span>
         <span class="name">get_function_names</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">filepath</span><span class="p">:</span> <span class="n">pathier</span><span class="o">.</span><span class="n">pathier</span><span class="o">.</span><span class="n">Pathier</span></span><span class="return-annotation">) -> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span>:</span></span>
 
                 <label class="view-source-button" for="get_function_names-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#get_function_names"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="get_function_names-44"><a href="#get_function_names-44"><span class="linenos">44</span></a><span class="k">def</span> <span class="nf">get_function_names</span><span class="p">(</span><span class="n">filepath</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]:</span>
-</span><span id="get_function_names-45"><a href="#get_function_names-45"><span class="linenos">45</span></a>    <span class="sd">&quot;&quot;&quot;Returns a list of function names from a .py file.&quot;&quot;&quot;</span>
-</span><span id="get_function_names-46"><a href="#get_function_names-46"><span class="linenos">46</span></a>    <span class="k">with</span> <span class="n">filepath</span><span class="o">.</span><span class="n">open</span><span class="p">(</span><span class="s2">&quot;r&quot;</span><span class="p">)</span> <span class="k">as</span> <span class="n">file</span><span class="p">:</span>
-</span><span id="get_function_names-47"><a href="#get_function_names-47"><span class="linenos">47</span></a>        <span class="n">tokens</span> <span class="o">=</span> <span class="nb">list</span><span class="p">(</span><span class="n">tokenize</span><span class="o">.</span><span class="n">generate_tokens</span><span class="p">(</span><span class="n">file</span><span class="o">.</span><span class="n">readline</span><span class="p">))</span>
-</span><span id="get_function_names-48"><a href="#get_function_names-48"><span class="linenos">48</span></a>    <span class="n">functions</span> <span class="o">=</span> <span class="p">[]</span>
-</span><span id="get_function_names-49"><a href="#get_function_names-49"><span class="linenos">49</span></a>    <span class="k">for</span> <span class="n">i</span><span class="p">,</span> <span class="n">token</span> <span class="ow">in</span> <span class="nb">enumerate</span><span class="p">(</span><span class="n">tokens</span><span class="p">):</span>
-</span><span id="get_function_names-50"><a href="#get_function_names-50"><span class="linenos">50</span></a>        <span class="c1"># If token.type is &quot;name&quot; and the preceeding token is &quot;def&quot;</span>
-</span><span id="get_function_names-51"><a href="#get_function_names-51"><span class="linenos">51</span></a>        <span class="k">if</span> <span class="p">(</span>
-</span><span id="get_function_names-52"><a href="#get_function_names-52"><span class="linenos">52</span></a>            <span class="n">token</span><span class="o">.</span><span class="n">type</span> <span class="o">==</span> <span class="mi">1</span>
-</span><span id="get_function_names-53"><a href="#get_function_names-53"><span class="linenos">53</span></a>            <span class="ow">and</span> <span class="n">tokens</span><span class="p">[</span><span class="n">i</span> <span class="o">-</span> <span class="mi">1</span><span class="p">]</span><span class="o">.</span><span class="n">type</span> <span class="o">==</span> <span class="mi">1</span>
-</span><span id="get_function_names-54"><a href="#get_function_names-54"><span class="linenos">54</span></a>            <span class="ow">and</span> <span class="n">tokens</span><span class="p">[</span><span class="n">i</span> <span class="o">-</span> <span class="mi">1</span><span class="p">]</span><span class="o">.</span><span class="n">string</span> <span class="o">==</span> <span class="s2">&quot;def&quot;</span>
-</span><span id="get_function_names-55"><a href="#get_function_names-55"><span class="linenos">55</span></a>        <span class="p">):</span>
-</span><span id="get_function_names-56"><a href="#get_function_names-56"><span class="linenos">56</span></a>            <span class="n">functions</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">token</span><span class="o">.</span><span class="n">string</span><span class="p">)</span>
-</span><span id="get_function_names-57"><a href="#get_function_names-57"><span class="linenos">57</span></a>    <span class="k">return</span> <span class="n">functions</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="get_function_names-46"><a href="#get_function_names-46"><span class="linenos">46</span></a><span class="k">def</span> <span class="nf">get_function_names</span><span class="p">(</span><span class="n">filepath</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]:</span>
+</span><span id="get_function_names-47"><a href="#get_function_names-47"><span class="linenos">47</span></a>    <span class="sd">&quot;&quot;&quot;Returns a list of function names from a .py file.&quot;&quot;&quot;</span>
+</span><span id="get_function_names-48"><a href="#get_function_names-48"><span class="linenos">48</span></a>    <span class="k">with</span> <span class="n">filepath</span><span class="o">.</span><span class="n">open</span><span class="p">(</span><span class="s2">&quot;r&quot;</span><span class="p">)</span> <span class="k">as</span> <span class="n">file</span><span class="p">:</span>
+</span><span id="get_function_names-49"><a href="#get_function_names-49"><span class="linenos">49</span></a>        <span class="n">tokens</span> <span class="o">=</span> <span class="nb">list</span><span class="p">(</span><span class="n">tokenize</span><span class="o">.</span><span class="n">generate_tokens</span><span class="p">(</span><span class="n">file</span><span class="o">.</span><span class="n">readline</span><span class="p">))</span>
+</span><span id="get_function_names-50"><a href="#get_function_names-50"><span class="linenos">50</span></a>    <span class="n">functions</span> <span class="o">=</span> <span class="p">[]</span>
+</span><span id="get_function_names-51"><a href="#get_function_names-51"><span class="linenos">51</span></a>    <span class="k">for</span> <span class="n">i</span><span class="p">,</span> <span class="n">token</span> <span class="ow">in</span> <span class="nb">enumerate</span><span class="p">(</span><span class="n">tokens</span><span class="p">):</span>
+</span><span id="get_function_names-52"><a href="#get_function_names-52"><span class="linenos">52</span></a>        <span class="c1"># If token.type is &quot;name&quot; and the preceeding token is &quot;def&quot;</span>
+</span><span id="get_function_names-53"><a href="#get_function_names-53"><span class="linenos">53</span></a>        <span class="k">if</span> <span class="p">(</span>
+</span><span id="get_function_names-54"><a href="#get_function_names-54"><span class="linenos">54</span></a>            <span class="n">token</span><span class="o">.</span><span class="n">type</span> <span class="o">==</span> <span class="mi">1</span>
+</span><span id="get_function_names-55"><a href="#get_function_names-55"><span class="linenos">55</span></a>            <span class="ow">and</span> <span class="n">tokens</span><span class="p">[</span><span class="n">i</span> <span class="o">-</span> <span class="mi">1</span><span class="p">]</span><span class="o">.</span><span class="n">type</span> <span class="o">==</span> <span class="mi">1</span>
+</span><span id="get_function_names-56"><a href="#get_function_names-56"><span class="linenos">56</span></a>            <span class="ow">and</span> <span class="n">tokens</span><span class="p">[</span><span class="n">i</span> <span class="o">-</span> <span class="mi">1</span><span class="p">]</span><span class="o">.</span><span class="n">string</span> <span class="o">==</span> <span class="s2">&quot;def&quot;</span>
+</span><span id="get_function_names-57"><a href="#get_function_names-57"><span class="linenos">57</span></a>        <span class="p">):</span>
+</span><span id="get_function_names-58"><a href="#get_function_names-58"><span class="linenos">58</span></a>            <span class="n">functions</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">token</span><span class="o">.</span><span class="n">string</span><span class="p">)</span>
+</span><span id="get_function_names-59"><a href="#get_function_names-59"><span class="linenos">59</span></a>    <span class="k">return</span> <span class="n">functions</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Returns a list of function names from a .py file.</p>
 </div>
 
 
@@ -283,50 +285,50 @@
         <span class="def">def</span>
         <span class="name">write_placeholders</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="n">package_path</span><span class="p">:</span> <span class="n">pathier</span><span class="o">.</span><span class="n">pathier</span><span class="o">.</span><span class="n">Pathier</span>,</span><span class="param">	<span class="n">pyfile</span><span class="p">:</span> <span class="n">pathier</span><span class="o">.</span><span class="n">pathier</span><span class="o">.</span><span class="n">Pathier</span> <span class="o">|</span> <span class="nb">str</span>,</span><span class="param">	<span class="n">functions</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span>,</span><span class="param">	<span class="n">tests_dir</span><span class="p">:</span> <span class="n">pathier</span><span class="o">.</span><span class="n">pathier</span><span class="o">.</span><span class="n">Pathier</span> <span class="o">=</span> <span class="kc">None</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="write_placeholders-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#write_placeholders"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="write_placeholders-60"><a href="#write_placeholders-60"><span class="linenos">60</span></a><span class="k">def</span> <span class="nf">write_placeholders</span><span class="p">(</span>
-</span><span id="write_placeholders-61"><a href="#write_placeholders-61"><span class="linenos">61</span></a>    <span class="n">package_path</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">,</span>
-</span><span id="write_placeholders-62"><a href="#write_placeholders-62"><span class="linenos">62</span></a>    <span class="n">pyfile</span><span class="p">:</span> <span class="n">Pathier</span> <span class="o">|</span> <span class="nb">str</span><span class="p">,</span>
-</span><span id="write_placeholders-63"><a href="#write_placeholders-63"><span class="linenos">63</span></a>    <span class="n">functions</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">],</span>
-</span><span id="write_placeholders-64"><a href="#write_placeholders-64"><span class="linenos">64</span></a>    <span class="n">tests_dir</span><span class="p">:</span> <span class="n">Pathier</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="write_placeholders-65"><a href="#write_placeholders-65"><span class="linenos">65</span></a><span class="p">):</span>
-</span><span id="write_placeholders-66"><a href="#write_placeholders-66"><span class="linenos">66</span></a>    <span class="sd">&quot;&quot;&quot;Write placeholder functions to the</span>
-</span><span id="write_placeholders-67"><a href="#write_placeholders-67"><span class="linenos">67</span></a><span class="sd">    tests/test_{pyfile} file if they don&#39;t already exist.</span>
-</span><span id="write_placeholders-68"><a href="#write_placeholders-68"><span class="linenos">68</span></a><span class="sd">    The placeholder functions use the naming convention</span>
-</span><span id="write_placeholders-69"><a href="#write_placeholders-69"><span class="linenos">69</span></a><span class="sd">    test_{function_name}</span>
-</span><span id="write_placeholders-70"><a href="#write_placeholders-70"><span class="linenos">70</span></a>
-</span><span id="write_placeholders-71"><a href="#write_placeholders-71"><span class="linenos">71</span></a><span class="sd">    :param package_path: Path to the package.</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="write_placeholders-62"><a href="#write_placeholders-62"><span class="linenos">62</span></a><span class="k">def</span> <span class="nf">write_placeholders</span><span class="p">(</span>
+</span><span id="write_placeholders-63"><a href="#write_placeholders-63"><span class="linenos">63</span></a>    <span class="n">package_path</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">,</span>
+</span><span id="write_placeholders-64"><a href="#write_placeholders-64"><span class="linenos">64</span></a>    <span class="n">pyfile</span><span class="p">:</span> <span class="n">Pathier</span> <span class="o">|</span> <span class="nb">str</span><span class="p">,</span>
+</span><span id="write_placeholders-65"><a href="#write_placeholders-65"><span class="linenos">65</span></a>    <span class="n">functions</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">],</span>
+</span><span id="write_placeholders-66"><a href="#write_placeholders-66"><span class="linenos">66</span></a>    <span class="n">tests_dir</span><span class="p">:</span> <span class="n">Pathier</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="write_placeholders-67"><a href="#write_placeholders-67"><span class="linenos">67</span></a><span class="p">):</span>
+</span><span id="write_placeholders-68"><a href="#write_placeholders-68"><span class="linenos">68</span></a>    <span class="sd">&quot;&quot;&quot;Write placeholder functions to the</span>
+</span><span id="write_placeholders-69"><a href="#write_placeholders-69"><span class="linenos">69</span></a><span class="sd">    tests/test_{pyfile} file if they don&#39;t already exist.</span>
+</span><span id="write_placeholders-70"><a href="#write_placeholders-70"><span class="linenos">70</span></a><span class="sd">    The placeholder functions use the naming convention</span>
+</span><span id="write_placeholders-71"><a href="#write_placeholders-71"><span class="linenos">71</span></a><span class="sd">    test_{function_name}</span>
 </span><span id="write_placeholders-72"><a href="#write_placeholders-72"><span class="linenos">72</span></a>
-</span><span id="write_placeholders-73"><a href="#write_placeholders-73"><span class="linenos">73</span></a><span class="sd">    :param pyfile: Path to the pyfile to write placeholders for.</span>
+</span><span id="write_placeholders-73"><a href="#write_placeholders-73"><span class="linenos">73</span></a><span class="sd">    :param package_path: Path to the package.</span>
 </span><span id="write_placeholders-74"><a href="#write_placeholders-74"><span class="linenos">74</span></a>
-</span><span id="write_placeholders-75"><a href="#write_placeholders-75"><span class="linenos">75</span></a><span class="sd">    :param functions: List of functions to generate</span>
-</span><span id="write_placeholders-76"><a href="#write_placeholders-76"><span class="linenos">76</span></a><span class="sd">    placehodlers for.&quot;&quot;&quot;</span>
-</span><span id="write_placeholders-77"><a href="#write_placeholders-77"><span class="linenos">77</span></a>    <span class="n">package_name</span> <span class="o">=</span> <span class="n">package_path</span><span class="o">.</span><span class="n">stem</span>
-</span><span id="write_placeholders-78"><a href="#write_placeholders-78"><span class="linenos">78</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">tests_dir</span><span class="p">:</span>
-</span><span id="write_placeholders-79"><a href="#write_placeholders-79"><span class="linenos">79</span></a>        <span class="n">tests_dir</span> <span class="o">=</span> <span class="n">package_path</span> <span class="o">/</span> <span class="s2">&quot;tests&quot;</span>
-</span><span id="write_placeholders-80"><a href="#write_placeholders-80"><span class="linenos">80</span></a>    <span class="n">tests_dir</span><span class="o">.</span><span class="n">mkdir</span><span class="p">()</span>
-</span><span id="write_placeholders-81"><a href="#write_placeholders-81"><span class="linenos">81</span></a>    <span class="n">pyfile</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="n">pyfile</span><span class="p">)</span>
-</span><span id="write_placeholders-82"><a href="#write_placeholders-82"><span class="linenos">82</span></a>    <span class="n">test_file</span> <span class="o">=</span> <span class="n">tests_dir</span> <span class="o">/</span> <span class="sa">f</span><span class="s2">&quot;test_</span><span class="si">{</span><span class="n">pyfile</span><span class="o">.</span><span class="n">name</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="write_placeholders-83"><a href="#write_placeholders-83"><span class="linenos">83</span></a>    <span class="c1"># Makes sure not to overwrite previously written tests</span>
-</span><span id="write_placeholders-84"><a href="#write_placeholders-84"><span class="linenos">84</span></a>    <span class="c1"># or additional imports.</span>
-</span><span id="write_placeholders-85"><a href="#write_placeholders-85"><span class="linenos">85</span></a>    <span class="k">if</span> <span class="n">test_file</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
-</span><span id="write_placeholders-86"><a href="#write_placeholders-86"><span class="linenos">86</span></a>        <span class="n">content</span> <span class="o">=</span> <span class="n">test_file</span><span class="o">.</span><span class="n">read_text</span><span class="p">()</span> <span class="o">+</span> <span class="s2">&quot;</span><span class="se">\n\n</span><span class="s2">&quot;</span>
-</span><span id="write_placeholders-87"><a href="#write_placeholders-87"><span class="linenos">87</span></a>    <span class="k">else</span><span class="p">:</span>
-</span><span id="write_placeholders-88"><a href="#write_placeholders-88"><span class="linenos">88</span></a>        <span class="n">content</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;import pytest</span><span class="se">\n</span><span class="s2">from </span><span class="si">{</span><span class="n">package_name</span><span class="si">}</span><span class="s2"> import </span><span class="si">{</span><span class="n">pyfile</span><span class="o">.</span><span class="n">stem</span><span class="si">}</span><span class="se">\n\n\n</span><span class="s2">&quot;</span>
-</span><span id="write_placeholders-89"><a href="#write_placeholders-89"><span class="linenos">89</span></a>    <span class="k">for</span> <span class="n">function</span> <span class="ow">in</span> <span class="n">functions</span><span class="p">:</span>
-</span><span id="write_placeholders-90"><a href="#write_placeholders-90"><span class="linenos">90</span></a>        <span class="n">test_function</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;def test_</span><span class="si">{</span><span class="n">function</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="write_placeholders-91"><a href="#write_placeholders-91"><span class="linenos">91</span></a>        <span class="k">if</span> <span class="n">test_function</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">content</span> <span class="ow">and</span> <span class="n">function</span> <span class="o">!=</span> <span class="s2">&quot;__init__&quot;</span><span class="p">:</span>
-</span><span id="write_placeholders-92"><a href="#write_placeholders-92"><span class="linenos">92</span></a>            <span class="n">content</span> <span class="o">+=</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">test_function</span><span class="si">}</span><span class="s2">():</span><span class="se">\n</span><span class="s2">    ...</span><span class="se">\n\n\n</span><span class="s2">&quot;</span>
-</span><span id="write_placeholders-93"><a href="#write_placeholders-93"><span class="linenos">93</span></a>    <span class="n">test_file</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span><span class="n">content</span><span class="p">)</span>
-</span><span id="write_placeholders-94"><a href="#write_placeholders-94"><span class="linenos">94</span></a>    <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;black </span><span class="si">{</span><span class="n">tests_dir</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="write_placeholders-95"><a href="#write_placeholders-95"><span class="linenos">95</span></a>    <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;isort </span><span class="si">{</span><span class="n">tests_dir</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="write_placeholders-75"><a href="#write_placeholders-75"><span class="linenos">75</span></a><span class="sd">    :param pyfile: Path to the pyfile to write placeholders for.</span>
+</span><span id="write_placeholders-76"><a href="#write_placeholders-76"><span class="linenos">76</span></a>
+</span><span id="write_placeholders-77"><a href="#write_placeholders-77"><span class="linenos">77</span></a><span class="sd">    :param functions: List of functions to generate</span>
+</span><span id="write_placeholders-78"><a href="#write_placeholders-78"><span class="linenos">78</span></a><span class="sd">    placehodlers for.&quot;&quot;&quot;</span>
+</span><span id="write_placeholders-79"><a href="#write_placeholders-79"><span class="linenos">79</span></a>    <span class="n">package_name</span> <span class="o">=</span> <span class="n">package_path</span><span class="o">.</span><span class="n">stem</span>
+</span><span id="write_placeholders-80"><a href="#write_placeholders-80"><span class="linenos">80</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">tests_dir</span><span class="p">:</span>
+</span><span id="write_placeholders-81"><a href="#write_placeholders-81"><span class="linenos">81</span></a>        <span class="n">tests_dir</span> <span class="o">=</span> <span class="n">package_path</span> <span class="o">/</span> <span class="s2">&quot;tests&quot;</span>
+</span><span id="write_placeholders-82"><a href="#write_placeholders-82"><span class="linenos">82</span></a>    <span class="n">tests_dir</span><span class="o">.</span><span class="n">mkdir</span><span class="p">()</span>
+</span><span id="write_placeholders-83"><a href="#write_placeholders-83"><span class="linenos">83</span></a>    <span class="n">pyfile</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="n">pyfile</span><span class="p">)</span>
+</span><span id="write_placeholders-84"><a href="#write_placeholders-84"><span class="linenos">84</span></a>    <span class="n">test_file</span> <span class="o">=</span> <span class="n">tests_dir</span> <span class="o">/</span> <span class="sa">f</span><span class="s2">&quot;test_</span><span class="si">{</span><span class="n">pyfile</span><span class="o">.</span><span class="n">name</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="write_placeholders-85"><a href="#write_placeholders-85"><span class="linenos">85</span></a>    <span class="c1"># Makes sure not to overwrite previously written tests</span>
+</span><span id="write_placeholders-86"><a href="#write_placeholders-86"><span class="linenos">86</span></a>    <span class="c1"># or additional imports.</span>
+</span><span id="write_placeholders-87"><a href="#write_placeholders-87"><span class="linenos">87</span></a>    <span class="k">if</span> <span class="n">test_file</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
+</span><span id="write_placeholders-88"><a href="#write_placeholders-88"><span class="linenos">88</span></a>        <span class="n">content</span> <span class="o">=</span> <span class="n">test_file</span><span class="o">.</span><span class="n">read_text</span><span class="p">()</span> <span class="o">+</span> <span class="s2">&quot;</span><span class="se">\n\n</span><span class="s2">&quot;</span>
+</span><span id="write_placeholders-89"><a href="#write_placeholders-89"><span class="linenos">89</span></a>    <span class="k">else</span><span class="p">:</span>
+</span><span id="write_placeholders-90"><a href="#write_placeholders-90"><span class="linenos">90</span></a>        <span class="n">content</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;import pytest</span><span class="se">\n</span><span class="s2">from </span><span class="si">{</span><span class="n">package_name</span><span class="si">}</span><span class="s2"> import </span><span class="si">{</span><span class="n">pyfile</span><span class="o">.</span><span class="n">stem</span><span class="si">}</span><span class="se">\n\n\n</span><span class="s2">&quot;</span>
+</span><span id="write_placeholders-91"><a href="#write_placeholders-91"><span class="linenos">91</span></a>    <span class="k">for</span> <span class="n">function</span> <span class="ow">in</span> <span class="n">functions</span><span class="p">:</span>
+</span><span id="write_placeholders-92"><a href="#write_placeholders-92"><span class="linenos">92</span></a>        <span class="n">test_function</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;def test_</span><span class="si">{</span><span class="n">function</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="write_placeholders-93"><a href="#write_placeholders-93"><span class="linenos">93</span></a>        <span class="k">if</span> <span class="n">test_function</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">content</span> <span class="ow">and</span> <span class="n">function</span> <span class="o">!=</span> <span class="s2">&quot;__init__&quot;</span><span class="p">:</span>
+</span><span id="write_placeholders-94"><a href="#write_placeholders-94"><span class="linenos">94</span></a>            <span class="n">content</span> <span class="o">+=</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">test_function</span><span class="si">}</span><span class="s2">():</span><span class="se">\n</span><span class="s2">    ...</span><span class="se">\n\n\n</span><span class="s2">&quot;</span>
+</span><span id="write_placeholders-95"><a href="#write_placeholders-95"><span class="linenos">95</span></a>    <span class="n">test_file</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span><span class="n">content</span><span class="p">)</span>
+</span><span id="write_placeholders-96"><a href="#write_placeholders-96"><span class="linenos">96</span></a>    <span class="n">hassle_utilities</span><span class="o">.</span><span class="n">format_files</span><span class="p">(</span><span class="n">tests_dir</span><span class="p">)</span>
+</span><span id="write_placeholders-97"><a href="#write_placeholders-97"><span class="linenos">97</span></a>    <span class="p">[</span><span class="n">isort</span><span class="o">.</span><span class="n">file</span><span class="p">(</span><span class="n">path</span><span class="p">)</span> <span class="k">for</span> <span class="n">path</span> <span class="ow">in</span> <span class="n">tests_dir</span><span class="o">.</span><span class="n">rglob</span><span class="p">(</span><span class="s2">&quot;*.py&quot;</span><span class="p">)]</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Write placeholder functions to the
 tests/test_{pyfile} file if they don't already exist.
 The placeholder functions use the naming convention
 test_{function_name}</p>
@@ -350,24 +352,24 @@
         <span class="def">def</span>
         <span class="name">generate_test_files</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="n">package_path</span><span class="p">:</span> <span class="n">pathier</span><span class="o">.</span><span class="n">pathier</span><span class="o">.</span><span class="n">Pathier</span>,</span><span class="param">	<span class="n">tests_dir</span><span class="p">:</span> <span class="n">pathier</span><span class="o">.</span><span class="n">pathier</span><span class="o">.</span><span class="n">Pathier</span> <span class="o">=</span> <span class="kc">None</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="generate_test_files-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#generate_test_files"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="generate_test_files-98"><a href="#generate_test_files-98"><span class="linenos"> 98</span></a><span class="k">def</span> <span class="nf">generate_test_files</span><span class="p">(</span><span class="n">package_path</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">,</span> <span class="n">tests_dir</span><span class="p">:</span> <span class="n">Pathier</span> <span class="o">=</span> <span class="kc">None</span><span class="p">):</span>
-</span><span id="generate_test_files-99"><a href="#generate_test_files-99"><span class="linenos"> 99</span></a>    <span class="sd">&quot;&quot;&quot;Generate test files for all .py files in &#39;src&#39;</span>
-</span><span id="generate_test_files-100"><a href="#generate_test_files-100"><span class="linenos">100</span></a><span class="sd">    directory of &#39;package_path&#39;.&quot;&quot;&quot;</span>
-</span><span id="generate_test_files-101"><a href="#generate_test_files-101"><span class="linenos">101</span></a>    <span class="n">pyfiles</span> <span class="o">=</span> <span class="p">[</span>
-</span><span id="generate_test_files-102"><a href="#generate_test_files-102"><span class="linenos">102</span></a>        <span class="n">file</span>
-</span><span id="generate_test_files-103"><a href="#generate_test_files-103"><span class="linenos">103</span></a>        <span class="k">for</span> <span class="n">file</span> <span class="ow">in</span> <span class="p">(</span><span class="n">package_path</span> <span class="o">/</span> <span class="s2">&quot;src&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">rglob</span><span class="p">(</span><span class="s2">&quot;*.py&quot;</span><span class="p">)</span>
-</span><span id="generate_test_files-104"><a href="#generate_test_files-104"><span class="linenos">104</span></a>        <span class="k">if</span> <span class="n">file</span><span class="o">.</span><span class="n">name</span> <span class="o">!=</span> <span class="s2">&quot;__init__.py&quot;</span>
-</span><span id="generate_test_files-105"><a href="#generate_test_files-105"><span class="linenos">105</span></a>    <span class="p">]</span>
-</span><span id="generate_test_files-106"><a href="#generate_test_files-106"><span class="linenos">106</span></a>    <span class="k">for</span> <span class="n">pyfile</span> <span class="ow">in</span> <span class="n">pyfiles</span><span class="p">:</span>
-</span><span id="generate_test_files-107"><a href="#generate_test_files-107"><span class="linenos">107</span></a>        <span class="n">write_placeholders</span><span class="p">(</span><span class="n">package_path</span><span class="p">,</span> <span class="n">pyfile</span><span class="p">,</span> <span class="n">get_function_names</span><span class="p">(</span><span class="n">pyfile</span><span class="p">),</span> <span class="n">tests_dir</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="generate_test_files-100"><a href="#generate_test_files-100"><span class="linenos">100</span></a><span class="k">def</span> <span class="nf">generate_test_files</span><span class="p">(</span><span class="n">package_path</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">,</span> <span class="n">tests_dir</span><span class="p">:</span> <span class="n">Pathier</span> <span class="o">=</span> <span class="kc">None</span><span class="p">):</span>
+</span><span id="generate_test_files-101"><a href="#generate_test_files-101"><span class="linenos">101</span></a>    <span class="sd">&quot;&quot;&quot;Generate test files for all .py files in &#39;src&#39;</span>
+</span><span id="generate_test_files-102"><a href="#generate_test_files-102"><span class="linenos">102</span></a><span class="sd">    directory of &#39;package_path&#39;.&quot;&quot;&quot;</span>
+</span><span id="generate_test_files-103"><a href="#generate_test_files-103"><span class="linenos">103</span></a>    <span class="n">pyfiles</span> <span class="o">=</span> <span class="p">[</span>
+</span><span id="generate_test_files-104"><a href="#generate_test_files-104"><span class="linenos">104</span></a>        <span class="n">file</span>
+</span><span id="generate_test_files-105"><a href="#generate_test_files-105"><span class="linenos">105</span></a>        <span class="k">for</span> <span class="n">file</span> <span class="ow">in</span> <span class="p">(</span><span class="n">package_path</span> <span class="o">/</span> <span class="s2">&quot;src&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">rglob</span><span class="p">(</span><span class="s2">&quot;*.py&quot;</span><span class="p">)</span>
+</span><span id="generate_test_files-106"><a href="#generate_test_files-106"><span class="linenos">106</span></a>        <span class="k">if</span> <span class="n">file</span><span class="o">.</span><span class="n">name</span> <span class="o">!=</span> <span class="s2">&quot;__init__.py&quot;</span>
+</span><span id="generate_test_files-107"><a href="#generate_test_files-107"><span class="linenos">107</span></a>    <span class="p">]</span>
+</span><span id="generate_test_files-108"><a href="#generate_test_files-108"><span class="linenos">108</span></a>    <span class="k">for</span> <span class="n">pyfile</span> <span class="ow">in</span> <span class="n">pyfiles</span><span class="p">:</span>
+</span><span id="generate_test_files-109"><a href="#generate_test_files-109"><span class="linenos">109</span></a>        <span class="n">write_placeholders</span><span class="p">(</span><span class="n">package_path</span><span class="p">,</span> <span class="n">pyfile</span><span class="p">,</span> <span class="n">get_function_names</span><span class="p">(</span><span class="n">pyfile</span><span class="p">),</span> <span class="n">tests_dir</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Generate test files for all .py files in 'src'
 directory of 'package_path'.</p>
 </div>
 
@@ -380,27 +382,27 @@
         <span class="def">def</span>
         <span class="name">main</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">args</span><span class="p">:</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span> <span class="o">=</span> <span class="kc">None</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="main-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#main"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="main-110"><a href="#main-110"><span class="linenos">110</span></a><span class="k">def</span> <span class="nf">main</span><span class="p">(</span><span class="n">args</span><span class="p">:</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span> <span class="o">=</span> <span class="kc">None</span><span class="p">):</span>
-</span><span id="main-111"><a href="#main-111"><span class="linenos">111</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="p">:</span>
-</span><span id="main-112"><a href="#main-112"><span class="linenos">112</span></a>        <span class="n">args</span> <span class="o">=</span> <span class="n">get_args</span><span class="p">()</span>
-</span><span id="main-113"><a href="#main-113"><span class="linenos">113</span></a>    <span class="n">args</span><span class="o">.</span><span class="n">paths</span> <span class="o">=</span> <span class="p">[</span><span class="n">Pathier</span><span class="p">(</span><span class="n">path</span><span class="p">)</span><span class="o">.</span><span class="n">resolve</span><span class="p">()</span> <span class="k">for</span> <span class="n">path</span> <span class="ow">in</span> <span class="n">args</span><span class="o">.</span><span class="n">paths</span><span class="p">]</span>
-</span><span id="main-114"><a href="#main-114"><span class="linenos">114</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">tests_dir</span><span class="p">:</span>
-</span><span id="main-115"><a href="#main-115"><span class="linenos">115</span></a>        <span class="n">args</span><span class="o">.</span><span class="n">tests_dir</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">tests_dir</span><span class="p">)</span><span class="o">.</span><span class="n">resolve</span><span class="p">()</span>
-</span><span id="main-116"><a href="#main-116"><span class="linenos">116</span></a>    <span class="k">for</span> <span class="n">path</span> <span class="ow">in</span> <span class="n">args</span><span class="o">.</span><span class="n">paths</span><span class="p">:</span>
-</span><span id="main-117"><a href="#main-117"><span class="linenos">117</span></a>        <span class="k">if</span> <span class="n">path</span><span class="o">.</span><span class="n">is_dir</span><span class="p">():</span>
-</span><span id="main-118"><a href="#main-118"><span class="linenos">118</span></a>            <span class="n">generate_test_files</span><span class="p">(</span><span class="n">path</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">tests_dir</span><span class="p">)</span>
-</span><span id="main-119"><a href="#main-119"><span class="linenos">119</span></a>        <span class="k">elif</span> <span class="n">path</span><span class="o">.</span><span class="n">is_file</span><span class="p">():</span>
-</span><span id="main-120"><a href="#main-120"><span class="linenos">120</span></a>            <span class="n">write_placeholders</span><span class="p">(</span>
-</span><span id="main-121"><a href="#main-121"><span class="linenos">121</span></a>                <span class="n">path</span><span class="o">.</span><span class="n">parent</span><span class="p">,</span> <span class="n">path</span><span class="p">,</span> <span class="n">get_function_names</span><span class="p">(</span><span class="n">path</span><span class="p">),</span> <span class="n">args</span><span class="o">.</span><span class="n">tests_dir</span>
-</span><span id="main-122"><a href="#main-122"><span class="linenos">122</span></a>            <span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="main-112"><a href="#main-112"><span class="linenos">112</span></a><span class="k">def</span> <span class="nf">main</span><span class="p">(</span><span class="n">args</span><span class="p">:</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span> <span class="o">=</span> <span class="kc">None</span><span class="p">):</span>
+</span><span id="main-113"><a href="#main-113"><span class="linenos">113</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="p">:</span>
+</span><span id="main-114"><a href="#main-114"><span class="linenos">114</span></a>        <span class="n">args</span> <span class="o">=</span> <span class="n">get_args</span><span class="p">()</span>
+</span><span id="main-115"><a href="#main-115"><span class="linenos">115</span></a>    <span class="n">args</span><span class="o">.</span><span class="n">paths</span> <span class="o">=</span> <span class="p">[</span><span class="n">Pathier</span><span class="p">(</span><span class="n">path</span><span class="p">)</span><span class="o">.</span><span class="n">resolve</span><span class="p">()</span> <span class="k">for</span> <span class="n">path</span> <span class="ow">in</span> <span class="n">args</span><span class="o">.</span><span class="n">paths</span><span class="p">]</span>
+</span><span id="main-116"><a href="#main-116"><span class="linenos">116</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">tests_dir</span><span class="p">:</span>
+</span><span id="main-117"><a href="#main-117"><span class="linenos">117</span></a>        <span class="n">args</span><span class="o">.</span><span class="n">tests_dir</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">tests_dir</span><span class="p">)</span><span class="o">.</span><span class="n">resolve</span><span class="p">()</span>
+</span><span id="main-118"><a href="#main-118"><span class="linenos">118</span></a>    <span class="k">for</span> <span class="n">path</span> <span class="ow">in</span> <span class="n">args</span><span class="o">.</span><span class="n">paths</span><span class="p">:</span>
+</span><span id="main-119"><a href="#main-119"><span class="linenos">119</span></a>        <span class="k">if</span> <span class="n">path</span><span class="o">.</span><span class="n">is_dir</span><span class="p">():</span>
+</span><span id="main-120"><a href="#main-120"><span class="linenos">120</span></a>            <span class="n">generate_test_files</span><span class="p">(</span><span class="n">path</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">tests_dir</span><span class="p">)</span>
+</span><span id="main-121"><a href="#main-121"><span class="linenos">121</span></a>        <span class="k">elif</span> <span class="n">path</span><span class="o">.</span><span class="n">is_file</span><span class="p">():</span>
+</span><span id="main-122"><a href="#main-122"><span class="linenos">122</span></a>            <span class="n">write_placeholders</span><span class="p">(</span>
+</span><span id="main-123"><a href="#main-123"><span class="linenos">123</span></a>                <span class="n">path</span><span class="o">.</span><span class="n">parent</span><span class="p">,</span> <span class="n">path</span><span class="p">,</span> <span class="n">get_function_names</span><span class="p">(</span><span class="n">path</span><span class="p">),</span> <span class="n">args</span><span class="o">.</span><span class="n">tests_dir</span>
+</span><span id="main-124"><a href="#main-124"><span class="linenos">124</span></a>            <span class="p">)</span>
 </span></pre></div>
 
 
     
 
                 </section>
     </main>
```

#### html2text {}

```diff
@@ -9,266 +9,268 @@
     * generate_test_files
     * main
 built_with_pdoc[pdoc_logo]
 
 ****** hassle.generate_tests ******
 ⁰ View Source
 __1import argparse
-__2import os
-__3import tokenize
-__4
+__2import tokenize
+__3
+__4import isort
 __5from pathier import Pathier
 __6
-__7root = Pathier(__file__).parent
+__7from hassle import hassle_utilities
 __8
-__9
-_10def get_args() -> argparse.Namespace:
-_11    parser = argparse.ArgumentParser()
-_12
-_13    parser.add_argument(
-_14        "paths",
-_15        type=str,
-_16        default=".",
-_17        nargs="*",
-_18        help=""" The name of the package or project to generate tests for,
-_19        assuming it's a subfolder of your current working directory.
-_20        Can also be a full path to the package. If nothing is given,
-_21        the current working directory will be used.
-_22        Can also be individual files.""",
-_23    )
-_24
-_25    parser.add_argument(
-_26        "-t",
-_27        "--tests_dir",
-_28        type=str,
-_29        default=None,
-_30        help=""" A specific tests directory path to write tests to.
-_31        When supplying individual files to paths arg, the default
-_32        behavior is to create a 'tests' directory in the parent
-_33        directory of the specified file, resulting in multiple
-_34        'tests' directories being created if the files exist in
-_35        subdirectories. Supply a path to this arg to override
-_36        this behavior.""",
-_37    )
-_38
-_39    args = parser.parse_args()
-_40    return args
-_41
-_42
-_43def get_function_names(filepath: Pathier) -> list[str]:
-_44    """Returns a list of function names from a .py file."""
-_45    with filepath.open("r") as file:
-_46        tokens = list(tokenize.generate_tokens(file.readline))
-_47    functions = []
-_48    for i, token in enumerate(tokens):
-_49        # If token.type is "name" and the preceeding token is "def"
-_50        if (
-_51            token.type == 1
-_52            and tokens[i - 1].type == 1
-_53            and tokens[i - 1].string == "def"
-_54        ):
-_55            functions.append(token.string)
-_56    return functions
-_57
-_58
-_59def write_placeholders(
-_60    package_path: Pathier,
-_61    pyfile: Pathier | str,
-_62    functions: list[str],
-_63    tests_dir: Pathier = None,
-_64):
-_65    """Write placeholder functions to the
-_66    tests/test_{pyfile} file if they don't already exist.
-_67    The placeholder functions use the naming convention
-_68    test_{function_name}
-_69
-_70    :param package_path: Path to the package.
+__9root = Pathier(__file__).parent
+_10
+_11
+_12def get_args() -> argparse.Namespace:
+_13    parser = argparse.ArgumentParser()
+_14
+_15    parser.add_argument(
+_16        "paths",
+_17        type=str,
+_18        default=".",
+_19        nargs="*",
+_20        help=""" The name of the package or project to generate tests for,
+_21        assuming it's a subfolder of your current working directory.
+_22        Can also be a full path to the package. If nothing is given,
+_23        the current working directory will be used.
+_24        Can also be individual files.""",
+_25    )
+_26
+_27    parser.add_argument(
+_28        "-t",
+_29        "--tests_dir",
+_30        type=str,
+_31        default=None,
+_32        help=""" A specific tests directory path to write tests to.
+_33        When supplying individual files to paths arg, the default
+_34        behavior is to create a 'tests' directory in the parent
+_35        directory of the specified file, resulting in multiple
+_36        'tests' directories being created if the files exist in
+_37        subdirectories. Supply a path to this arg to override
+_38        this behavior.""",
+_39    )
+_40
+_41    args = parser.parse_args()
+_42    return args
+_43
+_44
+_45def get_function_names(filepath: Pathier) -> list[str]:
+_46    """Returns a list of function names from a .py file."""
+_47    with filepath.open("r") as file:
+_48        tokens = list(tokenize.generate_tokens(file.readline))
+_49    functions = []
+_50    for i, token in enumerate(tokens):
+_51        # If token.type is "name" and the preceeding token is "def"
+_52        if (
+_53            token.type == 1
+_54            and tokens[i - 1].type == 1
+_55            and tokens[i - 1].string == "def"
+_56        ):
+_57            functions.append(token.string)
+_58    return functions
+_59
+_60
+_61def write_placeholders(
+_62    package_path: Pathier,
+_63    pyfile: Pathier | str,
+_64    functions: list[str],
+_65    tests_dir: Pathier = None,
+_66):
+_67    """Write placeholder functions to the
+_68    tests/test_{pyfile} file if they don't already exist.
+_69    The placeholder functions use the naming convention
+_70    test_{function_name}
 _71
-_72    :param pyfile: Path to the pyfile to write placeholders for.
+_72    :param package_path: Path to the package.
 _73
-_74    :param functions: List of functions to generate
-_75    placehodlers for."""
-_76    package_name = package_path.stem
-_77    if not tests_dir:
-_78        tests_dir = package_path / "tests"
-_79    tests_dir.mkdir()
-_80    pyfile = Pathier(pyfile)
-_81    test_file = tests_dir / f"test_{pyfile.name}"
-_82    # Makes sure not to overwrite previously written tests
-_83    # or additional imports.
-_84    if test_file.exists():
-_85        content = test_file.read_text() + "\n\n"
-_86    else:
-_87        content = f"import pytest\nfrom {package_name} import
+_74    :param pyfile: Path to the pyfile to write placeholders for.
+_75
+_76    :param functions: List of functions to generate
+_77    placehodlers for."""
+_78    package_name = package_path.stem
+_79    if not tests_dir:
+_80        tests_dir = package_path / "tests"
+_81    tests_dir.mkdir()
+_82    pyfile = Pathier(pyfile)
+_83    test_file = tests_dir / f"test_{pyfile.name}"
+_84    # Makes sure not to overwrite previously written tests
+_85    # or additional imports.
+_86    if test_file.exists():
+_87        content = test_file.read_text() + "\n\n"
+_88    else:
+_89        content = f"import pytest\nfrom {package_name} import
 {pyfile.stem}\n\n\n"
-_88    for function in functions:
-_89        test_function = f"def test_{function}"
-_90        if test_function not in content and function != "__init__":
-_91            content += f"{test_function}():\n    ...\n\n\n"
-_92    test_file.write_text(content)
-_93    os.system(f"black {tests_dir}")
-_94    os.system(f"isort {tests_dir}")
-_95
-_96
-_97def generate_test_files(package_path: Pathier, tests_dir: Pathier = None):
-_98    """Generate test files for all .py files in 'src'
-_99    directory of 'package_path'."""
-100    pyfiles = [
-101        file
-102        for file in (package_path / "src").rglob("*.py")
-103        if file.name != "__init__.py"
-104    ]
-105    for pyfile in pyfiles:
-106        write_placeholders(package_path, pyfile, get_function_names(pyfile),
+_90    for function in functions:
+_91        test_function = f"def test_{function}"
+_92        if test_function not in content and function != "__init__":
+_93            content += f"{test_function}():\n    ...\n\n\n"
+_94    test_file.write_text(content)
+_95    hassle_utilities.format_files(tests_dir)
+_96    [isort.file(path) for path in tests_dir.rglob("*.py")]
+_97
+_98
+_99def generate_test_files(package_path: Pathier, tests_dir: Pathier = None):
+100    """Generate test files for all .py files in 'src'
+101    directory of 'package_path'."""
+102    pyfiles = [
+103        file
+104        for file in (package_path / "src").rglob("*.py")
+105        if file.name != "__init__.py"
+106    ]
+107    for pyfile in pyfiles:
+108        write_placeholders(package_path, pyfile, get_function_names(pyfile),
 tests_dir)
-107
-108
-109def main(args: argparse.Namespace = None):
-110    if not args:
-111        args = get_args()
-112    args.paths = [Pathier(path).resolve() for path in args.paths]
-113    if args.tests_dir:
-114        args.tests_dir = Pathier(args.tests_dir).resolve()
-115    for path in args.paths:
-116        if path.is_dir():
-117            generate_test_files(path, args.tests_dir)
-118        elif path.is_file():
-119            write_placeholders(
-120                path.parent, path, get_function_names(path), args.tests_dir
-121            )
-122
-123
-124if __name__ == "__main__":
-125    main(get_args())
+109
+110
+111def main(args: argparse.Namespace = None):
+112    if not args:
+113        args = get_args()
+114    args.paths = [Pathier(path).resolve() for path in args.paths]
+115    if args.tests_dir:
+116        args.tests_dir = Pathier(args.tests_dir).resolve()
+117    for path in args.paths:
+118        if path.is_dir():
+119            generate_test_files(path, args.tests_dir)
+120        elif path.is_file():
+121            write_placeholders(
+122                path.parent, path, get_function_names(path), args.tests_dir
+123            )
+124
+125
+126if __name__ == "__main__":
+127    main(get_args())
   ⁰
 def get_args() -> argparse.Namespace: View Source
-11def get_args() -> argparse.Namespace:
-12    parser = argparse.ArgumentParser()
-13
-14    parser.add_argument(
-15        "paths",
-16        type=str,
-17        default=".",
-18        nargs="*",
-19        help=""" The name of the package or project to generate tests for,
-20        assuming it's a subfolder of your current working directory.
-21        Can also be a full path to the package. If nothing is given,
-22        the current working directory will be used.
-23        Can also be individual files.""",
-24    )
-25
-26    parser.add_argument(
-27        "-t",
-28        "--tests_dir",
-29        type=str,
-30        default=None,
-31        help=""" A specific tests directory path to write tests to.
-32        When supplying individual files to paths arg, the default
-33        behavior is to create a 'tests' directory in the parent
-34        directory of the specified file, resulting in multiple
-35        'tests' directories being created if the files exist in
-36        subdirectories. Supply a path to this arg to override
-37        this behavior.""",
-38    )
-39
-40    args = parser.parse_args()
-41    return args
+13def get_args() -> argparse.Namespace:
+14    parser = argparse.ArgumentParser()
+15
+16    parser.add_argument(
+17        "paths",
+18        type=str,
+19        default=".",
+20        nargs="*",
+21        help=""" The name of the package or project to generate tests for,
+22        assuming it's a subfolder of your current working directory.
+23        Can also be a full path to the package. If nothing is given,
+24        the current working directory will be used.
+25        Can also be individual files.""",
+26    )
+27
+28    parser.add_argument(
+29        "-t",
+30        "--tests_dir",
+31        type=str,
+32        default=None,
+33        help=""" A specific tests directory path to write tests to.
+34        When supplying individual files to paths arg, the default
+35        behavior is to create a 'tests' directory in the parent
+36        directory of the specified file, resulting in multiple
+37        'tests' directories being created if the files exist in
+38        subdirectories. Supply a path to this arg to override
+39        this behavior.""",
+40    )
+41
+42    args = parser.parse_args()
+43    return args
   ⁰
 def get_function_names(filepath: pathier.pathier.Pathier) -> list[str]: View
 Source
-44def get_function_names(filepath: Pathier) -> list[str]:
-45    """Returns a list of function names from a .py file."""
-46    with filepath.open("r") as file:
-47        tokens = list(tokenize.generate_tokens(file.readline))
-48    functions = []
-49    for i, token in enumerate(tokens):
-50        # If token.type is "name" and the preceeding token is "def"
-51        if (
-52            token.type == 1
-53            and tokens[i - 1].type == 1
-54            and tokens[i - 1].string == "def"
-55        ):
-56            functions.append(token.string)
-57    return functions
+46def get_function_names(filepath: Pathier) -> list[str]:
+47    """Returns a list of function names from a .py file."""
+48    with filepath.open("r") as file:
+49        tokens = list(tokenize.generate_tokens(file.readline))
+50    functions = []
+51    for i, token in enumerate(tokens):
+52        # If token.type is "name" and the preceeding token is "def"
+53        if (
+54            token.type == 1
+55            and tokens[i - 1].type == 1
+56            and tokens[i - 1].string == "def"
+57        ):
+58            functions.append(token.string)
+59    return functions
 Returns a list of function names from a .py file.
   ⁰
 def write_placeholders(
 package_path: pathier.pathier.Pathier,
 pyfile: pathier.pathier.Pathier | str,
 functions: list[str],
 tests_dir: pathier.pathier.Pathier = None): View Source
-60def write_placeholders(
-61    package_path: Pathier,
-62    pyfile: Pathier | str,
-63    functions: list[str],
-64    tests_dir: Pathier = None,
-65):
-66    """Write placeholder functions to the
-67    tests/test_{pyfile} file if they don't already exist.
-68    The placeholder functions use the naming convention
-69    test_{function_name}
-70
-71    :param package_path: Path to the package.
+62def write_placeholders(
+63    package_path: Pathier,
+64    pyfile: Pathier | str,
+65    functions: list[str],
+66    tests_dir: Pathier = None,
+67):
+68    """Write placeholder functions to the
+69    tests/test_{pyfile} file if they don't already exist.
+70    The placeholder functions use the naming convention
+71    test_{function_name}
 72
-73    :param pyfile: Path to the pyfile to write placeholders for.
+73    :param package_path: Path to the package.
 74
-75    :param functions: List of functions to generate
-76    placehodlers for."""
-77    package_name = package_path.stem
-78    if not tests_dir:
-79        tests_dir = package_path / "tests"
-80    tests_dir.mkdir()
-81    pyfile = Pathier(pyfile)
-82    test_file = tests_dir / f"test_{pyfile.name}"
-83    # Makes sure not to overwrite previously written tests
-84    # or additional imports.
-85    if test_file.exists():
-86        content = test_file.read_text() + "\n\n"
-87    else:
-88        content = f"import pytest\nfrom {package_name} import
+75    :param pyfile: Path to the pyfile to write placeholders for.
+76
+77    :param functions: List of functions to generate
+78    placehodlers for."""
+79    package_name = package_path.stem
+80    if not tests_dir:
+81        tests_dir = package_path / "tests"
+82    tests_dir.mkdir()
+83    pyfile = Pathier(pyfile)
+84    test_file = tests_dir / f"test_{pyfile.name}"
+85    # Makes sure not to overwrite previously written tests
+86    # or additional imports.
+87    if test_file.exists():
+88        content = test_file.read_text() + "\n\n"
+89    else:
+90        content = f"import pytest\nfrom {package_name} import
 {pyfile.stem}\n\n\n"
-89    for function in functions:
-90        test_function = f"def test_{function}"
-91        if test_function not in content and function != "__init__":
-92            content += f"{test_function}():\n    ...\n\n\n"
-93    test_file.write_text(content)
-94    os.system(f"black {tests_dir}")
-95    os.system(f"isort {tests_dir}")
+91    for function in functions:
+92        test_function = f"def test_{function}"
+93        if test_function not in content and function != "__init__":
+94            content += f"{test_function}():\n    ...\n\n\n"
+95    test_file.write_text(content)
+96    hassle_utilities.format_files(tests_dir)
+97    [isort.file(path) for path in tests_dir.rglob("*.py")]
 Write placeholder functions to the tests/test_{pyfile} file if they don't
 already exist. The placeholder functions use the naming convention test_
 {function_name}
 * Parameters *
     * package_path: Path to the package.
     * pyfile: Path to the pyfile to write placeholders for.
     * functions: List of functions to generate placehodlers for.
   ⁰
 def generate_test_files(
 package_path: pathier.pathier.Pathier,
 tests_dir: pathier.pathier.Pathier = None): View Source
-_98def generate_test_files(package_path: Pathier, tests_dir: Pathier = None):
-_99    """Generate test files for all .py files in 'src'
-100    directory of 'package_path'."""
-101    pyfiles = [
-102        file
-103        for file in (package_path / "src").rglob("*.py")
-104        if file.name != "__init__.py"
-105    ]
-106    for pyfile in pyfiles:
-107        write_placeholders(package_path, pyfile, get_function_names(pyfile),
+100def generate_test_files(package_path: Pathier, tests_dir: Pathier = None):
+101    """Generate test files for all .py files in 'src'
+102    directory of 'package_path'."""
+103    pyfiles = [
+104        file
+105        for file in (package_path / "src").rglob("*.py")
+106        if file.name != "__init__.py"
+107    ]
+108    for pyfile in pyfiles:
+109        write_placeholders(package_path, pyfile, get_function_names(pyfile),
 tests_dir)
 Generate test files for all .py files in 'src' directory of 'package_path'.
   ⁰
 def main(args: argparse.Namespace = None): View Source
-110def main(args: argparse.Namespace = None):
-111    if not args:
-112        args = get_args()
-113    args.paths = [Pathier(path).resolve() for path in args.paths]
-114    if args.tests_dir:
-115        args.tests_dir = Pathier(args.tests_dir).resolve()
-116    for path in args.paths:
-117        if path.is_dir():
-118            generate_test_files(path, args.tests_dir)
-119        elif path.is_file():
-120            write_placeholders(
-121                path.parent, path, get_function_names(path), args.tests_dir
-122            )
+112def main(args: argparse.Namespace = None):
+113    if not args:
+114        args = get_args()
+115    args.paths = [Pathier(path).resolve() for path in args.paths]
+116    if args.tests_dir:
+117        args.tests_dir = Pathier(args.tests_dir).resolve()
+118    for path in args.paths:
+119        if path.is_dir():
+120            generate_test_files(path, args.tests_dir)
+121        elif path.is_file():
+122            write_placeholders(
+123                path.parent, path, get_function_names(path), args.tests_dir
+124            )
```

### Comparing `hassle-2.7.1/docs/hassle/hassle.html` & `hassle-2.8.0/docs/hassle/hassle.html`

 * *Files 3% similar despite different names*

```diff
@@ -30,14 +30,17 @@
 
         <h2>API Documentation</h2>
             <ul class="memberlist">
             <li>
                     <a class="function" href="#get_args">get_args</a>
             </li>
             <li>
+                    <a class="function" href="#build">build</a>
+            </li>
+            <li>
                     <a class="function" href="#main">main</a>
             </li>
     </ul>
 
 
 
         <a class="attribution" title="pdoc: Python API documentation generator" href="https://pdoc.dev" target="_blank">
@@ -55,241 +58,271 @@
                 
                         <input id="mod-hassle-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 
                         <label class="view-source-button" for="mod-hassle-view-source"><span>View Source</span></label>
 
                         <div class="pdoc-code codehilite"><pre><span></span><span id="L-1"><a href="#L-1"><span class="linenos">  1</span></a><span class="kn">import</span> <span class="nn">argparse</span>
 </span><span id="L-2"><a href="#L-2"><span class="linenos">  2</span></a><span class="kn">import</span> <span class="nn">os</span>
-</span><span id="L-3"><a href="#L-3"><span class="linenos">  3</span></a>
-</span><span id="L-4"><a href="#L-4"><span class="linenos">  4</span></a><span class="kn">from</span> <span class="nn">pathier</span> <span class="kn">import</span> <span class="n">Pathier</span>
-</span><span id="L-5"><a href="#L-5"><span class="linenos">  5</span></a>
-</span><span id="L-6"><a href="#L-6"><span class="linenos">  6</span></a><span class="kn">from</span> <span class="nn">hassle</span> <span class="kn">import</span> <span class="n">hassle_utilities</span>
-</span><span id="L-7"><a href="#L-7"><span class="linenos">  7</span></a><span class="kn">from</span> <span class="nn">hassle.generate_tests</span> <span class="kn">import</span> <span class="n">generate_test_files</span>
-</span><span id="L-8"><a href="#L-8"><span class="linenos">  8</span></a><span class="kn">from</span> <span class="nn">hassle.run_tests</span> <span class="kn">import</span> <span class="n">run_tests</span>
-</span><span id="L-9"><a href="#L-9"><span class="linenos">  9</span></a>
-</span><span id="L-10"><a href="#L-10"><span class="linenos"> 10</span></a><span class="n">root</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="vm">__file__</span><span class="p">)</span><span class="o">.</span><span class="n">parent</span>
-</span><span id="L-11"><a href="#L-11"><span class="linenos"> 11</span></a>
+</span><span id="L-3"><a href="#L-3"><span class="linenos">  3</span></a><span class="kn">import</span> <span class="nn">sys</span>
+</span><span id="L-4"><a href="#L-4"><span class="linenos">  4</span></a>
+</span><span id="L-5"><a href="#L-5"><span class="linenos">  5</span></a><span class="kn">import</span> <span class="nn">isort</span>
+</span><span id="L-6"><a href="#L-6"><span class="linenos">  6</span></a><span class="kn">from</span> <span class="nn">gitbetter</span> <span class="kn">import</span> <span class="n">git</span>
+</span><span id="L-7"><a href="#L-7"><span class="linenos">  7</span></a><span class="kn">from</span> <span class="nn">pathier</span> <span class="kn">import</span> <span class="n">Pathier</span>
+</span><span id="L-8"><a href="#L-8"><span class="linenos">  8</span></a>
+</span><span id="L-9"><a href="#L-9"><span class="linenos">  9</span></a><span class="kn">from</span> <span class="nn">hassle</span> <span class="kn">import</span> <span class="n">hassle_utilities</span>
+</span><span id="L-10"><a href="#L-10"><span class="linenos"> 10</span></a><span class="kn">from</span> <span class="nn">hassle.generate_tests</span> <span class="kn">import</span> <span class="n">generate_test_files</span>
+</span><span id="L-11"><a href="#L-11"><span class="linenos"> 11</span></a><span class="kn">from</span> <span class="nn">hassle.run_tests</span> <span class="kn">import</span> <span class="n">run_tests</span>
 </span><span id="L-12"><a href="#L-12"><span class="linenos"> 12</span></a>
-</span><span id="L-13"><a href="#L-13"><span class="linenos"> 13</span></a><span class="k">def</span> <span class="nf">get_args</span><span class="p">()</span> <span class="o">-&gt;</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span><span class="p">:</span>
-</span><span id="L-14"><a href="#L-14"><span class="linenos"> 14</span></a>    <span class="n">parser</span> <span class="o">=</span> <span class="n">argparse</span><span class="o">.</span><span class="n">ArgumentParser</span><span class="p">()</span>
+</span><span id="L-13"><a href="#L-13"><span class="linenos"> 13</span></a><span class="n">root</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="vm">__file__</span><span class="p">)</span><span class="o">.</span><span class="n">parent</span>
+</span><span id="L-14"><a href="#L-14"><span class="linenos"> 14</span></a>
 </span><span id="L-15"><a href="#L-15"><span class="linenos"> 15</span></a>
-</span><span id="L-16"><a href="#L-16"><span class="linenos"> 16</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="L-17"><a href="#L-17"><span class="linenos"> 17</span></a>        <span class="s2">&quot;package&quot;</span><span class="p">,</span>
-</span><span id="L-18"><a href="#L-18"><span class="linenos"> 18</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
-</span><span id="L-19"><a href="#L-19"><span class="linenos"> 19</span></a>        <span class="n">default</span><span class="o">=</span><span class="s2">&quot;.&quot;</span><span class="p">,</span>
-</span><span id="L-20"><a href="#L-20"><span class="linenos"> 20</span></a>        <span class="n">nargs</span><span class="o">=</span><span class="s2">&quot;?&quot;</span><span class="p">,</span>
-</span><span id="L-21"><a href="#L-21"><span class="linenos"> 21</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; The name of the package or project to use,</span>
-</span><span id="L-22"><a href="#L-22"><span class="linenos"> 22</span></a><span class="s2">        assuming it&#39;s a subfolder of your current working directory.</span>
-</span><span id="L-23"><a href="#L-23"><span class="linenos"> 23</span></a><span class="s2">        Can also be a full path to the package. If nothing is given,</span>
-</span><span id="L-24"><a href="#L-24"><span class="linenos"> 24</span></a><span class="s2">        the current working directory will be used.&quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="L-25"><a href="#L-25"><span class="linenos"> 25</span></a>    <span class="p">)</span>
-</span><span id="L-26"><a href="#L-26"><span class="linenos"> 26</span></a>
-</span><span id="L-27"><a href="#L-27"><span class="linenos"> 27</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="L-28"><a href="#L-28"><span class="linenos"> 28</span></a>        <span class="s2">&quot;-b&quot;</span><span class="p">,</span> <span class="s2">&quot;--build&quot;</span><span class="p">,</span> <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span> <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Build the package. &quot;&quot;&quot;</span>
-</span><span id="L-29"><a href="#L-29"><span class="linenos"> 29</span></a>    <span class="p">)</span>
-</span><span id="L-30"><a href="#L-30"><span class="linenos"> 30</span></a>
-</span><span id="L-31"><a href="#L-31"><span class="linenos"> 31</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="L-32"><a href="#L-32"><span class="linenos"> 32</span></a>        <span class="s2">&quot;-t&quot;</span><span class="p">,</span>
-</span><span id="L-33"><a href="#L-33"><span class="linenos"> 33</span></a>        <span class="s2">&quot;--tag_version&quot;</span><span class="p">,</span>
-</span><span id="L-34"><a href="#L-34"><span class="linenos"> 34</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
-</span><span id="L-35"><a href="#L-35"><span class="linenos"> 35</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Add a git tag corresponding to the version in pyproject.toml. &quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="L-36"><a href="#L-36"><span class="linenos"> 36</span></a>    <span class="p">)</span>
-</span><span id="L-37"><a href="#L-37"><span class="linenos"> 37</span></a>
-</span><span id="L-38"><a href="#L-38"><span class="linenos"> 38</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="L-39"><a href="#L-39"><span class="linenos"> 39</span></a>        <span class="s2">&quot;-i&quot;</span><span class="p">,</span>
-</span><span id="L-40"><a href="#L-40"><span class="linenos"> 40</span></a>        <span class="s2">&quot;--install&quot;</span><span class="p">,</span>
-</span><span id="L-41"><a href="#L-41"><span class="linenos"> 41</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
-</span><span id="L-42"><a href="#L-42"><span class="linenos"> 42</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Install the package from source. &quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="L-43"><a href="#L-43"><span class="linenos"> 43</span></a>    <span class="p">)</span>
-</span><span id="L-44"><a href="#L-44"><span class="linenos"> 44</span></a>
-</span><span id="L-45"><a href="#L-45"><span class="linenos"> 45</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="L-46"><a href="#L-46"><span class="linenos"> 46</span></a>        <span class="s2">&quot;-iv&quot;</span><span class="p">,</span>
-</span><span id="L-47"><a href="#L-47"><span class="linenos"> 47</span></a>        <span class="s2">&quot;--increment_version&quot;</span><span class="p">,</span>
-</span><span id="L-48"><a href="#L-48"><span class="linenos"> 48</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
-</span><span id="L-49"><a href="#L-49"><span class="linenos"> 49</span></a>        <span class="n">default</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span>
-</span><span id="L-50"><a href="#L-50"><span class="linenos"> 50</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Increment version in pyproject.toml.</span>
-</span><span id="L-51"><a href="#L-51"><span class="linenos"> 51</span></a><span class="s2">        Can be one of &quot;major&quot;, &quot;minor&quot;, or &quot;patch&quot;. &quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="L-52"><a href="#L-52"><span class="linenos"> 52</span></a>    <span class="p">)</span>
-</span><span id="L-53"><a href="#L-53"><span class="linenos"> 53</span></a>
-</span><span id="L-54"><a href="#L-54"><span class="linenos"> 54</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="L-55"><a href="#L-55"><span class="linenos"> 55</span></a>        <span class="s2">&quot;-p&quot;</span><span class="p">,</span>
-</span><span id="L-56"><a href="#L-56"><span class="linenos"> 56</span></a>        <span class="s2">&quot;--publish&quot;</span><span class="p">,</span>
-</span><span id="L-57"><a href="#L-57"><span class="linenos"> 57</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
-</span><span id="L-58"><a href="#L-58"><span class="linenos"> 58</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Publish package to PyPi.</span>
-</span><span id="L-59"><a href="#L-59"><span class="linenos"> 59</span></a><span class="s2">        Note: You must have configured twine </span>
-</span><span id="L-60"><a href="#L-60"><span class="linenos"> 60</span></a><span class="s2">        and registered a PyPi account/generated an API</span>
-</span><span id="L-61"><a href="#L-61"><span class="linenos"> 61</span></a><span class="s2">        key to use this option.&quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="L-62"><a href="#L-62"><span class="linenos"> 62</span></a>    <span class="p">)</span>
-</span><span id="L-63"><a href="#L-63"><span class="linenos"> 63</span></a>
-</span><span id="L-64"><a href="#L-64"><span class="linenos"> 64</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="L-65"><a href="#L-65"><span class="linenos"> 65</span></a>        <span class="s2">&quot;-rt&quot;</span><span class="p">,</span>
-</span><span id="L-66"><a href="#L-66"><span class="linenos"> 66</span></a>        <span class="s2">&quot;--run_tests&quot;</span><span class="p">,</span>
-</span><span id="L-67"><a href="#L-67"><span class="linenos"> 67</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
-</span><span id="L-68"><a href="#L-68"><span class="linenos"> 68</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Run tests for the package. &quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="L-69"><a href="#L-69"><span class="linenos"> 69</span></a>    <span class="p">)</span>
-</span><span id="L-70"><a href="#L-70"><span class="linenos"> 70</span></a>
-</span><span id="L-71"><a href="#L-71"><span class="linenos"> 71</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="L-72"><a href="#L-72"><span class="linenos"> 72</span></a>        <span class="s2">&quot;-gt&quot;</span><span class="p">,</span>
-</span><span id="L-73"><a href="#L-73"><span class="linenos"> 73</span></a>        <span class="s2">&quot;--generate_tests&quot;</span><span class="p">,</span>
-</span><span id="L-74"><a href="#L-74"><span class="linenos"> 74</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
-</span><span id="L-75"><a href="#L-75"><span class="linenos"> 75</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Generate tests for the package. &quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="L-76"><a href="#L-76"><span class="linenos"> 76</span></a>    <span class="p">)</span>
-</span><span id="L-77"><a href="#L-77"><span class="linenos"> 77</span></a>
-</span><span id="L-78"><a href="#L-78"><span class="linenos"> 78</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="L-79"><a href="#L-79"><span class="linenos"> 79</span></a>        <span class="s2">&quot;-uc&quot;</span><span class="p">,</span>
-</span><span id="L-80"><a href="#L-80"><span class="linenos"> 80</span></a>        <span class="s2">&quot;--update_changelog&quot;</span><span class="p">,</span>
-</span><span id="L-81"><a href="#L-81"><span class="linenos"> 81</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
-</span><span id="L-82"><a href="#L-82"><span class="linenos"> 82</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Update changelog file. &quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="L-83"><a href="#L-83"><span class="linenos"> 83</span></a>    <span class="p">)</span>
-</span><span id="L-84"><a href="#L-84"><span class="linenos"> 84</span></a>
-</span><span id="L-85"><a href="#L-85"><span class="linenos"> 85</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="L-86"><a href="#L-86"><span class="linenos"> 86</span></a>        <span class="s2">&quot;-od&quot;</span><span class="p">,</span>
-</span><span id="L-87"><a href="#L-87"><span class="linenos"> 87</span></a>        <span class="s2">&quot;--overwrite_dependencies&quot;</span><span class="p">,</span>
-</span><span id="L-88"><a href="#L-88"><span class="linenos"> 88</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
-</span><span id="L-89"><a href="#L-89"><span class="linenos"> 89</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; When building a package, packagelister will be used</span>
-</span><span id="L-90"><a href="#L-90"><span class="linenos"> 90</span></a><span class="s2">        to update the dependencies list in pyproject.toml.</span>
-</span><span id="L-91"><a href="#L-91"><span class="linenos"> 91</span></a><span class="s2">        The default behavior is to append any new dependencies to</span>
-</span><span id="L-92"><a href="#L-92"><span class="linenos"> 92</span></a><span class="s2">        the current list so as not to erase any manually added dependencies</span>
-</span><span id="L-93"><a href="#L-93"><span class="linenos"> 93</span></a><span class="s2">        that packagelister may not detect. If you don&#39;t have any manually </span>
-</span><span id="L-94"><a href="#L-94"><span class="linenos"> 94</span></a><span class="s2">        added dependencies and want to remove any dependencies that your</span>
-</span><span id="L-95"><a href="#L-95"><span class="linenos"> 95</span></a><span class="s2">        project no longer uses, pass this flag.&quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="L-96"><a href="#L-96"><span class="linenos"> 96</span></a>    <span class="p">)</span>
-</span><span id="L-97"><a href="#L-97"><span class="linenos"> 97</span></a>
-</span><span id="L-98"><a href="#L-98"><span class="linenos"> 98</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="L-99"><a href="#L-99"><span class="linenos"> 99</span></a>        <span class="s2">&quot;-ca&quot;</span><span class="p">,</span>
-</span><span id="L-100"><a href="#L-100"><span class="linenos">100</span></a>        <span class="s2">&quot;--commit_all&quot;</span><span class="p">,</span>
-</span><span id="L-101"><a href="#L-101"><span class="linenos">101</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
-</span><span id="L-102"><a href="#L-102"><span class="linenos">102</span></a>        <span class="n">default</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span>
-</span><span id="L-103"><a href="#L-103"><span class="linenos">103</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Git stage and commit all tracked files</span>
-</span><span id="L-104"><a href="#L-104"><span class="linenos">104</span></a><span class="s2">        with this supplied commit message.</span>
-</span><span id="L-105"><a href="#L-105"><span class="linenos">105</span></a><span class="s2">        If &#39;build&#39; is passed, all commits will have</span>
-</span><span id="L-106"><a href="#L-106"><span class="linenos">106</span></a><span class="s2">        message: &#39;chore: build v</span><span class="si">{current_version}</span><span class="s2">&quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="L-107"><a href="#L-107"><span class="linenos">107</span></a>    <span class="p">)</span>
-</span><span id="L-108"><a href="#L-108"><span class="linenos">108</span></a>
-</span><span id="L-109"><a href="#L-109"><span class="linenos">109</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="L-110"><a href="#L-110"><span class="linenos">110</span></a>        <span class="s2">&quot;-s&quot;</span><span class="p">,</span>
-</span><span id="L-111"><a href="#L-111"><span class="linenos">111</span></a>        <span class="s2">&quot;--sync&quot;</span><span class="p">,</span>
-</span><span id="L-112"><a href="#L-112"><span class="linenos">112</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
-</span><span id="L-113"><a href="#L-113"><span class="linenos">113</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Pull from github, then push current commit to repo. &quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="L-114"><a href="#L-114"><span class="linenos">114</span></a>    <span class="p">)</span>
-</span><span id="L-115"><a href="#L-115"><span class="linenos">115</span></a>
-</span><span id="L-116"><a href="#L-116"><span class="linenos">116</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="L-117"><a href="#L-117"><span class="linenos">117</span></a>        <span class="s2">&quot;-dv&quot;</span><span class="p">,</span>
-</span><span id="L-118"><a href="#L-118"><span class="linenos">118</span></a>        <span class="s2">&quot;--dependency_versions&quot;</span><span class="p">,</span>
-</span><span id="L-119"><a href="#L-119"><span class="linenos">119</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
-</span><span id="L-120"><a href="#L-120"><span class="linenos">120</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Include version specifiers for dependencies in</span>
-</span><span id="L-121"><a href="#L-121"><span class="linenos">121</span></a><span class="s2">        pyproject.toml.&quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="L-122"><a href="#L-122"><span class="linenos">122</span></a>    <span class="p">)</span>
-</span><span id="L-123"><a href="#L-123"><span class="linenos">123</span></a>
-</span><span id="L-124"><a href="#L-124"><span class="linenos">124</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="L-125"><a href="#L-125"><span class="linenos">125</span></a>        <span class="s2">&quot;-up&quot;</span><span class="p">,</span>
-</span><span id="L-126"><a href="#L-126"><span class="linenos">126</span></a>        <span class="s2">&quot;--update&quot;</span><span class="p">,</span>
-</span><span id="L-127"><a href="#L-127"><span class="linenos">127</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
-</span><span id="L-128"><a href="#L-128"><span class="linenos">128</span></a>        <span class="n">default</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span>
-</span><span id="L-129"><a href="#L-129"><span class="linenos">129</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Excpects one argument: &quot;major&quot;, &quot;minor&quot;, or &quot;patch&quot;.</span>
-</span><span id="L-130"><a href="#L-130"><span class="linenos">130</span></a><span class="s2">        Passing &quot;-up minor&quot; is equivalent to passing the cli string: &quot;-b -t -i -iv minor -uc -ca build -s&quot;.</span>
-</span><span id="L-131"><a href="#L-131"><span class="linenos">131</span></a><span class="s2">        To publish the updated package, the -p/--publish switch needs to be added to the cli input.&quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="L-132"><a href="#L-132"><span class="linenos">132</span></a>    <span class="p">)</span>
-</span><span id="L-133"><a href="#L-133"><span class="linenos">133</span></a>
-</span><span id="L-134"><a href="#L-134"><span class="linenos">134</span></a>    <span class="n">args</span> <span class="o">=</span> <span class="n">parser</span><span class="o">.</span><span class="n">parse_args</span><span class="p">()</span>
-</span><span id="L-135"><a href="#L-135"><span class="linenos">135</span></a>
-</span><span id="L-136"><a href="#L-136"><span class="linenos">136</span></a>    <span class="n">args</span><span class="o">.</span><span class="n">package</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="p">)</span><span class="o">.</span><span class="n">resolve</span><span class="p">()</span>
-</span><span id="L-137"><a href="#L-137"><span class="linenos">137</span></a>
-</span><span id="L-138"><a href="#L-138"><span class="linenos">138</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">update</span><span class="p">:</span>
-</span><span id="L-139"><a href="#L-139"><span class="linenos">139</span></a>        <span class="n">args</span><span class="o">.</span><span class="n">build</span> <span class="o">=</span> <span class="kc">True</span>
-</span><span id="L-140"><a href="#L-140"><span class="linenos">140</span></a>        <span class="n">args</span><span class="o">.</span><span class="n">tag_version</span> <span class="o">=</span> <span class="kc">True</span>
-</span><span id="L-141"><a href="#L-141"><span class="linenos">141</span></a>        <span class="n">args</span><span class="o">.</span><span class="n">install</span> <span class="o">=</span> <span class="kc">True</span>
-</span><span id="L-142"><a href="#L-142"><span class="linenos">142</span></a>        <span class="n">args</span><span class="o">.</span><span class="n">increment_version</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">update</span>
-</span><span id="L-143"><a href="#L-143"><span class="linenos">143</span></a>        <span class="n">args</span><span class="o">.</span><span class="n">update_changelog</span> <span class="o">=</span> <span class="kc">True</span>
-</span><span id="L-144"><a href="#L-144"><span class="linenos">144</span></a>        <span class="n">args</span><span class="o">.</span><span class="n">commit_all</span> <span class="o">=</span> <span class="s2">&quot;build&quot;</span>
-</span><span id="L-145"><a href="#L-145"><span class="linenos">145</span></a>        <span class="n">args</span><span class="o">.</span><span class="n">sync</span> <span class="o">=</span> <span class="kc">True</span>
-</span><span id="L-146"><a href="#L-146"><span class="linenos">146</span></a>
-</span><span id="L-147"><a href="#L-147"><span class="linenos">147</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">increment_version</span> <span class="ow">and</span> <span class="n">args</span><span class="o">.</span><span class="n">increment_version</span> <span class="ow">not</span> <span class="ow">in</span> <span class="p">[</span>
-</span><span id="L-148"><a href="#L-148"><span class="linenos">148</span></a>        <span class="s2">&quot;major&quot;</span><span class="p">,</span>
-</span><span id="L-149"><a href="#L-149"><span class="linenos">149</span></a>        <span class="s2">&quot;minor&quot;</span><span class="p">,</span>
-</span><span id="L-150"><a href="#L-150"><span class="linenos">150</span></a>        <span class="s2">&quot;patch&quot;</span><span class="p">,</span>
-</span><span id="L-151"><a href="#L-151"><span class="linenos">151</span></a>    <span class="p">]:</span>
-</span><span id="L-152"><a href="#L-152"><span class="linenos">152</span></a>        <span class="k">raise</span> <span class="ne">ValueError</span><span class="p">(</span>
-</span><span id="L-153"><a href="#L-153"><span class="linenos">153</span></a>            <span class="sa">f</span><span class="s2">&quot;Invalid option for -iv/--increment_version: </span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">increment_version</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="L-154"><a href="#L-154"><span class="linenos">154</span></a>        <span class="p">)</span>
-</span><span id="L-155"><a href="#L-155"><span class="linenos">155</span></a>
-</span><span id="L-156"><a href="#L-156"><span class="linenos">156</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">commit_all</span> <span class="o">==</span> <span class="s2">&quot;&quot;</span><span class="p">:</span>
-</span><span id="L-157"><a href="#L-157"><span class="linenos">157</span></a>        <span class="k">raise</span> <span class="ne">ValueError</span><span class="p">(</span><span class="s2">&quot;Commit message for args.commit_all cannot be empty.&quot;</span><span class="p">)</span>
-</span><span id="L-158"><a href="#L-158"><span class="linenos">158</span></a>
-</span><span id="L-159"><a href="#L-159"><span class="linenos">159</span></a>    <span class="k">return</span> <span class="n">args</span>
-</span><span id="L-160"><a href="#L-160"><span class="linenos">160</span></a>
-</span><span id="L-161"><a href="#L-161"><span class="linenos">161</span></a>
-</span><span id="L-162"><a href="#L-162"><span class="linenos">162</span></a><span class="k">def</span> <span class="nf">main</span><span class="p">(</span><span class="n">args</span><span class="p">:</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span> <span class="o">=</span> <span class="kc">None</span><span class="p">):</span>
-</span><span id="L-163"><a href="#L-163"><span class="linenos">163</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="p">:</span>
-</span><span id="L-164"><a href="#L-164"><span class="linenos">164</span></a>        <span class="n">args</span> <span class="o">=</span> <span class="n">get_args</span><span class="p">()</span>
+</span><span id="L-16"><a href="#L-16"><span class="linenos"> 16</span></a><span class="k">def</span> <span class="nf">get_args</span><span class="p">()</span> <span class="o">-&gt;</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span><span class="p">:</span>
+</span><span id="L-17"><a href="#L-17"><span class="linenos"> 17</span></a>    <span class="n">parser</span> <span class="o">=</span> <span class="n">argparse</span><span class="o">.</span><span class="n">ArgumentParser</span><span class="p">()</span>
+</span><span id="L-18"><a href="#L-18"><span class="linenos"> 18</span></a>
+</span><span id="L-19"><a href="#L-19"><span class="linenos"> 19</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="L-20"><a href="#L-20"><span class="linenos"> 20</span></a>        <span class="s2">&quot;package&quot;</span><span class="p">,</span>
+</span><span id="L-21"><a href="#L-21"><span class="linenos"> 21</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
+</span><span id="L-22"><a href="#L-22"><span class="linenos"> 22</span></a>        <span class="n">default</span><span class="o">=</span><span class="s2">&quot;.&quot;</span><span class="p">,</span>
+</span><span id="L-23"><a href="#L-23"><span class="linenos"> 23</span></a>        <span class="n">nargs</span><span class="o">=</span><span class="s2">&quot;?&quot;</span><span class="p">,</span>
+</span><span id="L-24"><a href="#L-24"><span class="linenos"> 24</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; The name of the package or project to use,</span>
+</span><span id="L-25"><a href="#L-25"><span class="linenos"> 25</span></a><span class="s2">        assuming it&#39;s a subfolder of your current working directory.</span>
+</span><span id="L-26"><a href="#L-26"><span class="linenos"> 26</span></a><span class="s2">        Can also be a full path to the package. If nothing is given,</span>
+</span><span id="L-27"><a href="#L-27"><span class="linenos"> 27</span></a><span class="s2">        the current working directory will be used.&quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="L-28"><a href="#L-28"><span class="linenos"> 28</span></a>    <span class="p">)</span>
+</span><span id="L-29"><a href="#L-29"><span class="linenos"> 29</span></a>
+</span><span id="L-30"><a href="#L-30"><span class="linenos"> 30</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="L-31"><a href="#L-31"><span class="linenos"> 31</span></a>        <span class="s2">&quot;-b&quot;</span><span class="p">,</span> <span class="s2">&quot;--build&quot;</span><span class="p">,</span> <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span> <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Build the package. &quot;&quot;&quot;</span>
+</span><span id="L-32"><a href="#L-32"><span class="linenos"> 32</span></a>    <span class="p">)</span>
+</span><span id="L-33"><a href="#L-33"><span class="linenos"> 33</span></a>
+</span><span id="L-34"><a href="#L-34"><span class="linenos"> 34</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="L-35"><a href="#L-35"><span class="linenos"> 35</span></a>        <span class="s2">&quot;-t&quot;</span><span class="p">,</span>
+</span><span id="L-36"><a href="#L-36"><span class="linenos"> 36</span></a>        <span class="s2">&quot;--tag_version&quot;</span><span class="p">,</span>
+</span><span id="L-37"><a href="#L-37"><span class="linenos"> 37</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
+</span><span id="L-38"><a href="#L-38"><span class="linenos"> 38</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Add a git tag corresponding to the version in pyproject.toml. &quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="L-39"><a href="#L-39"><span class="linenos"> 39</span></a>    <span class="p">)</span>
+</span><span id="L-40"><a href="#L-40"><span class="linenos"> 40</span></a>
+</span><span id="L-41"><a href="#L-41"><span class="linenos"> 41</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="L-42"><a href="#L-42"><span class="linenos"> 42</span></a>        <span class="s2">&quot;-i&quot;</span><span class="p">,</span>
+</span><span id="L-43"><a href="#L-43"><span class="linenos"> 43</span></a>        <span class="s2">&quot;--install&quot;</span><span class="p">,</span>
+</span><span id="L-44"><a href="#L-44"><span class="linenos"> 44</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
+</span><span id="L-45"><a href="#L-45"><span class="linenos"> 45</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Install the package from source. &quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="L-46"><a href="#L-46"><span class="linenos"> 46</span></a>    <span class="p">)</span>
+</span><span id="L-47"><a href="#L-47"><span class="linenos"> 47</span></a>
+</span><span id="L-48"><a href="#L-48"><span class="linenos"> 48</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="L-49"><a href="#L-49"><span class="linenos"> 49</span></a>        <span class="s2">&quot;-iv&quot;</span><span class="p">,</span>
+</span><span id="L-50"><a href="#L-50"><span class="linenos"> 50</span></a>        <span class="s2">&quot;--increment_version&quot;</span><span class="p">,</span>
+</span><span id="L-51"><a href="#L-51"><span class="linenos"> 51</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
+</span><span id="L-52"><a href="#L-52"><span class="linenos"> 52</span></a>        <span class="n">default</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span>
+</span><span id="L-53"><a href="#L-53"><span class="linenos"> 53</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Increment version in pyproject.toml.</span>
+</span><span id="L-54"><a href="#L-54"><span class="linenos"> 54</span></a><span class="s2">        Can be one of &quot;major&quot;, &quot;minor&quot;, or &quot;patch&quot;. &quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="L-55"><a href="#L-55"><span class="linenos"> 55</span></a>    <span class="p">)</span>
+</span><span id="L-56"><a href="#L-56"><span class="linenos"> 56</span></a>
+</span><span id="L-57"><a href="#L-57"><span class="linenos"> 57</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="L-58"><a href="#L-58"><span class="linenos"> 58</span></a>        <span class="s2">&quot;-p&quot;</span><span class="p">,</span>
+</span><span id="L-59"><a href="#L-59"><span class="linenos"> 59</span></a>        <span class="s2">&quot;--publish&quot;</span><span class="p">,</span>
+</span><span id="L-60"><a href="#L-60"><span class="linenos"> 60</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
+</span><span id="L-61"><a href="#L-61"><span class="linenos"> 61</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Publish package to PyPi.</span>
+</span><span id="L-62"><a href="#L-62"><span class="linenos"> 62</span></a><span class="s2">        Note: You must have configured twine </span>
+</span><span id="L-63"><a href="#L-63"><span class="linenos"> 63</span></a><span class="s2">        and registered a PyPi account/generated an API</span>
+</span><span id="L-64"><a href="#L-64"><span class="linenos"> 64</span></a><span class="s2">        key to use this option.&quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="L-65"><a href="#L-65"><span class="linenos"> 65</span></a>    <span class="p">)</span>
+</span><span id="L-66"><a href="#L-66"><span class="linenos"> 66</span></a>
+</span><span id="L-67"><a href="#L-67"><span class="linenos"> 67</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="L-68"><a href="#L-68"><span class="linenos"> 68</span></a>        <span class="s2">&quot;-rt&quot;</span><span class="p">,</span>
+</span><span id="L-69"><a href="#L-69"><span class="linenos"> 69</span></a>        <span class="s2">&quot;--run_tests&quot;</span><span class="p">,</span>
+</span><span id="L-70"><a href="#L-70"><span class="linenos"> 70</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
+</span><span id="L-71"><a href="#L-71"><span class="linenos"> 71</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Run tests for the package. &quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="L-72"><a href="#L-72"><span class="linenos"> 72</span></a>    <span class="p">)</span>
+</span><span id="L-73"><a href="#L-73"><span class="linenos"> 73</span></a>
+</span><span id="L-74"><a href="#L-74"><span class="linenos"> 74</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="L-75"><a href="#L-75"><span class="linenos"> 75</span></a>        <span class="s2">&quot;-gt&quot;</span><span class="p">,</span>
+</span><span id="L-76"><a href="#L-76"><span class="linenos"> 76</span></a>        <span class="s2">&quot;--generate_tests&quot;</span><span class="p">,</span>
+</span><span id="L-77"><a href="#L-77"><span class="linenos"> 77</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
+</span><span id="L-78"><a href="#L-78"><span class="linenos"> 78</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Generate tests for the package. &quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="L-79"><a href="#L-79"><span class="linenos"> 79</span></a>    <span class="p">)</span>
+</span><span id="L-80"><a href="#L-80"><span class="linenos"> 80</span></a>
+</span><span id="L-81"><a href="#L-81"><span class="linenos"> 81</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="L-82"><a href="#L-82"><span class="linenos"> 82</span></a>        <span class="s2">&quot;-uc&quot;</span><span class="p">,</span>
+</span><span id="L-83"><a href="#L-83"><span class="linenos"> 83</span></a>        <span class="s2">&quot;--update_changelog&quot;</span><span class="p">,</span>
+</span><span id="L-84"><a href="#L-84"><span class="linenos"> 84</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
+</span><span id="L-85"><a href="#L-85"><span class="linenos"> 85</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Update changelog file. &quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="L-86"><a href="#L-86"><span class="linenos"> 86</span></a>    <span class="p">)</span>
+</span><span id="L-87"><a href="#L-87"><span class="linenos"> 87</span></a>
+</span><span id="L-88"><a href="#L-88"><span class="linenos"> 88</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="L-89"><a href="#L-89"><span class="linenos"> 89</span></a>        <span class="s2">&quot;-od&quot;</span><span class="p">,</span>
+</span><span id="L-90"><a href="#L-90"><span class="linenos"> 90</span></a>        <span class="s2">&quot;--overwrite_dependencies&quot;</span><span class="p">,</span>
+</span><span id="L-91"><a href="#L-91"><span class="linenos"> 91</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
+</span><span id="L-92"><a href="#L-92"><span class="linenos"> 92</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; When building a package, packagelister will be used</span>
+</span><span id="L-93"><a href="#L-93"><span class="linenos"> 93</span></a><span class="s2">        to update the dependencies list in pyproject.toml.</span>
+</span><span id="L-94"><a href="#L-94"><span class="linenos"> 94</span></a><span class="s2">        The default behavior is to append any new dependencies to</span>
+</span><span id="L-95"><a href="#L-95"><span class="linenos"> 95</span></a><span class="s2">        the current list so as not to erase any manually added dependencies</span>
+</span><span id="L-96"><a href="#L-96"><span class="linenos"> 96</span></a><span class="s2">        that packagelister may not detect. If you don&#39;t have any manually </span>
+</span><span id="L-97"><a href="#L-97"><span class="linenos"> 97</span></a><span class="s2">        added dependencies and want to remove any dependencies that your</span>
+</span><span id="L-98"><a href="#L-98"><span class="linenos"> 98</span></a><span class="s2">        project no longer uses, pass this flag.&quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="L-99"><a href="#L-99"><span class="linenos"> 99</span></a>    <span class="p">)</span>
+</span><span id="L-100"><a href="#L-100"><span class="linenos">100</span></a>
+</span><span id="L-101"><a href="#L-101"><span class="linenos">101</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="L-102"><a href="#L-102"><span class="linenos">102</span></a>        <span class="s2">&quot;-ca&quot;</span><span class="p">,</span>
+</span><span id="L-103"><a href="#L-103"><span class="linenos">103</span></a>        <span class="s2">&quot;--commit_all&quot;</span><span class="p">,</span>
+</span><span id="L-104"><a href="#L-104"><span class="linenos">104</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
+</span><span id="L-105"><a href="#L-105"><span class="linenos">105</span></a>        <span class="n">default</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span>
+</span><span id="L-106"><a href="#L-106"><span class="linenos">106</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Git stage and commit all tracked files</span>
+</span><span id="L-107"><a href="#L-107"><span class="linenos">107</span></a><span class="s2">        with this supplied commit message.</span>
+</span><span id="L-108"><a href="#L-108"><span class="linenos">108</span></a><span class="s2">        If &#39;build&#39; is passed, all commits will have</span>
+</span><span id="L-109"><a href="#L-109"><span class="linenos">109</span></a><span class="s2">        message: &#39;chore: build v</span><span class="si">{current_version}</span><span class="s2">&quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="L-110"><a href="#L-110"><span class="linenos">110</span></a>    <span class="p">)</span>
+</span><span id="L-111"><a href="#L-111"><span class="linenos">111</span></a>
+</span><span id="L-112"><a href="#L-112"><span class="linenos">112</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="L-113"><a href="#L-113"><span class="linenos">113</span></a>        <span class="s2">&quot;-s&quot;</span><span class="p">,</span>
+</span><span id="L-114"><a href="#L-114"><span class="linenos">114</span></a>        <span class="s2">&quot;--sync&quot;</span><span class="p">,</span>
+</span><span id="L-115"><a href="#L-115"><span class="linenos">115</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
+</span><span id="L-116"><a href="#L-116"><span class="linenos">116</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Pull from github, then push current commit to repo. &quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="L-117"><a href="#L-117"><span class="linenos">117</span></a>    <span class="p">)</span>
+</span><span id="L-118"><a href="#L-118"><span class="linenos">118</span></a>
+</span><span id="L-119"><a href="#L-119"><span class="linenos">119</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="L-120"><a href="#L-120"><span class="linenos">120</span></a>        <span class="s2">&quot;-dv&quot;</span><span class="p">,</span>
+</span><span id="L-121"><a href="#L-121"><span class="linenos">121</span></a>        <span class="s2">&quot;--dependency_versions&quot;</span><span class="p">,</span>
+</span><span id="L-122"><a href="#L-122"><span class="linenos">122</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
+</span><span id="L-123"><a href="#L-123"><span class="linenos">123</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Include version specifiers for dependencies in</span>
+</span><span id="L-124"><a href="#L-124"><span class="linenos">124</span></a><span class="s2">        pyproject.toml.&quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="L-125"><a href="#L-125"><span class="linenos">125</span></a>    <span class="p">)</span>
+</span><span id="L-126"><a href="#L-126"><span class="linenos">126</span></a>
+</span><span id="L-127"><a href="#L-127"><span class="linenos">127</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="L-128"><a href="#L-128"><span class="linenos">128</span></a>        <span class="s2">&quot;-up&quot;</span><span class="p">,</span>
+</span><span id="L-129"><a href="#L-129"><span class="linenos">129</span></a>        <span class="s2">&quot;--update&quot;</span><span class="p">,</span>
+</span><span id="L-130"><a href="#L-130"><span class="linenos">130</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
+</span><span id="L-131"><a href="#L-131"><span class="linenos">131</span></a>        <span class="n">default</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span>
+</span><span id="L-132"><a href="#L-132"><span class="linenos">132</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Excpects one argument: &quot;major&quot;, &quot;minor&quot;, or &quot;patch&quot;.</span>
+</span><span id="L-133"><a href="#L-133"><span class="linenos">133</span></a><span class="s2">        Passing &quot;-up minor&quot; is equivalent to passing the cli string: &quot;-b -t -i -iv minor -uc -ca build -s&quot;.</span>
+</span><span id="L-134"><a href="#L-134"><span class="linenos">134</span></a><span class="s2">        To publish the updated package, the -p/--publish switch needs to be added to the cli input.&quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="L-135"><a href="#L-135"><span class="linenos">135</span></a>    <span class="p">)</span>
+</span><span id="L-136"><a href="#L-136"><span class="linenos">136</span></a>
+</span><span id="L-137"><a href="#L-137"><span class="linenos">137</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="L-138"><a href="#L-138"><span class="linenos">138</span></a>        <span class="s2">&quot;-st&quot;</span><span class="p">,</span>
+</span><span id="L-139"><a href="#L-139"><span class="linenos">139</span></a>        <span class="s2">&quot;--skip_tests&quot;</span><span class="p">,</span>
+</span><span id="L-140"><a href="#L-140"><span class="linenos">140</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
+</span><span id="L-141"><a href="#L-141"><span class="linenos">141</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Don&#39;t run tests when using the -b/--build command. &quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="L-142"><a href="#L-142"><span class="linenos">142</span></a>    <span class="p">)</span>
+</span><span id="L-143"><a href="#L-143"><span class="linenos">143</span></a>
+</span><span id="L-144"><a href="#L-144"><span class="linenos">144</span></a>    <span class="n">args</span> <span class="o">=</span> <span class="n">parser</span><span class="o">.</span><span class="n">parse_args</span><span class="p">()</span>
+</span><span id="L-145"><a href="#L-145"><span class="linenos">145</span></a>
+</span><span id="L-146"><a href="#L-146"><span class="linenos">146</span></a>    <span class="n">args</span><span class="o">.</span><span class="n">package</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="p">)</span><span class="o">.</span><span class="n">resolve</span><span class="p">()</span>
+</span><span id="L-147"><a href="#L-147"><span class="linenos">147</span></a>
+</span><span id="L-148"><a href="#L-148"><span class="linenos">148</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">update</span><span class="p">:</span>
+</span><span id="L-149"><a href="#L-149"><span class="linenos">149</span></a>        <span class="n">args</span><span class="o">.</span><span class="n">build</span> <span class="o">=</span> <span class="kc">True</span>
+</span><span id="L-150"><a href="#L-150"><span class="linenos">150</span></a>        <span class="n">args</span><span class="o">.</span><span class="n">tag_version</span> <span class="o">=</span> <span class="kc">True</span>
+</span><span id="L-151"><a href="#L-151"><span class="linenos">151</span></a>        <span class="n">args</span><span class="o">.</span><span class="n">install</span> <span class="o">=</span> <span class="kc">True</span>
+</span><span id="L-152"><a href="#L-152"><span class="linenos">152</span></a>        <span class="n">args</span><span class="o">.</span><span class="n">increment_version</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">update</span>
+</span><span id="L-153"><a href="#L-153"><span class="linenos">153</span></a>        <span class="n">args</span><span class="o">.</span><span class="n">update_changelog</span> <span class="o">=</span> <span class="kc">True</span>
+</span><span id="L-154"><a href="#L-154"><span class="linenos">154</span></a>        <span class="n">args</span><span class="o">.</span><span class="n">commit_all</span> <span class="o">=</span> <span class="s2">&quot;build&quot;</span>
+</span><span id="L-155"><a href="#L-155"><span class="linenos">155</span></a>        <span class="n">args</span><span class="o">.</span><span class="n">sync</span> <span class="o">=</span> <span class="kc">True</span>
+</span><span id="L-156"><a href="#L-156"><span class="linenos">156</span></a>
+</span><span id="L-157"><a href="#L-157"><span class="linenos">157</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">increment_version</span> <span class="ow">and</span> <span class="n">args</span><span class="o">.</span><span class="n">increment_version</span> <span class="ow">not</span> <span class="ow">in</span> <span class="p">[</span>
+</span><span id="L-158"><a href="#L-158"><span class="linenos">158</span></a>        <span class="s2">&quot;major&quot;</span><span class="p">,</span>
+</span><span id="L-159"><a href="#L-159"><span class="linenos">159</span></a>        <span class="s2">&quot;minor&quot;</span><span class="p">,</span>
+</span><span id="L-160"><a href="#L-160"><span class="linenos">160</span></a>        <span class="s2">&quot;patch&quot;</span><span class="p">,</span>
+</span><span id="L-161"><a href="#L-161"><span class="linenos">161</span></a>    <span class="p">]:</span>
+</span><span id="L-162"><a href="#L-162"><span class="linenos">162</span></a>        <span class="k">raise</span> <span class="ne">ValueError</span><span class="p">(</span>
+</span><span id="L-163"><a href="#L-163"><span class="linenos">163</span></a>            <span class="sa">f</span><span class="s2">&quot;Invalid option for -iv/--increment_version: </span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">increment_version</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="L-164"><a href="#L-164"><span class="linenos">164</span></a>        <span class="p">)</span>
 </span><span id="L-165"><a href="#L-165"><span class="linenos">165</span></a>
-</span><span id="L-166"><a href="#L-166"><span class="linenos">166</span></a>    <span class="n">pyproject_path</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">package</span> <span class="o">/</span> <span class="s2">&quot;pyproject.toml&quot;</span>
-</span><span id="L-167"><a href="#L-167"><span class="linenos">167</span></a>
-</span><span id="L-168"><a href="#L-168"><span class="linenos">168</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">pyproject_path</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
-</span><span id="L-169"><a href="#L-169"><span class="linenos">169</span></a>        <span class="k">raise</span> <span class="ne">FileNotFoundError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Could not locate pyproject.toml for </span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="L-166"><a href="#L-166"><span class="linenos">166</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">commit_all</span> <span class="o">==</span> <span class="s2">&quot;&quot;</span><span class="p">:</span>
+</span><span id="L-167"><a href="#L-167"><span class="linenos">167</span></a>        <span class="k">raise</span> <span class="ne">ValueError</span><span class="p">(</span><span class="s2">&quot;Commit message for args.commit_all cannot be empty.&quot;</span><span class="p">)</span>
+</span><span id="L-168"><a href="#L-168"><span class="linenos">168</span></a>
+</span><span id="L-169"><a href="#L-169"><span class="linenos">169</span></a>    <span class="k">return</span> <span class="n">args</span>
 </span><span id="L-170"><a href="#L-170"><span class="linenos">170</span></a>
-</span><span id="L-171"><a href="#L-171"><span class="linenos">171</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">generate_tests</span><span class="p">:</span>
-</span><span id="L-172"><a href="#L-172"><span class="linenos">172</span></a>        <span class="n">generate_test_files</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="p">)</span>
-</span><span id="L-173"><a href="#L-173"><span class="linenos">173</span></a>
-</span><span id="L-174"><a href="#L-174"><span class="linenos">174</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">run_tests</span><span class="p">:</span>
-</span><span id="L-175"><a href="#L-175"><span class="linenos">175</span></a>        <span class="n">run_tests</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="p">)</span>
+</span><span id="L-171"><a href="#L-171"><span class="linenos">171</span></a>
+</span><span id="L-172"><a href="#L-172"><span class="linenos">172</span></a><span class="k">def</span> <span class="nf">build</span><span class="p">(</span>
+</span><span id="L-173"><a href="#L-173"><span class="linenos">173</span></a>    <span class="n">package_dir</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">,</span> <span class="n">skip_tests</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">,</span> <span class="n">overwrite_dependencies</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span>
+</span><span id="L-174"><a href="#L-174"><span class="linenos">174</span></a><span class="p">):</span>
+</span><span id="L-175"><a href="#L-175"><span class="linenos">175</span></a>    <span class="sd">&quot;&quot;&quot;Perform the build process.</span>
 </span><span id="L-176"><a href="#L-176"><span class="linenos">176</span></a>
-</span><span id="L-177"><a href="#L-177"><span class="linenos">177</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">increment_version</span><span class="p">:</span>
-</span><span id="L-178"><a href="#L-178"><span class="linenos">178</span></a>        <span class="n">hassle_utilities</span><span class="o">.</span><span class="n">increment_version</span><span class="p">(</span><span class="n">pyproject_path</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">increment_version</span><span class="p">)</span>
-</span><span id="L-179"><a href="#L-179"><span class="linenos">179</span></a>
-</span><span id="L-180"><a href="#L-180"><span class="linenos">180</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">build</span><span class="p">:</span>
-</span><span id="L-181"><a href="#L-181"><span class="linenos">181</span></a>        <span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">package</span> <span class="o">/</span> <span class="s2">&quot;dist&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">delete</span><span class="p">()</span>
-</span><span id="L-182"><a href="#L-182"><span class="linenos">182</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;black </span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="L-183"><a href="#L-183"><span class="linenos">183</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;isort </span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="L-184"><a href="#L-184"><span class="linenos">184</span></a>        <span class="n">hassle_utilities</span><span class="o">.</span><span class="n">update_dependencies</span><span class="p">(</span>
-</span><span id="L-185"><a href="#L-185"><span class="linenos">185</span></a>            <span class="n">pyproject_path</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">overwrite_dependencies</span>
-</span><span id="L-186"><a href="#L-186"><span class="linenos">186</span></a>        <span class="p">)</span>
-</span><span id="L-187"><a href="#L-187"><span class="linenos">187</span></a>        <span class="c1"># Vermin isn&#39;t taking into account the minimum version of dependencies.</span>
-</span><span id="L-188"><a href="#L-188"><span class="linenos">188</span></a>        <span class="c1"># Removing from now and defaulting to &gt;=3.10</span>
-</span><span id="L-189"><a href="#L-189"><span class="linenos">189</span></a>        <span class="c1"># hassle_utilities.update_minimum_python_version(pyproject_path)</span>
-</span><span id="L-190"><a href="#L-190"><span class="linenos">190</span></a>        <span class="n">hassle_utilities</span><span class="o">.</span><span class="n">generate_docs</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="p">)</span>
-</span><span id="L-191"><a href="#L-191"><span class="linenos">191</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;py -m build </span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="L-192"><a href="#L-192"><span class="linenos">192</span></a>
-</span><span id="L-193"><a href="#L-193"><span class="linenos">193</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">update_changelog</span><span class="p">:</span>
-</span><span id="L-194"><a href="#L-194"><span class="linenos">194</span></a>        <span class="n">hassle_utilities</span><span class="o">.</span><span class="n">update_changelog</span><span class="p">(</span><span class="n">pyproject_path</span><span class="p">)</span>
-</span><span id="L-195"><a href="#L-195"><span class="linenos">195</span></a>        <span class="c1"># If we&#39;re going to add tag for current version</span>
-</span><span id="L-196"><a href="#L-196"><span class="linenos">196</span></a>        <span class="c1"># commit changelog first</span>
-</span><span id="L-197"><a href="#L-197"><span class="linenos">197</span></a>        <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">tag_version</span><span class="p">:</span>
-</span><span id="L-198"><a href="#L-198"><span class="linenos">198</span></a>            <span class="nb">input</span><span class="p">(</span>
-</span><span id="L-199"><a href="#L-199"><span class="linenos">199</span></a>                <span class="s2">&quot;Press enter to continue after optionally pruning the updated changelog...&quot;</span>
-</span><span id="L-200"><a href="#L-200"><span class="linenos">200</span></a>            <span class="p">)</span>
-</span><span id="L-201"><a href="#L-201"><span class="linenos">201</span></a>            <span class="n">os</span><span class="o">.</span><span class="n">chdir</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="p">)</span>
-</span><span id="L-202"><a href="#L-202"><span class="linenos">202</span></a>            <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="s2">&quot;git add CHANGELOG.md&quot;</span><span class="p">)</span>
-</span><span id="L-203"><a href="#L-203"><span class="linenos">203</span></a>            <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="s1">&#39;git commit CHANGELOG.md -m &quot;chore: update changelog&quot;&#39;</span><span class="p">)</span>
-</span><span id="L-204"><a href="#L-204"><span class="linenos">204</span></a>
-</span><span id="L-205"><a href="#L-205"><span class="linenos">205</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">commit_all</span><span class="p">:</span>
-</span><span id="L-206"><a href="#L-206"><span class="linenos">206</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">chdir</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="p">)</span>
-</span><span id="L-207"><a href="#L-207"><span class="linenos">207</span></a>        <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">commit_all</span> <span class="o">==</span> <span class="s2">&quot;build&quot;</span><span class="p">:</span>
-</span><span id="L-208"><a href="#L-208"><span class="linenos">208</span></a>            <span class="n">version</span> <span class="o">=</span> <span class="n">pyproject_path</span><span class="o">.</span><span class="n">loads</span><span class="p">()[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;version&quot;</span><span class="p">]</span>
-</span><span id="L-209"><a href="#L-209"><span class="linenos">209</span></a>            <span class="n">args</span><span class="o">.</span><span class="n">commit_all</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;chore: build v</span><span class="si">{</span><span class="n">version</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="L-210"><a href="#L-210"><span class="linenos">210</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="s2">&quot;git add .&quot;</span><span class="p">)</span>
-</span><span id="L-211"><a href="#L-211"><span class="linenos">211</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;git commit -m &quot;</span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">commit_all</span><span class="si">}</span><span class="s1">&quot;&#39;</span><span class="p">)</span>
+</span><span id="L-177"><a href="#L-177"><span class="linenos">177</span></a><span class="sd">    Steps:</span>
+</span><span id="L-178"><a href="#L-178"><span class="linenos">178</span></a><span class="sd">    * Run tests (unless `skip_tests` is `True`)</span>
+</span><span id="L-179"><a href="#L-179"><span class="linenos">179</span></a><span class="sd">    * Raise error and abandon build if tests fail</span>
+</span><span id="L-180"><a href="#L-180"><span class="linenos">180</span></a><span class="sd">    * Format source code with `Black`</span>
+</span><span id="L-181"><a href="#L-181"><span class="linenos">181</span></a><span class="sd">    * Sort source code imports with `isort`</span>
+</span><span id="L-182"><a href="#L-182"><span class="linenos">182</span></a><span class="sd">    * Update project dependencies in `pyproject.toml`</span>
+</span><span id="L-183"><a href="#L-183"><span class="linenos">183</span></a><span class="sd">    * Generate docs</span>
+</span><span id="L-184"><a href="#L-184"><span class="linenos">184</span></a><span class="sd">    * Delete previous `dist` folder contents</span>
+</span><span id="L-185"><a href="#L-185"><span class="linenos">185</span></a><span class="sd">    * Invoke build module&quot;&quot;&quot;</span>
+</span><span id="L-186"><a href="#L-186"><span class="linenos">186</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">skip_tests</span> <span class="ow">and</span> <span class="ow">not</span> <span class="n">run_tests</span><span class="p">(</span><span class="n">package_dir</span><span class="p">):</span>
+</span><span id="L-187"><a href="#L-187"><span class="linenos">187</span></a>        <span class="k">raise</span> <span class="ne">RuntimeError</span><span class="p">(</span>
+</span><span id="L-188"><a href="#L-188"><span class="linenos">188</span></a>            <span class="sa">f</span><span class="s2">&quot;ERROR: </span><span class="si">{</span><span class="n">package_dir</span><span class="o">.</span><span class="n">stem</span><span class="si">}</span><span class="s2"> failed testing.</span><span class="se">\n</span><span class="s2">Abandoning build.&quot;</span>
+</span><span id="L-189"><a href="#L-189"><span class="linenos">189</span></a>        <span class="p">)</span>
+</span><span id="L-190"><a href="#L-190"><span class="linenos">190</span></a>    <span class="n">hassle_utilities</span><span class="o">.</span><span class="n">format_files</span><span class="p">(</span><span class="n">package_dir</span><span class="p">)</span>
+</span><span id="L-191"><a href="#L-191"><span class="linenos">191</span></a>    <span class="p">[</span><span class="n">isort</span><span class="o">.</span><span class="n">file</span><span class="p">(</span><span class="n">path</span><span class="p">)</span> <span class="k">for</span> <span class="n">path</span> <span class="ow">in</span> <span class="n">package_dir</span><span class="o">.</span><span class="n">rglob</span><span class="p">(</span><span class="s2">&quot;*.py&quot;</span><span class="p">)]</span>
+</span><span id="L-192"><a href="#L-192"><span class="linenos">192</span></a>    <span class="n">hassle_utilities</span><span class="o">.</span><span class="n">update_dependencies</span><span class="p">(</span>
+</span><span id="L-193"><a href="#L-193"><span class="linenos">193</span></a>        <span class="n">package_dir</span> <span class="o">/</span> <span class="s2">&quot;pyproject.toml&quot;</span><span class="p">,</span> <span class="n">overwrite_dependencies</span>
+</span><span id="L-194"><a href="#L-194"><span class="linenos">194</span></a>    <span class="p">)</span>
+</span><span id="L-195"><a href="#L-195"><span class="linenos">195</span></a>    <span class="c1"># Vermin isn&#39;t taking into account the minimum version of dependencies.</span>
+</span><span id="L-196"><a href="#L-196"><span class="linenos">196</span></a>    <span class="c1"># Removing from now and defaulting to &gt;=3.10</span>
+</span><span id="L-197"><a href="#L-197"><span class="linenos">197</span></a>    <span class="c1"># hassle_utilities.update_minimum_python_version(pyproject_path)</span>
+</span><span id="L-198"><a href="#L-198"><span class="linenos">198</span></a>    <span class="n">hassle_utilities</span><span class="o">.</span><span class="n">generate_docs</span><span class="p">(</span><span class="n">package_dir</span><span class="p">)</span>
+</span><span id="L-199"><a href="#L-199"><span class="linenos">199</span></a>    <span class="p">(</span><span class="n">package_dir</span> <span class="o">/</span> <span class="s2">&quot;dist&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">delete</span><span class="p">()</span>
+</span><span id="L-200"><a href="#L-200"><span class="linenos">200</span></a>    <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">sys</span><span class="o">.</span><span class="n">executable</span><span class="si">}</span><span class="s2"> -m build </span><span class="si">{</span><span class="n">package_dir</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="L-201"><a href="#L-201"><span class="linenos">201</span></a>
+</span><span id="L-202"><a href="#L-202"><span class="linenos">202</span></a>
+</span><span id="L-203"><a href="#L-203"><span class="linenos">203</span></a><span class="k">def</span> <span class="nf">main</span><span class="p">(</span><span class="n">args</span><span class="p">:</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span> <span class="o">=</span> <span class="kc">None</span><span class="p">):</span>
+</span><span id="L-204"><a href="#L-204"><span class="linenos">204</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="p">:</span>
+</span><span id="L-205"><a href="#L-205"><span class="linenos">205</span></a>        <span class="n">args</span> <span class="o">=</span> <span class="n">get_args</span><span class="p">()</span>
+</span><span id="L-206"><a href="#L-206"><span class="linenos">206</span></a>
+</span><span id="L-207"><a href="#L-207"><span class="linenos">207</span></a>    <span class="n">pyproject_path</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">package</span> <span class="o">/</span> <span class="s2">&quot;pyproject.toml&quot;</span>
+</span><span id="L-208"><a href="#L-208"><span class="linenos">208</span></a>    <span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="o">.</span><span class="n">mkcwd</span><span class="p">()</span>
+</span><span id="L-209"><a href="#L-209"><span class="linenos">209</span></a>
+</span><span id="L-210"><a href="#L-210"><span class="linenos">210</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">pyproject_path</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
+</span><span id="L-211"><a href="#L-211"><span class="linenos">211</span></a>        <span class="k">raise</span> <span class="ne">FileNotFoundError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Could not locate pyproject.toml for </span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
 </span><span id="L-212"><a href="#L-212"><span class="linenos">212</span></a>
-</span><span id="L-213"><a href="#L-213"><span class="linenos">213</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">tag_version</span><span class="p">:</span>
-</span><span id="L-214"><a href="#L-214"><span class="linenos">214</span></a>        <span class="n">hassle_utilities</span><span class="o">.</span><span class="n">tag_version</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="p">)</span>
+</span><span id="L-213"><a href="#L-213"><span class="linenos">213</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">generate_tests</span><span class="p">:</span>
+</span><span id="L-214"><a href="#L-214"><span class="linenos">214</span></a>        <span class="n">generate_test_files</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="p">)</span>
 </span><span id="L-215"><a href="#L-215"><span class="linenos">215</span></a>
-</span><span id="L-216"><a href="#L-216"><span class="linenos">216</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">publish</span><span class="p">:</span>
-</span><span id="L-217"><a href="#L-217"><span class="linenos">217</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;twine upload </span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">package</span> <span class="o">/</span> <span class="s1">&#39;dist&#39;</span> <span class="o">/</span> <span class="s1">&#39;*&#39;</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="L-216"><a href="#L-216"><span class="linenos">216</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">run_tests</span><span class="p">:</span>
+</span><span id="L-217"><a href="#L-217"><span class="linenos">217</span></a>        <span class="n">run_tests</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="p">)</span>
 </span><span id="L-218"><a href="#L-218"><span class="linenos">218</span></a>
-</span><span id="L-219"><a href="#L-219"><span class="linenos">219</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">install</span><span class="p">:</span>
-</span><span id="L-220"><a href="#L-220"><span class="linenos">220</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;pip install </span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="si">}</span><span class="s2"> --no-deps --upgrade --no-cache-dir&quot;</span><span class="p">)</span>
+</span><span id="L-219"><a href="#L-219"><span class="linenos">219</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">increment_version</span><span class="p">:</span>
+</span><span id="L-220"><a href="#L-220"><span class="linenos">220</span></a>        <span class="n">hassle_utilities</span><span class="o">.</span><span class="n">increment_version</span><span class="p">(</span><span class="n">pyproject_path</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">increment_version</span><span class="p">)</span>
 </span><span id="L-221"><a href="#L-221"><span class="linenos">221</span></a>
-</span><span id="L-222"><a href="#L-222"><span class="linenos">222</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">sync</span><span class="p">:</span>
-</span><span id="L-223"><a href="#L-223"><span class="linenos">223</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">chdir</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="p">)</span>
-</span><span id="L-224"><a href="#L-224"><span class="linenos">224</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;git pull --tags origin main&quot;</span><span class="p">)</span>
-</span><span id="L-225"><a href="#L-225"><span class="linenos">225</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;git push origin main:main --tags&quot;</span><span class="p">)</span>
-</span><span id="L-226"><a href="#L-226"><span class="linenos">226</span></a>
-</span><span id="L-227"><a href="#L-227"><span class="linenos">227</span></a>
-</span><span id="L-228"><a href="#L-228"><span class="linenos">228</span></a><span class="k">if</span> <span class="vm">__name__</span> <span class="o">==</span> <span class="s2">&quot;__main__&quot;</span><span class="p">:</span>
-</span><span id="L-229"><a href="#L-229"><span class="linenos">229</span></a>    <span class="n">main</span><span class="p">(</span><span class="n">get_args</span><span class="p">())</span>
+</span><span id="L-222"><a href="#L-222"><span class="linenos">222</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">build</span><span class="p">:</span>
+</span><span id="L-223"><a href="#L-223"><span class="linenos">223</span></a>        <span class="n">build</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">skip_tests</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">overwrite_dependencies</span><span class="p">)</span>
+</span><span id="L-224"><a href="#L-224"><span class="linenos">224</span></a>
+</span><span id="L-225"><a href="#L-225"><span class="linenos">225</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">update_changelog</span><span class="p">:</span>
+</span><span id="L-226"><a href="#L-226"><span class="linenos">226</span></a>        <span class="n">hassle_utilities</span><span class="o">.</span><span class="n">update_changelog</span><span class="p">(</span><span class="n">pyproject_path</span><span class="p">)</span>
+</span><span id="L-227"><a href="#L-227"><span class="linenos">227</span></a>        <span class="c1"># If we&#39;re going to add tag for current version</span>
+</span><span id="L-228"><a href="#L-228"><span class="linenos">228</span></a>        <span class="c1"># commit changelog first</span>
+</span><span id="L-229"><a href="#L-229"><span class="linenos">229</span></a>        <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">tag_version</span><span class="p">:</span>
+</span><span id="L-230"><a href="#L-230"><span class="linenos">230</span></a>            <span class="nb">input</span><span class="p">(</span>
+</span><span id="L-231"><a href="#L-231"><span class="linenos">231</span></a>                <span class="s2">&quot;Press enter to continue after optionally pruning the updated changelog...&quot;</span>
+</span><span id="L-232"><a href="#L-232"><span class="linenos">232</span></a>            <span class="p">)</span>
+</span><span id="L-233"><a href="#L-233"><span class="linenos">233</span></a>            <span class="n">git</span><span class="o">.</span><span class="n">commit_files</span><span class="p">(</span>
+</span><span id="L-234"><a href="#L-234"><span class="linenos">234</span></a>                <span class="p">[</span><span class="nb">str</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">package</span> <span class="o">/</span> <span class="s2">&quot;CHANGELOG.md&quot;</span><span class="p">)],</span> <span class="s2">&quot;chore: update changelog&quot;</span>
+</span><span id="L-235"><a href="#L-235"><span class="linenos">235</span></a>            <span class="p">)</span>
+</span><span id="L-236"><a href="#L-236"><span class="linenos">236</span></a>
+</span><span id="L-237"><a href="#L-237"><span class="linenos">237</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">commit_all</span><span class="p">:</span>
+</span><span id="L-238"><a href="#L-238"><span class="linenos">238</span></a>        <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">commit_all</span> <span class="o">==</span> <span class="s2">&quot;build&quot;</span><span class="p">:</span>
+</span><span id="L-239"><a href="#L-239"><span class="linenos">239</span></a>            <span class="n">version</span> <span class="o">=</span> <span class="n">pyproject_path</span><span class="o">.</span><span class="n">loads</span><span class="p">()[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;version&quot;</span><span class="p">]</span>
+</span><span id="L-240"><a href="#L-240"><span class="linenos">240</span></a>            <span class="n">args</span><span class="o">.</span><span class="n">commit_all</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;chore: build v</span><span class="si">{</span><span class="n">version</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="L-241"><a href="#L-241"><span class="linenos">241</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">add</span><span class="p">()</span>
+</span><span id="L-242"><a href="#L-242"><span class="linenos">242</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">commit</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;-m &quot;</span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">commit_all</span><span class="si">}</span><span class="s1">&quot;&#39;</span><span class="p">)</span>
+</span><span id="L-243"><a href="#L-243"><span class="linenos">243</span></a>
+</span><span id="L-244"><a href="#L-244"><span class="linenos">244</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">tag_version</span><span class="p">:</span>
+</span><span id="L-245"><a href="#L-245"><span class="linenos">245</span></a>        <span class="n">hassle_utilities</span><span class="o">.</span><span class="n">tag_version</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="p">)</span>
+</span><span id="L-246"><a href="#L-246"><span class="linenos">246</span></a>
+</span><span id="L-247"><a href="#L-247"><span class="linenos">247</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">publish</span><span class="p">:</span>
+</span><span id="L-248"><a href="#L-248"><span class="linenos">248</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;twine upload </span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">package</span> <span class="o">/</span> <span class="s1">&#39;dist&#39;</span> <span class="o">/</span> <span class="s1">&#39;*&#39;</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="L-249"><a href="#L-249"><span class="linenos">249</span></a>
+</span><span id="L-250"><a href="#L-250"><span class="linenos">250</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">install</span><span class="p">:</span>
+</span><span id="L-251"><a href="#L-251"><span class="linenos">251</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;pip install </span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="si">}</span><span class="s2"> --no-deps --upgrade --no-cache-dir&quot;</span><span class="p">)</span>
+</span><span id="L-252"><a href="#L-252"><span class="linenos">252</span></a>
+</span><span id="L-253"><a href="#L-253"><span class="linenos">253</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">sync</span><span class="p">:</span>
+</span><span id="L-254"><a href="#L-254"><span class="linenos">254</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">pull</span><span class="p">(</span><span class="s2">&quot;--tags&quot;</span><span class="p">)</span>
+</span><span id="L-255"><a href="#L-255"><span class="linenos">255</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">push</span><span class="p">(</span><span class="s2">&quot;--tags&quot;</span><span class="p">)</span>
+</span><span id="L-256"><a href="#L-256"><span class="linenos">256</span></a>
+</span><span id="L-257"><a href="#L-257"><span class="linenos">257</span></a>
+</span><span id="L-258"><a href="#L-258"><span class="linenos">258</span></a><span class="k">if</span> <span class="vm">__name__</span> <span class="o">==</span> <span class="s2">&quot;__main__&quot;</span><span class="p">:</span>
+</span><span id="L-259"><a href="#L-259"><span class="linenos">259</span></a>    <span class="n">main</span><span class="p">(</span><span class="n">get_args</span><span class="p">())</span>
 </span></pre></div>
 
 
             </section>
                 <section id="get_args">
                             <input id="get_args-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
@@ -297,242 +330,299 @@
         <span class="def">def</span>
         <span class="name">get_args</span><span class="signature pdoc-code condensed">(<span class="return-annotation">) -> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span>:</span></span>
 
                 <label class="view-source-button" for="get_args-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#get_args"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="get_args-14"><a href="#get_args-14"><span class="linenos"> 14</span></a><span class="k">def</span> <span class="nf">get_args</span><span class="p">()</span> <span class="o">-&gt;</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span><span class="p">:</span>
-</span><span id="get_args-15"><a href="#get_args-15"><span class="linenos"> 15</span></a>    <span class="n">parser</span> <span class="o">=</span> <span class="n">argparse</span><span class="o">.</span><span class="n">ArgumentParser</span><span class="p">()</span>
-</span><span id="get_args-16"><a href="#get_args-16"><span class="linenos"> 16</span></a>
-</span><span id="get_args-17"><a href="#get_args-17"><span class="linenos"> 17</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="get_args-18"><a href="#get_args-18"><span class="linenos"> 18</span></a>        <span class="s2">&quot;package&quot;</span><span class="p">,</span>
-</span><span id="get_args-19"><a href="#get_args-19"><span class="linenos"> 19</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
-</span><span id="get_args-20"><a href="#get_args-20"><span class="linenos"> 20</span></a>        <span class="n">default</span><span class="o">=</span><span class="s2">&quot;.&quot;</span><span class="p">,</span>
-</span><span id="get_args-21"><a href="#get_args-21"><span class="linenos"> 21</span></a>        <span class="n">nargs</span><span class="o">=</span><span class="s2">&quot;?&quot;</span><span class="p">,</span>
-</span><span id="get_args-22"><a href="#get_args-22"><span class="linenos"> 22</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; The name of the package or project to use,</span>
-</span><span id="get_args-23"><a href="#get_args-23"><span class="linenos"> 23</span></a><span class="s2">        assuming it&#39;s a subfolder of your current working directory.</span>
-</span><span id="get_args-24"><a href="#get_args-24"><span class="linenos"> 24</span></a><span class="s2">        Can also be a full path to the package. If nothing is given,</span>
-</span><span id="get_args-25"><a href="#get_args-25"><span class="linenos"> 25</span></a><span class="s2">        the current working directory will be used.&quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="get_args-26"><a href="#get_args-26"><span class="linenos"> 26</span></a>    <span class="p">)</span>
-</span><span id="get_args-27"><a href="#get_args-27"><span class="linenos"> 27</span></a>
-</span><span id="get_args-28"><a href="#get_args-28"><span class="linenos"> 28</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="get_args-29"><a href="#get_args-29"><span class="linenos"> 29</span></a>        <span class="s2">&quot;-b&quot;</span><span class="p">,</span> <span class="s2">&quot;--build&quot;</span><span class="p">,</span> <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span> <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Build the package. &quot;&quot;&quot;</span>
-</span><span id="get_args-30"><a href="#get_args-30"><span class="linenos"> 30</span></a>    <span class="p">)</span>
-</span><span id="get_args-31"><a href="#get_args-31"><span class="linenos"> 31</span></a>
-</span><span id="get_args-32"><a href="#get_args-32"><span class="linenos"> 32</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="get_args-33"><a href="#get_args-33"><span class="linenos"> 33</span></a>        <span class="s2">&quot;-t&quot;</span><span class="p">,</span>
-</span><span id="get_args-34"><a href="#get_args-34"><span class="linenos"> 34</span></a>        <span class="s2">&quot;--tag_version&quot;</span><span class="p">,</span>
-</span><span id="get_args-35"><a href="#get_args-35"><span class="linenos"> 35</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
-</span><span id="get_args-36"><a href="#get_args-36"><span class="linenos"> 36</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Add a git tag corresponding to the version in pyproject.toml. &quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="get_args-37"><a href="#get_args-37"><span class="linenos"> 37</span></a>    <span class="p">)</span>
-</span><span id="get_args-38"><a href="#get_args-38"><span class="linenos"> 38</span></a>
-</span><span id="get_args-39"><a href="#get_args-39"><span class="linenos"> 39</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="get_args-40"><a href="#get_args-40"><span class="linenos"> 40</span></a>        <span class="s2">&quot;-i&quot;</span><span class="p">,</span>
-</span><span id="get_args-41"><a href="#get_args-41"><span class="linenos"> 41</span></a>        <span class="s2">&quot;--install&quot;</span><span class="p">,</span>
-</span><span id="get_args-42"><a href="#get_args-42"><span class="linenos"> 42</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
-</span><span id="get_args-43"><a href="#get_args-43"><span class="linenos"> 43</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Install the package from source. &quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="get_args-44"><a href="#get_args-44"><span class="linenos"> 44</span></a>    <span class="p">)</span>
-</span><span id="get_args-45"><a href="#get_args-45"><span class="linenos"> 45</span></a>
-</span><span id="get_args-46"><a href="#get_args-46"><span class="linenos"> 46</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="get_args-47"><a href="#get_args-47"><span class="linenos"> 47</span></a>        <span class="s2">&quot;-iv&quot;</span><span class="p">,</span>
-</span><span id="get_args-48"><a href="#get_args-48"><span class="linenos"> 48</span></a>        <span class="s2">&quot;--increment_version&quot;</span><span class="p">,</span>
-</span><span id="get_args-49"><a href="#get_args-49"><span class="linenos"> 49</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
-</span><span id="get_args-50"><a href="#get_args-50"><span class="linenos"> 50</span></a>        <span class="n">default</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span>
-</span><span id="get_args-51"><a href="#get_args-51"><span class="linenos"> 51</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Increment version in pyproject.toml.</span>
-</span><span id="get_args-52"><a href="#get_args-52"><span class="linenos"> 52</span></a><span class="s2">        Can be one of &quot;major&quot;, &quot;minor&quot;, or &quot;patch&quot;. &quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="get_args-53"><a href="#get_args-53"><span class="linenos"> 53</span></a>    <span class="p">)</span>
-</span><span id="get_args-54"><a href="#get_args-54"><span class="linenos"> 54</span></a>
-</span><span id="get_args-55"><a href="#get_args-55"><span class="linenos"> 55</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="get_args-56"><a href="#get_args-56"><span class="linenos"> 56</span></a>        <span class="s2">&quot;-p&quot;</span><span class="p">,</span>
-</span><span id="get_args-57"><a href="#get_args-57"><span class="linenos"> 57</span></a>        <span class="s2">&quot;--publish&quot;</span><span class="p">,</span>
-</span><span id="get_args-58"><a href="#get_args-58"><span class="linenos"> 58</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
-</span><span id="get_args-59"><a href="#get_args-59"><span class="linenos"> 59</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Publish package to PyPi.</span>
-</span><span id="get_args-60"><a href="#get_args-60"><span class="linenos"> 60</span></a><span class="s2">        Note: You must have configured twine </span>
-</span><span id="get_args-61"><a href="#get_args-61"><span class="linenos"> 61</span></a><span class="s2">        and registered a PyPi account/generated an API</span>
-</span><span id="get_args-62"><a href="#get_args-62"><span class="linenos"> 62</span></a><span class="s2">        key to use this option.&quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="get_args-63"><a href="#get_args-63"><span class="linenos"> 63</span></a>    <span class="p">)</span>
-</span><span id="get_args-64"><a href="#get_args-64"><span class="linenos"> 64</span></a>
-</span><span id="get_args-65"><a href="#get_args-65"><span class="linenos"> 65</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="get_args-66"><a href="#get_args-66"><span class="linenos"> 66</span></a>        <span class="s2">&quot;-rt&quot;</span><span class="p">,</span>
-</span><span id="get_args-67"><a href="#get_args-67"><span class="linenos"> 67</span></a>        <span class="s2">&quot;--run_tests&quot;</span><span class="p">,</span>
-</span><span id="get_args-68"><a href="#get_args-68"><span class="linenos"> 68</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
-</span><span id="get_args-69"><a href="#get_args-69"><span class="linenos"> 69</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Run tests for the package. &quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="get_args-70"><a href="#get_args-70"><span class="linenos"> 70</span></a>    <span class="p">)</span>
-</span><span id="get_args-71"><a href="#get_args-71"><span class="linenos"> 71</span></a>
-</span><span id="get_args-72"><a href="#get_args-72"><span class="linenos"> 72</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="get_args-73"><a href="#get_args-73"><span class="linenos"> 73</span></a>        <span class="s2">&quot;-gt&quot;</span><span class="p">,</span>
-</span><span id="get_args-74"><a href="#get_args-74"><span class="linenos"> 74</span></a>        <span class="s2">&quot;--generate_tests&quot;</span><span class="p">,</span>
-</span><span id="get_args-75"><a href="#get_args-75"><span class="linenos"> 75</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
-</span><span id="get_args-76"><a href="#get_args-76"><span class="linenos"> 76</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Generate tests for the package. &quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="get_args-77"><a href="#get_args-77"><span class="linenos"> 77</span></a>    <span class="p">)</span>
-</span><span id="get_args-78"><a href="#get_args-78"><span class="linenos"> 78</span></a>
-</span><span id="get_args-79"><a href="#get_args-79"><span class="linenos"> 79</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="get_args-80"><a href="#get_args-80"><span class="linenos"> 80</span></a>        <span class="s2">&quot;-uc&quot;</span><span class="p">,</span>
-</span><span id="get_args-81"><a href="#get_args-81"><span class="linenos"> 81</span></a>        <span class="s2">&quot;--update_changelog&quot;</span><span class="p">,</span>
-</span><span id="get_args-82"><a href="#get_args-82"><span class="linenos"> 82</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
-</span><span id="get_args-83"><a href="#get_args-83"><span class="linenos"> 83</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Update changelog file. &quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="get_args-84"><a href="#get_args-84"><span class="linenos"> 84</span></a>    <span class="p">)</span>
-</span><span id="get_args-85"><a href="#get_args-85"><span class="linenos"> 85</span></a>
-</span><span id="get_args-86"><a href="#get_args-86"><span class="linenos"> 86</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="get_args-87"><a href="#get_args-87"><span class="linenos"> 87</span></a>        <span class="s2">&quot;-od&quot;</span><span class="p">,</span>
-</span><span id="get_args-88"><a href="#get_args-88"><span class="linenos"> 88</span></a>        <span class="s2">&quot;--overwrite_dependencies&quot;</span><span class="p">,</span>
-</span><span id="get_args-89"><a href="#get_args-89"><span class="linenos"> 89</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
-</span><span id="get_args-90"><a href="#get_args-90"><span class="linenos"> 90</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; When building a package, packagelister will be used</span>
-</span><span id="get_args-91"><a href="#get_args-91"><span class="linenos"> 91</span></a><span class="s2">        to update the dependencies list in pyproject.toml.</span>
-</span><span id="get_args-92"><a href="#get_args-92"><span class="linenos"> 92</span></a><span class="s2">        The default behavior is to append any new dependencies to</span>
-</span><span id="get_args-93"><a href="#get_args-93"><span class="linenos"> 93</span></a><span class="s2">        the current list so as not to erase any manually added dependencies</span>
-</span><span id="get_args-94"><a href="#get_args-94"><span class="linenos"> 94</span></a><span class="s2">        that packagelister may not detect. If you don&#39;t have any manually </span>
-</span><span id="get_args-95"><a href="#get_args-95"><span class="linenos"> 95</span></a><span class="s2">        added dependencies and want to remove any dependencies that your</span>
-</span><span id="get_args-96"><a href="#get_args-96"><span class="linenos"> 96</span></a><span class="s2">        project no longer uses, pass this flag.&quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="get_args-97"><a href="#get_args-97"><span class="linenos"> 97</span></a>    <span class="p">)</span>
-</span><span id="get_args-98"><a href="#get_args-98"><span class="linenos"> 98</span></a>
-</span><span id="get_args-99"><a href="#get_args-99"><span class="linenos"> 99</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="get_args-100"><a href="#get_args-100"><span class="linenos">100</span></a>        <span class="s2">&quot;-ca&quot;</span><span class="p">,</span>
-</span><span id="get_args-101"><a href="#get_args-101"><span class="linenos">101</span></a>        <span class="s2">&quot;--commit_all&quot;</span><span class="p">,</span>
-</span><span id="get_args-102"><a href="#get_args-102"><span class="linenos">102</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
-</span><span id="get_args-103"><a href="#get_args-103"><span class="linenos">103</span></a>        <span class="n">default</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span>
-</span><span id="get_args-104"><a href="#get_args-104"><span class="linenos">104</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Git stage and commit all tracked files</span>
-</span><span id="get_args-105"><a href="#get_args-105"><span class="linenos">105</span></a><span class="s2">        with this supplied commit message.</span>
-</span><span id="get_args-106"><a href="#get_args-106"><span class="linenos">106</span></a><span class="s2">        If &#39;build&#39; is passed, all commits will have</span>
-</span><span id="get_args-107"><a href="#get_args-107"><span class="linenos">107</span></a><span class="s2">        message: &#39;chore: build v</span><span class="si">{current_version}</span><span class="s2">&quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="get_args-108"><a href="#get_args-108"><span class="linenos">108</span></a>    <span class="p">)</span>
-</span><span id="get_args-109"><a href="#get_args-109"><span class="linenos">109</span></a>
-</span><span id="get_args-110"><a href="#get_args-110"><span class="linenos">110</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="get_args-111"><a href="#get_args-111"><span class="linenos">111</span></a>        <span class="s2">&quot;-s&quot;</span><span class="p">,</span>
-</span><span id="get_args-112"><a href="#get_args-112"><span class="linenos">112</span></a>        <span class="s2">&quot;--sync&quot;</span><span class="p">,</span>
-</span><span id="get_args-113"><a href="#get_args-113"><span class="linenos">113</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
-</span><span id="get_args-114"><a href="#get_args-114"><span class="linenos">114</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Pull from github, then push current commit to repo. &quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="get_args-115"><a href="#get_args-115"><span class="linenos">115</span></a>    <span class="p">)</span>
-</span><span id="get_args-116"><a href="#get_args-116"><span class="linenos">116</span></a>
-</span><span id="get_args-117"><a href="#get_args-117"><span class="linenos">117</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="get_args-118"><a href="#get_args-118"><span class="linenos">118</span></a>        <span class="s2">&quot;-dv&quot;</span><span class="p">,</span>
-</span><span id="get_args-119"><a href="#get_args-119"><span class="linenos">119</span></a>        <span class="s2">&quot;--dependency_versions&quot;</span><span class="p">,</span>
-</span><span id="get_args-120"><a href="#get_args-120"><span class="linenos">120</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
-</span><span id="get_args-121"><a href="#get_args-121"><span class="linenos">121</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Include version specifiers for dependencies in</span>
-</span><span id="get_args-122"><a href="#get_args-122"><span class="linenos">122</span></a><span class="s2">        pyproject.toml.&quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="get_args-123"><a href="#get_args-123"><span class="linenos">123</span></a>    <span class="p">)</span>
-</span><span id="get_args-124"><a href="#get_args-124"><span class="linenos">124</span></a>
-</span><span id="get_args-125"><a href="#get_args-125"><span class="linenos">125</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="get_args-126"><a href="#get_args-126"><span class="linenos">126</span></a>        <span class="s2">&quot;-up&quot;</span><span class="p">,</span>
-</span><span id="get_args-127"><a href="#get_args-127"><span class="linenos">127</span></a>        <span class="s2">&quot;--update&quot;</span><span class="p">,</span>
-</span><span id="get_args-128"><a href="#get_args-128"><span class="linenos">128</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
-</span><span id="get_args-129"><a href="#get_args-129"><span class="linenos">129</span></a>        <span class="n">default</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span>
-</span><span id="get_args-130"><a href="#get_args-130"><span class="linenos">130</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Excpects one argument: &quot;major&quot;, &quot;minor&quot;, or &quot;patch&quot;.</span>
-</span><span id="get_args-131"><a href="#get_args-131"><span class="linenos">131</span></a><span class="s2">        Passing &quot;-up minor&quot; is equivalent to passing the cli string: &quot;-b -t -i -iv minor -uc -ca build -s&quot;.</span>
-</span><span id="get_args-132"><a href="#get_args-132"><span class="linenos">132</span></a><span class="s2">        To publish the updated package, the -p/--publish switch needs to be added to the cli input.&quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="get_args-133"><a href="#get_args-133"><span class="linenos">133</span></a>    <span class="p">)</span>
-</span><span id="get_args-134"><a href="#get_args-134"><span class="linenos">134</span></a>
-</span><span id="get_args-135"><a href="#get_args-135"><span class="linenos">135</span></a>    <span class="n">args</span> <span class="o">=</span> <span class="n">parser</span><span class="o">.</span><span class="n">parse_args</span><span class="p">()</span>
-</span><span id="get_args-136"><a href="#get_args-136"><span class="linenos">136</span></a>
-</span><span id="get_args-137"><a href="#get_args-137"><span class="linenos">137</span></a>    <span class="n">args</span><span class="o">.</span><span class="n">package</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="p">)</span><span class="o">.</span><span class="n">resolve</span><span class="p">()</span>
-</span><span id="get_args-138"><a href="#get_args-138"><span class="linenos">138</span></a>
-</span><span id="get_args-139"><a href="#get_args-139"><span class="linenos">139</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">update</span><span class="p">:</span>
-</span><span id="get_args-140"><a href="#get_args-140"><span class="linenos">140</span></a>        <span class="n">args</span><span class="o">.</span><span class="n">build</span> <span class="o">=</span> <span class="kc">True</span>
-</span><span id="get_args-141"><a href="#get_args-141"><span class="linenos">141</span></a>        <span class="n">args</span><span class="o">.</span><span class="n">tag_version</span> <span class="o">=</span> <span class="kc">True</span>
-</span><span id="get_args-142"><a href="#get_args-142"><span class="linenos">142</span></a>        <span class="n">args</span><span class="o">.</span><span class="n">install</span> <span class="o">=</span> <span class="kc">True</span>
-</span><span id="get_args-143"><a href="#get_args-143"><span class="linenos">143</span></a>        <span class="n">args</span><span class="o">.</span><span class="n">increment_version</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">update</span>
-</span><span id="get_args-144"><a href="#get_args-144"><span class="linenos">144</span></a>        <span class="n">args</span><span class="o">.</span><span class="n">update_changelog</span> <span class="o">=</span> <span class="kc">True</span>
-</span><span id="get_args-145"><a href="#get_args-145"><span class="linenos">145</span></a>        <span class="n">args</span><span class="o">.</span><span class="n">commit_all</span> <span class="o">=</span> <span class="s2">&quot;build&quot;</span>
-</span><span id="get_args-146"><a href="#get_args-146"><span class="linenos">146</span></a>        <span class="n">args</span><span class="o">.</span><span class="n">sync</span> <span class="o">=</span> <span class="kc">True</span>
-</span><span id="get_args-147"><a href="#get_args-147"><span class="linenos">147</span></a>
-</span><span id="get_args-148"><a href="#get_args-148"><span class="linenos">148</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">increment_version</span> <span class="ow">and</span> <span class="n">args</span><span class="o">.</span><span class="n">increment_version</span> <span class="ow">not</span> <span class="ow">in</span> <span class="p">[</span>
-</span><span id="get_args-149"><a href="#get_args-149"><span class="linenos">149</span></a>        <span class="s2">&quot;major&quot;</span><span class="p">,</span>
-</span><span id="get_args-150"><a href="#get_args-150"><span class="linenos">150</span></a>        <span class="s2">&quot;minor&quot;</span><span class="p">,</span>
-</span><span id="get_args-151"><a href="#get_args-151"><span class="linenos">151</span></a>        <span class="s2">&quot;patch&quot;</span><span class="p">,</span>
-</span><span id="get_args-152"><a href="#get_args-152"><span class="linenos">152</span></a>    <span class="p">]:</span>
-</span><span id="get_args-153"><a href="#get_args-153"><span class="linenos">153</span></a>        <span class="k">raise</span> <span class="ne">ValueError</span><span class="p">(</span>
-</span><span id="get_args-154"><a href="#get_args-154"><span class="linenos">154</span></a>            <span class="sa">f</span><span class="s2">&quot;Invalid option for -iv/--increment_version: </span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">increment_version</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="get_args-155"><a href="#get_args-155"><span class="linenos">155</span></a>        <span class="p">)</span>
-</span><span id="get_args-156"><a href="#get_args-156"><span class="linenos">156</span></a>
-</span><span id="get_args-157"><a href="#get_args-157"><span class="linenos">157</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">commit_all</span> <span class="o">==</span> <span class="s2">&quot;&quot;</span><span class="p">:</span>
-</span><span id="get_args-158"><a href="#get_args-158"><span class="linenos">158</span></a>        <span class="k">raise</span> <span class="ne">ValueError</span><span class="p">(</span><span class="s2">&quot;Commit message for args.commit_all cannot be empty.&quot;</span><span class="p">)</span>
-</span><span id="get_args-159"><a href="#get_args-159"><span class="linenos">159</span></a>
-</span><span id="get_args-160"><a href="#get_args-160"><span class="linenos">160</span></a>    <span class="k">return</span> <span class="n">args</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="get_args-17"><a href="#get_args-17"><span class="linenos"> 17</span></a><span class="k">def</span> <span class="nf">get_args</span><span class="p">()</span> <span class="o">-&gt;</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span><span class="p">:</span>
+</span><span id="get_args-18"><a href="#get_args-18"><span class="linenos"> 18</span></a>    <span class="n">parser</span> <span class="o">=</span> <span class="n">argparse</span><span class="o">.</span><span class="n">ArgumentParser</span><span class="p">()</span>
+</span><span id="get_args-19"><a href="#get_args-19"><span class="linenos"> 19</span></a>
+</span><span id="get_args-20"><a href="#get_args-20"><span class="linenos"> 20</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="get_args-21"><a href="#get_args-21"><span class="linenos"> 21</span></a>        <span class="s2">&quot;package&quot;</span><span class="p">,</span>
+</span><span id="get_args-22"><a href="#get_args-22"><span class="linenos"> 22</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
+</span><span id="get_args-23"><a href="#get_args-23"><span class="linenos"> 23</span></a>        <span class="n">default</span><span class="o">=</span><span class="s2">&quot;.&quot;</span><span class="p">,</span>
+</span><span id="get_args-24"><a href="#get_args-24"><span class="linenos"> 24</span></a>        <span class="n">nargs</span><span class="o">=</span><span class="s2">&quot;?&quot;</span><span class="p">,</span>
+</span><span id="get_args-25"><a href="#get_args-25"><span class="linenos"> 25</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; The name of the package or project to use,</span>
+</span><span id="get_args-26"><a href="#get_args-26"><span class="linenos"> 26</span></a><span class="s2">        assuming it&#39;s a subfolder of your current working directory.</span>
+</span><span id="get_args-27"><a href="#get_args-27"><span class="linenos"> 27</span></a><span class="s2">        Can also be a full path to the package. If nothing is given,</span>
+</span><span id="get_args-28"><a href="#get_args-28"><span class="linenos"> 28</span></a><span class="s2">        the current working directory will be used.&quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="get_args-29"><a href="#get_args-29"><span class="linenos"> 29</span></a>    <span class="p">)</span>
+</span><span id="get_args-30"><a href="#get_args-30"><span class="linenos"> 30</span></a>
+</span><span id="get_args-31"><a href="#get_args-31"><span class="linenos"> 31</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="get_args-32"><a href="#get_args-32"><span class="linenos"> 32</span></a>        <span class="s2">&quot;-b&quot;</span><span class="p">,</span> <span class="s2">&quot;--build&quot;</span><span class="p">,</span> <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span> <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Build the package. &quot;&quot;&quot;</span>
+</span><span id="get_args-33"><a href="#get_args-33"><span class="linenos"> 33</span></a>    <span class="p">)</span>
+</span><span id="get_args-34"><a href="#get_args-34"><span class="linenos"> 34</span></a>
+</span><span id="get_args-35"><a href="#get_args-35"><span class="linenos"> 35</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="get_args-36"><a href="#get_args-36"><span class="linenos"> 36</span></a>        <span class="s2">&quot;-t&quot;</span><span class="p">,</span>
+</span><span id="get_args-37"><a href="#get_args-37"><span class="linenos"> 37</span></a>        <span class="s2">&quot;--tag_version&quot;</span><span class="p">,</span>
+</span><span id="get_args-38"><a href="#get_args-38"><span class="linenos"> 38</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
+</span><span id="get_args-39"><a href="#get_args-39"><span class="linenos"> 39</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Add a git tag corresponding to the version in pyproject.toml. &quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="get_args-40"><a href="#get_args-40"><span class="linenos"> 40</span></a>    <span class="p">)</span>
+</span><span id="get_args-41"><a href="#get_args-41"><span class="linenos"> 41</span></a>
+</span><span id="get_args-42"><a href="#get_args-42"><span class="linenos"> 42</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="get_args-43"><a href="#get_args-43"><span class="linenos"> 43</span></a>        <span class="s2">&quot;-i&quot;</span><span class="p">,</span>
+</span><span id="get_args-44"><a href="#get_args-44"><span class="linenos"> 44</span></a>        <span class="s2">&quot;--install&quot;</span><span class="p">,</span>
+</span><span id="get_args-45"><a href="#get_args-45"><span class="linenos"> 45</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
+</span><span id="get_args-46"><a href="#get_args-46"><span class="linenos"> 46</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Install the package from source. &quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="get_args-47"><a href="#get_args-47"><span class="linenos"> 47</span></a>    <span class="p">)</span>
+</span><span id="get_args-48"><a href="#get_args-48"><span class="linenos"> 48</span></a>
+</span><span id="get_args-49"><a href="#get_args-49"><span class="linenos"> 49</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="get_args-50"><a href="#get_args-50"><span class="linenos"> 50</span></a>        <span class="s2">&quot;-iv&quot;</span><span class="p">,</span>
+</span><span id="get_args-51"><a href="#get_args-51"><span class="linenos"> 51</span></a>        <span class="s2">&quot;--increment_version&quot;</span><span class="p">,</span>
+</span><span id="get_args-52"><a href="#get_args-52"><span class="linenos"> 52</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
+</span><span id="get_args-53"><a href="#get_args-53"><span class="linenos"> 53</span></a>        <span class="n">default</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span>
+</span><span id="get_args-54"><a href="#get_args-54"><span class="linenos"> 54</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Increment version in pyproject.toml.</span>
+</span><span id="get_args-55"><a href="#get_args-55"><span class="linenos"> 55</span></a><span class="s2">        Can be one of &quot;major&quot;, &quot;minor&quot;, or &quot;patch&quot;. &quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="get_args-56"><a href="#get_args-56"><span class="linenos"> 56</span></a>    <span class="p">)</span>
+</span><span id="get_args-57"><a href="#get_args-57"><span class="linenos"> 57</span></a>
+</span><span id="get_args-58"><a href="#get_args-58"><span class="linenos"> 58</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="get_args-59"><a href="#get_args-59"><span class="linenos"> 59</span></a>        <span class="s2">&quot;-p&quot;</span><span class="p">,</span>
+</span><span id="get_args-60"><a href="#get_args-60"><span class="linenos"> 60</span></a>        <span class="s2">&quot;--publish&quot;</span><span class="p">,</span>
+</span><span id="get_args-61"><a href="#get_args-61"><span class="linenos"> 61</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
+</span><span id="get_args-62"><a href="#get_args-62"><span class="linenos"> 62</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Publish package to PyPi.</span>
+</span><span id="get_args-63"><a href="#get_args-63"><span class="linenos"> 63</span></a><span class="s2">        Note: You must have configured twine </span>
+</span><span id="get_args-64"><a href="#get_args-64"><span class="linenos"> 64</span></a><span class="s2">        and registered a PyPi account/generated an API</span>
+</span><span id="get_args-65"><a href="#get_args-65"><span class="linenos"> 65</span></a><span class="s2">        key to use this option.&quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="get_args-66"><a href="#get_args-66"><span class="linenos"> 66</span></a>    <span class="p">)</span>
+</span><span id="get_args-67"><a href="#get_args-67"><span class="linenos"> 67</span></a>
+</span><span id="get_args-68"><a href="#get_args-68"><span class="linenos"> 68</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="get_args-69"><a href="#get_args-69"><span class="linenos"> 69</span></a>        <span class="s2">&quot;-rt&quot;</span><span class="p">,</span>
+</span><span id="get_args-70"><a href="#get_args-70"><span class="linenos"> 70</span></a>        <span class="s2">&quot;--run_tests&quot;</span><span class="p">,</span>
+</span><span id="get_args-71"><a href="#get_args-71"><span class="linenos"> 71</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
+</span><span id="get_args-72"><a href="#get_args-72"><span class="linenos"> 72</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Run tests for the package. &quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="get_args-73"><a href="#get_args-73"><span class="linenos"> 73</span></a>    <span class="p">)</span>
+</span><span id="get_args-74"><a href="#get_args-74"><span class="linenos"> 74</span></a>
+</span><span id="get_args-75"><a href="#get_args-75"><span class="linenos"> 75</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="get_args-76"><a href="#get_args-76"><span class="linenos"> 76</span></a>        <span class="s2">&quot;-gt&quot;</span><span class="p">,</span>
+</span><span id="get_args-77"><a href="#get_args-77"><span class="linenos"> 77</span></a>        <span class="s2">&quot;--generate_tests&quot;</span><span class="p">,</span>
+</span><span id="get_args-78"><a href="#get_args-78"><span class="linenos"> 78</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
+</span><span id="get_args-79"><a href="#get_args-79"><span class="linenos"> 79</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Generate tests for the package. &quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="get_args-80"><a href="#get_args-80"><span class="linenos"> 80</span></a>    <span class="p">)</span>
+</span><span id="get_args-81"><a href="#get_args-81"><span class="linenos"> 81</span></a>
+</span><span id="get_args-82"><a href="#get_args-82"><span class="linenos"> 82</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="get_args-83"><a href="#get_args-83"><span class="linenos"> 83</span></a>        <span class="s2">&quot;-uc&quot;</span><span class="p">,</span>
+</span><span id="get_args-84"><a href="#get_args-84"><span class="linenos"> 84</span></a>        <span class="s2">&quot;--update_changelog&quot;</span><span class="p">,</span>
+</span><span id="get_args-85"><a href="#get_args-85"><span class="linenos"> 85</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
+</span><span id="get_args-86"><a href="#get_args-86"><span class="linenos"> 86</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Update changelog file. &quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="get_args-87"><a href="#get_args-87"><span class="linenos"> 87</span></a>    <span class="p">)</span>
+</span><span id="get_args-88"><a href="#get_args-88"><span class="linenos"> 88</span></a>
+</span><span id="get_args-89"><a href="#get_args-89"><span class="linenos"> 89</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="get_args-90"><a href="#get_args-90"><span class="linenos"> 90</span></a>        <span class="s2">&quot;-od&quot;</span><span class="p">,</span>
+</span><span id="get_args-91"><a href="#get_args-91"><span class="linenos"> 91</span></a>        <span class="s2">&quot;--overwrite_dependencies&quot;</span><span class="p">,</span>
+</span><span id="get_args-92"><a href="#get_args-92"><span class="linenos"> 92</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
+</span><span id="get_args-93"><a href="#get_args-93"><span class="linenos"> 93</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; When building a package, packagelister will be used</span>
+</span><span id="get_args-94"><a href="#get_args-94"><span class="linenos"> 94</span></a><span class="s2">        to update the dependencies list in pyproject.toml.</span>
+</span><span id="get_args-95"><a href="#get_args-95"><span class="linenos"> 95</span></a><span class="s2">        The default behavior is to append any new dependencies to</span>
+</span><span id="get_args-96"><a href="#get_args-96"><span class="linenos"> 96</span></a><span class="s2">        the current list so as not to erase any manually added dependencies</span>
+</span><span id="get_args-97"><a href="#get_args-97"><span class="linenos"> 97</span></a><span class="s2">        that packagelister may not detect. If you don&#39;t have any manually </span>
+</span><span id="get_args-98"><a href="#get_args-98"><span class="linenos"> 98</span></a><span class="s2">        added dependencies and want to remove any dependencies that your</span>
+</span><span id="get_args-99"><a href="#get_args-99"><span class="linenos"> 99</span></a><span class="s2">        project no longer uses, pass this flag.&quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="get_args-100"><a href="#get_args-100"><span class="linenos">100</span></a>    <span class="p">)</span>
+</span><span id="get_args-101"><a href="#get_args-101"><span class="linenos">101</span></a>
+</span><span id="get_args-102"><a href="#get_args-102"><span class="linenos">102</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="get_args-103"><a href="#get_args-103"><span class="linenos">103</span></a>        <span class="s2">&quot;-ca&quot;</span><span class="p">,</span>
+</span><span id="get_args-104"><a href="#get_args-104"><span class="linenos">104</span></a>        <span class="s2">&quot;--commit_all&quot;</span><span class="p">,</span>
+</span><span id="get_args-105"><a href="#get_args-105"><span class="linenos">105</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
+</span><span id="get_args-106"><a href="#get_args-106"><span class="linenos">106</span></a>        <span class="n">default</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span>
+</span><span id="get_args-107"><a href="#get_args-107"><span class="linenos">107</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Git stage and commit all tracked files</span>
+</span><span id="get_args-108"><a href="#get_args-108"><span class="linenos">108</span></a><span class="s2">        with this supplied commit message.</span>
+</span><span id="get_args-109"><a href="#get_args-109"><span class="linenos">109</span></a><span class="s2">        If &#39;build&#39; is passed, all commits will have</span>
+</span><span id="get_args-110"><a href="#get_args-110"><span class="linenos">110</span></a><span class="s2">        message: &#39;chore: build v</span><span class="si">{current_version}</span><span class="s2">&quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="get_args-111"><a href="#get_args-111"><span class="linenos">111</span></a>    <span class="p">)</span>
+</span><span id="get_args-112"><a href="#get_args-112"><span class="linenos">112</span></a>
+</span><span id="get_args-113"><a href="#get_args-113"><span class="linenos">113</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="get_args-114"><a href="#get_args-114"><span class="linenos">114</span></a>        <span class="s2">&quot;-s&quot;</span><span class="p">,</span>
+</span><span id="get_args-115"><a href="#get_args-115"><span class="linenos">115</span></a>        <span class="s2">&quot;--sync&quot;</span><span class="p">,</span>
+</span><span id="get_args-116"><a href="#get_args-116"><span class="linenos">116</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
+</span><span id="get_args-117"><a href="#get_args-117"><span class="linenos">117</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Pull from github, then push current commit to repo. &quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="get_args-118"><a href="#get_args-118"><span class="linenos">118</span></a>    <span class="p">)</span>
+</span><span id="get_args-119"><a href="#get_args-119"><span class="linenos">119</span></a>
+</span><span id="get_args-120"><a href="#get_args-120"><span class="linenos">120</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="get_args-121"><a href="#get_args-121"><span class="linenos">121</span></a>        <span class="s2">&quot;-dv&quot;</span><span class="p">,</span>
+</span><span id="get_args-122"><a href="#get_args-122"><span class="linenos">122</span></a>        <span class="s2">&quot;--dependency_versions&quot;</span><span class="p">,</span>
+</span><span id="get_args-123"><a href="#get_args-123"><span class="linenos">123</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
+</span><span id="get_args-124"><a href="#get_args-124"><span class="linenos">124</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Include version specifiers for dependencies in</span>
+</span><span id="get_args-125"><a href="#get_args-125"><span class="linenos">125</span></a><span class="s2">        pyproject.toml.&quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="get_args-126"><a href="#get_args-126"><span class="linenos">126</span></a>    <span class="p">)</span>
+</span><span id="get_args-127"><a href="#get_args-127"><span class="linenos">127</span></a>
+</span><span id="get_args-128"><a href="#get_args-128"><span class="linenos">128</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="get_args-129"><a href="#get_args-129"><span class="linenos">129</span></a>        <span class="s2">&quot;-up&quot;</span><span class="p">,</span>
+</span><span id="get_args-130"><a href="#get_args-130"><span class="linenos">130</span></a>        <span class="s2">&quot;--update&quot;</span><span class="p">,</span>
+</span><span id="get_args-131"><a href="#get_args-131"><span class="linenos">131</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
+</span><span id="get_args-132"><a href="#get_args-132"><span class="linenos">132</span></a>        <span class="n">default</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span>
+</span><span id="get_args-133"><a href="#get_args-133"><span class="linenos">133</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Excpects one argument: &quot;major&quot;, &quot;minor&quot;, or &quot;patch&quot;.</span>
+</span><span id="get_args-134"><a href="#get_args-134"><span class="linenos">134</span></a><span class="s2">        Passing &quot;-up minor&quot; is equivalent to passing the cli string: &quot;-b -t -i -iv minor -uc -ca build -s&quot;.</span>
+</span><span id="get_args-135"><a href="#get_args-135"><span class="linenos">135</span></a><span class="s2">        To publish the updated package, the -p/--publish switch needs to be added to the cli input.&quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="get_args-136"><a href="#get_args-136"><span class="linenos">136</span></a>    <span class="p">)</span>
+</span><span id="get_args-137"><a href="#get_args-137"><span class="linenos">137</span></a>
+</span><span id="get_args-138"><a href="#get_args-138"><span class="linenos">138</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="get_args-139"><a href="#get_args-139"><span class="linenos">139</span></a>        <span class="s2">&quot;-st&quot;</span><span class="p">,</span>
+</span><span id="get_args-140"><a href="#get_args-140"><span class="linenos">140</span></a>        <span class="s2">&quot;--skip_tests&quot;</span><span class="p">,</span>
+</span><span id="get_args-141"><a href="#get_args-141"><span class="linenos">141</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
+</span><span id="get_args-142"><a href="#get_args-142"><span class="linenos">142</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Don&#39;t run tests when using the -b/--build command. &quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="get_args-143"><a href="#get_args-143"><span class="linenos">143</span></a>    <span class="p">)</span>
+</span><span id="get_args-144"><a href="#get_args-144"><span class="linenos">144</span></a>
+</span><span id="get_args-145"><a href="#get_args-145"><span class="linenos">145</span></a>    <span class="n">args</span> <span class="o">=</span> <span class="n">parser</span><span class="o">.</span><span class="n">parse_args</span><span class="p">()</span>
+</span><span id="get_args-146"><a href="#get_args-146"><span class="linenos">146</span></a>
+</span><span id="get_args-147"><a href="#get_args-147"><span class="linenos">147</span></a>    <span class="n">args</span><span class="o">.</span><span class="n">package</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="p">)</span><span class="o">.</span><span class="n">resolve</span><span class="p">()</span>
+</span><span id="get_args-148"><a href="#get_args-148"><span class="linenos">148</span></a>
+</span><span id="get_args-149"><a href="#get_args-149"><span class="linenos">149</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">update</span><span class="p">:</span>
+</span><span id="get_args-150"><a href="#get_args-150"><span class="linenos">150</span></a>        <span class="n">args</span><span class="o">.</span><span class="n">build</span> <span class="o">=</span> <span class="kc">True</span>
+</span><span id="get_args-151"><a href="#get_args-151"><span class="linenos">151</span></a>        <span class="n">args</span><span class="o">.</span><span class="n">tag_version</span> <span class="o">=</span> <span class="kc">True</span>
+</span><span id="get_args-152"><a href="#get_args-152"><span class="linenos">152</span></a>        <span class="n">args</span><span class="o">.</span><span class="n">install</span> <span class="o">=</span> <span class="kc">True</span>
+</span><span id="get_args-153"><a href="#get_args-153"><span class="linenos">153</span></a>        <span class="n">args</span><span class="o">.</span><span class="n">increment_version</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">update</span>
+</span><span id="get_args-154"><a href="#get_args-154"><span class="linenos">154</span></a>        <span class="n">args</span><span class="o">.</span><span class="n">update_changelog</span> <span class="o">=</span> <span class="kc">True</span>
+</span><span id="get_args-155"><a href="#get_args-155"><span class="linenos">155</span></a>        <span class="n">args</span><span class="o">.</span><span class="n">commit_all</span> <span class="o">=</span> <span class="s2">&quot;build&quot;</span>
+</span><span id="get_args-156"><a href="#get_args-156"><span class="linenos">156</span></a>        <span class="n">args</span><span class="o">.</span><span class="n">sync</span> <span class="o">=</span> <span class="kc">True</span>
+</span><span id="get_args-157"><a href="#get_args-157"><span class="linenos">157</span></a>
+</span><span id="get_args-158"><a href="#get_args-158"><span class="linenos">158</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">increment_version</span> <span class="ow">and</span> <span class="n">args</span><span class="o">.</span><span class="n">increment_version</span> <span class="ow">not</span> <span class="ow">in</span> <span class="p">[</span>
+</span><span id="get_args-159"><a href="#get_args-159"><span class="linenos">159</span></a>        <span class="s2">&quot;major&quot;</span><span class="p">,</span>
+</span><span id="get_args-160"><a href="#get_args-160"><span class="linenos">160</span></a>        <span class="s2">&quot;minor&quot;</span><span class="p">,</span>
+</span><span id="get_args-161"><a href="#get_args-161"><span class="linenos">161</span></a>        <span class="s2">&quot;patch&quot;</span><span class="p">,</span>
+</span><span id="get_args-162"><a href="#get_args-162"><span class="linenos">162</span></a>    <span class="p">]:</span>
+</span><span id="get_args-163"><a href="#get_args-163"><span class="linenos">163</span></a>        <span class="k">raise</span> <span class="ne">ValueError</span><span class="p">(</span>
+</span><span id="get_args-164"><a href="#get_args-164"><span class="linenos">164</span></a>            <span class="sa">f</span><span class="s2">&quot;Invalid option for -iv/--increment_version: </span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">increment_version</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="get_args-165"><a href="#get_args-165"><span class="linenos">165</span></a>        <span class="p">)</span>
+</span><span id="get_args-166"><a href="#get_args-166"><span class="linenos">166</span></a>
+</span><span id="get_args-167"><a href="#get_args-167"><span class="linenos">167</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">commit_all</span> <span class="o">==</span> <span class="s2">&quot;&quot;</span><span class="p">:</span>
+</span><span id="get_args-168"><a href="#get_args-168"><span class="linenos">168</span></a>        <span class="k">raise</span> <span class="ne">ValueError</span><span class="p">(</span><span class="s2">&quot;Commit message for args.commit_all cannot be empty.&quot;</span><span class="p">)</span>
+</span><span id="get_args-169"><a href="#get_args-169"><span class="linenos">169</span></a>
+</span><span id="get_args-170"><a href="#get_args-170"><span class="linenos">170</span></a>    <span class="k">return</span> <span class="n">args</span>
 </span></pre></div>
 
 
     
 
                 </section>
+                <section id="build">
+                            <input id="build-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
+<div class="attr function">
+            
+        <span class="def">def</span>
+        <span class="name">build</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="n">package_dir</span><span class="p">:</span> <span class="n">pathier</span><span class="o">.</span><span class="n">pathier</span><span class="o">.</span><span class="n">Pathier</span>,</span><span class="param">	<span class="n">skip_tests</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span>,</span><span class="param">	<span class="n">overwrite_dependencies</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span></span><span class="return-annotation">):</span></span>
+
+                <label class="view-source-button" for="build-view-source"><span>View Source</span></label>
+
+    </div>
+    <a class="headerlink" href="#build"></a>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="build-173"><a href="#build-173"><span class="linenos">173</span></a><span class="k">def</span> <span class="nf">build</span><span class="p">(</span>
+</span><span id="build-174"><a href="#build-174"><span class="linenos">174</span></a>    <span class="n">package_dir</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">,</span> <span class="n">skip_tests</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">,</span> <span class="n">overwrite_dependencies</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span>
+</span><span id="build-175"><a href="#build-175"><span class="linenos">175</span></a><span class="p">):</span>
+</span><span id="build-176"><a href="#build-176"><span class="linenos">176</span></a>    <span class="sd">&quot;&quot;&quot;Perform the build process.</span>
+</span><span id="build-177"><a href="#build-177"><span class="linenos">177</span></a>
+</span><span id="build-178"><a href="#build-178"><span class="linenos">178</span></a><span class="sd">    Steps:</span>
+</span><span id="build-179"><a href="#build-179"><span class="linenos">179</span></a><span class="sd">    * Run tests (unless `skip_tests` is `True`)</span>
+</span><span id="build-180"><a href="#build-180"><span class="linenos">180</span></a><span class="sd">    * Raise error and abandon build if tests fail</span>
+</span><span id="build-181"><a href="#build-181"><span class="linenos">181</span></a><span class="sd">    * Format source code with `Black`</span>
+</span><span id="build-182"><a href="#build-182"><span class="linenos">182</span></a><span class="sd">    * Sort source code imports with `isort`</span>
+</span><span id="build-183"><a href="#build-183"><span class="linenos">183</span></a><span class="sd">    * Update project dependencies in `pyproject.toml`</span>
+</span><span id="build-184"><a href="#build-184"><span class="linenos">184</span></a><span class="sd">    * Generate docs</span>
+</span><span id="build-185"><a href="#build-185"><span class="linenos">185</span></a><span class="sd">    * Delete previous `dist` folder contents</span>
+</span><span id="build-186"><a href="#build-186"><span class="linenos">186</span></a><span class="sd">    * Invoke build module&quot;&quot;&quot;</span>
+</span><span id="build-187"><a href="#build-187"><span class="linenos">187</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">skip_tests</span> <span class="ow">and</span> <span class="ow">not</span> <span class="n">run_tests</span><span class="p">(</span><span class="n">package_dir</span><span class="p">):</span>
+</span><span id="build-188"><a href="#build-188"><span class="linenos">188</span></a>        <span class="k">raise</span> <span class="ne">RuntimeError</span><span class="p">(</span>
+</span><span id="build-189"><a href="#build-189"><span class="linenos">189</span></a>            <span class="sa">f</span><span class="s2">&quot;ERROR: </span><span class="si">{</span><span class="n">package_dir</span><span class="o">.</span><span class="n">stem</span><span class="si">}</span><span class="s2"> failed testing.</span><span class="se">\n</span><span class="s2">Abandoning build.&quot;</span>
+</span><span id="build-190"><a href="#build-190"><span class="linenos">190</span></a>        <span class="p">)</span>
+</span><span id="build-191"><a href="#build-191"><span class="linenos">191</span></a>    <span class="n">hassle_utilities</span><span class="o">.</span><span class="n">format_files</span><span class="p">(</span><span class="n">package_dir</span><span class="p">)</span>
+</span><span id="build-192"><a href="#build-192"><span class="linenos">192</span></a>    <span class="p">[</span><span class="n">isort</span><span class="o">.</span><span class="n">file</span><span class="p">(</span><span class="n">path</span><span class="p">)</span> <span class="k">for</span> <span class="n">path</span> <span class="ow">in</span> <span class="n">package_dir</span><span class="o">.</span><span class="n">rglob</span><span class="p">(</span><span class="s2">&quot;*.py&quot;</span><span class="p">)]</span>
+</span><span id="build-193"><a href="#build-193"><span class="linenos">193</span></a>    <span class="n">hassle_utilities</span><span class="o">.</span><span class="n">update_dependencies</span><span class="p">(</span>
+</span><span id="build-194"><a href="#build-194"><span class="linenos">194</span></a>        <span class="n">package_dir</span> <span class="o">/</span> <span class="s2">&quot;pyproject.toml&quot;</span><span class="p">,</span> <span class="n">overwrite_dependencies</span>
+</span><span id="build-195"><a href="#build-195"><span class="linenos">195</span></a>    <span class="p">)</span>
+</span><span id="build-196"><a href="#build-196"><span class="linenos">196</span></a>    <span class="c1"># Vermin isn&#39;t taking into account the minimum version of dependencies.</span>
+</span><span id="build-197"><a href="#build-197"><span class="linenos">197</span></a>    <span class="c1"># Removing from now and defaulting to &gt;=3.10</span>
+</span><span id="build-198"><a href="#build-198"><span class="linenos">198</span></a>    <span class="c1"># hassle_utilities.update_minimum_python_version(pyproject_path)</span>
+</span><span id="build-199"><a href="#build-199"><span class="linenos">199</span></a>    <span class="n">hassle_utilities</span><span class="o">.</span><span class="n">generate_docs</span><span class="p">(</span><span class="n">package_dir</span><span class="p">)</span>
+</span><span id="build-200"><a href="#build-200"><span class="linenos">200</span></a>    <span class="p">(</span><span class="n">package_dir</span> <span class="o">/</span> <span class="s2">&quot;dist&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">delete</span><span class="p">()</span>
+</span><span id="build-201"><a href="#build-201"><span class="linenos">201</span></a>    <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">sys</span><span class="o">.</span><span class="n">executable</span><span class="si">}</span><span class="s2"> -m build </span><span class="si">{</span><span class="n">package_dir</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span></pre></div>
+
+
+            <div class="docstring"><p>Perform the build process.</p>
+
+<p>Steps:</p>
+
+<ul>
+<li>Run tests (unless <code>skip_tests</code> is <code>True</code>)</li>
+<li>Raise error and abandon build if tests fail</li>
+<li>Format source code with <code>Black</code></li>
+<li>Sort source code imports with <code>isort</code></li>
+<li>Update project dependencies in <code>pyproject.toml</code></li>
+<li>Generate docs</li>
+<li>Delete previous <code>dist</code> folder contents</li>
+<li>Invoke build module</li>
+</ul>
+</div>
+
+
+                </section>
                 <section id="main">
                             <input id="main-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
             
         <span class="def">def</span>
         <span class="name">main</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">args</span><span class="p">:</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span> <span class="o">=</span> <span class="kc">None</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="main-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#main"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="main-163"><a href="#main-163"><span class="linenos">163</span></a><span class="k">def</span> <span class="nf">main</span><span class="p">(</span><span class="n">args</span><span class="p">:</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span> <span class="o">=</span> <span class="kc">None</span><span class="p">):</span>
-</span><span id="main-164"><a href="#main-164"><span class="linenos">164</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="p">:</span>
-</span><span id="main-165"><a href="#main-165"><span class="linenos">165</span></a>        <span class="n">args</span> <span class="o">=</span> <span class="n">get_args</span><span class="p">()</span>
-</span><span id="main-166"><a href="#main-166"><span class="linenos">166</span></a>
-</span><span id="main-167"><a href="#main-167"><span class="linenos">167</span></a>    <span class="n">pyproject_path</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">package</span> <span class="o">/</span> <span class="s2">&quot;pyproject.toml&quot;</span>
-</span><span id="main-168"><a href="#main-168"><span class="linenos">168</span></a>
-</span><span id="main-169"><a href="#main-169"><span class="linenos">169</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">pyproject_path</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
-</span><span id="main-170"><a href="#main-170"><span class="linenos">170</span></a>        <span class="k">raise</span> <span class="ne">FileNotFoundError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Could not locate pyproject.toml for </span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="main-171"><a href="#main-171"><span class="linenos">171</span></a>
-</span><span id="main-172"><a href="#main-172"><span class="linenos">172</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">generate_tests</span><span class="p">:</span>
-</span><span id="main-173"><a href="#main-173"><span class="linenos">173</span></a>        <span class="n">generate_test_files</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="p">)</span>
-</span><span id="main-174"><a href="#main-174"><span class="linenos">174</span></a>
-</span><span id="main-175"><a href="#main-175"><span class="linenos">175</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">run_tests</span><span class="p">:</span>
-</span><span id="main-176"><a href="#main-176"><span class="linenos">176</span></a>        <span class="n">run_tests</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="p">)</span>
-</span><span id="main-177"><a href="#main-177"><span class="linenos">177</span></a>
-</span><span id="main-178"><a href="#main-178"><span class="linenos">178</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">increment_version</span><span class="p">:</span>
-</span><span id="main-179"><a href="#main-179"><span class="linenos">179</span></a>        <span class="n">hassle_utilities</span><span class="o">.</span><span class="n">increment_version</span><span class="p">(</span><span class="n">pyproject_path</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">increment_version</span><span class="p">)</span>
-</span><span id="main-180"><a href="#main-180"><span class="linenos">180</span></a>
-</span><span id="main-181"><a href="#main-181"><span class="linenos">181</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">build</span><span class="p">:</span>
-</span><span id="main-182"><a href="#main-182"><span class="linenos">182</span></a>        <span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">package</span> <span class="o">/</span> <span class="s2">&quot;dist&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">delete</span><span class="p">()</span>
-</span><span id="main-183"><a href="#main-183"><span class="linenos">183</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;black </span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="main-184"><a href="#main-184"><span class="linenos">184</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;isort </span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="main-185"><a href="#main-185"><span class="linenos">185</span></a>        <span class="n">hassle_utilities</span><span class="o">.</span><span class="n">update_dependencies</span><span class="p">(</span>
-</span><span id="main-186"><a href="#main-186"><span class="linenos">186</span></a>            <span class="n">pyproject_path</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">overwrite_dependencies</span>
-</span><span id="main-187"><a href="#main-187"><span class="linenos">187</span></a>        <span class="p">)</span>
-</span><span id="main-188"><a href="#main-188"><span class="linenos">188</span></a>        <span class="c1"># Vermin isn&#39;t taking into account the minimum version of dependencies.</span>
-</span><span id="main-189"><a href="#main-189"><span class="linenos">189</span></a>        <span class="c1"># Removing from now and defaulting to &gt;=3.10</span>
-</span><span id="main-190"><a href="#main-190"><span class="linenos">190</span></a>        <span class="c1"># hassle_utilities.update_minimum_python_version(pyproject_path)</span>
-</span><span id="main-191"><a href="#main-191"><span class="linenos">191</span></a>        <span class="n">hassle_utilities</span><span class="o">.</span><span class="n">generate_docs</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="p">)</span>
-</span><span id="main-192"><a href="#main-192"><span class="linenos">192</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;py -m build </span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="main-193"><a href="#main-193"><span class="linenos">193</span></a>
-</span><span id="main-194"><a href="#main-194"><span class="linenos">194</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">update_changelog</span><span class="p">:</span>
-</span><span id="main-195"><a href="#main-195"><span class="linenos">195</span></a>        <span class="n">hassle_utilities</span><span class="o">.</span><span class="n">update_changelog</span><span class="p">(</span><span class="n">pyproject_path</span><span class="p">)</span>
-</span><span id="main-196"><a href="#main-196"><span class="linenos">196</span></a>        <span class="c1"># If we&#39;re going to add tag for current version</span>
-</span><span id="main-197"><a href="#main-197"><span class="linenos">197</span></a>        <span class="c1"># commit changelog first</span>
-</span><span id="main-198"><a href="#main-198"><span class="linenos">198</span></a>        <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">tag_version</span><span class="p">:</span>
-</span><span id="main-199"><a href="#main-199"><span class="linenos">199</span></a>            <span class="nb">input</span><span class="p">(</span>
-</span><span id="main-200"><a href="#main-200"><span class="linenos">200</span></a>                <span class="s2">&quot;Press enter to continue after optionally pruning the updated changelog...&quot;</span>
-</span><span id="main-201"><a href="#main-201"><span class="linenos">201</span></a>            <span class="p">)</span>
-</span><span id="main-202"><a href="#main-202"><span class="linenos">202</span></a>            <span class="n">os</span><span class="o">.</span><span class="n">chdir</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="p">)</span>
-</span><span id="main-203"><a href="#main-203"><span class="linenos">203</span></a>            <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="s2">&quot;git add CHANGELOG.md&quot;</span><span class="p">)</span>
-</span><span id="main-204"><a href="#main-204"><span class="linenos">204</span></a>            <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="s1">&#39;git commit CHANGELOG.md -m &quot;chore: update changelog&quot;&#39;</span><span class="p">)</span>
-</span><span id="main-205"><a href="#main-205"><span class="linenos">205</span></a>
-</span><span id="main-206"><a href="#main-206"><span class="linenos">206</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">commit_all</span><span class="p">:</span>
-</span><span id="main-207"><a href="#main-207"><span class="linenos">207</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">chdir</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="p">)</span>
-</span><span id="main-208"><a href="#main-208"><span class="linenos">208</span></a>        <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">commit_all</span> <span class="o">==</span> <span class="s2">&quot;build&quot;</span><span class="p">:</span>
-</span><span id="main-209"><a href="#main-209"><span class="linenos">209</span></a>            <span class="n">version</span> <span class="o">=</span> <span class="n">pyproject_path</span><span class="o">.</span><span class="n">loads</span><span class="p">()[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;version&quot;</span><span class="p">]</span>
-</span><span id="main-210"><a href="#main-210"><span class="linenos">210</span></a>            <span class="n">args</span><span class="o">.</span><span class="n">commit_all</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;chore: build v</span><span class="si">{</span><span class="n">version</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="main-211"><a href="#main-211"><span class="linenos">211</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="s2">&quot;git add .&quot;</span><span class="p">)</span>
-</span><span id="main-212"><a href="#main-212"><span class="linenos">212</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;git commit -m &quot;</span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">commit_all</span><span class="si">}</span><span class="s1">&quot;&#39;</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="main-204"><a href="#main-204"><span class="linenos">204</span></a><span class="k">def</span> <span class="nf">main</span><span class="p">(</span><span class="n">args</span><span class="p">:</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span> <span class="o">=</span> <span class="kc">None</span><span class="p">):</span>
+</span><span id="main-205"><a href="#main-205"><span class="linenos">205</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="p">:</span>
+</span><span id="main-206"><a href="#main-206"><span class="linenos">206</span></a>        <span class="n">args</span> <span class="o">=</span> <span class="n">get_args</span><span class="p">()</span>
+</span><span id="main-207"><a href="#main-207"><span class="linenos">207</span></a>
+</span><span id="main-208"><a href="#main-208"><span class="linenos">208</span></a>    <span class="n">pyproject_path</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">package</span> <span class="o">/</span> <span class="s2">&quot;pyproject.toml&quot;</span>
+</span><span id="main-209"><a href="#main-209"><span class="linenos">209</span></a>    <span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="o">.</span><span class="n">mkcwd</span><span class="p">()</span>
+</span><span id="main-210"><a href="#main-210"><span class="linenos">210</span></a>
+</span><span id="main-211"><a href="#main-211"><span class="linenos">211</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">pyproject_path</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
+</span><span id="main-212"><a href="#main-212"><span class="linenos">212</span></a>        <span class="k">raise</span> <span class="ne">FileNotFoundError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Could not locate pyproject.toml for </span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
 </span><span id="main-213"><a href="#main-213"><span class="linenos">213</span></a>
-</span><span id="main-214"><a href="#main-214"><span class="linenos">214</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">tag_version</span><span class="p">:</span>
-</span><span id="main-215"><a href="#main-215"><span class="linenos">215</span></a>        <span class="n">hassle_utilities</span><span class="o">.</span><span class="n">tag_version</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="p">)</span>
+</span><span id="main-214"><a href="#main-214"><span class="linenos">214</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">generate_tests</span><span class="p">:</span>
+</span><span id="main-215"><a href="#main-215"><span class="linenos">215</span></a>        <span class="n">generate_test_files</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="p">)</span>
 </span><span id="main-216"><a href="#main-216"><span class="linenos">216</span></a>
-</span><span id="main-217"><a href="#main-217"><span class="linenos">217</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">publish</span><span class="p">:</span>
-</span><span id="main-218"><a href="#main-218"><span class="linenos">218</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;twine upload </span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">package</span> <span class="o">/</span> <span class="s1">&#39;dist&#39;</span> <span class="o">/</span> <span class="s1">&#39;*&#39;</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="main-217"><a href="#main-217"><span class="linenos">217</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">run_tests</span><span class="p">:</span>
+</span><span id="main-218"><a href="#main-218"><span class="linenos">218</span></a>        <span class="n">run_tests</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="p">)</span>
 </span><span id="main-219"><a href="#main-219"><span class="linenos">219</span></a>
-</span><span id="main-220"><a href="#main-220"><span class="linenos">220</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">install</span><span class="p">:</span>
-</span><span id="main-221"><a href="#main-221"><span class="linenos">221</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;pip install </span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="si">}</span><span class="s2"> --no-deps --upgrade --no-cache-dir&quot;</span><span class="p">)</span>
+</span><span id="main-220"><a href="#main-220"><span class="linenos">220</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">increment_version</span><span class="p">:</span>
+</span><span id="main-221"><a href="#main-221"><span class="linenos">221</span></a>        <span class="n">hassle_utilities</span><span class="o">.</span><span class="n">increment_version</span><span class="p">(</span><span class="n">pyproject_path</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">increment_version</span><span class="p">)</span>
 </span><span id="main-222"><a href="#main-222"><span class="linenos">222</span></a>
-</span><span id="main-223"><a href="#main-223"><span class="linenos">223</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">sync</span><span class="p">:</span>
-</span><span id="main-224"><a href="#main-224"><span class="linenos">224</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">chdir</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="p">)</span>
-</span><span id="main-225"><a href="#main-225"><span class="linenos">225</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;git pull --tags origin main&quot;</span><span class="p">)</span>
-</span><span id="main-226"><a href="#main-226"><span class="linenos">226</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;git push origin main:main --tags&quot;</span><span class="p">)</span>
+</span><span id="main-223"><a href="#main-223"><span class="linenos">223</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">build</span><span class="p">:</span>
+</span><span id="main-224"><a href="#main-224"><span class="linenos">224</span></a>        <span class="n">build</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">skip_tests</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">overwrite_dependencies</span><span class="p">)</span>
+</span><span id="main-225"><a href="#main-225"><span class="linenos">225</span></a>
+</span><span id="main-226"><a href="#main-226"><span class="linenos">226</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">update_changelog</span><span class="p">:</span>
+</span><span id="main-227"><a href="#main-227"><span class="linenos">227</span></a>        <span class="n">hassle_utilities</span><span class="o">.</span><span class="n">update_changelog</span><span class="p">(</span><span class="n">pyproject_path</span><span class="p">)</span>
+</span><span id="main-228"><a href="#main-228"><span class="linenos">228</span></a>        <span class="c1"># If we&#39;re going to add tag for current version</span>
+</span><span id="main-229"><a href="#main-229"><span class="linenos">229</span></a>        <span class="c1"># commit changelog first</span>
+</span><span id="main-230"><a href="#main-230"><span class="linenos">230</span></a>        <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">tag_version</span><span class="p">:</span>
+</span><span id="main-231"><a href="#main-231"><span class="linenos">231</span></a>            <span class="nb">input</span><span class="p">(</span>
+</span><span id="main-232"><a href="#main-232"><span class="linenos">232</span></a>                <span class="s2">&quot;Press enter to continue after optionally pruning the updated changelog...&quot;</span>
+</span><span id="main-233"><a href="#main-233"><span class="linenos">233</span></a>            <span class="p">)</span>
+</span><span id="main-234"><a href="#main-234"><span class="linenos">234</span></a>            <span class="n">git</span><span class="o">.</span><span class="n">commit_files</span><span class="p">(</span>
+</span><span id="main-235"><a href="#main-235"><span class="linenos">235</span></a>                <span class="p">[</span><span class="nb">str</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">package</span> <span class="o">/</span> <span class="s2">&quot;CHANGELOG.md&quot;</span><span class="p">)],</span> <span class="s2">&quot;chore: update changelog&quot;</span>
+</span><span id="main-236"><a href="#main-236"><span class="linenos">236</span></a>            <span class="p">)</span>
+</span><span id="main-237"><a href="#main-237"><span class="linenos">237</span></a>
+</span><span id="main-238"><a href="#main-238"><span class="linenos">238</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">commit_all</span><span class="p">:</span>
+</span><span id="main-239"><a href="#main-239"><span class="linenos">239</span></a>        <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">commit_all</span> <span class="o">==</span> <span class="s2">&quot;build&quot;</span><span class="p">:</span>
+</span><span id="main-240"><a href="#main-240"><span class="linenos">240</span></a>            <span class="n">version</span> <span class="o">=</span> <span class="n">pyproject_path</span><span class="o">.</span><span class="n">loads</span><span class="p">()[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;version&quot;</span><span class="p">]</span>
+</span><span id="main-241"><a href="#main-241"><span class="linenos">241</span></a>            <span class="n">args</span><span class="o">.</span><span class="n">commit_all</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;chore: build v</span><span class="si">{</span><span class="n">version</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="main-242"><a href="#main-242"><span class="linenos">242</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">add</span><span class="p">()</span>
+</span><span id="main-243"><a href="#main-243"><span class="linenos">243</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">commit</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;-m &quot;</span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">commit_all</span><span class="si">}</span><span class="s1">&quot;&#39;</span><span class="p">)</span>
+</span><span id="main-244"><a href="#main-244"><span class="linenos">244</span></a>
+</span><span id="main-245"><a href="#main-245"><span class="linenos">245</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">tag_version</span><span class="p">:</span>
+</span><span id="main-246"><a href="#main-246"><span class="linenos">246</span></a>        <span class="n">hassle_utilities</span><span class="o">.</span><span class="n">tag_version</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="p">)</span>
+</span><span id="main-247"><a href="#main-247"><span class="linenos">247</span></a>
+</span><span id="main-248"><a href="#main-248"><span class="linenos">248</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">publish</span><span class="p">:</span>
+</span><span id="main-249"><a href="#main-249"><span class="linenos">249</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;twine upload </span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">package</span> <span class="o">/</span> <span class="s1">&#39;dist&#39;</span> <span class="o">/</span> <span class="s1">&#39;*&#39;</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="main-250"><a href="#main-250"><span class="linenos">250</span></a>
+</span><span id="main-251"><a href="#main-251"><span class="linenos">251</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">install</span><span class="p">:</span>
+</span><span id="main-252"><a href="#main-252"><span class="linenos">252</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;pip install </span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="si">}</span><span class="s2"> --no-deps --upgrade --no-cache-dir&quot;</span><span class="p">)</span>
+</span><span id="main-253"><a href="#main-253"><span class="linenos">253</span></a>
+</span><span id="main-254"><a href="#main-254"><span class="linenos">254</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">sync</span><span class="p">:</span>
+</span><span id="main-255"><a href="#main-255"><span class="linenos">255</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">pull</span><span class="p">(</span><span class="s2">&quot;--tags&quot;</span><span class="p">)</span>
+</span><span id="main-256"><a href="#main-256"><span class="linenos">256</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">push</span><span class="p">(</span><span class="s2">&quot;--tags&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
     
 
                 </section>
     </main>
```

#### html2text {}

```diff
@@ -1,480 +1,551 @@
 
 
   ⁰
 ____ hassle [Unknown INPUT type]
 ***** API Documentation *****
     * get_args
+    * build
     * main
 built_with_pdoc[pdoc_logo]
 
 ****** hassle.hassle ******
 ⁰ View Source
 __1import argparse
 __2import os
-__3
-__4from pathier import Pathier
-__5
-__6from hassle import hassle_utilities
-__7from hassle.generate_tests import generate_test_files
-__8from hassle.run_tests import run_tests
-__9
-_10root = Pathier(__file__).parent
-_11
+__3import sys
+__4
+__5import isort
+__6from gitbetter import git
+__7from pathier import Pathier
+__8
+__9from hassle import hassle_utilities
+_10from hassle.generate_tests import generate_test_files
+_11from hassle.run_tests import run_tests
 _12
-_13def get_args() -> argparse.Namespace:
-_14    parser = argparse.ArgumentParser()
+_13root = Pathier(__file__).parent
+_14
 _15
-_16    parser.add_argument(
-_17        "package",
-_18        type=str,
-_19        default=".",
-_20        nargs="?",
-_21        help=""" The name of the package or project to use,
-_22        assuming it's a subfolder of your current working directory.
-_23        Can also be a full path to the package. If nothing is given,
-_24        the current working directory will be used.""",
-_25    )
-_26
-_27    parser.add_argument(
-_28        "-b", "--build", action="store_true", help=""" Build the package.
+_16def get_args() -> argparse.Namespace:
+_17    parser = argparse.ArgumentParser()
+_18
+_19    parser.add_argument(
+_20        "package",
+_21        type=str,
+_22        default=".",
+_23        nargs="?",
+_24        help=""" The name of the package or project to use,
+_25        assuming it's a subfolder of your current working directory.
+_26        Can also be a full path to the package. If nothing is given,
+_27        the current working directory will be used.""",
+_28    )
+_29
+_30    parser.add_argument(
+_31        "-b", "--build", action="store_true", help=""" Build the package.
 """
-_29    )
-_30
-_31    parser.add_argument(
-_32        "-t",
-_33        "--tag_version",
-_34        action="store_true",
-_35        help=""" Add a git tag corresponding to the version in
+_32    )
+_33
+_34    parser.add_argument(
+_35        "-t",
+_36        "--tag_version",
+_37        action="store_true",
+_38        help=""" Add a git tag corresponding to the version in
 pyproject.toml. """,
-_36    )
-_37
-_38    parser.add_argument(
-_39        "-i",
-_40        "--install",
-_41        action="store_true",
-_42        help=""" Install the package from source. """,
-_43    )
-_44
-_45    parser.add_argument(
-_46        "-iv",
-_47        "--increment_version",
-_48        type=str,
-_49        default=None,
-_50        help=""" Increment version in pyproject.toml.
-_51        Can be one of "major", "minor", or "patch". """,
-_52    )
-_53
-_54    parser.add_argument(
-_55        "-p",
-_56        "--publish",
-_57        action="store_true",
-_58        help=""" Publish package to PyPi.
-_59        Note: You must have configured twine
-_60        and registered a PyPi account/generated an API
-_61        key to use this option.""",
-_62    )
-_63
-_64    parser.add_argument(
-_65        "-rt",
-_66        "--run_tests",
-_67        action="store_true",
-_68        help=""" Run tests for the package. """,
-_69    )
-_70
-_71    parser.add_argument(
-_72        "-gt",
-_73        "--generate_tests",
-_74        action="store_true",
-_75        help=""" Generate tests for the package. """,
-_76    )
-_77
-_78    parser.add_argument(
-_79        "-uc",
-_80        "--update_changelog",
-_81        action="store_true",
-_82        help=""" Update changelog file. """,
-_83    )
-_84
-_85    parser.add_argument(
-_86        "-od",
-_87        "--overwrite_dependencies",
-_88        action="store_true",
-_89        help=""" When building a package, packagelister will be used
-_90        to update the dependencies list in pyproject.toml.
-_91        The default behavior is to append any new dependencies to
-_92        the current list so as not to erase any manually added dependencies
-_93        that packagelister may not detect. If you don't have any manually
-_94        added dependencies and want to remove any dependencies that your
-_95        project no longer uses, pass this flag.""",
-_96    )
-_97
-_98    parser.add_argument(
-_99        "-ca",
-100        "--commit_all",
-101        type=str,
-102        default=None,
-103        help=""" Git stage and commit all tracked files
-104        with this supplied commit message.
-105        If 'build' is passed, all commits will have
-106        message: 'chore: build v{current_version}""",
-107    )
-108
-109    parser.add_argument(
-110        "-s",
-111        "--sync",
-112        action="store_true",
-113        help=""" Pull from github, then push current commit to repo. """,
-114    )
-115
-116    parser.add_argument(
-117        "-dv",
-118        "--dependency_versions",
-119        action="store_true",
-120        help=""" Include version specifiers for dependencies in
-121        pyproject.toml.""",
-122    )
-123
-124    parser.add_argument(
-125        "-up",
-126        "--update",
-127        type=str,
-128        default=None,
-129        help=""" Excpects one argument: "major", "minor", or "patch".
-130        Passing "-up minor" is equivalent to passing the cli string: "-b -
+_39    )
+_40
+_41    parser.add_argument(
+_42        "-i",
+_43        "--install",
+_44        action="store_true",
+_45        help=""" Install the package from source. """,
+_46    )
+_47
+_48    parser.add_argument(
+_49        "-iv",
+_50        "--increment_version",
+_51        type=str,
+_52        default=None,
+_53        help=""" Increment version in pyproject.toml.
+_54        Can be one of "major", "minor", or "patch". """,
+_55    )
+_56
+_57    parser.add_argument(
+_58        "-p",
+_59        "--publish",
+_60        action="store_true",
+_61        help=""" Publish package to PyPi.
+_62        Note: You must have configured twine
+_63        and registered a PyPi account/generated an API
+_64        key to use this option.""",
+_65    )
+_66
+_67    parser.add_argument(
+_68        "-rt",
+_69        "--run_tests",
+_70        action="store_true",
+_71        help=""" Run tests for the package. """,
+_72    )
+_73
+_74    parser.add_argument(
+_75        "-gt",
+_76        "--generate_tests",
+_77        action="store_true",
+_78        help=""" Generate tests for the package. """,
+_79    )
+_80
+_81    parser.add_argument(
+_82        "-uc",
+_83        "--update_changelog",
+_84        action="store_true",
+_85        help=""" Update changelog file. """,
+_86    )
+_87
+_88    parser.add_argument(
+_89        "-od",
+_90        "--overwrite_dependencies",
+_91        action="store_true",
+_92        help=""" When building a package, packagelister will be used
+_93        to update the dependencies list in pyproject.toml.
+_94        The default behavior is to append any new dependencies to
+_95        the current list so as not to erase any manually added dependencies
+_96        that packagelister may not detect. If you don't have any manually
+_97        added dependencies and want to remove any dependencies that your
+_98        project no longer uses, pass this flag.""",
+_99    )
+100
+101    parser.add_argument(
+102        "-ca",
+103        "--commit_all",
+104        type=str,
+105        default=None,
+106        help=""" Git stage and commit all tracked files
+107        with this supplied commit message.
+108        If 'build' is passed, all commits will have
+109        message: 'chore: build v{current_version}""",
+110    )
+111
+112    parser.add_argument(
+113        "-s",
+114        "--sync",
+115        action="store_true",
+116        help=""" Pull from github, then push current commit to repo. """,
+117    )
+118
+119    parser.add_argument(
+120        "-dv",
+121        "--dependency_versions",
+122        action="store_true",
+123        help=""" Include version specifiers for dependencies in
+124        pyproject.toml.""",
+125    )
+126
+127    parser.add_argument(
+128        "-up",
+129        "--update",
+130        type=str,
+131        default=None,
+132        help=""" Excpects one argument: "major", "minor", or "patch".
+133        Passing "-up minor" is equivalent to passing the cli string: "-b -
 t -i -iv minor -uc -ca build -s".
-131        To publish the updated package, the -p/--publish switch needs to be
+134        To publish the updated package, the -p/--publish switch needs to be
 added to the cli input.""",
-132    )
-133
-134    args = parser.parse_args()
-135
-136    args.package = Pathier(args.package).resolve()
-137
-138    if args.update:
-139        args.build = True
-140        args.tag_version = True
-141        args.install = True
-142        args.increment_version = args.update
-143        args.update_changelog = True
-144        args.commit_all = "build"
-145        args.sync = True
-146
-147    if args.increment_version and args.increment_version not in [
-148        "major",
-149        "minor",
-150        "patch",
-151    ]:
-152        raise ValueError(
-153            f"Invalid option for -iv/--increment_version:
+135    )
+136
+137    parser.add_argument(
+138        "-st",
+139        "--skip_tests",
+140        action="store_true",
+141        help=""" Don't run tests when using the -b/--build command. """,
+142    )
+143
+144    args = parser.parse_args()
+145
+146    args.package = Pathier(args.package).resolve()
+147
+148    if args.update:
+149        args.build = True
+150        args.tag_version = True
+151        args.install = True
+152        args.increment_version = args.update
+153        args.update_changelog = True
+154        args.commit_all = "build"
+155        args.sync = True
+156
+157    if args.increment_version and args.increment_version not in [
+158        "major",
+159        "minor",
+160        "patch",
+161    ]:
+162        raise ValueError(
+163            f"Invalid option for -iv/--increment_version:
 {args.increment_version}"
-154        )
-155
-156    if args.commit_all == "":
-157        raise ValueError("Commit message for args.commit_all cannot be
-empty.")
-158
-159    return args
-160
-161
-162def main(args: argparse.Namespace = None):
-163    if not args:
-164        args = get_args()
+164        )
 165
-166    pyproject_path = args.package / "pyproject.toml"
-167
-168    if not pyproject_path.exists():
-169        raise FileNotFoundError(f"Could not locate pyproject.toml for
-{args.package}")
+166    if args.commit_all == "":
+167        raise ValueError("Commit message for args.commit_all cannot be
+empty.")
+168
+169    return args
 170
-171    if args.generate_tests:
-172        generate_test_files(args.package)
-173
-174    if args.run_tests:
-175        run_tests(args.package)
+171
+172def build(
+173    package_dir: Pathier, skip_tests: bool = False, overwrite_dependencies:
+bool = False
+174):
+175    """Perform the build process.
 176
-177    if args.increment_version:
-178        hassle_utilities.increment_version(pyproject_path,
-args.increment_version)
-179
-180    if args.build:
-181        (args.package / "dist").delete()
-182        os.system(f"black {args.package}")
-183        os.system(f"isort {args.package}")
-184        hassle_utilities.update_dependencies(
-185            pyproject_path, args.overwrite_dependencies
-186        )
-187        # Vermin isn't taking into account the minimum version of
-dependencies.
-188        # Removing from now and defaulting to >=3.10
-189        # hassle_utilities.update_minimum_python_version(pyproject_path)
-190        hassle_utilities.generate_docs(args.package)
-191        os.system(f"py -m build {args.package}")
-192
-193    if args.update_changelog:
-194        hassle_utilities.update_changelog(pyproject_path)
-195        # If we're going to add tag for current version
-196        # commit changelog first
-197        if args.tag_version:
-198            input(
-199                "Press enter to continue after optionally pruning the
-updated changelog..."
-200            )
-201            os.chdir(args.package)
-202            os.system("git add CHANGELOG.md")
-203            os.system('git commit CHANGELOG.md -m "chore: update
-changelog"')
-204
-205    if args.commit_all:
-206        os.chdir(args.package)
-207        if args.commit_all == "build":
-208            version = pyproject_path.loads()["project"]["version"]
-209            args.commit_all = f"chore: build v{version}"
-210        os.system("git add .")
-211        os.system(f'git commit -m "{args.commit_all}"')
+177    Steps:
+178    * Run tests (unless `skip_tests` is `True`)
+179    * Raise error and abandon build if tests fail
+180    * Format source code with `Black`
+181    * Sort source code imports with `isort`
+182    * Update project dependencies in `pyproject.toml`
+183    * Generate docs
+184    * Delete previous `dist` folder contents
+185    * Invoke build module"""
+186    if not skip_tests and not run_tests(package_dir):
+187        raise RuntimeError(
+188            f"ERROR: {package_dir.stem} failed testing.\nAbandoning build."
+189        )
+190    hassle_utilities.format_files(package_dir)
+191    [isort.file(path) for path in package_dir.rglob("*.py")]
+192    hassle_utilities.update_dependencies(
+193        package_dir / "pyproject.toml", overwrite_dependencies
+194    )
+195    # Vermin isn't taking into account the minimum version of dependencies.
+196    # Removing from now and defaulting to >=3.10
+197    # hassle_utilities.update_minimum_python_version(pyproject_path)
+198    hassle_utilities.generate_docs(package_dir)
+199    (package_dir / "dist").delete()
+200    os.system(f"{sys.executable} -m build {package_dir}")
+201
+202
+203def main(args: argparse.Namespace = None):
+204    if not args:
+205        args = get_args()
+206
+207    pyproject_path = args.package / "pyproject.toml"
+208    args.package.mkcwd()
+209
+210    if not pyproject_path.exists():
+211        raise FileNotFoundError(f"Could not locate pyproject.toml for
+{args.package}")
 212
-213    if args.tag_version:
-214        hassle_utilities.tag_version(args.package)
+213    if args.generate_tests:
+214        generate_test_files(args.package)
 215
-216    if args.publish:
-217        os.system(f"twine upload {args.package / 'dist' / '*'}")
+216    if args.run_tests:
+217        run_tests(args.package)
 218
-219    if args.install:
-220        os.system(f"pip install {args.package} --no-deps --upgrade --no-
-cache-dir")
+219    if args.increment_version:
+220        hassle_utilities.increment_version(pyproject_path,
+args.increment_version)
 221
-222    if args.sync:
-223        os.chdir(args.package)
-224        os.system(f"git pull --tags origin main")
-225        os.system(f"git push origin main:main --tags")
-226
-227
-228if __name__ == "__main__":
-229    main(get_args())
+222    if args.build:
+223        build(args.package, args.skip_tests, args.overwrite_dependencies)
+224
+225    if args.update_changelog:
+226        hassle_utilities.update_changelog(pyproject_path)
+227        # If we're going to add tag for current version
+228        # commit changelog first
+229        if args.tag_version:
+230            input(
+231                "Press enter to continue after optionally pruning the
+updated changelog..."
+232            )
+233            git.commit_files(
+234                [str(args.package / "CHANGELOG.md")], "chore: update
+changelog"
+235            )
+236
+237    if args.commit_all:
+238        if args.commit_all == "build":
+239            version = pyproject_path.loads()["project"]["version"]
+240            args.commit_all = f"chore: build v{version}"
+241        git.add()
+242        git.commit(f'-m "{args.commit_all}"')
+243
+244    if args.tag_version:
+245        hassle_utilities.tag_version(args.package)
+246
+247    if args.publish:
+248        os.system(f"twine upload {args.package / 'dist' / '*'}")
+249
+250    if args.install:
+251        os.system(f"pip install {args.package} --no-deps --upgrade --no-
+cache-dir")
+252
+253    if args.sync:
+254        git.pull("--tags")
+255        git.push("--tags")
+256
+257
+258if __name__ == "__main__":
+259    main(get_args())
   ⁰
 def get_args() -> argparse.Namespace: View Source
-_14def get_args() -> argparse.Namespace:
-_15    parser = argparse.ArgumentParser()
-_16
-_17    parser.add_argument(
-_18        "package",
-_19        type=str,
-_20        default=".",
-_21        nargs="?",
-_22        help=""" The name of the package or project to use,
-_23        assuming it's a subfolder of your current working directory.
-_24        Can also be a full path to the package. If nothing is given,
-_25        the current working directory will be used.""",
-_26    )
-_27
-_28    parser.add_argument(
-_29        "-b", "--build", action="store_true", help=""" Build the package.
+_17def get_args() -> argparse.Namespace:
+_18    parser = argparse.ArgumentParser()
+_19
+_20    parser.add_argument(
+_21        "package",
+_22        type=str,
+_23        default=".",
+_24        nargs="?",
+_25        help=""" The name of the package or project to use,
+_26        assuming it's a subfolder of your current working directory.
+_27        Can also be a full path to the package. If nothing is given,
+_28        the current working directory will be used.""",
+_29    )
+_30
+_31    parser.add_argument(
+_32        "-b", "--build", action="store_true", help=""" Build the package.
 """
-_30    )
-_31
-_32    parser.add_argument(
-_33        "-t",
-_34        "--tag_version",
-_35        action="store_true",
-_36        help=""" Add a git tag corresponding to the version in
+_33    )
+_34
+_35    parser.add_argument(
+_36        "-t",
+_37        "--tag_version",
+_38        action="store_true",
+_39        help=""" Add a git tag corresponding to the version in
 pyproject.toml. """,
-_37    )
-_38
-_39    parser.add_argument(
-_40        "-i",
-_41        "--install",
-_42        action="store_true",
-_43        help=""" Install the package from source. """,
-_44    )
-_45
-_46    parser.add_argument(
-_47        "-iv",
-_48        "--increment_version",
-_49        type=str,
-_50        default=None,
-_51        help=""" Increment version in pyproject.toml.
-_52        Can be one of "major", "minor", or "patch". """,
-_53    )
-_54
-_55    parser.add_argument(
-_56        "-p",
-_57        "--publish",
-_58        action="store_true",
-_59        help=""" Publish package to PyPi.
-_60        Note: You must have configured twine
-_61        and registered a PyPi account/generated an API
-_62        key to use this option.""",
-_63    )
-_64
-_65    parser.add_argument(
-_66        "-rt",
-_67        "--run_tests",
-_68        action="store_true",
-_69        help=""" Run tests for the package. """,
-_70    )
-_71
-_72    parser.add_argument(
-_73        "-gt",
-_74        "--generate_tests",
-_75        action="store_true",
-_76        help=""" Generate tests for the package. """,
-_77    )
-_78
-_79    parser.add_argument(
-_80        "-uc",
-_81        "--update_changelog",
-_82        action="store_true",
-_83        help=""" Update changelog file. """,
-_84    )
-_85
-_86    parser.add_argument(
-_87        "-od",
-_88        "--overwrite_dependencies",
-_89        action="store_true",
-_90        help=""" When building a package, packagelister will be used
-_91        to update the dependencies list in pyproject.toml.
-_92        The default behavior is to append any new dependencies to
-_93        the current list so as not to erase any manually added dependencies
-_94        that packagelister may not detect. If you don't have any manually
-_95        added dependencies and want to remove any dependencies that your
-_96        project no longer uses, pass this flag.""",
-_97    )
-_98
-_99    parser.add_argument(
-100        "-ca",
-101        "--commit_all",
-102        type=str,
-103        default=None,
-104        help=""" Git stage and commit all tracked files
-105        with this supplied commit message.
-106        If 'build' is passed, all commits will have
-107        message: 'chore: build v{current_version}""",
-108    )
-109
-110    parser.add_argument(
-111        "-s",
-112        "--sync",
-113        action="store_true",
-114        help=""" Pull from github, then push current commit to repo. """,
-115    )
-116
-117    parser.add_argument(
-118        "-dv",
-119        "--dependency_versions",
-120        action="store_true",
-121        help=""" Include version specifiers for dependencies in
-122        pyproject.toml.""",
-123    )
-124
-125    parser.add_argument(
-126        "-up",
-127        "--update",
-128        type=str,
-129        default=None,
-130        help=""" Excpects one argument: "major", "minor", or "patch".
-131        Passing "-up minor" is equivalent to passing the cli string: "-b -
+_40    )
+_41
+_42    parser.add_argument(
+_43        "-i",
+_44        "--install",
+_45        action="store_true",
+_46        help=""" Install the package from source. """,
+_47    )
+_48
+_49    parser.add_argument(
+_50        "-iv",
+_51        "--increment_version",
+_52        type=str,
+_53        default=None,
+_54        help=""" Increment version in pyproject.toml.
+_55        Can be one of "major", "minor", or "patch". """,
+_56    )
+_57
+_58    parser.add_argument(
+_59        "-p",
+_60        "--publish",
+_61        action="store_true",
+_62        help=""" Publish package to PyPi.
+_63        Note: You must have configured twine
+_64        and registered a PyPi account/generated an API
+_65        key to use this option.""",
+_66    )
+_67
+_68    parser.add_argument(
+_69        "-rt",
+_70        "--run_tests",
+_71        action="store_true",
+_72        help=""" Run tests for the package. """,
+_73    )
+_74
+_75    parser.add_argument(
+_76        "-gt",
+_77        "--generate_tests",
+_78        action="store_true",
+_79        help=""" Generate tests for the package. """,
+_80    )
+_81
+_82    parser.add_argument(
+_83        "-uc",
+_84        "--update_changelog",
+_85        action="store_true",
+_86        help=""" Update changelog file. """,
+_87    )
+_88
+_89    parser.add_argument(
+_90        "-od",
+_91        "--overwrite_dependencies",
+_92        action="store_true",
+_93        help=""" When building a package, packagelister will be used
+_94        to update the dependencies list in pyproject.toml.
+_95        The default behavior is to append any new dependencies to
+_96        the current list so as not to erase any manually added dependencies
+_97        that packagelister may not detect. If you don't have any manually
+_98        added dependencies and want to remove any dependencies that your
+_99        project no longer uses, pass this flag.""",
+100    )
+101
+102    parser.add_argument(
+103        "-ca",
+104        "--commit_all",
+105        type=str,
+106        default=None,
+107        help=""" Git stage and commit all tracked files
+108        with this supplied commit message.
+109        If 'build' is passed, all commits will have
+110        message: 'chore: build v{current_version}""",
+111    )
+112
+113    parser.add_argument(
+114        "-s",
+115        "--sync",
+116        action="store_true",
+117        help=""" Pull from github, then push current commit to repo. """,
+118    )
+119
+120    parser.add_argument(
+121        "-dv",
+122        "--dependency_versions",
+123        action="store_true",
+124        help=""" Include version specifiers for dependencies in
+125        pyproject.toml.""",
+126    )
+127
+128    parser.add_argument(
+129        "-up",
+130        "--update",
+131        type=str,
+132        default=None,
+133        help=""" Excpects one argument: "major", "minor", or "patch".
+134        Passing "-up minor" is equivalent to passing the cli string: "-b -
 t -i -iv minor -uc -ca build -s".
-132        To publish the updated package, the -p/--publish switch needs to be
+135        To publish the updated package, the -p/--publish switch needs to be
 added to the cli input.""",
-133    )
-134
-135    args = parser.parse_args()
-136
-137    args.package = Pathier(args.package).resolve()
-138
-139    if args.update:
-140        args.build = True
-141        args.tag_version = True
-142        args.install = True
-143        args.increment_version = args.update
-144        args.update_changelog = True
-145        args.commit_all = "build"
-146        args.sync = True
-147
-148    if args.increment_version and args.increment_version not in [
-149        "major",
-150        "minor",
-151        "patch",
-152    ]:
-153        raise ValueError(
-154            f"Invalid option for -iv/--increment_version:
+136    )
+137
+138    parser.add_argument(
+139        "-st",
+140        "--skip_tests",
+141        action="store_true",
+142        help=""" Don't run tests when using the -b/--build command. """,
+143    )
+144
+145    args = parser.parse_args()
+146
+147    args.package = Pathier(args.package).resolve()
+148
+149    if args.update:
+150        args.build = True
+151        args.tag_version = True
+152        args.install = True
+153        args.increment_version = args.update
+154        args.update_changelog = True
+155        args.commit_all = "build"
+156        args.sync = True
+157
+158    if args.increment_version and args.increment_version not in [
+159        "major",
+160        "minor",
+161        "patch",
+162    ]:
+163        raise ValueError(
+164            f"Invalid option for -iv/--increment_version:
 {args.increment_version}"
-155        )
-156
-157    if args.commit_all == "":
-158        raise ValueError("Commit message for args.commit_all cannot be
+165        )
+166
+167    if args.commit_all == "":
+168        raise ValueError("Commit message for args.commit_all cannot be
 empty.")
-159
-160    return args
+169
+170    return args
+  ⁰
+def build(
+package_dir: pathier.pathier.Pathier,
+skip_tests: bool = False,
+overwrite_dependencies: bool = False): View Source
+173def build(
+174    package_dir: Pathier, skip_tests: bool = False, overwrite_dependencies:
+bool = False
+175):
+176    """Perform the build process.
+177
+178    Steps:
+179    * Run tests (unless `skip_tests` is `True`)
+180    * Raise error and abandon build if tests fail
+181    * Format source code with `Black`
+182    * Sort source code imports with `isort`
+183    * Update project dependencies in `pyproject.toml`
+184    * Generate docs
+185    * Delete previous `dist` folder contents
+186    * Invoke build module"""
+187    if not skip_tests and not run_tests(package_dir):
+188        raise RuntimeError(
+189            f"ERROR: {package_dir.stem} failed testing.\nAbandoning build."
+190        )
+191    hassle_utilities.format_files(package_dir)
+192    [isort.file(path) for path in package_dir.rglob("*.py")]
+193    hassle_utilities.update_dependencies(
+194        package_dir / "pyproject.toml", overwrite_dependencies
+195    )
+196    # Vermin isn't taking into account the minimum version of dependencies.
+197    # Removing from now and defaulting to >=3.10
+198    # hassle_utilities.update_minimum_python_version(pyproject_path)
+199    hassle_utilities.generate_docs(package_dir)
+200    (package_dir / "dist").delete()
+201    os.system(f"{sys.executable} -m build {package_dir}")
+Perform the build process.
+Steps:
+    * Run tests (unless skip_tests is True)
+    * Raise error and abandon build if tests fail
+    * Format source code with Black
+    * Sort source code imports with isort
+    * Update project dependencies in pyproject.toml
+    * Generate docs
+    * Delete previous dist folder contents
+    * Invoke build module
   ⁰
 def main(args: argparse.Namespace = None): View Source
-163def main(args: argparse.Namespace = None):
-164    if not args:
-165        args = get_args()
-166
-167    pyproject_path = args.package / "pyproject.toml"
-168
-169    if not pyproject_path.exists():
-170        raise FileNotFoundError(f"Could not locate pyproject.toml for
+204def main(args: argparse.Namespace = None):
+205    if not args:
+206        args = get_args()
+207
+208    pyproject_path = args.package / "pyproject.toml"
+209    args.package.mkcwd()
+210
+211    if not pyproject_path.exists():
+212        raise FileNotFoundError(f"Could not locate pyproject.toml for
 {args.package}")
-171
-172    if args.generate_tests:
-173        generate_test_files(args.package)
-174
-175    if args.run_tests:
-176        run_tests(args.package)
-177
-178    if args.increment_version:
-179        hassle_utilities.increment_version(pyproject_path,
-args.increment_version)
-180
-181    if args.build:
-182        (args.package / "dist").delete()
-183        os.system(f"black {args.package}")
-184        os.system(f"isort {args.package}")
-185        hassle_utilities.update_dependencies(
-186            pyproject_path, args.overwrite_dependencies
-187        )
-188        # Vermin isn't taking into account the minimum version of
-dependencies.
-189        # Removing from now and defaulting to >=3.10
-190        # hassle_utilities.update_minimum_python_version(pyproject_path)
-191        hassle_utilities.generate_docs(args.package)
-192        os.system(f"py -m build {args.package}")
-193
-194    if args.update_changelog:
-195        hassle_utilities.update_changelog(pyproject_path)
-196        # If we're going to add tag for current version
-197        # commit changelog first
-198        if args.tag_version:
-199            input(
-200                "Press enter to continue after optionally pruning the
-updated changelog..."
-201            )
-202            os.chdir(args.package)
-203            os.system("git add CHANGELOG.md")
-204            os.system('git commit CHANGELOG.md -m "chore: update
-changelog"')
-205
-206    if args.commit_all:
-207        os.chdir(args.package)
-208        if args.commit_all == "build":
-209            version = pyproject_path.loads()["project"]["version"]
-210            args.commit_all = f"chore: build v{version}"
-211        os.system("git add .")
-212        os.system(f'git commit -m "{args.commit_all}"')
 213
-214    if args.tag_version:
-215        hassle_utilities.tag_version(args.package)
+214    if args.generate_tests:
+215        generate_test_files(args.package)
 216
-217    if args.publish:
-218        os.system(f"twine upload {args.package / 'dist' / '*'}")
+217    if args.run_tests:
+218        run_tests(args.package)
 219
-220    if args.install:
-221        os.system(f"pip install {args.package} --no-deps --upgrade --no-
-cache-dir")
+220    if args.increment_version:
+221        hassle_utilities.increment_version(pyproject_path,
+args.increment_version)
 222
-223    if args.sync:
-224        os.chdir(args.package)
-225        os.system(f"git pull --tags origin main")
-226        os.system(f"git push origin main:main --tags")
+223    if args.build:
+224        build(args.package, args.skip_tests, args.overwrite_dependencies)
+225
+226    if args.update_changelog:
+227        hassle_utilities.update_changelog(pyproject_path)
+228        # If we're going to add tag for current version
+229        # commit changelog first
+230        if args.tag_version:
+231            input(
+232                "Press enter to continue after optionally pruning the
+updated changelog..."
+233            )
+234            git.commit_files(
+235                [str(args.package / "CHANGELOG.md")], "chore: update
+changelog"
+236            )
+237
+238    if args.commit_all:
+239        if args.commit_all == "build":
+240            version = pyproject_path.loads()["project"]["version"]
+241            args.commit_all = f"chore: build v{version}"
+242        git.add()
+243        git.commit(f'-m "{args.commit_all}"')
+244
+245    if args.tag_version:
+246        hassle_utilities.tag_version(args.package)
+247
+248    if args.publish:
+249        os.system(f"twine upload {args.package / 'dist' / '*'}")
+250
+251    if args.install:
+252        os.system(f"pip install {args.package} --no-deps --upgrade --no-
+cache-dir")
+253
+254    if args.sync:
+255        git.pull("--tags")
+256        git.push("--tags")
```

### Comparing `hassle-2.7.1/docs/hassle/hassle_config.html` & `hassle-2.8.0/docs/hassle/hassle_config.html`

 * *Files identical despite different names*

### Comparing `hassle-2.7.1/docs/hassle/hassle_utilities.html` & `hassle-2.8.0/docs/hassle/hassle_utilities.html`

 * *Files 1% similar despite different names*

```diff
@@ -50,14 +50,17 @@
             </li>
             <li>
                     <a class="function" href="#update_changelog">update_changelog</a>
             </li>
             <li>
                     <a class="function" href="#tag_version">tag_version</a>
             </li>
+            <li>
+                    <a class="function" href="#format_files">format_files</a>
+            </li>
     </ul>
 
 
 
         <a class="attribution" title="pdoc: Python API documentation generator" href="https://pdoc.dev" target="_blank">
             built with <span class="visually-hidden">pdoc</span><img
                 alt="pdoc logo"
@@ -73,155 +76,165 @@
                 
                         <input id="mod-hassle_utilities-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 
                         <label class="view-source-button" for="mod-hassle_utilities-view-source"><span>View Source</span></label>
 
                         <div class="pdoc-code codehilite"><pre><span></span><span id="L-1"><a href="#L-1"><span class="linenos">  1</span></a><span class="kn">import</span> <span class="nn">os</span>
 </span><span id="L-2"><a href="#L-2"><span class="linenos">  2</span></a>
-</span><span id="L-3"><a href="#L-3"><span class="linenos">  3</span></a><span class="kn">import</span> <span class="nn">packagelister</span>
-</span><span id="L-4"><a href="#L-4"><span class="linenos">  4</span></a><span class="kn">import</span> <span class="nn">vermin</span>
-</span><span id="L-5"><a href="#L-5"><span class="linenos">  5</span></a><span class="kn">from</span> <span class="nn">pathier</span> <span class="kn">import</span> <span class="n">Pathier</span>
-</span><span id="L-6"><a href="#L-6"><span class="linenos">  6</span></a>
-</span><span id="L-7"><a href="#L-7"><span class="linenos">  7</span></a><span class="kn">from</span> <span class="nn">hassle</span> <span class="kn">import</span> <span class="n">hassle_config</span>
+</span><span id="L-3"><a href="#L-3"><span class="linenos">  3</span></a><span class="kn">import</span> <span class="nn">black</span>
+</span><span id="L-4"><a href="#L-4"><span class="linenos">  4</span></a><span class="kn">import</span> <span class="nn">packagelister</span>
+</span><span id="L-5"><a href="#L-5"><span class="linenos">  5</span></a><span class="kn">import</span> <span class="nn">vermin</span>
+</span><span id="L-6"><a href="#L-6"><span class="linenos">  6</span></a><span class="kn">from</span> <span class="nn">gitbetter</span> <span class="kn">import</span> <span class="n">git</span>
+</span><span id="L-7"><a href="#L-7"><span class="linenos">  7</span></a><span class="kn">from</span> <span class="nn">pathier</span> <span class="kn">import</span> <span class="n">Pathier</span>
 </span><span id="L-8"><a href="#L-8"><span class="linenos">  8</span></a>
-</span><span id="L-9"><a href="#L-9"><span class="linenos">  9</span></a><span class="n">root</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="vm">__file__</span><span class="p">)</span><span class="o">.</span><span class="n">parent</span>
+</span><span id="L-9"><a href="#L-9"><span class="linenos">  9</span></a><span class="kn">from</span> <span class="nn">hassle</span> <span class="kn">import</span> <span class="n">hassle_config</span>
 </span><span id="L-10"><a href="#L-10"><span class="linenos"> 10</span></a>
-</span><span id="L-11"><a href="#L-11"><span class="linenos"> 11</span></a>
-</span><span id="L-12"><a href="#L-12"><span class="linenos"> 12</span></a><span class="k">def</span> <span class="nf">increment_version</span><span class="p">(</span><span class="n">pyproject_path</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">,</span> <span class="n">increment_type</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-13"><a href="#L-13"><span class="linenos"> 13</span></a>    <span class="sd">&quot;&quot;&quot;Increment the project.version field in pyproject.toml.</span>
-</span><span id="L-14"><a href="#L-14"><span class="linenos"> 14</span></a>
-</span><span id="L-15"><a href="#L-15"><span class="linenos"> 15</span></a><span class="sd">    :param package_path: Path to the package/project directory.</span>
+</span><span id="L-11"><a href="#L-11"><span class="linenos"> 11</span></a><span class="n">root</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="vm">__file__</span><span class="p">)</span><span class="o">.</span><span class="n">parent</span>
+</span><span id="L-12"><a href="#L-12"><span class="linenos"> 12</span></a>
+</span><span id="L-13"><a href="#L-13"><span class="linenos"> 13</span></a>
+</span><span id="L-14"><a href="#L-14"><span class="linenos"> 14</span></a><span class="k">def</span> <span class="nf">increment_version</span><span class="p">(</span><span class="n">pyproject_path</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">,</span> <span class="n">increment_type</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-15"><a href="#L-15"><span class="linenos"> 15</span></a>    <span class="sd">&quot;&quot;&quot;Increment the project.version field in pyproject.toml.</span>
 </span><span id="L-16"><a href="#L-16"><span class="linenos"> 16</span></a>
-</span><span id="L-17"><a href="#L-17"><span class="linenos"> 17</span></a><span class="sd">    :param increment_type: One from &#39;major&#39;, &#39;minor&#39;, or &#39;patch&#39;.&quot;&quot;&quot;</span>
-</span><span id="L-18"><a href="#L-18"><span class="linenos"> 18</span></a>    <span class="n">meta</span> <span class="o">=</span> <span class="n">pyproject_path</span><span class="o">.</span><span class="n">loads</span><span class="p">()</span>
-</span><span id="L-19"><a href="#L-19"><span class="linenos"> 19</span></a>    <span class="n">major</span><span class="p">,</span> <span class="n">minor</span><span class="p">,</span> <span class="n">patch</span> <span class="o">=</span> <span class="p">[</span><span class="nb">int</span><span class="p">(</span><span class="n">num</span><span class="p">)</span> <span class="k">for</span> <span class="n">num</span> <span class="ow">in</span> <span class="n">meta</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;version&quot;</span><span class="p">]</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="s2">&quot;.&quot;</span><span class="p">)]</span>
-</span><span id="L-20"><a href="#L-20"><span class="linenos"> 20</span></a>    <span class="k">if</span> <span class="n">increment_type</span> <span class="o">==</span> <span class="s2">&quot;major&quot;</span><span class="p">:</span>
-</span><span id="L-21"><a href="#L-21"><span class="linenos"> 21</span></a>        <span class="n">major</span> <span class="o">+=</span> <span class="mi">1</span>
-</span><span id="L-22"><a href="#L-22"><span class="linenos"> 22</span></a>        <span class="n">minor</span> <span class="o">=</span> <span class="mi">0</span>
-</span><span id="L-23"><a href="#L-23"><span class="linenos"> 23</span></a>        <span class="n">patch</span> <span class="o">=</span> <span class="mi">0</span>
-</span><span id="L-24"><a href="#L-24"><span class="linenos"> 24</span></a>    <span class="k">elif</span> <span class="n">increment_type</span> <span class="o">==</span> <span class="s2">&quot;minor&quot;</span><span class="p">:</span>
-</span><span id="L-25"><a href="#L-25"><span class="linenos"> 25</span></a>        <span class="n">minor</span> <span class="o">+=</span> <span class="mi">1</span>
-</span><span id="L-26"><a href="#L-26"><span class="linenos"> 26</span></a>        <span class="n">patch</span> <span class="o">=</span> <span class="mi">0</span>
-</span><span id="L-27"><a href="#L-27"><span class="linenos"> 27</span></a>    <span class="k">elif</span> <span class="n">increment_type</span> <span class="o">==</span> <span class="s2">&quot;patch&quot;</span><span class="p">:</span>
-</span><span id="L-28"><a href="#L-28"><span class="linenos"> 28</span></a>        <span class="n">patch</span> <span class="o">+=</span> <span class="mi">1</span>
-</span><span id="L-29"><a href="#L-29"><span class="linenos"> 29</span></a>    <span class="n">incremented_version</span> <span class="o">=</span> <span class="s2">&quot;.&quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="nb">str</span><span class="p">(</span><span class="n">num</span><span class="p">)</span> <span class="k">for</span> <span class="n">num</span> <span class="ow">in</span> <span class="p">[</span><span class="n">major</span><span class="p">,</span> <span class="n">minor</span><span class="p">,</span> <span class="n">patch</span><span class="p">])</span>
-</span><span id="L-30"><a href="#L-30"><span class="linenos"> 30</span></a>    <span class="n">meta</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;version&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="n">incremented_version</span>
-</span><span id="L-31"><a href="#L-31"><span class="linenos"> 31</span></a>    <span class="n">pyproject_path</span><span class="o">.</span><span class="n">dumps</span><span class="p">(</span><span class="n">meta</span><span class="p">)</span>
-</span><span id="L-32"><a href="#L-32"><span class="linenos"> 32</span></a>
-</span><span id="L-33"><a href="#L-33"><span class="linenos"> 33</span></a>
-</span><span id="L-34"><a href="#L-34"><span class="linenos"> 34</span></a><span class="k">def</span> <span class="nf">get_minimum_py_version</span><span class="p">(</span><span class="n">src</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
-</span><span id="L-35"><a href="#L-35"><span class="linenos"> 35</span></a>    <span class="sd">&quot;&quot;&quot;Scan src with vermin and return minimum</span>
-</span><span id="L-36"><a href="#L-36"><span class="linenos"> 36</span></a><span class="sd">    python version.&quot;&quot;&quot;</span>
-</span><span id="L-37"><a href="#L-37"><span class="linenos"> 37</span></a>    <span class="n">config</span> <span class="o">=</span> <span class="n">vermin</span><span class="o">.</span><span class="n">Config</span><span class="p">()</span>
-</span><span id="L-38"><a href="#L-38"><span class="linenos"> 38</span></a>    <span class="n">config</span><span class="o">.</span><span class="n">add_backport</span><span class="p">(</span><span class="s2">&quot;typing&quot;</span><span class="p">)</span>
-</span><span id="L-39"><a href="#L-39"><span class="linenos"> 39</span></a>    <span class="n">config</span><span class="o">.</span><span class="n">add_backport</span><span class="p">(</span><span class="s2">&quot;typing_extensions&quot;</span><span class="p">)</span>
-</span><span id="L-40"><a href="#L-40"><span class="linenos"> 40</span></a>    <span class="n">config</span><span class="o">.</span><span class="n">set_eval_annotations</span><span class="p">(</span><span class="kc">True</span><span class="p">)</span>
-</span><span id="L-41"><a href="#L-41"><span class="linenos"> 41</span></a>    <span class="n">result</span> <span class="o">=</span> <span class="n">vermin</span><span class="o">.</span><span class="n">visit</span><span class="p">(</span><span class="n">src</span><span class="p">,</span> <span class="n">config</span><span class="p">)</span><span class="o">.</span><span class="n">minimum_versions</span><span class="p">()[</span><span class="mi">1</span><span class="p">]</span>
-</span><span id="L-42"><a href="#L-42"><span class="linenos"> 42</span></a>    <span class="k">return</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">result</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span><span class="si">}</span><span class="s2">.</span><span class="si">{</span><span class="n">result</span><span class="p">[</span><span class="mi">1</span><span class="p">]</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="L-43"><a href="#L-43"><span class="linenos"> 43</span></a>
-</span><span id="L-44"><a href="#L-44"><span class="linenos"> 44</span></a>
-</span><span id="L-45"><a href="#L-45"><span class="linenos"> 45</span></a><span class="k">def</span> <span class="nf">get_project_code</span><span class="p">(</span><span class="n">project_path</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
-</span><span id="L-46"><a href="#L-46"><span class="linenos"> 46</span></a>    <span class="sd">&quot;&quot;&quot;Read and return all code from project_path</span>
-</span><span id="L-47"><a href="#L-47"><span class="linenos"> 47</span></a><span class="sd">    as one string.&quot;&quot;&quot;</span>
-</span><span id="L-48"><a href="#L-48"><span class="linenos"> 48</span></a>    <span class="k">return</span> <span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">file</span><span class="o">.</span><span class="n">read_text</span><span class="p">()</span> <span class="k">for</span> <span class="n">file</span> <span class="ow">in</span> <span class="n">project_path</span><span class="o">.</span><span class="n">rglob</span><span class="p">(</span><span class="s2">&quot;*.py&quot;</span><span class="p">))</span>
-</span><span id="L-49"><a href="#L-49"><span class="linenos"> 49</span></a>
-</span><span id="L-50"><a href="#L-50"><span class="linenos"> 50</span></a>
-</span><span id="L-51"><a href="#L-51"><span class="linenos"> 51</span></a><span class="k">def</span> <span class="nf">update_minimum_python_version</span><span class="p">(</span><span class="n">pyproject_path</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">):</span>
-</span><span id="L-52"><a href="#L-52"><span class="linenos"> 52</span></a>    <span class="sd">&quot;&quot;&quot;Use vermin to determine the minimum compatible</span>
-</span><span id="L-53"><a href="#L-53"><span class="linenos"> 53</span></a><span class="sd">    Python version and update the corresponding field</span>
-</span><span id="L-54"><a href="#L-54"><span class="linenos"> 54</span></a><span class="sd">    in pyproject.toml.&quot;&quot;&quot;</span>
-</span><span id="L-55"><a href="#L-55"><span class="linenos"> 55</span></a>    <span class="n">project_code</span> <span class="o">=</span> <span class="n">get_project_code</span><span class="p">(</span><span class="n">pyproject_path</span><span class="o">.</span><span class="n">parent</span> <span class="o">/</span> <span class="s2">&quot;src&quot;</span><span class="p">)</span>
-</span><span id="L-56"><a href="#L-56"><span class="linenos"> 56</span></a>    <span class="n">meta</span> <span class="o">=</span> <span class="n">pyproject_path</span><span class="o">.</span><span class="n">loads</span><span class="p">()</span>
-</span><span id="L-57"><a href="#L-57"><span class="linenos"> 57</span></a>    <span class="n">minimum_version</span> <span class="o">=</span> <span class="n">get_minimum_py_version</span><span class="p">(</span><span class="n">project_code</span><span class="p">)</span>
-</span><span id="L-58"><a href="#L-58"><span class="linenos"> 58</span></a>    <span class="n">minimum_version</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;&gt;=</span><span class="si">{</span><span class="n">minimum_version</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="L-59"><a href="#L-59"><span class="linenos"> 59</span></a>    <span class="n">meta</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;requires-python&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="n">minimum_version</span>
-</span><span id="L-60"><a href="#L-60"><span class="linenos"> 60</span></a>    <span class="n">pyproject_path</span><span class="o">.</span><span class="n">dumps</span><span class="p">(</span><span class="n">meta</span><span class="p">)</span>
-</span><span id="L-61"><a href="#L-61"><span class="linenos"> 61</span></a>
-</span><span id="L-62"><a href="#L-62"><span class="linenos"> 62</span></a>
-</span><span id="L-63"><a href="#L-63"><span class="linenos"> 63</span></a><span class="k">def</span> <span class="nf">generate_docs</span><span class="p">(</span><span class="n">package_path</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">):</span>
-</span><span id="L-64"><a href="#L-64"><span class="linenos"> 64</span></a>    <span class="sd">&quot;&quot;&quot;Generate project documentation using pdoc.&quot;&quot;&quot;</span>
-</span><span id="L-65"><a href="#L-65"><span class="linenos"> 65</span></a>    <span class="k">try</span><span class="p">:</span>
-</span><span id="L-66"><a href="#L-66"><span class="linenos"> 66</span></a>        <span class="p">(</span><span class="n">package_path</span> <span class="o">/</span> <span class="s2">&quot;docs&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">delete</span><span class="p">()</span>
-</span><span id="L-67"><a href="#L-67"><span class="linenos"> 67</span></a>    <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
-</span><span id="L-68"><a href="#L-68"><span class="linenos"> 68</span></a>        <span class="k">pass</span>
-</span><span id="L-69"><a href="#L-69"><span class="linenos"> 69</span></a>    <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span>
-</span><span id="L-70"><a href="#L-70"><span class="linenos"> 70</span></a>        <span class="sa">f</span><span class="s2">&quot;pdoc -o </span><span class="si">{</span><span class="n">package_path</span> <span class="o">/</span> <span class="s1">&#39;docs&#39;</span><span class="si">}</span><span class="s2"> </span><span class="si">{</span><span class="n">package_path</span> <span class="o">/</span> <span class="s1">&#39;src&#39;</span> <span class="o">/</span> <span class="n">package_path</span><span class="o">.</span><span class="n">stem</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="L-71"><a href="#L-71"><span class="linenos"> 71</span></a>    <span class="p">)</span>
-</span><span id="L-72"><a href="#L-72"><span class="linenos"> 72</span></a>
-</span><span id="L-73"><a href="#L-73"><span class="linenos"> 73</span></a>
-</span><span id="L-74"><a href="#L-74"><span class="linenos"> 74</span></a><span class="k">def</span> <span class="nf">update_dependencies</span><span class="p">(</span>
-</span><span id="L-75"><a href="#L-75"><span class="linenos"> 75</span></a>    <span class="n">pyproject_path</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">,</span> <span class="n">overwrite</span><span class="p">:</span> <span class="nb">bool</span><span class="p">,</span> <span class="n">include_versions</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span>
-</span><span id="L-76"><a href="#L-76"><span class="linenos"> 76</span></a><span class="p">):</span>
-</span><span id="L-77"><a href="#L-77"><span class="linenos"> 77</span></a>    <span class="sd">&quot;&quot;&quot;Update dependencies list in pyproject.toml.</span>
-</span><span id="L-78"><a href="#L-78"><span class="linenos"> 78</span></a>
-</span><span id="L-79"><a href="#L-79"><span class="linenos"> 79</span></a><span class="sd">    :param overwrite: If True, replace the dependencies in pyproject.toml</span>
-</span><span id="L-80"><a href="#L-80"><span class="linenos"> 80</span></a><span class="sd">    with the results of packagelister.scan() .</span>
-</span><span id="L-81"><a href="#L-81"><span class="linenos"> 81</span></a><span class="sd">    If False, packages returned by packagelister are appended to</span>
-</span><span id="L-82"><a href="#L-82"><span class="linenos"> 82</span></a><span class="sd">    the current dependencies in pyproject.toml if they don&#39;t already</span>
-</span><span id="L-83"><a href="#L-83"><span class="linenos"> 83</span></a><span class="sd">    exist in the field.&quot;&quot;&quot;</span>
-</span><span id="L-84"><a href="#L-84"><span class="linenos"> 84</span></a>    <span class="n">packages</span> <span class="o">=</span> <span class="n">packagelister</span><span class="o">.</span><span class="n">scan</span><span class="p">(</span><span class="n">pyproject_path</span><span class="o">.</span><span class="n">parent</span><span class="p">)</span>
-</span><span id="L-85"><a href="#L-85"><span class="linenos"> 85</span></a>
-</span><span id="L-86"><a href="#L-86"><span class="linenos"> 86</span></a>    <span class="n">packages</span> <span class="o">=</span> <span class="p">[</span>
-</span><span id="L-87"><a href="#L-87"><span class="linenos"> 87</span></a>        <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">package</span><span class="si">}</span><span class="s2">~=</span><span class="si">{</span><span class="n">packages</span><span class="p">[</span><span class="n">package</span><span class="p">][</span><span class="s1">&#39;version&#39;</span><span class="p">]</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="L-88"><a href="#L-88"><span class="linenos"> 88</span></a>        <span class="k">if</span> <span class="n">packages</span><span class="p">[</span><span class="n">package</span><span class="p">][</span><span class="s2">&quot;version&quot;</span><span class="p">]</span> <span class="ow">and</span> <span class="n">include_versions</span>
-</span><span id="L-89"><a href="#L-89"><span class="linenos"> 89</span></a>        <span class="k">else</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">package</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="L-90"><a href="#L-90"><span class="linenos"> 90</span></a>        <span class="k">for</span> <span class="n">package</span> <span class="ow">in</span> <span class="n">packages</span>
-</span><span id="L-91"><a href="#L-91"><span class="linenos"> 91</span></a>        <span class="k">if</span> <span class="n">package</span> <span class="o">!=</span> <span class="n">pyproject_path</span><span class="o">.</span><span class="n">parent</span><span class="o">.</span><span class="n">stem</span>
-</span><span id="L-92"><a href="#L-92"><span class="linenos"> 92</span></a>    <span class="p">]</span>
-</span><span id="L-93"><a href="#L-93"><span class="linenos"> 93</span></a>    <span class="n">packages</span> <span class="o">=</span> <span class="p">[</span>
-</span><span id="L-94"><a href="#L-94"><span class="linenos"> 94</span></a>        <span class="n">package</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span><span class="s2">&quot;speech_recognition&quot;</span><span class="p">,</span> <span class="s2">&quot;speechRecognition&quot;</span><span class="p">)</span>
-</span><span id="L-95"><a href="#L-95"><span class="linenos"> 95</span></a>        <span class="k">for</span> <span class="n">package</span> <span class="ow">in</span> <span class="n">packages</span>
-</span><span id="L-96"><a href="#L-96"><span class="linenos"> 96</span></a>    <span class="p">]</span>
-</span><span id="L-97"><a href="#L-97"><span class="linenos"> 97</span></a>    <span class="n">meta</span> <span class="o">=</span> <span class="n">pyproject_path</span><span class="o">.</span><span class="n">loads</span><span class="p">()</span>
-</span><span id="L-98"><a href="#L-98"><span class="linenos"> 98</span></a>    <span class="k">if</span> <span class="n">overwrite</span><span class="p">:</span>
-</span><span id="L-99"><a href="#L-99"><span class="linenos"> 99</span></a>        <span class="n">meta</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;dependencies&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="n">packages</span>
-</span><span id="L-100"><a href="#L-100"><span class="linenos">100</span></a>    <span class="k">else</span><span class="p">:</span>
-</span><span id="L-101"><a href="#L-101"><span class="linenos">101</span></a>        <span class="k">for</span> <span class="n">package</span> <span class="ow">in</span> <span class="n">packages</span><span class="p">:</span>
-</span><span id="L-102"><a href="#L-102"><span class="linenos">102</span></a>            <span class="k">if</span> <span class="s2">&quot;~&quot;</span> <span class="ow">in</span> <span class="n">package</span><span class="p">:</span>
-</span><span id="L-103"><a href="#L-103"><span class="linenos">103</span></a>                <span class="n">name</span> <span class="o">=</span> <span class="n">package</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="s2">&quot;~&quot;</span><span class="p">)[</span><span class="mi">0</span><span class="p">]</span>
-</span><span id="L-104"><a href="#L-104"><span class="linenos">104</span></a>            <span class="k">elif</span> <span class="s2">&quot;=&quot;</span> <span class="ow">in</span> <span class="n">package</span><span class="p">:</span>
-</span><span id="L-105"><a href="#L-105"><span class="linenos">105</span></a>                <span class="n">name</span> <span class="o">=</span> <span class="n">package</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="s2">&quot;=&quot;</span><span class="p">)[</span><span class="mi">0</span><span class="p">]</span>
-</span><span id="L-106"><a href="#L-106"><span class="linenos">106</span></a>            <span class="k">else</span><span class="p">:</span>
-</span><span id="L-107"><a href="#L-107"><span class="linenos">107</span></a>                <span class="n">name</span> <span class="o">=</span> <span class="n">package</span>
-</span><span id="L-108"><a href="#L-108"><span class="linenos">108</span></a>            <span class="k">if</span> <span class="nb">all</span><span class="p">(</span>
-</span><span id="L-109"><a href="#L-109"><span class="linenos">109</span></a>                <span class="n">name</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">dependency</span> <span class="k">for</span> <span class="n">dependency</span> <span class="ow">in</span> <span class="n">meta</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;dependencies&quot;</span><span class="p">]</span>
-</span><span id="L-110"><a href="#L-110"><span class="linenos">110</span></a>            <span class="p">):</span>
-</span><span id="L-111"><a href="#L-111"><span class="linenos">111</span></a>                <span class="n">meta</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;dependencies&quot;</span><span class="p">]</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">package</span><span class="p">)</span>
-</span><span id="L-112"><a href="#L-112"><span class="linenos">112</span></a>    <span class="n">pyproject_path</span><span class="o">.</span><span class="n">dumps</span><span class="p">(</span><span class="n">meta</span><span class="p">)</span>
-</span><span id="L-113"><a href="#L-113"><span class="linenos">113</span></a>
-</span><span id="L-114"><a href="#L-114"><span class="linenos">114</span></a>
-</span><span id="L-115"><a href="#L-115"><span class="linenos">115</span></a><span class="k">def</span> <span class="nf">update_changelog</span><span class="p">(</span><span class="n">pyproject_path</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">):</span>
-</span><span id="L-116"><a href="#L-116"><span class="linenos">116</span></a>    <span class="sd">&quot;&quot;&quot;Update project changelog.&quot;&quot;&quot;</span>
-</span><span id="L-117"><a href="#L-117"><span class="linenos">117</span></a>    <span class="n">meta</span> <span class="o">=</span> <span class="n">pyproject_path</span><span class="o">.</span><span class="n">loads</span><span class="p">()</span>
-</span><span id="L-118"><a href="#L-118"><span class="linenos">118</span></a>    <span class="k">if</span> <span class="n">hassle_config</span><span class="o">.</span><span class="n">config_exists</span><span class="p">():</span>
-</span><span id="L-119"><a href="#L-119"><span class="linenos">119</span></a>        <span class="n">config</span> <span class="o">=</span> <span class="n">hassle_config</span><span class="o">.</span><span class="n">load_config</span><span class="p">()</span>
-</span><span id="L-120"><a href="#L-120"><span class="linenos">120</span></a>    <span class="k">else</span><span class="p">:</span>
-</span><span id="L-121"><a href="#L-121"><span class="linenos">121</span></a>        <span class="n">hassle_config</span><span class="o">.</span><span class="n">warn</span><span class="p">()</span>
-</span><span id="L-122"><a href="#L-122"><span class="linenos">122</span></a>        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Creating blank hassle_config.toml...&quot;</span><span class="p">)</span>
-</span><span id="L-123"><a href="#L-123"><span class="linenos">123</span></a>        <span class="n">config</span> <span class="o">=</span> <span class="n">hassle_config</span><span class="o">.</span><span class="n">load_config</span><span class="p">()</span>
-</span><span id="L-124"><a href="#L-124"><span class="linenos">124</span></a>    <span class="n">changelog_path</span> <span class="o">=</span> <span class="n">pyproject_path</span><span class="o">.</span><span class="n">parent</span> <span class="o">/</span> <span class="s2">&quot;CHANGELOG.md&quot;</span>
-</span><span id="L-125"><a href="#L-125"><span class="linenos">125</span></a>    <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span>
-</span><span id="L-126"><a href="#L-126"><span class="linenos">126</span></a>        <span class="sa">f</span><span class="s2">&quot;auto-changelog -p </span><span class="si">{</span><span class="n">pyproject_path</span><span class="o">.</span><span class="n">parent</span><span class="si">}</span><span class="s2"> --tag-prefix </span><span class="si">{</span><span class="n">config</span><span class="p">[</span><span class="s1">&#39;git&#39;</span><span class="p">][</span><span class="s1">&#39;tag_prefix&#39;</span><span class="p">]</span><span class="si">}</span><span class="s2"> --unreleased -v </span><span class="si">{</span><span class="n">meta</span><span class="p">[</span><span class="s1">&#39;project&#39;</span><span class="p">][</span><span class="s1">&#39;version&#39;</span><span class="p">]</span><span class="si">}</span><span class="s2"> -o </span><span class="si">{</span><span class="n">changelog_path</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="L-127"><a href="#L-127"><span class="linenos">127</span></a>    <span class="p">)</span>
-</span><span id="L-128"><a href="#L-128"><span class="linenos">128</span></a>    <span class="n">changelog</span> <span class="o">=</span> <span class="n">changelog_path</span><span class="o">.</span><span class="n">read_text</span><span class="p">()</span><span class="o">.</span><span class="n">splitlines</span><span class="p">()</span>
-</span><span id="L-129"><a href="#L-129"><span class="linenos">129</span></a>    <span class="n">changelog</span> <span class="o">=</span> <span class="p">[</span><span class="n">line</span> <span class="k">for</span> <span class="n">line</span> <span class="ow">in</span> <span class="n">changelog</span> <span class="k">if</span> <span class="s2">&quot;Full set of changes:&quot;</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">line</span><span class="p">]</span>
-</span><span id="L-130"><a href="#L-130"><span class="linenos">130</span></a>    <span class="n">changelog_path</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span><span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">changelog</span><span class="p">))</span>
-</span><span id="L-131"><a href="#L-131"><span class="linenos">131</span></a>
-</span><span id="L-132"><a href="#L-132"><span class="linenos">132</span></a>
-</span><span id="L-133"><a href="#L-133"><span class="linenos">133</span></a><span class="k">def</span> <span class="nf">tag_version</span><span class="p">(</span><span class="n">package_path</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">):</span>
-</span><span id="L-134"><a href="#L-134"><span class="linenos">134</span></a>    <span class="sd">&quot;&quot;&quot;Add a git tag corresponding</span>
-</span><span id="L-135"><a href="#L-135"><span class="linenos">135</span></a><span class="sd">    to the version number in pyproject.toml.&quot;&quot;&quot;</span>
-</span><span id="L-136"><a href="#L-136"><span class="linenos">136</span></a>    <span class="k">if</span> <span class="n">hassle_config</span><span class="o">.</span><span class="n">config_exists</span><span class="p">():</span>
-</span><span id="L-137"><a href="#L-137"><span class="linenos">137</span></a>        <span class="n">tag_prefix</span> <span class="o">=</span> <span class="n">hassle_config</span><span class="o">.</span><span class="n">load_config</span><span class="p">()[</span><span class="s2">&quot;git&quot;</span><span class="p">][</span><span class="s2">&quot;tag_prefix&quot;</span><span class="p">]</span>
-</span><span id="L-138"><a href="#L-138"><span class="linenos">138</span></a>    <span class="k">else</span><span class="p">:</span>
-</span><span id="L-139"><a href="#L-139"><span class="linenos">139</span></a>        <span class="n">hassle_config</span><span class="o">.</span><span class="n">warn</span><span class="p">()</span>
-</span><span id="L-140"><a href="#L-140"><span class="linenos">140</span></a>        <span class="n">tag_prefix</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
-</span><span id="L-141"><a href="#L-141"><span class="linenos">141</span></a>    <span class="n">version</span> <span class="o">=</span> <span class="p">(</span><span class="n">package_path</span> <span class="o">/</span> <span class="s2">&quot;pyproject.toml&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">loads</span><span class="p">()[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;version&quot;</span><span class="p">]</span>
-</span><span id="L-142"><a href="#L-142"><span class="linenos">142</span></a>    <span class="n">os</span><span class="o">.</span><span class="n">chdir</span><span class="p">(</span><span class="n">package_path</span><span class="p">)</span>
-</span><span id="L-143"><a href="#L-143"><span class="linenos">143</span></a>    <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;git tag </span><span class="si">{</span><span class="n">tag_prefix</span><span class="si">}{</span><span class="n">version</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="L-17"><a href="#L-17"><span class="linenos"> 17</span></a><span class="sd">    :param package_path: Path to the package/project directory.</span>
+</span><span id="L-18"><a href="#L-18"><span class="linenos"> 18</span></a>
+</span><span id="L-19"><a href="#L-19"><span class="linenos"> 19</span></a><span class="sd">    :param increment_type: One from &#39;major&#39;, &#39;minor&#39;, or &#39;patch&#39;.&quot;&quot;&quot;</span>
+</span><span id="L-20"><a href="#L-20"><span class="linenos"> 20</span></a>    <span class="n">meta</span> <span class="o">=</span> <span class="n">pyproject_path</span><span class="o">.</span><span class="n">loads</span><span class="p">()</span>
+</span><span id="L-21"><a href="#L-21"><span class="linenos"> 21</span></a>    <span class="n">major</span><span class="p">,</span> <span class="n">minor</span><span class="p">,</span> <span class="n">patch</span> <span class="o">=</span> <span class="p">[</span><span class="nb">int</span><span class="p">(</span><span class="n">num</span><span class="p">)</span> <span class="k">for</span> <span class="n">num</span> <span class="ow">in</span> <span class="n">meta</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;version&quot;</span><span class="p">]</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="s2">&quot;.&quot;</span><span class="p">)]</span>
+</span><span id="L-22"><a href="#L-22"><span class="linenos"> 22</span></a>    <span class="k">if</span> <span class="n">increment_type</span> <span class="o">==</span> <span class="s2">&quot;major&quot;</span><span class="p">:</span>
+</span><span id="L-23"><a href="#L-23"><span class="linenos"> 23</span></a>        <span class="n">major</span> <span class="o">+=</span> <span class="mi">1</span>
+</span><span id="L-24"><a href="#L-24"><span class="linenos"> 24</span></a>        <span class="n">minor</span> <span class="o">=</span> <span class="mi">0</span>
+</span><span id="L-25"><a href="#L-25"><span class="linenos"> 25</span></a>        <span class="n">patch</span> <span class="o">=</span> <span class="mi">0</span>
+</span><span id="L-26"><a href="#L-26"><span class="linenos"> 26</span></a>    <span class="k">elif</span> <span class="n">increment_type</span> <span class="o">==</span> <span class="s2">&quot;minor&quot;</span><span class="p">:</span>
+</span><span id="L-27"><a href="#L-27"><span class="linenos"> 27</span></a>        <span class="n">minor</span> <span class="o">+=</span> <span class="mi">1</span>
+</span><span id="L-28"><a href="#L-28"><span class="linenos"> 28</span></a>        <span class="n">patch</span> <span class="o">=</span> <span class="mi">0</span>
+</span><span id="L-29"><a href="#L-29"><span class="linenos"> 29</span></a>    <span class="k">elif</span> <span class="n">increment_type</span> <span class="o">==</span> <span class="s2">&quot;patch&quot;</span><span class="p">:</span>
+</span><span id="L-30"><a href="#L-30"><span class="linenos"> 30</span></a>        <span class="n">patch</span> <span class="o">+=</span> <span class="mi">1</span>
+</span><span id="L-31"><a href="#L-31"><span class="linenos"> 31</span></a>    <span class="n">incremented_version</span> <span class="o">=</span> <span class="s2">&quot;.&quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="nb">str</span><span class="p">(</span><span class="n">num</span><span class="p">)</span> <span class="k">for</span> <span class="n">num</span> <span class="ow">in</span> <span class="p">[</span><span class="n">major</span><span class="p">,</span> <span class="n">minor</span><span class="p">,</span> <span class="n">patch</span><span class="p">])</span>
+</span><span id="L-32"><a href="#L-32"><span class="linenos"> 32</span></a>    <span class="n">meta</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;version&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="n">incremented_version</span>
+</span><span id="L-33"><a href="#L-33"><span class="linenos"> 33</span></a>    <span class="n">pyproject_path</span><span class="o">.</span><span class="n">dumps</span><span class="p">(</span><span class="n">meta</span><span class="p">)</span>
+</span><span id="L-34"><a href="#L-34"><span class="linenos"> 34</span></a>
+</span><span id="L-35"><a href="#L-35"><span class="linenos"> 35</span></a>
+</span><span id="L-36"><a href="#L-36"><span class="linenos"> 36</span></a><span class="k">def</span> <span class="nf">get_minimum_py_version</span><span class="p">(</span><span class="n">src</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
+</span><span id="L-37"><a href="#L-37"><span class="linenos"> 37</span></a>    <span class="sd">&quot;&quot;&quot;Scan src with vermin and return minimum</span>
+</span><span id="L-38"><a href="#L-38"><span class="linenos"> 38</span></a><span class="sd">    python version.&quot;&quot;&quot;</span>
+</span><span id="L-39"><a href="#L-39"><span class="linenos"> 39</span></a>    <span class="n">config</span> <span class="o">=</span> <span class="n">vermin</span><span class="o">.</span><span class="n">Config</span><span class="p">()</span>
+</span><span id="L-40"><a href="#L-40"><span class="linenos"> 40</span></a>    <span class="n">config</span><span class="o">.</span><span class="n">add_backport</span><span class="p">(</span><span class="s2">&quot;typing&quot;</span><span class="p">)</span>
+</span><span id="L-41"><a href="#L-41"><span class="linenos"> 41</span></a>    <span class="n">config</span><span class="o">.</span><span class="n">add_backport</span><span class="p">(</span><span class="s2">&quot;typing_extensions&quot;</span><span class="p">)</span>
+</span><span id="L-42"><a href="#L-42"><span class="linenos"> 42</span></a>    <span class="n">config</span><span class="o">.</span><span class="n">set_eval_annotations</span><span class="p">(</span><span class="kc">True</span><span class="p">)</span>
+</span><span id="L-43"><a href="#L-43"><span class="linenos"> 43</span></a>    <span class="n">result</span> <span class="o">=</span> <span class="n">vermin</span><span class="o">.</span><span class="n">visit</span><span class="p">(</span><span class="n">src</span><span class="p">,</span> <span class="n">config</span><span class="p">)</span><span class="o">.</span><span class="n">minimum_versions</span><span class="p">()[</span><span class="mi">1</span><span class="p">]</span>
+</span><span id="L-44"><a href="#L-44"><span class="linenos"> 44</span></a>    <span class="k">return</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">result</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span><span class="si">}</span><span class="s2">.</span><span class="si">{</span><span class="n">result</span><span class="p">[</span><span class="mi">1</span><span class="p">]</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="L-45"><a href="#L-45"><span class="linenos"> 45</span></a>
+</span><span id="L-46"><a href="#L-46"><span class="linenos"> 46</span></a>
+</span><span id="L-47"><a href="#L-47"><span class="linenos"> 47</span></a><span class="k">def</span> <span class="nf">get_project_code</span><span class="p">(</span><span class="n">project_path</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
+</span><span id="L-48"><a href="#L-48"><span class="linenos"> 48</span></a>    <span class="sd">&quot;&quot;&quot;Read and return all code from project_path</span>
+</span><span id="L-49"><a href="#L-49"><span class="linenos"> 49</span></a><span class="sd">    as one string.&quot;&quot;&quot;</span>
+</span><span id="L-50"><a href="#L-50"><span class="linenos"> 50</span></a>    <span class="k">return</span> <span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">file</span><span class="o">.</span><span class="n">read_text</span><span class="p">()</span> <span class="k">for</span> <span class="n">file</span> <span class="ow">in</span> <span class="n">project_path</span><span class="o">.</span><span class="n">rglob</span><span class="p">(</span><span class="s2">&quot;*.py&quot;</span><span class="p">))</span>
+</span><span id="L-51"><a href="#L-51"><span class="linenos"> 51</span></a>
+</span><span id="L-52"><a href="#L-52"><span class="linenos"> 52</span></a>
+</span><span id="L-53"><a href="#L-53"><span class="linenos"> 53</span></a><span class="k">def</span> <span class="nf">update_minimum_python_version</span><span class="p">(</span><span class="n">pyproject_path</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">):</span>
+</span><span id="L-54"><a href="#L-54"><span class="linenos"> 54</span></a>    <span class="sd">&quot;&quot;&quot;Use vermin to determine the minimum compatible</span>
+</span><span id="L-55"><a href="#L-55"><span class="linenos"> 55</span></a><span class="sd">    Python version and update the corresponding field</span>
+</span><span id="L-56"><a href="#L-56"><span class="linenos"> 56</span></a><span class="sd">    in pyproject.toml.&quot;&quot;&quot;</span>
+</span><span id="L-57"><a href="#L-57"><span class="linenos"> 57</span></a>    <span class="n">project_code</span> <span class="o">=</span> <span class="n">get_project_code</span><span class="p">(</span><span class="n">pyproject_path</span><span class="o">.</span><span class="n">parent</span> <span class="o">/</span> <span class="s2">&quot;src&quot;</span><span class="p">)</span>
+</span><span id="L-58"><a href="#L-58"><span class="linenos"> 58</span></a>    <span class="n">meta</span> <span class="o">=</span> <span class="n">pyproject_path</span><span class="o">.</span><span class="n">loads</span><span class="p">()</span>
+</span><span id="L-59"><a href="#L-59"><span class="linenos"> 59</span></a>    <span class="n">minimum_version</span> <span class="o">=</span> <span class="n">get_minimum_py_version</span><span class="p">(</span><span class="n">project_code</span><span class="p">)</span>
+</span><span id="L-60"><a href="#L-60"><span class="linenos"> 60</span></a>    <span class="n">minimum_version</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;&gt;=</span><span class="si">{</span><span class="n">minimum_version</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="L-61"><a href="#L-61"><span class="linenos"> 61</span></a>    <span class="n">meta</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;requires-python&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="n">minimum_version</span>
+</span><span id="L-62"><a href="#L-62"><span class="linenos"> 62</span></a>    <span class="n">pyproject_path</span><span class="o">.</span><span class="n">dumps</span><span class="p">(</span><span class="n">meta</span><span class="p">)</span>
+</span><span id="L-63"><a href="#L-63"><span class="linenos"> 63</span></a>
+</span><span id="L-64"><a href="#L-64"><span class="linenos"> 64</span></a>
+</span><span id="L-65"><a href="#L-65"><span class="linenos"> 65</span></a><span class="k">def</span> <span class="nf">generate_docs</span><span class="p">(</span><span class="n">package_path</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">):</span>
+</span><span id="L-66"><a href="#L-66"><span class="linenos"> 66</span></a>    <span class="sd">&quot;&quot;&quot;Generate project documentation using pdoc.&quot;&quot;&quot;</span>
+</span><span id="L-67"><a href="#L-67"><span class="linenos"> 67</span></a>    <span class="k">try</span><span class="p">:</span>
+</span><span id="L-68"><a href="#L-68"><span class="linenos"> 68</span></a>        <span class="p">(</span><span class="n">package_path</span> <span class="o">/</span> <span class="s2">&quot;docs&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">delete</span><span class="p">()</span>
+</span><span id="L-69"><a href="#L-69"><span class="linenos"> 69</span></a>    <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="L-70"><a href="#L-70"><span class="linenos"> 70</span></a>        <span class="k">pass</span>
+</span><span id="L-71"><a href="#L-71"><span class="linenos"> 71</span></a>    <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span>
+</span><span id="L-72"><a href="#L-72"><span class="linenos"> 72</span></a>        <span class="sa">f</span><span class="s2">&quot;pdoc -o </span><span class="si">{</span><span class="n">package_path</span> <span class="o">/</span> <span class="s1">&#39;docs&#39;</span><span class="si">}</span><span class="s2"> </span><span class="si">{</span><span class="n">package_path</span> <span class="o">/</span> <span class="s1">&#39;src&#39;</span> <span class="o">/</span> <span class="n">package_path</span><span class="o">.</span><span class="n">stem</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="L-73"><a href="#L-73"><span class="linenos"> 73</span></a>    <span class="p">)</span>
+</span><span id="L-74"><a href="#L-74"><span class="linenos"> 74</span></a>
+</span><span id="L-75"><a href="#L-75"><span class="linenos"> 75</span></a>
+</span><span id="L-76"><a href="#L-76"><span class="linenos"> 76</span></a><span class="k">def</span> <span class="nf">update_dependencies</span><span class="p">(</span>
+</span><span id="L-77"><a href="#L-77"><span class="linenos"> 77</span></a>    <span class="n">pyproject_path</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">,</span> <span class="n">overwrite</span><span class="p">:</span> <span class="nb">bool</span><span class="p">,</span> <span class="n">include_versions</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span>
+</span><span id="L-78"><a href="#L-78"><span class="linenos"> 78</span></a><span class="p">):</span>
+</span><span id="L-79"><a href="#L-79"><span class="linenos"> 79</span></a>    <span class="sd">&quot;&quot;&quot;Update dependencies list in pyproject.toml.</span>
+</span><span id="L-80"><a href="#L-80"><span class="linenos"> 80</span></a>
+</span><span id="L-81"><a href="#L-81"><span class="linenos"> 81</span></a><span class="sd">    :param overwrite: If True, replace the dependencies in pyproject.toml</span>
+</span><span id="L-82"><a href="#L-82"><span class="linenos"> 82</span></a><span class="sd">    with the results of packagelister.scan() .</span>
+</span><span id="L-83"><a href="#L-83"><span class="linenos"> 83</span></a><span class="sd">    If False, packages returned by packagelister are appended to</span>
+</span><span id="L-84"><a href="#L-84"><span class="linenos"> 84</span></a><span class="sd">    the current dependencies in pyproject.toml if they don&#39;t already</span>
+</span><span id="L-85"><a href="#L-85"><span class="linenos"> 85</span></a><span class="sd">    exist in the field.&quot;&quot;&quot;</span>
+</span><span id="L-86"><a href="#L-86"><span class="linenos"> 86</span></a>    <span class="n">packages</span> <span class="o">=</span> <span class="n">packagelister</span><span class="o">.</span><span class="n">scan</span><span class="p">(</span><span class="n">pyproject_path</span><span class="o">.</span><span class="n">parent</span><span class="p">)</span>
+</span><span id="L-87"><a href="#L-87"><span class="linenos"> 87</span></a>
+</span><span id="L-88"><a href="#L-88"><span class="linenos"> 88</span></a>    <span class="n">packages</span> <span class="o">=</span> <span class="p">[</span>
+</span><span id="L-89"><a href="#L-89"><span class="linenos"> 89</span></a>        <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">package</span><span class="si">}</span><span class="s2">~=</span><span class="si">{</span><span class="n">packages</span><span class="p">[</span><span class="n">package</span><span class="p">][</span><span class="s1">&#39;version&#39;</span><span class="p">]</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="L-90"><a href="#L-90"><span class="linenos"> 90</span></a>        <span class="k">if</span> <span class="n">packages</span><span class="p">[</span><span class="n">package</span><span class="p">][</span><span class="s2">&quot;version&quot;</span><span class="p">]</span> <span class="ow">and</span> <span class="n">include_versions</span>
+</span><span id="L-91"><a href="#L-91"><span class="linenos"> 91</span></a>        <span class="k">else</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">package</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="L-92"><a href="#L-92"><span class="linenos"> 92</span></a>        <span class="k">for</span> <span class="n">package</span> <span class="ow">in</span> <span class="n">packages</span>
+</span><span id="L-93"><a href="#L-93"><span class="linenos"> 93</span></a>        <span class="k">if</span> <span class="n">package</span> <span class="o">!=</span> <span class="n">pyproject_path</span><span class="o">.</span><span class="n">parent</span><span class="o">.</span><span class="n">stem</span>
+</span><span id="L-94"><a href="#L-94"><span class="linenos"> 94</span></a>    <span class="p">]</span>
+</span><span id="L-95"><a href="#L-95"><span class="linenos"> 95</span></a>    <span class="n">packages</span> <span class="o">=</span> <span class="p">[</span>
+</span><span id="L-96"><a href="#L-96"><span class="linenos"> 96</span></a>        <span class="n">package</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span><span class="s2">&quot;speech_recognition&quot;</span><span class="p">,</span> <span class="s2">&quot;speechRecognition&quot;</span><span class="p">)</span>
+</span><span id="L-97"><a href="#L-97"><span class="linenos"> 97</span></a>        <span class="k">for</span> <span class="n">package</span> <span class="ow">in</span> <span class="n">packages</span>
+</span><span id="L-98"><a href="#L-98"><span class="linenos"> 98</span></a>    <span class="p">]</span>
+</span><span id="L-99"><a href="#L-99"><span class="linenos"> 99</span></a>    <span class="n">meta</span> <span class="o">=</span> <span class="n">pyproject_path</span><span class="o">.</span><span class="n">loads</span><span class="p">()</span>
+</span><span id="L-100"><a href="#L-100"><span class="linenos">100</span></a>    <span class="k">if</span> <span class="n">overwrite</span><span class="p">:</span>
+</span><span id="L-101"><a href="#L-101"><span class="linenos">101</span></a>        <span class="n">meta</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;dependencies&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="n">packages</span>
+</span><span id="L-102"><a href="#L-102"><span class="linenos">102</span></a>    <span class="k">else</span><span class="p">:</span>
+</span><span id="L-103"><a href="#L-103"><span class="linenos">103</span></a>        <span class="k">for</span> <span class="n">package</span> <span class="ow">in</span> <span class="n">packages</span><span class="p">:</span>
+</span><span id="L-104"><a href="#L-104"><span class="linenos">104</span></a>            <span class="k">if</span> <span class="s2">&quot;~&quot;</span> <span class="ow">in</span> <span class="n">package</span><span class="p">:</span>
+</span><span id="L-105"><a href="#L-105"><span class="linenos">105</span></a>                <span class="n">name</span> <span class="o">=</span> <span class="n">package</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="s2">&quot;~&quot;</span><span class="p">)[</span><span class="mi">0</span><span class="p">]</span>
+</span><span id="L-106"><a href="#L-106"><span class="linenos">106</span></a>            <span class="k">elif</span> <span class="s2">&quot;=&quot;</span> <span class="ow">in</span> <span class="n">package</span><span class="p">:</span>
+</span><span id="L-107"><a href="#L-107"><span class="linenos">107</span></a>                <span class="n">name</span> <span class="o">=</span> <span class="n">package</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="s2">&quot;=&quot;</span><span class="p">)[</span><span class="mi">0</span><span class="p">]</span>
+</span><span id="L-108"><a href="#L-108"><span class="linenos">108</span></a>            <span class="k">else</span><span class="p">:</span>
+</span><span id="L-109"><a href="#L-109"><span class="linenos">109</span></a>                <span class="n">name</span> <span class="o">=</span> <span class="n">package</span>
+</span><span id="L-110"><a href="#L-110"><span class="linenos">110</span></a>            <span class="k">if</span> <span class="nb">all</span><span class="p">(</span>
+</span><span id="L-111"><a href="#L-111"><span class="linenos">111</span></a>                <span class="n">name</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">dependency</span> <span class="k">for</span> <span class="n">dependency</span> <span class="ow">in</span> <span class="n">meta</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;dependencies&quot;</span><span class="p">]</span>
+</span><span id="L-112"><a href="#L-112"><span class="linenos">112</span></a>            <span class="p">):</span>
+</span><span id="L-113"><a href="#L-113"><span class="linenos">113</span></a>                <span class="n">meta</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;dependencies&quot;</span><span class="p">]</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">package</span><span class="p">)</span>
+</span><span id="L-114"><a href="#L-114"><span class="linenos">114</span></a>    <span class="n">pyproject_path</span><span class="o">.</span><span class="n">dumps</span><span class="p">(</span><span class="n">meta</span><span class="p">)</span>
+</span><span id="L-115"><a href="#L-115"><span class="linenos">115</span></a>
+</span><span id="L-116"><a href="#L-116"><span class="linenos">116</span></a>
+</span><span id="L-117"><a href="#L-117"><span class="linenos">117</span></a><span class="k">def</span> <span class="nf">update_changelog</span><span class="p">(</span><span class="n">pyproject_path</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">):</span>
+</span><span id="L-118"><a href="#L-118"><span class="linenos">118</span></a>    <span class="sd">&quot;&quot;&quot;Update project changelog.&quot;&quot;&quot;</span>
+</span><span id="L-119"><a href="#L-119"><span class="linenos">119</span></a>    <span class="n">meta</span> <span class="o">=</span> <span class="n">pyproject_path</span><span class="o">.</span><span class="n">loads</span><span class="p">()</span>
+</span><span id="L-120"><a href="#L-120"><span class="linenos">120</span></a>    <span class="k">if</span> <span class="n">hassle_config</span><span class="o">.</span><span class="n">config_exists</span><span class="p">():</span>
+</span><span id="L-121"><a href="#L-121"><span class="linenos">121</span></a>        <span class="n">config</span> <span class="o">=</span> <span class="n">hassle_config</span><span class="o">.</span><span class="n">load_config</span><span class="p">()</span>
+</span><span id="L-122"><a href="#L-122"><span class="linenos">122</span></a>    <span class="k">else</span><span class="p">:</span>
+</span><span id="L-123"><a href="#L-123"><span class="linenos">123</span></a>        <span class="n">hassle_config</span><span class="o">.</span><span class="n">warn</span><span class="p">()</span>
+</span><span id="L-124"><a href="#L-124"><span class="linenos">124</span></a>        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Creating blank hassle_config.toml...&quot;</span><span class="p">)</span>
+</span><span id="L-125"><a href="#L-125"><span class="linenos">125</span></a>        <span class="n">config</span> <span class="o">=</span> <span class="n">hassle_config</span><span class="o">.</span><span class="n">load_config</span><span class="p">()</span>
+</span><span id="L-126"><a href="#L-126"><span class="linenos">126</span></a>    <span class="n">changelog_path</span> <span class="o">=</span> <span class="n">pyproject_path</span><span class="o">.</span><span class="n">parent</span> <span class="o">/</span> <span class="s2">&quot;CHANGELOG.md&quot;</span>
+</span><span id="L-127"><a href="#L-127"><span class="linenos">127</span></a>    <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span>
+</span><span id="L-128"><a href="#L-128"><span class="linenos">128</span></a>        <span class="sa">f</span><span class="s2">&quot;auto-changelog -p </span><span class="si">{</span><span class="n">pyproject_path</span><span class="o">.</span><span class="n">parent</span><span class="si">}</span><span class="s2"> --tag-prefix </span><span class="si">{</span><span class="n">config</span><span class="p">[</span><span class="s1">&#39;git&#39;</span><span class="p">][</span><span class="s1">&#39;tag_prefix&#39;</span><span class="p">]</span><span class="si">}</span><span class="s2"> --unreleased -v </span><span class="si">{</span><span class="n">meta</span><span class="p">[</span><span class="s1">&#39;project&#39;</span><span class="p">][</span><span class="s1">&#39;version&#39;</span><span class="p">]</span><span class="si">}</span><span class="s2"> -o </span><span class="si">{</span><span class="n">changelog_path</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="L-129"><a href="#L-129"><span class="linenos">129</span></a>    <span class="p">)</span>
+</span><span id="L-130"><a href="#L-130"><span class="linenos">130</span></a>    <span class="n">changelog</span> <span class="o">=</span> <span class="n">changelog_path</span><span class="o">.</span><span class="n">read_text</span><span class="p">()</span><span class="o">.</span><span class="n">splitlines</span><span class="p">()</span>
+</span><span id="L-131"><a href="#L-131"><span class="linenos">131</span></a>    <span class="n">changelog</span> <span class="o">=</span> <span class="p">[</span><span class="n">line</span> <span class="k">for</span> <span class="n">line</span> <span class="ow">in</span> <span class="n">changelog</span> <span class="k">if</span> <span class="s2">&quot;Full set of changes:&quot;</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">line</span><span class="p">]</span>
+</span><span id="L-132"><a href="#L-132"><span class="linenos">132</span></a>    <span class="n">changelog_path</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span><span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">changelog</span><span class="p">))</span>
+</span><span id="L-133"><a href="#L-133"><span class="linenos">133</span></a>
+</span><span id="L-134"><a href="#L-134"><span class="linenos">134</span></a>
+</span><span id="L-135"><a href="#L-135"><span class="linenos">135</span></a><span class="k">def</span> <span class="nf">tag_version</span><span class="p">(</span><span class="n">package_path</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">):</span>
+</span><span id="L-136"><a href="#L-136"><span class="linenos">136</span></a>    <span class="sd">&quot;&quot;&quot;Add a git tag corresponding</span>
+</span><span id="L-137"><a href="#L-137"><span class="linenos">137</span></a><span class="sd">    to the version number in pyproject.toml.&quot;&quot;&quot;</span>
+</span><span id="L-138"><a href="#L-138"><span class="linenos">138</span></a>    <span class="k">if</span> <span class="n">hassle_config</span><span class="o">.</span><span class="n">config_exists</span><span class="p">():</span>
+</span><span id="L-139"><a href="#L-139"><span class="linenos">139</span></a>        <span class="n">tag_prefix</span> <span class="o">=</span> <span class="n">hassle_config</span><span class="o">.</span><span class="n">load_config</span><span class="p">()[</span><span class="s2">&quot;git&quot;</span><span class="p">][</span><span class="s2">&quot;tag_prefix&quot;</span><span class="p">]</span>
+</span><span id="L-140"><a href="#L-140"><span class="linenos">140</span></a>    <span class="k">else</span><span class="p">:</span>
+</span><span id="L-141"><a href="#L-141"><span class="linenos">141</span></a>        <span class="n">hassle_config</span><span class="o">.</span><span class="n">warn</span><span class="p">()</span>
+</span><span id="L-142"><a href="#L-142"><span class="linenos">142</span></a>        <span class="n">tag_prefix</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
+</span><span id="L-143"><a href="#L-143"><span class="linenos">143</span></a>    <span class="n">version</span> <span class="o">=</span> <span class="p">(</span><span class="n">package_path</span> <span class="o">/</span> <span class="s2">&quot;pyproject.toml&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">loads</span><span class="p">()[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;version&quot;</span><span class="p">]</span>
+</span><span id="L-144"><a href="#L-144"><span class="linenos">144</span></a>    <span class="n">os</span><span class="o">.</span><span class="n">chdir</span><span class="p">(</span><span class="n">package_path</span><span class="p">)</span>
+</span><span id="L-145"><a href="#L-145"><span class="linenos">145</span></a>    <span class="n">git</span><span class="o">.</span><span class="n">tag</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">tag_prefix</span><span class="si">}{</span><span class="n">version</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="L-146"><a href="#L-146"><span class="linenos">146</span></a>
+</span><span id="L-147"><a href="#L-147"><span class="linenos">147</span></a>
+</span><span id="L-148"><a href="#L-148"><span class="linenos">148</span></a><span class="k">def</span> <span class="nf">format_files</span><span class="p">(</span><span class="n">path</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">):</span>
+</span><span id="L-149"><a href="#L-149"><span class="linenos">149</span></a>    <span class="sd">&quot;&quot;&quot;Use `Black` to format file(s).&quot;&quot;&quot;</span>
+</span><span id="L-150"><a href="#L-150"><span class="linenos">150</span></a>    <span class="k">try</span><span class="p">:</span>
+</span><span id="L-151"><a href="#L-151"><span class="linenos">151</span></a>        <span class="n">black</span><span class="o">.</span><span class="n">main</span><span class="p">([</span><span class="nb">str</span><span class="p">(</span><span class="n">path</span><span class="p">)])</span>
+</span><span id="L-152"><a href="#L-152"><span class="linenos">152</span></a>    <span class="k">except</span> <span class="ne">SystemExit</span><span class="p">:</span>
+</span><span id="L-153"><a href="#L-153"><span class="linenos">153</span></a>        <span class="o">...</span>
 </span></pre></div>
 
 
             </section>
                 <section id="increment_version">
                             <input id="increment_version-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
@@ -229,34 +242,34 @@
         <span class="def">def</span>
         <span class="name">increment_version</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">pyproject_path</span><span class="p">:</span> <span class="n">pathier</span><span class="o">.</span><span class="n">pathier</span><span class="o">.</span><span class="n">Pathier</span>, </span><span class="param"><span class="n">increment_type</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="increment_version-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#increment_version"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="increment_version-13"><a href="#increment_version-13"><span class="linenos">13</span></a><span class="k">def</span> <span class="nf">increment_version</span><span class="p">(</span><span class="n">pyproject_path</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">,</span> <span class="n">increment_type</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="increment_version-14"><a href="#increment_version-14"><span class="linenos">14</span></a>    <span class="sd">&quot;&quot;&quot;Increment the project.version field in pyproject.toml.</span>
-</span><span id="increment_version-15"><a href="#increment_version-15"><span class="linenos">15</span></a>
-</span><span id="increment_version-16"><a href="#increment_version-16"><span class="linenos">16</span></a><span class="sd">    :param package_path: Path to the package/project directory.</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="increment_version-15"><a href="#increment_version-15"><span class="linenos">15</span></a><span class="k">def</span> <span class="nf">increment_version</span><span class="p">(</span><span class="n">pyproject_path</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">,</span> <span class="n">increment_type</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="increment_version-16"><a href="#increment_version-16"><span class="linenos">16</span></a>    <span class="sd">&quot;&quot;&quot;Increment the project.version field in pyproject.toml.</span>
 </span><span id="increment_version-17"><a href="#increment_version-17"><span class="linenos">17</span></a>
-</span><span id="increment_version-18"><a href="#increment_version-18"><span class="linenos">18</span></a><span class="sd">    :param increment_type: One from &#39;major&#39;, &#39;minor&#39;, or &#39;patch&#39;.&quot;&quot;&quot;</span>
-</span><span id="increment_version-19"><a href="#increment_version-19"><span class="linenos">19</span></a>    <span class="n">meta</span> <span class="o">=</span> <span class="n">pyproject_path</span><span class="o">.</span><span class="n">loads</span><span class="p">()</span>
-</span><span id="increment_version-20"><a href="#increment_version-20"><span class="linenos">20</span></a>    <span class="n">major</span><span class="p">,</span> <span class="n">minor</span><span class="p">,</span> <span class="n">patch</span> <span class="o">=</span> <span class="p">[</span><span class="nb">int</span><span class="p">(</span><span class="n">num</span><span class="p">)</span> <span class="k">for</span> <span class="n">num</span> <span class="ow">in</span> <span class="n">meta</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;version&quot;</span><span class="p">]</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="s2">&quot;.&quot;</span><span class="p">)]</span>
-</span><span id="increment_version-21"><a href="#increment_version-21"><span class="linenos">21</span></a>    <span class="k">if</span> <span class="n">increment_type</span> <span class="o">==</span> <span class="s2">&quot;major&quot;</span><span class="p">:</span>
-</span><span id="increment_version-22"><a href="#increment_version-22"><span class="linenos">22</span></a>        <span class="n">major</span> <span class="o">+=</span> <span class="mi">1</span>
-</span><span id="increment_version-23"><a href="#increment_version-23"><span class="linenos">23</span></a>        <span class="n">minor</span> <span class="o">=</span> <span class="mi">0</span>
-</span><span id="increment_version-24"><a href="#increment_version-24"><span class="linenos">24</span></a>        <span class="n">patch</span> <span class="o">=</span> <span class="mi">0</span>
-</span><span id="increment_version-25"><a href="#increment_version-25"><span class="linenos">25</span></a>    <span class="k">elif</span> <span class="n">increment_type</span> <span class="o">==</span> <span class="s2">&quot;minor&quot;</span><span class="p">:</span>
-</span><span id="increment_version-26"><a href="#increment_version-26"><span class="linenos">26</span></a>        <span class="n">minor</span> <span class="o">+=</span> <span class="mi">1</span>
-</span><span id="increment_version-27"><a href="#increment_version-27"><span class="linenos">27</span></a>        <span class="n">patch</span> <span class="o">=</span> <span class="mi">0</span>
-</span><span id="increment_version-28"><a href="#increment_version-28"><span class="linenos">28</span></a>    <span class="k">elif</span> <span class="n">increment_type</span> <span class="o">==</span> <span class="s2">&quot;patch&quot;</span><span class="p">:</span>
-</span><span id="increment_version-29"><a href="#increment_version-29"><span class="linenos">29</span></a>        <span class="n">patch</span> <span class="o">+=</span> <span class="mi">1</span>
-</span><span id="increment_version-30"><a href="#increment_version-30"><span class="linenos">30</span></a>    <span class="n">incremented_version</span> <span class="o">=</span> <span class="s2">&quot;.&quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="nb">str</span><span class="p">(</span><span class="n">num</span><span class="p">)</span> <span class="k">for</span> <span class="n">num</span> <span class="ow">in</span> <span class="p">[</span><span class="n">major</span><span class="p">,</span> <span class="n">minor</span><span class="p">,</span> <span class="n">patch</span><span class="p">])</span>
-</span><span id="increment_version-31"><a href="#increment_version-31"><span class="linenos">31</span></a>    <span class="n">meta</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;version&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="n">incremented_version</span>
-</span><span id="increment_version-32"><a href="#increment_version-32"><span class="linenos">32</span></a>    <span class="n">pyproject_path</span><span class="o">.</span><span class="n">dumps</span><span class="p">(</span><span class="n">meta</span><span class="p">)</span>
+</span><span id="increment_version-18"><a href="#increment_version-18"><span class="linenos">18</span></a><span class="sd">    :param package_path: Path to the package/project directory.</span>
+</span><span id="increment_version-19"><a href="#increment_version-19"><span class="linenos">19</span></a>
+</span><span id="increment_version-20"><a href="#increment_version-20"><span class="linenos">20</span></a><span class="sd">    :param increment_type: One from &#39;major&#39;, &#39;minor&#39;, or &#39;patch&#39;.&quot;&quot;&quot;</span>
+</span><span id="increment_version-21"><a href="#increment_version-21"><span class="linenos">21</span></a>    <span class="n">meta</span> <span class="o">=</span> <span class="n">pyproject_path</span><span class="o">.</span><span class="n">loads</span><span class="p">()</span>
+</span><span id="increment_version-22"><a href="#increment_version-22"><span class="linenos">22</span></a>    <span class="n">major</span><span class="p">,</span> <span class="n">minor</span><span class="p">,</span> <span class="n">patch</span> <span class="o">=</span> <span class="p">[</span><span class="nb">int</span><span class="p">(</span><span class="n">num</span><span class="p">)</span> <span class="k">for</span> <span class="n">num</span> <span class="ow">in</span> <span class="n">meta</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;version&quot;</span><span class="p">]</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="s2">&quot;.&quot;</span><span class="p">)]</span>
+</span><span id="increment_version-23"><a href="#increment_version-23"><span class="linenos">23</span></a>    <span class="k">if</span> <span class="n">increment_type</span> <span class="o">==</span> <span class="s2">&quot;major&quot;</span><span class="p">:</span>
+</span><span id="increment_version-24"><a href="#increment_version-24"><span class="linenos">24</span></a>        <span class="n">major</span> <span class="o">+=</span> <span class="mi">1</span>
+</span><span id="increment_version-25"><a href="#increment_version-25"><span class="linenos">25</span></a>        <span class="n">minor</span> <span class="o">=</span> <span class="mi">0</span>
+</span><span id="increment_version-26"><a href="#increment_version-26"><span class="linenos">26</span></a>        <span class="n">patch</span> <span class="o">=</span> <span class="mi">0</span>
+</span><span id="increment_version-27"><a href="#increment_version-27"><span class="linenos">27</span></a>    <span class="k">elif</span> <span class="n">increment_type</span> <span class="o">==</span> <span class="s2">&quot;minor&quot;</span><span class="p">:</span>
+</span><span id="increment_version-28"><a href="#increment_version-28"><span class="linenos">28</span></a>        <span class="n">minor</span> <span class="o">+=</span> <span class="mi">1</span>
+</span><span id="increment_version-29"><a href="#increment_version-29"><span class="linenos">29</span></a>        <span class="n">patch</span> <span class="o">=</span> <span class="mi">0</span>
+</span><span id="increment_version-30"><a href="#increment_version-30"><span class="linenos">30</span></a>    <span class="k">elif</span> <span class="n">increment_type</span> <span class="o">==</span> <span class="s2">&quot;patch&quot;</span><span class="p">:</span>
+</span><span id="increment_version-31"><a href="#increment_version-31"><span class="linenos">31</span></a>        <span class="n">patch</span> <span class="o">+=</span> <span class="mi">1</span>
+</span><span id="increment_version-32"><a href="#increment_version-32"><span class="linenos">32</span></a>    <span class="n">incremented_version</span> <span class="o">=</span> <span class="s2">&quot;.&quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="nb">str</span><span class="p">(</span><span class="n">num</span><span class="p">)</span> <span class="k">for</span> <span class="n">num</span> <span class="ow">in</span> <span class="p">[</span><span class="n">major</span><span class="p">,</span> <span class="n">minor</span><span class="p">,</span> <span class="n">patch</span><span class="p">])</span>
+</span><span id="increment_version-33"><a href="#increment_version-33"><span class="linenos">33</span></a>    <span class="n">meta</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;version&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="n">incremented_version</span>
+</span><span id="increment_version-34"><a href="#increment_version-34"><span class="linenos">34</span></a>    <span class="n">pyproject_path</span><span class="o">.</span><span class="n">dumps</span><span class="p">(</span><span class="n">meta</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Increment the project.version field in pyproject.toml.</p>
 
 <h6 id="parameters">Parameters</h6>
 
@@ -275,23 +288,23 @@
         <span class="def">def</span>
         <span class="name">get_minimum_py_version</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">src</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">) -> <span class="nb">str</span>:</span></span>
 
                 <label class="view-source-button" for="get_minimum_py_version-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#get_minimum_py_version"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="get_minimum_py_version-35"><a href="#get_minimum_py_version-35"><span class="linenos">35</span></a><span class="k">def</span> <span class="nf">get_minimum_py_version</span><span class="p">(</span><span class="n">src</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
-</span><span id="get_minimum_py_version-36"><a href="#get_minimum_py_version-36"><span class="linenos">36</span></a>    <span class="sd">&quot;&quot;&quot;Scan src with vermin and return minimum</span>
-</span><span id="get_minimum_py_version-37"><a href="#get_minimum_py_version-37"><span class="linenos">37</span></a><span class="sd">    python version.&quot;&quot;&quot;</span>
-</span><span id="get_minimum_py_version-38"><a href="#get_minimum_py_version-38"><span class="linenos">38</span></a>    <span class="n">config</span> <span class="o">=</span> <span class="n">vermin</span><span class="o">.</span><span class="n">Config</span><span class="p">()</span>
-</span><span id="get_minimum_py_version-39"><a href="#get_minimum_py_version-39"><span class="linenos">39</span></a>    <span class="n">config</span><span class="o">.</span><span class="n">add_backport</span><span class="p">(</span><span class="s2">&quot;typing&quot;</span><span class="p">)</span>
-</span><span id="get_minimum_py_version-40"><a href="#get_minimum_py_version-40"><span class="linenos">40</span></a>    <span class="n">config</span><span class="o">.</span><span class="n">add_backport</span><span class="p">(</span><span class="s2">&quot;typing_extensions&quot;</span><span class="p">)</span>
-</span><span id="get_minimum_py_version-41"><a href="#get_minimum_py_version-41"><span class="linenos">41</span></a>    <span class="n">config</span><span class="o">.</span><span class="n">set_eval_annotations</span><span class="p">(</span><span class="kc">True</span><span class="p">)</span>
-</span><span id="get_minimum_py_version-42"><a href="#get_minimum_py_version-42"><span class="linenos">42</span></a>    <span class="n">result</span> <span class="o">=</span> <span class="n">vermin</span><span class="o">.</span><span class="n">visit</span><span class="p">(</span><span class="n">src</span><span class="p">,</span> <span class="n">config</span><span class="p">)</span><span class="o">.</span><span class="n">minimum_versions</span><span class="p">()[</span><span class="mi">1</span><span class="p">]</span>
-</span><span id="get_minimum_py_version-43"><a href="#get_minimum_py_version-43"><span class="linenos">43</span></a>    <span class="k">return</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">result</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span><span class="si">}</span><span class="s2">.</span><span class="si">{</span><span class="n">result</span><span class="p">[</span><span class="mi">1</span><span class="p">]</span><span class="si">}</span><span class="s2">&quot;</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="get_minimum_py_version-37"><a href="#get_minimum_py_version-37"><span class="linenos">37</span></a><span class="k">def</span> <span class="nf">get_minimum_py_version</span><span class="p">(</span><span class="n">src</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
+</span><span id="get_minimum_py_version-38"><a href="#get_minimum_py_version-38"><span class="linenos">38</span></a>    <span class="sd">&quot;&quot;&quot;Scan src with vermin and return minimum</span>
+</span><span id="get_minimum_py_version-39"><a href="#get_minimum_py_version-39"><span class="linenos">39</span></a><span class="sd">    python version.&quot;&quot;&quot;</span>
+</span><span id="get_minimum_py_version-40"><a href="#get_minimum_py_version-40"><span class="linenos">40</span></a>    <span class="n">config</span> <span class="o">=</span> <span class="n">vermin</span><span class="o">.</span><span class="n">Config</span><span class="p">()</span>
+</span><span id="get_minimum_py_version-41"><a href="#get_minimum_py_version-41"><span class="linenos">41</span></a>    <span class="n">config</span><span class="o">.</span><span class="n">add_backport</span><span class="p">(</span><span class="s2">&quot;typing&quot;</span><span class="p">)</span>
+</span><span id="get_minimum_py_version-42"><a href="#get_minimum_py_version-42"><span class="linenos">42</span></a>    <span class="n">config</span><span class="o">.</span><span class="n">add_backport</span><span class="p">(</span><span class="s2">&quot;typing_extensions&quot;</span><span class="p">)</span>
+</span><span id="get_minimum_py_version-43"><a href="#get_minimum_py_version-43"><span class="linenos">43</span></a>    <span class="n">config</span><span class="o">.</span><span class="n">set_eval_annotations</span><span class="p">(</span><span class="kc">True</span><span class="p">)</span>
+</span><span id="get_minimum_py_version-44"><a href="#get_minimum_py_version-44"><span class="linenos">44</span></a>    <span class="n">result</span> <span class="o">=</span> <span class="n">vermin</span><span class="o">.</span><span class="n">visit</span><span class="p">(</span><span class="n">src</span><span class="p">,</span> <span class="n">config</span><span class="p">)</span><span class="o">.</span><span class="n">minimum_versions</span><span class="p">()[</span><span class="mi">1</span><span class="p">]</span>
+</span><span id="get_minimum_py_version-45"><a href="#get_minimum_py_version-45"><span class="linenos">45</span></a>    <span class="k">return</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">result</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span><span class="si">}</span><span class="s2">.</span><span class="si">{</span><span class="n">result</span><span class="p">[</span><span class="mi">1</span><span class="p">]</span><span class="si">}</span><span class="s2">&quot;</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Scan src with vermin and return minimum
 python version.</p>
 </div>
 
@@ -304,18 +317,18 @@
         <span class="def">def</span>
         <span class="name">get_project_code</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">project_path</span><span class="p">:</span> <span class="n">pathier</span><span class="o">.</span><span class="n">pathier</span><span class="o">.</span><span class="n">Pathier</span></span><span class="return-annotation">) -> <span class="nb">str</span>:</span></span>
 
                 <label class="view-source-button" for="get_project_code-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#get_project_code"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="get_project_code-46"><a href="#get_project_code-46"><span class="linenos">46</span></a><span class="k">def</span> <span class="nf">get_project_code</span><span class="p">(</span><span class="n">project_path</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
-</span><span id="get_project_code-47"><a href="#get_project_code-47"><span class="linenos">47</span></a>    <span class="sd">&quot;&quot;&quot;Read and return all code from project_path</span>
-</span><span id="get_project_code-48"><a href="#get_project_code-48"><span class="linenos">48</span></a><span class="sd">    as one string.&quot;&quot;&quot;</span>
-</span><span id="get_project_code-49"><a href="#get_project_code-49"><span class="linenos">49</span></a>    <span class="k">return</span> <span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">file</span><span class="o">.</span><span class="n">read_text</span><span class="p">()</span> <span class="k">for</span> <span class="n">file</span> <span class="ow">in</span> <span class="n">project_path</span><span class="o">.</span><span class="n">rglob</span><span class="p">(</span><span class="s2">&quot;*.py&quot;</span><span class="p">))</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="get_project_code-48"><a href="#get_project_code-48"><span class="linenos">48</span></a><span class="k">def</span> <span class="nf">get_project_code</span><span class="p">(</span><span class="n">project_path</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
+</span><span id="get_project_code-49"><a href="#get_project_code-49"><span class="linenos">49</span></a>    <span class="sd">&quot;&quot;&quot;Read and return all code from project_path</span>
+</span><span id="get_project_code-50"><a href="#get_project_code-50"><span class="linenos">50</span></a><span class="sd">    as one string.&quot;&quot;&quot;</span>
+</span><span id="get_project_code-51"><a href="#get_project_code-51"><span class="linenos">51</span></a>    <span class="k">return</span> <span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">file</span><span class="o">.</span><span class="n">read_text</span><span class="p">()</span> <span class="k">for</span> <span class="n">file</span> <span class="ow">in</span> <span class="n">project_path</span><span class="o">.</span><span class="n">rglob</span><span class="p">(</span><span class="s2">&quot;*.py&quot;</span><span class="p">))</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Read and return all code from project_path
 as one string.</p>
 </div>
 
@@ -328,24 +341,24 @@
         <span class="def">def</span>
         <span class="name">update_minimum_python_version</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">pyproject_path</span><span class="p">:</span> <span class="n">pathier</span><span class="o">.</span><span class="n">pathier</span><span class="o">.</span><span class="n">Pathier</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="update_minimum_python_version-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#update_minimum_python_version"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="update_minimum_python_version-52"><a href="#update_minimum_python_version-52"><span class="linenos">52</span></a><span class="k">def</span> <span class="nf">update_minimum_python_version</span><span class="p">(</span><span class="n">pyproject_path</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">):</span>
-</span><span id="update_minimum_python_version-53"><a href="#update_minimum_python_version-53"><span class="linenos">53</span></a>    <span class="sd">&quot;&quot;&quot;Use vermin to determine the minimum compatible</span>
-</span><span id="update_minimum_python_version-54"><a href="#update_minimum_python_version-54"><span class="linenos">54</span></a><span class="sd">    Python version and update the corresponding field</span>
-</span><span id="update_minimum_python_version-55"><a href="#update_minimum_python_version-55"><span class="linenos">55</span></a><span class="sd">    in pyproject.toml.&quot;&quot;&quot;</span>
-</span><span id="update_minimum_python_version-56"><a href="#update_minimum_python_version-56"><span class="linenos">56</span></a>    <span class="n">project_code</span> <span class="o">=</span> <span class="n">get_project_code</span><span class="p">(</span><span class="n">pyproject_path</span><span class="o">.</span><span class="n">parent</span> <span class="o">/</span> <span class="s2">&quot;src&quot;</span><span class="p">)</span>
-</span><span id="update_minimum_python_version-57"><a href="#update_minimum_python_version-57"><span class="linenos">57</span></a>    <span class="n">meta</span> <span class="o">=</span> <span class="n">pyproject_path</span><span class="o">.</span><span class="n">loads</span><span class="p">()</span>
-</span><span id="update_minimum_python_version-58"><a href="#update_minimum_python_version-58"><span class="linenos">58</span></a>    <span class="n">minimum_version</span> <span class="o">=</span> <span class="n">get_minimum_py_version</span><span class="p">(</span><span class="n">project_code</span><span class="p">)</span>
-</span><span id="update_minimum_python_version-59"><a href="#update_minimum_python_version-59"><span class="linenos">59</span></a>    <span class="n">minimum_version</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;&gt;=</span><span class="si">{</span><span class="n">minimum_version</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="update_minimum_python_version-60"><a href="#update_minimum_python_version-60"><span class="linenos">60</span></a>    <span class="n">meta</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;requires-python&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="n">minimum_version</span>
-</span><span id="update_minimum_python_version-61"><a href="#update_minimum_python_version-61"><span class="linenos">61</span></a>    <span class="n">pyproject_path</span><span class="o">.</span><span class="n">dumps</span><span class="p">(</span><span class="n">meta</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="update_minimum_python_version-54"><a href="#update_minimum_python_version-54"><span class="linenos">54</span></a><span class="k">def</span> <span class="nf">update_minimum_python_version</span><span class="p">(</span><span class="n">pyproject_path</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">):</span>
+</span><span id="update_minimum_python_version-55"><a href="#update_minimum_python_version-55"><span class="linenos">55</span></a>    <span class="sd">&quot;&quot;&quot;Use vermin to determine the minimum compatible</span>
+</span><span id="update_minimum_python_version-56"><a href="#update_minimum_python_version-56"><span class="linenos">56</span></a><span class="sd">    Python version and update the corresponding field</span>
+</span><span id="update_minimum_python_version-57"><a href="#update_minimum_python_version-57"><span class="linenos">57</span></a><span class="sd">    in pyproject.toml.&quot;&quot;&quot;</span>
+</span><span id="update_minimum_python_version-58"><a href="#update_minimum_python_version-58"><span class="linenos">58</span></a>    <span class="n">project_code</span> <span class="o">=</span> <span class="n">get_project_code</span><span class="p">(</span><span class="n">pyproject_path</span><span class="o">.</span><span class="n">parent</span> <span class="o">/</span> <span class="s2">&quot;src&quot;</span><span class="p">)</span>
+</span><span id="update_minimum_python_version-59"><a href="#update_minimum_python_version-59"><span class="linenos">59</span></a>    <span class="n">meta</span> <span class="o">=</span> <span class="n">pyproject_path</span><span class="o">.</span><span class="n">loads</span><span class="p">()</span>
+</span><span id="update_minimum_python_version-60"><a href="#update_minimum_python_version-60"><span class="linenos">60</span></a>    <span class="n">minimum_version</span> <span class="o">=</span> <span class="n">get_minimum_py_version</span><span class="p">(</span><span class="n">project_code</span><span class="p">)</span>
+</span><span id="update_minimum_python_version-61"><a href="#update_minimum_python_version-61"><span class="linenos">61</span></a>    <span class="n">minimum_version</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;&gt;=</span><span class="si">{</span><span class="n">minimum_version</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="update_minimum_python_version-62"><a href="#update_minimum_python_version-62"><span class="linenos">62</span></a>    <span class="n">meta</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;requires-python&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="n">minimum_version</span>
+</span><span id="update_minimum_python_version-63"><a href="#update_minimum_python_version-63"><span class="linenos">63</span></a>    <span class="n">pyproject_path</span><span class="o">.</span><span class="n">dumps</span><span class="p">(</span><span class="n">meta</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Use vermin to determine the minimum compatible
 Python version and update the corresponding field
 in pyproject.toml.</p>
 </div>
@@ -359,23 +372,23 @@
         <span class="def">def</span>
         <span class="name">generate_docs</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">package_path</span><span class="p">:</span> <span class="n">pathier</span><span class="o">.</span><span class="n">pathier</span><span class="o">.</span><span class="n">Pathier</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="generate_docs-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#generate_docs"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="generate_docs-64"><a href="#generate_docs-64"><span class="linenos">64</span></a><span class="k">def</span> <span class="nf">generate_docs</span><span class="p">(</span><span class="n">package_path</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">):</span>
-</span><span id="generate_docs-65"><a href="#generate_docs-65"><span class="linenos">65</span></a>    <span class="sd">&quot;&quot;&quot;Generate project documentation using pdoc.&quot;&quot;&quot;</span>
-</span><span id="generate_docs-66"><a href="#generate_docs-66"><span class="linenos">66</span></a>    <span class="k">try</span><span class="p">:</span>
-</span><span id="generate_docs-67"><a href="#generate_docs-67"><span class="linenos">67</span></a>        <span class="p">(</span><span class="n">package_path</span> <span class="o">/</span> <span class="s2">&quot;docs&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">delete</span><span class="p">()</span>
-</span><span id="generate_docs-68"><a href="#generate_docs-68"><span class="linenos">68</span></a>    <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
-</span><span id="generate_docs-69"><a href="#generate_docs-69"><span class="linenos">69</span></a>        <span class="k">pass</span>
-</span><span id="generate_docs-70"><a href="#generate_docs-70"><span class="linenos">70</span></a>    <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span>
-</span><span id="generate_docs-71"><a href="#generate_docs-71"><span class="linenos">71</span></a>        <span class="sa">f</span><span class="s2">&quot;pdoc -o </span><span class="si">{</span><span class="n">package_path</span> <span class="o">/</span> <span class="s1">&#39;docs&#39;</span><span class="si">}</span><span class="s2"> </span><span class="si">{</span><span class="n">package_path</span> <span class="o">/</span> <span class="s1">&#39;src&#39;</span> <span class="o">/</span> <span class="n">package_path</span><span class="o">.</span><span class="n">stem</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="generate_docs-72"><a href="#generate_docs-72"><span class="linenos">72</span></a>    <span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="generate_docs-66"><a href="#generate_docs-66"><span class="linenos">66</span></a><span class="k">def</span> <span class="nf">generate_docs</span><span class="p">(</span><span class="n">package_path</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">):</span>
+</span><span id="generate_docs-67"><a href="#generate_docs-67"><span class="linenos">67</span></a>    <span class="sd">&quot;&quot;&quot;Generate project documentation using pdoc.&quot;&quot;&quot;</span>
+</span><span id="generate_docs-68"><a href="#generate_docs-68"><span class="linenos">68</span></a>    <span class="k">try</span><span class="p">:</span>
+</span><span id="generate_docs-69"><a href="#generate_docs-69"><span class="linenos">69</span></a>        <span class="p">(</span><span class="n">package_path</span> <span class="o">/</span> <span class="s2">&quot;docs&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">delete</span><span class="p">()</span>
+</span><span id="generate_docs-70"><a href="#generate_docs-70"><span class="linenos">70</span></a>    <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="generate_docs-71"><a href="#generate_docs-71"><span class="linenos">71</span></a>        <span class="k">pass</span>
+</span><span id="generate_docs-72"><a href="#generate_docs-72"><span class="linenos">72</span></a>    <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span>
+</span><span id="generate_docs-73"><a href="#generate_docs-73"><span class="linenos">73</span></a>        <span class="sa">f</span><span class="s2">&quot;pdoc -o </span><span class="si">{</span><span class="n">package_path</span> <span class="o">/</span> <span class="s1">&#39;docs&#39;</span><span class="si">}</span><span class="s2"> </span><span class="si">{</span><span class="n">package_path</span> <span class="o">/</span> <span class="s1">&#39;src&#39;</span> <span class="o">/</span> <span class="n">package_path</span><span class="o">.</span><span class="n">stem</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="generate_docs-74"><a href="#generate_docs-74"><span class="linenos">74</span></a>    <span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Generate project documentation using pdoc.</p>
 </div>
 
 
@@ -387,53 +400,53 @@
         <span class="def">def</span>
         <span class="name">update_dependencies</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="n">pyproject_path</span><span class="p">:</span> <span class="n">pathier</span><span class="o">.</span><span class="n">pathier</span><span class="o">.</span><span class="n">Pathier</span>,</span><span class="param">	<span class="n">overwrite</span><span class="p">:</span> <span class="nb">bool</span>,</span><span class="param">	<span class="n">include_versions</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="update_dependencies-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#update_dependencies"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="update_dependencies-75"><a href="#update_dependencies-75"><span class="linenos"> 75</span></a><span class="k">def</span> <span class="nf">update_dependencies</span><span class="p">(</span>
-</span><span id="update_dependencies-76"><a href="#update_dependencies-76"><span class="linenos"> 76</span></a>    <span class="n">pyproject_path</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">,</span> <span class="n">overwrite</span><span class="p">:</span> <span class="nb">bool</span><span class="p">,</span> <span class="n">include_versions</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span>
-</span><span id="update_dependencies-77"><a href="#update_dependencies-77"><span class="linenos"> 77</span></a><span class="p">):</span>
-</span><span id="update_dependencies-78"><a href="#update_dependencies-78"><span class="linenos"> 78</span></a>    <span class="sd">&quot;&quot;&quot;Update dependencies list in pyproject.toml.</span>
-</span><span id="update_dependencies-79"><a href="#update_dependencies-79"><span class="linenos"> 79</span></a>
-</span><span id="update_dependencies-80"><a href="#update_dependencies-80"><span class="linenos"> 80</span></a><span class="sd">    :param overwrite: If True, replace the dependencies in pyproject.toml</span>
-</span><span id="update_dependencies-81"><a href="#update_dependencies-81"><span class="linenos"> 81</span></a><span class="sd">    with the results of packagelister.scan() .</span>
-</span><span id="update_dependencies-82"><a href="#update_dependencies-82"><span class="linenos"> 82</span></a><span class="sd">    If False, packages returned by packagelister are appended to</span>
-</span><span id="update_dependencies-83"><a href="#update_dependencies-83"><span class="linenos"> 83</span></a><span class="sd">    the current dependencies in pyproject.toml if they don&#39;t already</span>
-</span><span id="update_dependencies-84"><a href="#update_dependencies-84"><span class="linenos"> 84</span></a><span class="sd">    exist in the field.&quot;&quot;&quot;</span>
-</span><span id="update_dependencies-85"><a href="#update_dependencies-85"><span class="linenos"> 85</span></a>    <span class="n">packages</span> <span class="o">=</span> <span class="n">packagelister</span><span class="o">.</span><span class="n">scan</span><span class="p">(</span><span class="n">pyproject_path</span><span class="o">.</span><span class="n">parent</span><span class="p">)</span>
-</span><span id="update_dependencies-86"><a href="#update_dependencies-86"><span class="linenos"> 86</span></a>
-</span><span id="update_dependencies-87"><a href="#update_dependencies-87"><span class="linenos"> 87</span></a>    <span class="n">packages</span> <span class="o">=</span> <span class="p">[</span>
-</span><span id="update_dependencies-88"><a href="#update_dependencies-88"><span class="linenos"> 88</span></a>        <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">package</span><span class="si">}</span><span class="s2">~=</span><span class="si">{</span><span class="n">packages</span><span class="p">[</span><span class="n">package</span><span class="p">][</span><span class="s1">&#39;version&#39;</span><span class="p">]</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="update_dependencies-89"><a href="#update_dependencies-89"><span class="linenos"> 89</span></a>        <span class="k">if</span> <span class="n">packages</span><span class="p">[</span><span class="n">package</span><span class="p">][</span><span class="s2">&quot;version&quot;</span><span class="p">]</span> <span class="ow">and</span> <span class="n">include_versions</span>
-</span><span id="update_dependencies-90"><a href="#update_dependencies-90"><span class="linenos"> 90</span></a>        <span class="k">else</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">package</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="update_dependencies-91"><a href="#update_dependencies-91"><span class="linenos"> 91</span></a>        <span class="k">for</span> <span class="n">package</span> <span class="ow">in</span> <span class="n">packages</span>
-</span><span id="update_dependencies-92"><a href="#update_dependencies-92"><span class="linenos"> 92</span></a>        <span class="k">if</span> <span class="n">package</span> <span class="o">!=</span> <span class="n">pyproject_path</span><span class="o">.</span><span class="n">parent</span><span class="o">.</span><span class="n">stem</span>
-</span><span id="update_dependencies-93"><a href="#update_dependencies-93"><span class="linenos"> 93</span></a>    <span class="p">]</span>
-</span><span id="update_dependencies-94"><a href="#update_dependencies-94"><span class="linenos"> 94</span></a>    <span class="n">packages</span> <span class="o">=</span> <span class="p">[</span>
-</span><span id="update_dependencies-95"><a href="#update_dependencies-95"><span class="linenos"> 95</span></a>        <span class="n">package</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span><span class="s2">&quot;speech_recognition&quot;</span><span class="p">,</span> <span class="s2">&quot;speechRecognition&quot;</span><span class="p">)</span>
-</span><span id="update_dependencies-96"><a href="#update_dependencies-96"><span class="linenos"> 96</span></a>        <span class="k">for</span> <span class="n">package</span> <span class="ow">in</span> <span class="n">packages</span>
-</span><span id="update_dependencies-97"><a href="#update_dependencies-97"><span class="linenos"> 97</span></a>    <span class="p">]</span>
-</span><span id="update_dependencies-98"><a href="#update_dependencies-98"><span class="linenos"> 98</span></a>    <span class="n">meta</span> <span class="o">=</span> <span class="n">pyproject_path</span><span class="o">.</span><span class="n">loads</span><span class="p">()</span>
-</span><span id="update_dependencies-99"><a href="#update_dependencies-99"><span class="linenos"> 99</span></a>    <span class="k">if</span> <span class="n">overwrite</span><span class="p">:</span>
-</span><span id="update_dependencies-100"><a href="#update_dependencies-100"><span class="linenos">100</span></a>        <span class="n">meta</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;dependencies&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="n">packages</span>
-</span><span id="update_dependencies-101"><a href="#update_dependencies-101"><span class="linenos">101</span></a>    <span class="k">else</span><span class="p">:</span>
-</span><span id="update_dependencies-102"><a href="#update_dependencies-102"><span class="linenos">102</span></a>        <span class="k">for</span> <span class="n">package</span> <span class="ow">in</span> <span class="n">packages</span><span class="p">:</span>
-</span><span id="update_dependencies-103"><a href="#update_dependencies-103"><span class="linenos">103</span></a>            <span class="k">if</span> <span class="s2">&quot;~&quot;</span> <span class="ow">in</span> <span class="n">package</span><span class="p">:</span>
-</span><span id="update_dependencies-104"><a href="#update_dependencies-104"><span class="linenos">104</span></a>                <span class="n">name</span> <span class="o">=</span> <span class="n">package</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="s2">&quot;~&quot;</span><span class="p">)[</span><span class="mi">0</span><span class="p">]</span>
-</span><span id="update_dependencies-105"><a href="#update_dependencies-105"><span class="linenos">105</span></a>            <span class="k">elif</span> <span class="s2">&quot;=&quot;</span> <span class="ow">in</span> <span class="n">package</span><span class="p">:</span>
-</span><span id="update_dependencies-106"><a href="#update_dependencies-106"><span class="linenos">106</span></a>                <span class="n">name</span> <span class="o">=</span> <span class="n">package</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="s2">&quot;=&quot;</span><span class="p">)[</span><span class="mi">0</span><span class="p">]</span>
-</span><span id="update_dependencies-107"><a href="#update_dependencies-107"><span class="linenos">107</span></a>            <span class="k">else</span><span class="p">:</span>
-</span><span id="update_dependencies-108"><a href="#update_dependencies-108"><span class="linenos">108</span></a>                <span class="n">name</span> <span class="o">=</span> <span class="n">package</span>
-</span><span id="update_dependencies-109"><a href="#update_dependencies-109"><span class="linenos">109</span></a>            <span class="k">if</span> <span class="nb">all</span><span class="p">(</span>
-</span><span id="update_dependencies-110"><a href="#update_dependencies-110"><span class="linenos">110</span></a>                <span class="n">name</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">dependency</span> <span class="k">for</span> <span class="n">dependency</span> <span class="ow">in</span> <span class="n">meta</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;dependencies&quot;</span><span class="p">]</span>
-</span><span id="update_dependencies-111"><a href="#update_dependencies-111"><span class="linenos">111</span></a>            <span class="p">):</span>
-</span><span id="update_dependencies-112"><a href="#update_dependencies-112"><span class="linenos">112</span></a>                <span class="n">meta</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;dependencies&quot;</span><span class="p">]</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">package</span><span class="p">)</span>
-</span><span id="update_dependencies-113"><a href="#update_dependencies-113"><span class="linenos">113</span></a>    <span class="n">pyproject_path</span><span class="o">.</span><span class="n">dumps</span><span class="p">(</span><span class="n">meta</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="update_dependencies-77"><a href="#update_dependencies-77"><span class="linenos"> 77</span></a><span class="k">def</span> <span class="nf">update_dependencies</span><span class="p">(</span>
+</span><span id="update_dependencies-78"><a href="#update_dependencies-78"><span class="linenos"> 78</span></a>    <span class="n">pyproject_path</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">,</span> <span class="n">overwrite</span><span class="p">:</span> <span class="nb">bool</span><span class="p">,</span> <span class="n">include_versions</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span>
+</span><span id="update_dependencies-79"><a href="#update_dependencies-79"><span class="linenos"> 79</span></a><span class="p">):</span>
+</span><span id="update_dependencies-80"><a href="#update_dependencies-80"><span class="linenos"> 80</span></a>    <span class="sd">&quot;&quot;&quot;Update dependencies list in pyproject.toml.</span>
+</span><span id="update_dependencies-81"><a href="#update_dependencies-81"><span class="linenos"> 81</span></a>
+</span><span id="update_dependencies-82"><a href="#update_dependencies-82"><span class="linenos"> 82</span></a><span class="sd">    :param overwrite: If True, replace the dependencies in pyproject.toml</span>
+</span><span id="update_dependencies-83"><a href="#update_dependencies-83"><span class="linenos"> 83</span></a><span class="sd">    with the results of packagelister.scan() .</span>
+</span><span id="update_dependencies-84"><a href="#update_dependencies-84"><span class="linenos"> 84</span></a><span class="sd">    If False, packages returned by packagelister are appended to</span>
+</span><span id="update_dependencies-85"><a href="#update_dependencies-85"><span class="linenos"> 85</span></a><span class="sd">    the current dependencies in pyproject.toml if they don&#39;t already</span>
+</span><span id="update_dependencies-86"><a href="#update_dependencies-86"><span class="linenos"> 86</span></a><span class="sd">    exist in the field.&quot;&quot;&quot;</span>
+</span><span id="update_dependencies-87"><a href="#update_dependencies-87"><span class="linenos"> 87</span></a>    <span class="n">packages</span> <span class="o">=</span> <span class="n">packagelister</span><span class="o">.</span><span class="n">scan</span><span class="p">(</span><span class="n">pyproject_path</span><span class="o">.</span><span class="n">parent</span><span class="p">)</span>
+</span><span id="update_dependencies-88"><a href="#update_dependencies-88"><span class="linenos"> 88</span></a>
+</span><span id="update_dependencies-89"><a href="#update_dependencies-89"><span class="linenos"> 89</span></a>    <span class="n">packages</span> <span class="o">=</span> <span class="p">[</span>
+</span><span id="update_dependencies-90"><a href="#update_dependencies-90"><span class="linenos"> 90</span></a>        <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">package</span><span class="si">}</span><span class="s2">~=</span><span class="si">{</span><span class="n">packages</span><span class="p">[</span><span class="n">package</span><span class="p">][</span><span class="s1">&#39;version&#39;</span><span class="p">]</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="update_dependencies-91"><a href="#update_dependencies-91"><span class="linenos"> 91</span></a>        <span class="k">if</span> <span class="n">packages</span><span class="p">[</span><span class="n">package</span><span class="p">][</span><span class="s2">&quot;version&quot;</span><span class="p">]</span> <span class="ow">and</span> <span class="n">include_versions</span>
+</span><span id="update_dependencies-92"><a href="#update_dependencies-92"><span class="linenos"> 92</span></a>        <span class="k">else</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">package</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="update_dependencies-93"><a href="#update_dependencies-93"><span class="linenos"> 93</span></a>        <span class="k">for</span> <span class="n">package</span> <span class="ow">in</span> <span class="n">packages</span>
+</span><span id="update_dependencies-94"><a href="#update_dependencies-94"><span class="linenos"> 94</span></a>        <span class="k">if</span> <span class="n">package</span> <span class="o">!=</span> <span class="n">pyproject_path</span><span class="o">.</span><span class="n">parent</span><span class="o">.</span><span class="n">stem</span>
+</span><span id="update_dependencies-95"><a href="#update_dependencies-95"><span class="linenos"> 95</span></a>    <span class="p">]</span>
+</span><span id="update_dependencies-96"><a href="#update_dependencies-96"><span class="linenos"> 96</span></a>    <span class="n">packages</span> <span class="o">=</span> <span class="p">[</span>
+</span><span id="update_dependencies-97"><a href="#update_dependencies-97"><span class="linenos"> 97</span></a>        <span class="n">package</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span><span class="s2">&quot;speech_recognition&quot;</span><span class="p">,</span> <span class="s2">&quot;speechRecognition&quot;</span><span class="p">)</span>
+</span><span id="update_dependencies-98"><a href="#update_dependencies-98"><span class="linenos"> 98</span></a>        <span class="k">for</span> <span class="n">package</span> <span class="ow">in</span> <span class="n">packages</span>
+</span><span id="update_dependencies-99"><a href="#update_dependencies-99"><span class="linenos"> 99</span></a>    <span class="p">]</span>
+</span><span id="update_dependencies-100"><a href="#update_dependencies-100"><span class="linenos">100</span></a>    <span class="n">meta</span> <span class="o">=</span> <span class="n">pyproject_path</span><span class="o">.</span><span class="n">loads</span><span class="p">()</span>
+</span><span id="update_dependencies-101"><a href="#update_dependencies-101"><span class="linenos">101</span></a>    <span class="k">if</span> <span class="n">overwrite</span><span class="p">:</span>
+</span><span id="update_dependencies-102"><a href="#update_dependencies-102"><span class="linenos">102</span></a>        <span class="n">meta</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;dependencies&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="n">packages</span>
+</span><span id="update_dependencies-103"><a href="#update_dependencies-103"><span class="linenos">103</span></a>    <span class="k">else</span><span class="p">:</span>
+</span><span id="update_dependencies-104"><a href="#update_dependencies-104"><span class="linenos">104</span></a>        <span class="k">for</span> <span class="n">package</span> <span class="ow">in</span> <span class="n">packages</span><span class="p">:</span>
+</span><span id="update_dependencies-105"><a href="#update_dependencies-105"><span class="linenos">105</span></a>            <span class="k">if</span> <span class="s2">&quot;~&quot;</span> <span class="ow">in</span> <span class="n">package</span><span class="p">:</span>
+</span><span id="update_dependencies-106"><a href="#update_dependencies-106"><span class="linenos">106</span></a>                <span class="n">name</span> <span class="o">=</span> <span class="n">package</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="s2">&quot;~&quot;</span><span class="p">)[</span><span class="mi">0</span><span class="p">]</span>
+</span><span id="update_dependencies-107"><a href="#update_dependencies-107"><span class="linenos">107</span></a>            <span class="k">elif</span> <span class="s2">&quot;=&quot;</span> <span class="ow">in</span> <span class="n">package</span><span class="p">:</span>
+</span><span id="update_dependencies-108"><a href="#update_dependencies-108"><span class="linenos">108</span></a>                <span class="n">name</span> <span class="o">=</span> <span class="n">package</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="s2">&quot;=&quot;</span><span class="p">)[</span><span class="mi">0</span><span class="p">]</span>
+</span><span id="update_dependencies-109"><a href="#update_dependencies-109"><span class="linenos">109</span></a>            <span class="k">else</span><span class="p">:</span>
+</span><span id="update_dependencies-110"><a href="#update_dependencies-110"><span class="linenos">110</span></a>                <span class="n">name</span> <span class="o">=</span> <span class="n">package</span>
+</span><span id="update_dependencies-111"><a href="#update_dependencies-111"><span class="linenos">111</span></a>            <span class="k">if</span> <span class="nb">all</span><span class="p">(</span>
+</span><span id="update_dependencies-112"><a href="#update_dependencies-112"><span class="linenos">112</span></a>                <span class="n">name</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">dependency</span> <span class="k">for</span> <span class="n">dependency</span> <span class="ow">in</span> <span class="n">meta</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;dependencies&quot;</span><span class="p">]</span>
+</span><span id="update_dependencies-113"><a href="#update_dependencies-113"><span class="linenos">113</span></a>            <span class="p">):</span>
+</span><span id="update_dependencies-114"><a href="#update_dependencies-114"><span class="linenos">114</span></a>                <span class="n">meta</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;dependencies&quot;</span><span class="p">]</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">package</span><span class="p">)</span>
+</span><span id="update_dependencies-115"><a href="#update_dependencies-115"><span class="linenos">115</span></a>    <span class="n">pyproject_path</span><span class="o">.</span><span class="n">dumps</span><span class="p">(</span><span class="n">meta</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Update dependencies list in pyproject.toml.</p>
 
 <h6 id="parameters">Parameters</h6>
 
@@ -455,30 +468,30 @@
         <span class="def">def</span>
         <span class="name">update_changelog</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">pyproject_path</span><span class="p">:</span> <span class="n">pathier</span><span class="o">.</span><span class="n">pathier</span><span class="o">.</span><span class="n">Pathier</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="update_changelog-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#update_changelog"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="update_changelog-116"><a href="#update_changelog-116"><span class="linenos">116</span></a><span class="k">def</span> <span class="nf">update_changelog</span><span class="p">(</span><span class="n">pyproject_path</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">):</span>
-</span><span id="update_changelog-117"><a href="#update_changelog-117"><span class="linenos">117</span></a>    <span class="sd">&quot;&quot;&quot;Update project changelog.&quot;&quot;&quot;</span>
-</span><span id="update_changelog-118"><a href="#update_changelog-118"><span class="linenos">118</span></a>    <span class="n">meta</span> <span class="o">=</span> <span class="n">pyproject_path</span><span class="o">.</span><span class="n">loads</span><span class="p">()</span>
-</span><span id="update_changelog-119"><a href="#update_changelog-119"><span class="linenos">119</span></a>    <span class="k">if</span> <span class="n">hassle_config</span><span class="o">.</span><span class="n">config_exists</span><span class="p">():</span>
-</span><span id="update_changelog-120"><a href="#update_changelog-120"><span class="linenos">120</span></a>        <span class="n">config</span> <span class="o">=</span> <span class="n">hassle_config</span><span class="o">.</span><span class="n">load_config</span><span class="p">()</span>
-</span><span id="update_changelog-121"><a href="#update_changelog-121"><span class="linenos">121</span></a>    <span class="k">else</span><span class="p">:</span>
-</span><span id="update_changelog-122"><a href="#update_changelog-122"><span class="linenos">122</span></a>        <span class="n">hassle_config</span><span class="o">.</span><span class="n">warn</span><span class="p">()</span>
-</span><span id="update_changelog-123"><a href="#update_changelog-123"><span class="linenos">123</span></a>        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Creating blank hassle_config.toml...&quot;</span><span class="p">)</span>
-</span><span id="update_changelog-124"><a href="#update_changelog-124"><span class="linenos">124</span></a>        <span class="n">config</span> <span class="o">=</span> <span class="n">hassle_config</span><span class="o">.</span><span class="n">load_config</span><span class="p">()</span>
-</span><span id="update_changelog-125"><a href="#update_changelog-125"><span class="linenos">125</span></a>    <span class="n">changelog_path</span> <span class="o">=</span> <span class="n">pyproject_path</span><span class="o">.</span><span class="n">parent</span> <span class="o">/</span> <span class="s2">&quot;CHANGELOG.md&quot;</span>
-</span><span id="update_changelog-126"><a href="#update_changelog-126"><span class="linenos">126</span></a>    <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span>
-</span><span id="update_changelog-127"><a href="#update_changelog-127"><span class="linenos">127</span></a>        <span class="sa">f</span><span class="s2">&quot;auto-changelog -p </span><span class="si">{</span><span class="n">pyproject_path</span><span class="o">.</span><span class="n">parent</span><span class="si">}</span><span class="s2"> --tag-prefix </span><span class="si">{</span><span class="n">config</span><span class="p">[</span><span class="s1">&#39;git&#39;</span><span class="p">][</span><span class="s1">&#39;tag_prefix&#39;</span><span class="p">]</span><span class="si">}</span><span class="s2"> --unreleased -v </span><span class="si">{</span><span class="n">meta</span><span class="p">[</span><span class="s1">&#39;project&#39;</span><span class="p">][</span><span class="s1">&#39;version&#39;</span><span class="p">]</span><span class="si">}</span><span class="s2"> -o </span><span class="si">{</span><span class="n">changelog_path</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="update_changelog-128"><a href="#update_changelog-128"><span class="linenos">128</span></a>    <span class="p">)</span>
-</span><span id="update_changelog-129"><a href="#update_changelog-129"><span class="linenos">129</span></a>    <span class="n">changelog</span> <span class="o">=</span> <span class="n">changelog_path</span><span class="o">.</span><span class="n">read_text</span><span class="p">()</span><span class="o">.</span><span class="n">splitlines</span><span class="p">()</span>
-</span><span id="update_changelog-130"><a href="#update_changelog-130"><span class="linenos">130</span></a>    <span class="n">changelog</span> <span class="o">=</span> <span class="p">[</span><span class="n">line</span> <span class="k">for</span> <span class="n">line</span> <span class="ow">in</span> <span class="n">changelog</span> <span class="k">if</span> <span class="s2">&quot;Full set of changes:&quot;</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">line</span><span class="p">]</span>
-</span><span id="update_changelog-131"><a href="#update_changelog-131"><span class="linenos">131</span></a>    <span class="n">changelog_path</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span><span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">changelog</span><span class="p">))</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="update_changelog-118"><a href="#update_changelog-118"><span class="linenos">118</span></a><span class="k">def</span> <span class="nf">update_changelog</span><span class="p">(</span><span class="n">pyproject_path</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">):</span>
+</span><span id="update_changelog-119"><a href="#update_changelog-119"><span class="linenos">119</span></a>    <span class="sd">&quot;&quot;&quot;Update project changelog.&quot;&quot;&quot;</span>
+</span><span id="update_changelog-120"><a href="#update_changelog-120"><span class="linenos">120</span></a>    <span class="n">meta</span> <span class="o">=</span> <span class="n">pyproject_path</span><span class="o">.</span><span class="n">loads</span><span class="p">()</span>
+</span><span id="update_changelog-121"><a href="#update_changelog-121"><span class="linenos">121</span></a>    <span class="k">if</span> <span class="n">hassle_config</span><span class="o">.</span><span class="n">config_exists</span><span class="p">():</span>
+</span><span id="update_changelog-122"><a href="#update_changelog-122"><span class="linenos">122</span></a>        <span class="n">config</span> <span class="o">=</span> <span class="n">hassle_config</span><span class="o">.</span><span class="n">load_config</span><span class="p">()</span>
+</span><span id="update_changelog-123"><a href="#update_changelog-123"><span class="linenos">123</span></a>    <span class="k">else</span><span class="p">:</span>
+</span><span id="update_changelog-124"><a href="#update_changelog-124"><span class="linenos">124</span></a>        <span class="n">hassle_config</span><span class="o">.</span><span class="n">warn</span><span class="p">()</span>
+</span><span id="update_changelog-125"><a href="#update_changelog-125"><span class="linenos">125</span></a>        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Creating blank hassle_config.toml...&quot;</span><span class="p">)</span>
+</span><span id="update_changelog-126"><a href="#update_changelog-126"><span class="linenos">126</span></a>        <span class="n">config</span> <span class="o">=</span> <span class="n">hassle_config</span><span class="o">.</span><span class="n">load_config</span><span class="p">()</span>
+</span><span id="update_changelog-127"><a href="#update_changelog-127"><span class="linenos">127</span></a>    <span class="n">changelog_path</span> <span class="o">=</span> <span class="n">pyproject_path</span><span class="o">.</span><span class="n">parent</span> <span class="o">/</span> <span class="s2">&quot;CHANGELOG.md&quot;</span>
+</span><span id="update_changelog-128"><a href="#update_changelog-128"><span class="linenos">128</span></a>    <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span>
+</span><span id="update_changelog-129"><a href="#update_changelog-129"><span class="linenos">129</span></a>        <span class="sa">f</span><span class="s2">&quot;auto-changelog -p </span><span class="si">{</span><span class="n">pyproject_path</span><span class="o">.</span><span class="n">parent</span><span class="si">}</span><span class="s2"> --tag-prefix </span><span class="si">{</span><span class="n">config</span><span class="p">[</span><span class="s1">&#39;git&#39;</span><span class="p">][</span><span class="s1">&#39;tag_prefix&#39;</span><span class="p">]</span><span class="si">}</span><span class="s2"> --unreleased -v </span><span class="si">{</span><span class="n">meta</span><span class="p">[</span><span class="s1">&#39;project&#39;</span><span class="p">][</span><span class="s1">&#39;version&#39;</span><span class="p">]</span><span class="si">}</span><span class="s2"> -o </span><span class="si">{</span><span class="n">changelog_path</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="update_changelog-130"><a href="#update_changelog-130"><span class="linenos">130</span></a>    <span class="p">)</span>
+</span><span id="update_changelog-131"><a href="#update_changelog-131"><span class="linenos">131</span></a>    <span class="n">changelog</span> <span class="o">=</span> <span class="n">changelog_path</span><span class="o">.</span><span class="n">read_text</span><span class="p">()</span><span class="o">.</span><span class="n">splitlines</span><span class="p">()</span>
+</span><span id="update_changelog-132"><a href="#update_changelog-132"><span class="linenos">132</span></a>    <span class="n">changelog</span> <span class="o">=</span> <span class="p">[</span><span class="n">line</span> <span class="k">for</span> <span class="n">line</span> <span class="ow">in</span> <span class="n">changelog</span> <span class="k">if</span> <span class="s2">&quot;Full set of changes:&quot;</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">line</span><span class="p">]</span>
+</span><span id="update_changelog-133"><a href="#update_changelog-133"><span class="linenos">133</span></a>    <span class="n">changelog_path</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span><span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">changelog</span><span class="p">))</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Update project changelog.</p>
 </div>
 
 
@@ -490,34 +503,59 @@
         <span class="def">def</span>
         <span class="name">tag_version</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">package_path</span><span class="p">:</span> <span class="n">pathier</span><span class="o">.</span><span class="n">pathier</span><span class="o">.</span><span class="n">Pathier</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="tag_version-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#tag_version"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="tag_version-134"><a href="#tag_version-134"><span class="linenos">134</span></a><span class="k">def</span> <span class="nf">tag_version</span><span class="p">(</span><span class="n">package_path</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">):</span>
-</span><span id="tag_version-135"><a href="#tag_version-135"><span class="linenos">135</span></a>    <span class="sd">&quot;&quot;&quot;Add a git tag corresponding</span>
-</span><span id="tag_version-136"><a href="#tag_version-136"><span class="linenos">136</span></a><span class="sd">    to the version number in pyproject.toml.&quot;&quot;&quot;</span>
-</span><span id="tag_version-137"><a href="#tag_version-137"><span class="linenos">137</span></a>    <span class="k">if</span> <span class="n">hassle_config</span><span class="o">.</span><span class="n">config_exists</span><span class="p">():</span>
-</span><span id="tag_version-138"><a href="#tag_version-138"><span class="linenos">138</span></a>        <span class="n">tag_prefix</span> <span class="o">=</span> <span class="n">hassle_config</span><span class="o">.</span><span class="n">load_config</span><span class="p">()[</span><span class="s2">&quot;git&quot;</span><span class="p">][</span><span class="s2">&quot;tag_prefix&quot;</span><span class="p">]</span>
-</span><span id="tag_version-139"><a href="#tag_version-139"><span class="linenos">139</span></a>    <span class="k">else</span><span class="p">:</span>
-</span><span id="tag_version-140"><a href="#tag_version-140"><span class="linenos">140</span></a>        <span class="n">hassle_config</span><span class="o">.</span><span class="n">warn</span><span class="p">()</span>
-</span><span id="tag_version-141"><a href="#tag_version-141"><span class="linenos">141</span></a>        <span class="n">tag_prefix</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
-</span><span id="tag_version-142"><a href="#tag_version-142"><span class="linenos">142</span></a>    <span class="n">version</span> <span class="o">=</span> <span class="p">(</span><span class="n">package_path</span> <span class="o">/</span> <span class="s2">&quot;pyproject.toml&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">loads</span><span class="p">()[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;version&quot;</span><span class="p">]</span>
-</span><span id="tag_version-143"><a href="#tag_version-143"><span class="linenos">143</span></a>    <span class="n">os</span><span class="o">.</span><span class="n">chdir</span><span class="p">(</span><span class="n">package_path</span><span class="p">)</span>
-</span><span id="tag_version-144"><a href="#tag_version-144"><span class="linenos">144</span></a>    <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;git tag </span><span class="si">{</span><span class="n">tag_prefix</span><span class="si">}{</span><span class="n">version</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="tag_version-136"><a href="#tag_version-136"><span class="linenos">136</span></a><span class="k">def</span> <span class="nf">tag_version</span><span class="p">(</span><span class="n">package_path</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">):</span>
+</span><span id="tag_version-137"><a href="#tag_version-137"><span class="linenos">137</span></a>    <span class="sd">&quot;&quot;&quot;Add a git tag corresponding</span>
+</span><span id="tag_version-138"><a href="#tag_version-138"><span class="linenos">138</span></a><span class="sd">    to the version number in pyproject.toml.&quot;&quot;&quot;</span>
+</span><span id="tag_version-139"><a href="#tag_version-139"><span class="linenos">139</span></a>    <span class="k">if</span> <span class="n">hassle_config</span><span class="o">.</span><span class="n">config_exists</span><span class="p">():</span>
+</span><span id="tag_version-140"><a href="#tag_version-140"><span class="linenos">140</span></a>        <span class="n">tag_prefix</span> <span class="o">=</span> <span class="n">hassle_config</span><span class="o">.</span><span class="n">load_config</span><span class="p">()[</span><span class="s2">&quot;git&quot;</span><span class="p">][</span><span class="s2">&quot;tag_prefix&quot;</span><span class="p">]</span>
+</span><span id="tag_version-141"><a href="#tag_version-141"><span class="linenos">141</span></a>    <span class="k">else</span><span class="p">:</span>
+</span><span id="tag_version-142"><a href="#tag_version-142"><span class="linenos">142</span></a>        <span class="n">hassle_config</span><span class="o">.</span><span class="n">warn</span><span class="p">()</span>
+</span><span id="tag_version-143"><a href="#tag_version-143"><span class="linenos">143</span></a>        <span class="n">tag_prefix</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
+</span><span id="tag_version-144"><a href="#tag_version-144"><span class="linenos">144</span></a>    <span class="n">version</span> <span class="o">=</span> <span class="p">(</span><span class="n">package_path</span> <span class="o">/</span> <span class="s2">&quot;pyproject.toml&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">loads</span><span class="p">()[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;version&quot;</span><span class="p">]</span>
+</span><span id="tag_version-145"><a href="#tag_version-145"><span class="linenos">145</span></a>    <span class="n">os</span><span class="o">.</span><span class="n">chdir</span><span class="p">(</span><span class="n">package_path</span><span class="p">)</span>
+</span><span id="tag_version-146"><a href="#tag_version-146"><span class="linenos">146</span></a>    <span class="n">git</span><span class="o">.</span><span class="n">tag</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">tag_prefix</span><span class="si">}{</span><span class="n">version</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Add a git tag corresponding
 to the version number in pyproject.toml.</p>
 </div>
 
 
                 </section>
+                <section id="format_files">
+                            <input id="format_files-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
+<div class="attr function">
+            
+        <span class="def">def</span>
+        <span class="name">format_files</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">path</span><span class="p">:</span> <span class="n">pathier</span><span class="o">.</span><span class="n">pathier</span><span class="o">.</span><span class="n">Pathier</span></span><span class="return-annotation">):</span></span>
+
+                <label class="view-source-button" for="format_files-view-source"><span>View Source</span></label>
+
+    </div>
+    <a class="headerlink" href="#format_files"></a>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="format_files-149"><a href="#format_files-149"><span class="linenos">149</span></a><span class="k">def</span> <span class="nf">format_files</span><span class="p">(</span><span class="n">path</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">):</span>
+</span><span id="format_files-150"><a href="#format_files-150"><span class="linenos">150</span></a>    <span class="sd">&quot;&quot;&quot;Use `Black` to format file(s).&quot;&quot;&quot;</span>
+</span><span id="format_files-151"><a href="#format_files-151"><span class="linenos">151</span></a>    <span class="k">try</span><span class="p">:</span>
+</span><span id="format_files-152"><a href="#format_files-152"><span class="linenos">152</span></a>        <span class="n">black</span><span class="o">.</span><span class="n">main</span><span class="p">([</span><span class="nb">str</span><span class="p">(</span><span class="n">path</span><span class="p">)])</span>
+</span><span id="format_files-153"><a href="#format_files-153"><span class="linenos">153</span></a>    <span class="k">except</span> <span class="ne">SystemExit</span><span class="p">:</span>
+</span><span id="format_files-154"><a href="#format_files-154"><span class="linenos">154</span></a>        <span class="o">...</span>
+</span></pre></div>
+
+
+            <div class="docstring"><p>Use <code>Black</code> to format file(s).</p>
+</div>
+
+
+                </section>
     </main>
 <script>
     function escapeHTML(html) {
         return document.createElement('div').appendChild(document.createTextNode(html)).parentNode.innerHTML;
     }
 
     const originalContent = document.querySelector("main.pdoc");
```

#### html2text {}

```diff
@@ -7,327 +7,347 @@
     * get_minimum_py_version
     * get_project_code
     * update_minimum_python_version
     * generate_docs
     * update_dependencies
     * update_changelog
     * tag_version
+    * format_files
 built_with_pdoc[pdoc_logo]
 
 ****** hassle.hassle_utilities ******
 ⁰ View Source
 __1import os
 __2
-__3import packagelister
-__4import vermin
-__5from pathier import Pathier
-__6
-__7from hassle import hassle_config
+__3import black
+__4import packagelister
+__5import vermin
+__6from gitbetter import git
+__7from pathier import Pathier
 __8
-__9root = Pathier(__file__).parent
+__9from hassle import hassle_config
 _10
-_11
-_12def increment_version(pyproject_path: Pathier, increment_type: str):
-_13    """Increment the project.version field in pyproject.toml.
-_14
-_15    :param package_path: Path to the package/project directory.
+_11root = Pathier(__file__).parent
+_12
+_13
+_14def increment_version(pyproject_path: Pathier, increment_type: str):
+_15    """Increment the project.version field in pyproject.toml.
 _16
-_17    :param increment_type: One from 'major', 'minor', or 'patch'."""
-_18    meta = pyproject_path.loads()
-_19    major, minor, patch = [int(num) for num in meta["project"]
+_17    :param package_path: Path to the package/project directory.
+_18
+_19    :param increment_type: One from 'major', 'minor', or 'patch'."""
+_20    meta = pyproject_path.loads()
+_21    major, minor, patch = [int(num) for num in meta["project"]
 ["version"].split(".")]
-_20    if increment_type == "major":
-_21        major += 1
-_22        minor = 0
-_23        patch = 0
-_24    elif increment_type == "minor":
-_25        minor += 1
-_26        patch = 0
-_27    elif increment_type == "patch":
-_28        patch += 1
-_29    incremented_version = ".".join(str(num) for num in [major, minor,
+_22    if increment_type == "major":
+_23        major += 1
+_24        minor = 0
+_25        patch = 0
+_26    elif increment_type == "minor":
+_27        minor += 1
+_28        patch = 0
+_29    elif increment_type == "patch":
+_30        patch += 1
+_31    incremented_version = ".".join(str(num) for num in [major, minor,
 patch])
-_30    meta["project"]["version"] = incremented_version
-_31    pyproject_path.dumps(meta)
-_32
-_33
-_34def get_minimum_py_version(src: str) -> str:
-_35    """Scan src with vermin and return minimum
-_36    python version."""
-_37    config = vermin.Config()
-_38    config.add_backport("typing")
-_39    config.add_backport("typing_extensions")
-_40    config.set_eval_annotations(True)
-_41    result = vermin.visit(src, config).minimum_versions()[1]
-_42    return f"{result[0]}.{result[1]}"
-_43
-_44
-_45def get_project_code(project_path: Pathier) -> str:
-_46    """Read and return all code from project_path
-_47    as one string."""
-_48    return "\n".join(file.read_text() for file in project_path.rglob
+_32    meta["project"]["version"] = incremented_version
+_33    pyproject_path.dumps(meta)
+_34
+_35
+_36def get_minimum_py_version(src: str) -> str:
+_37    """Scan src with vermin and return minimum
+_38    python version."""
+_39    config = vermin.Config()
+_40    config.add_backport("typing")
+_41    config.add_backport("typing_extensions")
+_42    config.set_eval_annotations(True)
+_43    result = vermin.visit(src, config).minimum_versions()[1]
+_44    return f"{result[0]}.{result[1]}"
+_45
+_46
+_47def get_project_code(project_path: Pathier) -> str:
+_48    """Read and return all code from project_path
+_49    as one string."""
+_50    return "\n".join(file.read_text() for file in project_path.rglob
 ("*.py"))
-_49
-_50
-_51def update_minimum_python_version(pyproject_path: Pathier):
-_52    """Use vermin to determine the minimum compatible
-_53    Python version and update the corresponding field
-_54    in pyproject.toml."""
-_55    project_code = get_project_code(pyproject_path.parent / "src")
-_56    meta = pyproject_path.loads()
-_57    minimum_version = get_minimum_py_version(project_code)
-_58    minimum_version = f">={minimum_version}"
-_59    meta["project"]["requires-python"] = minimum_version
-_60    pyproject_path.dumps(meta)
-_61
-_62
-_63def generate_docs(package_path: Pathier):
-_64    """Generate project documentation using pdoc."""
-_65    try:
-_66        (package_path / "docs").delete()
-_67    except Exception as e:
-_68        pass
-_69    os.system(
-_70        f"pdoc -o {package_path / 'docs'} {package_path / 'src' /
+_51
+_52
+_53def update_minimum_python_version(pyproject_path: Pathier):
+_54    """Use vermin to determine the minimum compatible
+_55    Python version and update the corresponding field
+_56    in pyproject.toml."""
+_57    project_code = get_project_code(pyproject_path.parent / "src")
+_58    meta = pyproject_path.loads()
+_59    minimum_version = get_minimum_py_version(project_code)
+_60    minimum_version = f">={minimum_version}"
+_61    meta["project"]["requires-python"] = minimum_version
+_62    pyproject_path.dumps(meta)
+_63
+_64
+_65def generate_docs(package_path: Pathier):
+_66    """Generate project documentation using pdoc."""
+_67    try:
+_68        (package_path / "docs").delete()
+_69    except Exception as e:
+_70        pass
+_71    os.system(
+_72        f"pdoc -o {package_path / 'docs'} {package_path / 'src' /
 package_path.stem}"
-_71    )
-_72
-_73
-_74def update_dependencies(
-_75    pyproject_path: Pathier, overwrite: bool, include_versions: bool = False
-_76):
-_77    """Update dependencies list in pyproject.toml.
-_78
-_79    :param overwrite: If True, replace the dependencies in pyproject.toml
-_80    with the results of packagelister.scan() .
-_81    If False, packages returned by packagelister are appended to
-_82    the current dependencies in pyproject.toml if they don't already
-_83    exist in the field."""
-_84    packages = packagelister.scan(pyproject_path.parent)
-_85
-_86    packages = [
-_87        f"{package}~={packages[package]['version']}"
-_88        if packages[package]["version"] and include_versions
-_89        else f"{package}"
-_90        for package in packages
-_91        if package != pyproject_path.parent.stem
-_92    ]
-_93    packages = [
-_94        package.replace("speech_recognition", "speechRecognition")
-_95        for package in packages
-_96    ]
-_97    meta = pyproject_path.loads()
-_98    if overwrite:
-_99        meta["project"]["dependencies"] = packages
-100    else:
-101        for package in packages:
-102            if "~" in package:
-103                name = package.split("~")[0]
-104            elif "=" in package:
-105                name = package.split("=")[0]
-106            else:
-107                name = package
-108            if all(
-109                name not in dependency for dependency in meta["project"]
+_73    )
+_74
+_75
+_76def update_dependencies(
+_77    pyproject_path: Pathier, overwrite: bool, include_versions: bool = False
+_78):
+_79    """Update dependencies list in pyproject.toml.
+_80
+_81    :param overwrite: If True, replace the dependencies in pyproject.toml
+_82    with the results of packagelister.scan() .
+_83    If False, packages returned by packagelister are appended to
+_84    the current dependencies in pyproject.toml if they don't already
+_85    exist in the field."""
+_86    packages = packagelister.scan(pyproject_path.parent)
+_87
+_88    packages = [
+_89        f"{package}~={packages[package]['version']}"
+_90        if packages[package]["version"] and include_versions
+_91        else f"{package}"
+_92        for package in packages
+_93        if package != pyproject_path.parent.stem
+_94    ]
+_95    packages = [
+_96        package.replace("speech_recognition", "speechRecognition")
+_97        for package in packages
+_98    ]
+_99    meta = pyproject_path.loads()
+100    if overwrite:
+101        meta["project"]["dependencies"] = packages
+102    else:
+103        for package in packages:
+104            if "~" in package:
+105                name = package.split("~")[0]
+106            elif "=" in package:
+107                name = package.split("=")[0]
+108            else:
+109                name = package
+110            if all(
+111                name not in dependency for dependency in meta["project"]
 ["dependencies"]
-110            ):
-111                meta["project"]["dependencies"].append(package)
-112    pyproject_path.dumps(meta)
-113
-114
-115def update_changelog(pyproject_path: Pathier):
-116    """Update project changelog."""
-117    meta = pyproject_path.loads()
-118    if hassle_config.config_exists():
-119        config = hassle_config.load_config()
-120    else:
-121        hassle_config.warn()
-122        print("Creating blank hassle_config.toml...")
-123        config = hassle_config.load_config()
-124    changelog_path = pyproject_path.parent / "CHANGELOG.md"
-125    os.system(
-126        f"auto-changelog -p {pyproject_path.parent} --tag-prefix {config
+112            ):
+113                meta["project"]["dependencies"].append(package)
+114    pyproject_path.dumps(meta)
+115
+116
+117def update_changelog(pyproject_path: Pathier):
+118    """Update project changelog."""
+119    meta = pyproject_path.loads()
+120    if hassle_config.config_exists():
+121        config = hassle_config.load_config()
+122    else:
+123        hassle_config.warn()
+124        print("Creating blank hassle_config.toml...")
+125        config = hassle_config.load_config()
+126    changelog_path = pyproject_path.parent / "CHANGELOG.md"
+127    os.system(
+128        f"auto-changelog -p {pyproject_path.parent} --tag-prefix {config
 ['git']['tag_prefix']} --unreleased -v {meta['project']['version']} -o
 {changelog_path}"
-127    )
-128    changelog = changelog_path.read_text().splitlines()
-129    changelog = [line for line in changelog if "Full set of changes:" not in
+129    )
+130    changelog = changelog_path.read_text().splitlines()
+131    changelog = [line for line in changelog if "Full set of changes:" not in
 line]
-130    changelog_path.write_text("\n".join(changelog))
-131
-132
-133def tag_version(package_path: Pathier):
-134    """Add a git tag corresponding
-135    to the version number in pyproject.toml."""
-136    if hassle_config.config_exists():
-137        tag_prefix = hassle_config.load_config()["git"]["tag_prefix"]
-138    else:
-139        hassle_config.warn()
-140        tag_prefix = ""
-141    version = (package_path / "pyproject.toml").loads()["project"]
+132    changelog_path.write_text("\n".join(changelog))
+133
+134
+135def tag_version(package_path: Pathier):
+136    """Add a git tag corresponding
+137    to the version number in pyproject.toml."""
+138    if hassle_config.config_exists():
+139        tag_prefix = hassle_config.load_config()["git"]["tag_prefix"]
+140    else:
+141        hassle_config.warn()
+142        tag_prefix = ""
+143    version = (package_path / "pyproject.toml").loads()["project"]
 ["version"]
-142    os.chdir(package_path)
-143    os.system(f"git tag {tag_prefix}{version}")
+144    os.chdir(package_path)
+145    git.tag(f"{tag_prefix}{version}")
+146
+147
+148def format_files(path: Pathier):
+149    """Use `Black` to format file(s)."""
+150    try:
+151        black.main([str(path)])
+152    except SystemExit:
+153        ...
   ⁰
 def increment_version(pyproject_path: pathier.pathier.Pathier, increment_type:
 str): View Source
-13def increment_version(pyproject_path: Pathier, increment_type: str):
-14    """Increment the project.version field in pyproject.toml.
-15
-16    :param package_path: Path to the package/project directory.
+15def increment_version(pyproject_path: Pathier, increment_type: str):
+16    """Increment the project.version field in pyproject.toml.
 17
-18    :param increment_type: One from 'major', 'minor', or 'patch'."""
-19    meta = pyproject_path.loads()
-20    major, minor, patch = [int(num) for num in meta["project"]
+18    :param package_path: Path to the package/project directory.
+19
+20    :param increment_type: One from 'major', 'minor', or 'patch'."""
+21    meta = pyproject_path.loads()
+22    major, minor, patch = [int(num) for num in meta["project"]
 ["version"].split(".")]
-21    if increment_type == "major":
-22        major += 1
-23        minor = 0
-24        patch = 0
-25    elif increment_type == "minor":
-26        minor += 1
-27        patch = 0
-28    elif increment_type == "patch":
-29        patch += 1
-30    incremented_version = ".".join(str(num) for num in [major, minor, patch])
-31    meta["project"]["version"] = incremented_version
-32    pyproject_path.dumps(meta)
+23    if increment_type == "major":
+24        major += 1
+25        minor = 0
+26        patch = 0
+27    elif increment_type == "minor":
+28        minor += 1
+29        patch = 0
+30    elif increment_type == "patch":
+31        patch += 1
+32    incremented_version = ".".join(str(num) for num in [major, minor, patch])
+33    meta["project"]["version"] = incremented_version
+34    pyproject_path.dumps(meta)
 Increment the project.version field in pyproject.toml.
 * Parameters *
     * package_path: Path to the package/project directory.
     * increment_type: One from 'major', 'minor', or 'patch'.
   ⁰
 def get_minimum_py_version(src: str) -> str: View Source
-35def get_minimum_py_version(src: str) -> str:
-36    """Scan src with vermin and return minimum
-37    python version."""
-38    config = vermin.Config()
-39    config.add_backport("typing")
-40    config.add_backport("typing_extensions")
-41    config.set_eval_annotations(True)
-42    result = vermin.visit(src, config).minimum_versions()[1]
-43    return f"{result[0]}.{result[1]}"
+37def get_minimum_py_version(src: str) -> str:
+38    """Scan src with vermin and return minimum
+39    python version."""
+40    config = vermin.Config()
+41    config.add_backport("typing")
+42    config.add_backport("typing_extensions")
+43    config.set_eval_annotations(True)
+44    result = vermin.visit(src, config).minimum_versions()[1]
+45    return f"{result[0]}.{result[1]}"
 Scan src with vermin and return minimum python version.
   ⁰
 def get_project_code(project_path: pathier.pathier.Pathier) -> str: View Source
-46def get_project_code(project_path: Pathier) -> str:
-47    """Read and return all code from project_path
-48    as one string."""
-49    return "\n".join(file.read_text() for file in project_path.rglob("*.py"))
+48def get_project_code(project_path: Pathier) -> str:
+49    """Read and return all code from project_path
+50    as one string."""
+51    return "\n".join(file.read_text() for file in project_path.rglob("*.py"))
 Read and return all code from project_path as one string.
   ⁰
 def update_minimum_python_version(pyproject_path: pathier.pathier.Pathier):
 View Source
-52def update_minimum_python_version(pyproject_path: Pathier):
-53    """Use vermin to determine the minimum compatible
-54    Python version and update the corresponding field
-55    in pyproject.toml."""
-56    project_code = get_project_code(pyproject_path.parent / "src")
-57    meta = pyproject_path.loads()
-58    minimum_version = get_minimum_py_version(project_code)
-59    minimum_version = f">={minimum_version}"
-60    meta["project"]["requires-python"] = minimum_version
-61    pyproject_path.dumps(meta)
+54def update_minimum_python_version(pyproject_path: Pathier):
+55    """Use vermin to determine the minimum compatible
+56    Python version and update the corresponding field
+57    in pyproject.toml."""
+58    project_code = get_project_code(pyproject_path.parent / "src")
+59    meta = pyproject_path.loads()
+60    minimum_version = get_minimum_py_version(project_code)
+61    minimum_version = f">={minimum_version}"
+62    meta["project"]["requires-python"] = minimum_version
+63    pyproject_path.dumps(meta)
 Use vermin to determine the minimum compatible Python version and update the
 corresponding field in pyproject.toml.
   ⁰
 def generate_docs(package_path: pathier.pathier.Pathier): View Source
-64def generate_docs(package_path: Pathier):
-65    """Generate project documentation using pdoc."""
-66    try:
-67        (package_path / "docs").delete()
-68    except Exception as e:
-69        pass
-70    os.system(
-71        f"pdoc -o {package_path / 'docs'} {package_path / 'src' /
+66def generate_docs(package_path: Pathier):
+67    """Generate project documentation using pdoc."""
+68    try:
+69        (package_path / "docs").delete()
+70    except Exception as e:
+71        pass
+72    os.system(
+73        f"pdoc -o {package_path / 'docs'} {package_path / 'src' /
 package_path.stem}"
-72    )
+74    )
 Generate project documentation using pdoc.
   ⁰
 def update_dependencies(
 pyproject_path: pathier.pathier.Pathier,
 overwrite: bool,
 include_versions: bool = False): View Source
-_75def update_dependencies(
-_76    pyproject_path: Pathier, overwrite: bool, include_versions: bool = False
-_77):
-_78    """Update dependencies list in pyproject.toml.
-_79
-_80    :param overwrite: If True, replace the dependencies in pyproject.toml
-_81    with the results of packagelister.scan() .
-_82    If False, packages returned by packagelister are appended to
-_83    the current dependencies in pyproject.toml if they don't already
-_84    exist in the field."""
-_85    packages = packagelister.scan(pyproject_path.parent)
-_86
-_87    packages = [
-_88        f"{package}~={packages[package]['version']}"
-_89        if packages[package]["version"] and include_versions
-_90        else f"{package}"
-_91        for package in packages
-_92        if package != pyproject_path.parent.stem
-_93    ]
-_94    packages = [
-_95        package.replace("speech_recognition", "speechRecognition")
-_96        for package in packages
-_97    ]
-_98    meta = pyproject_path.loads()
-_99    if overwrite:
-100        meta["project"]["dependencies"] = packages
-101    else:
-102        for package in packages:
-103            if "~" in package:
-104                name = package.split("~")[0]
-105            elif "=" in package:
-106                name = package.split("=")[0]
-107            else:
-108                name = package
-109            if all(
-110                name not in dependency for dependency in meta["project"]
+_77def update_dependencies(
+_78    pyproject_path: Pathier, overwrite: bool, include_versions: bool = False
+_79):
+_80    """Update dependencies list in pyproject.toml.
+_81
+_82    :param overwrite: If True, replace the dependencies in pyproject.toml
+_83    with the results of packagelister.scan() .
+_84    If False, packages returned by packagelister are appended to
+_85    the current dependencies in pyproject.toml if they don't already
+_86    exist in the field."""
+_87    packages = packagelister.scan(pyproject_path.parent)
+_88
+_89    packages = [
+_90        f"{package}~={packages[package]['version']}"
+_91        if packages[package]["version"] and include_versions
+_92        else f"{package}"
+_93        for package in packages
+_94        if package != pyproject_path.parent.stem
+_95    ]
+_96    packages = [
+_97        package.replace("speech_recognition", "speechRecognition")
+_98        for package in packages
+_99    ]
+100    meta = pyproject_path.loads()
+101    if overwrite:
+102        meta["project"]["dependencies"] = packages
+103    else:
+104        for package in packages:
+105            if "~" in package:
+106                name = package.split("~")[0]
+107            elif "=" in package:
+108                name = package.split("=")[0]
+109            else:
+110                name = package
+111            if all(
+112                name not in dependency for dependency in meta["project"]
 ["dependencies"]
-111            ):
-112                meta["project"]["dependencies"].append(package)
-113    pyproject_path.dumps(meta)
+113            ):
+114                meta["project"]["dependencies"].append(package)
+115    pyproject_path.dumps(meta)
 Update dependencies list in pyproject.toml.
 * Parameters *
     * overwrite: If True, replace the dependencies in pyproject.toml with the
       results of packagelister.scan() . If False, packages returned by
       packagelister are appended to the current dependencies in pyproject.toml
       if they don't already exist in the field.
   ⁰
 def update_changelog(pyproject_path: pathier.pathier.Pathier): View Source
-116def update_changelog(pyproject_path: Pathier):
-117    """Update project changelog."""
-118    meta = pyproject_path.loads()
-119    if hassle_config.config_exists():
-120        config = hassle_config.load_config()
-121    else:
-122        hassle_config.warn()
-123        print("Creating blank hassle_config.toml...")
-124        config = hassle_config.load_config()
-125    changelog_path = pyproject_path.parent / "CHANGELOG.md"
-126    os.system(
-127        f"auto-changelog -p {pyproject_path.parent} --tag-prefix {config
+118def update_changelog(pyproject_path: Pathier):
+119    """Update project changelog."""
+120    meta = pyproject_path.loads()
+121    if hassle_config.config_exists():
+122        config = hassle_config.load_config()
+123    else:
+124        hassle_config.warn()
+125        print("Creating blank hassle_config.toml...")
+126        config = hassle_config.load_config()
+127    changelog_path = pyproject_path.parent / "CHANGELOG.md"
+128    os.system(
+129        f"auto-changelog -p {pyproject_path.parent} --tag-prefix {config
 ['git']['tag_prefix']} --unreleased -v {meta['project']['version']} -o
 {changelog_path}"
-128    )
-129    changelog = changelog_path.read_text().splitlines()
-130    changelog = [line for line in changelog if "Full set of changes:" not in
+130    )
+131    changelog = changelog_path.read_text().splitlines()
+132    changelog = [line for line in changelog if "Full set of changes:" not in
 line]
-131    changelog_path.write_text("\n".join(changelog))
+133    changelog_path.write_text("\n".join(changelog))
 Update project changelog.
   ⁰
 def tag_version(package_path: pathier.pathier.Pathier): View Source
-134def tag_version(package_path: Pathier):
-135    """Add a git tag corresponding
-136    to the version number in pyproject.toml."""
-137    if hassle_config.config_exists():
-138        tag_prefix = hassle_config.load_config()["git"]["tag_prefix"]
-139    else:
-140        hassle_config.warn()
-141        tag_prefix = ""
-142    version = (package_path / "pyproject.toml").loads()["project"]
+136def tag_version(package_path: Pathier):
+137    """Add a git tag corresponding
+138    to the version number in pyproject.toml."""
+139    if hassle_config.config_exists():
+140        tag_prefix = hassle_config.load_config()["git"]["tag_prefix"]
+141    else:
+142        hassle_config.warn()
+143        tag_prefix = ""
+144    version = (package_path / "pyproject.toml").loads()["project"]
 ["version"]
-143    os.chdir(package_path)
-144    os.system(f"git tag {tag_prefix}{version}")
+145    os.chdir(package_path)
+146    git.tag(f"{tag_prefix}{version}")
 Add a git tag corresponding to the version number in pyproject.toml.
+  ⁰
+def format_files(path: pathier.pathier.Pathier): View Source
+149def format_files(path: Pathier):
+150    """Use `Black` to format file(s)."""
+151    try:
+152        black.main([str(path)])
+153    except SystemExit:
+154        ...
+Use Black to format file(s).
```

### Comparing `hassle-2.7.1/docs/hassle/new_project.html` & `hassle-2.8.0/docs/hassle/new_project.html`

 * *Files 0% similar despite different names*

```diff
@@ -87,275 +87,276 @@
                         <div class="pdoc-code codehilite"><pre><span></span><span id="L-1"><a href="#L-1"><span class="linenos">  1</span></a><span class="kn">import</span> <span class="nn">argparse</span>
 </span><span id="L-2"><a href="#L-2"><span class="linenos">  2</span></a><span class="kn">import</span> <span class="nn">os</span>
 </span><span id="L-3"><a href="#L-3"><span class="linenos">  3</span></a><span class="kn">import</span> <span class="nn">sys</span>
 </span><span id="L-4"><a href="#L-4"><span class="linenos">  4</span></a><span class="kn">from</span> <span class="nn">datetime</span> <span class="kn">import</span> <span class="n">datetime</span>
 </span><span id="L-5"><a href="#L-5"><span class="linenos">  5</span></a>
 </span><span id="L-6"><a href="#L-6"><span class="linenos">  6</span></a><span class="kn">import</span> <span class="nn">requests</span>
 </span><span id="L-7"><a href="#L-7"><span class="linenos">  7</span></a><span class="kn">from</span> <span class="nn">bs4</span> <span class="kn">import</span> <span class="n">BeautifulSoup</span>
-</span><span id="L-8"><a href="#L-8"><span class="linenos">  8</span></a><span class="kn">from</span> <span class="nn">pathier</span> <span class="kn">import</span> <span class="n">Pathier</span>
-</span><span id="L-9"><a href="#L-9"><span class="linenos">  9</span></a>
-</span><span id="L-10"><a href="#L-10"><span class="linenos"> 10</span></a><span class="kn">import</span> <span class="nn">hassle.hassle_config</span> <span class="k">as</span> <span class="nn">hassle_config</span>
-</span><span id="L-11"><a href="#L-11"><span class="linenos"> 11</span></a><span class="kn">from</span> <span class="nn">hassle.generate_tests</span> <span class="kn">import</span> <span class="n">generate_test_files</span>
-</span><span id="L-12"><a href="#L-12"><span class="linenos"> 12</span></a>
-</span><span id="L-13"><a href="#L-13"><span class="linenos"> 13</span></a><span class="n">root</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="vm">__file__</span><span class="p">)</span><span class="o">.</span><span class="n">parent</span>
-</span><span id="L-14"><a href="#L-14"><span class="linenos"> 14</span></a>
+</span><span id="L-8"><a href="#L-8"><span class="linenos">  8</span></a><span class="kn">from</span> <span class="nn">gitbetter</span> <span class="kn">import</span> <span class="n">git</span>
+</span><span id="L-9"><a href="#L-9"><span class="linenos">  9</span></a><span class="kn">from</span> <span class="nn">pathier</span> <span class="kn">import</span> <span class="n">Pathier</span>
+</span><span id="L-10"><a href="#L-10"><span class="linenos"> 10</span></a>
+</span><span id="L-11"><a href="#L-11"><span class="linenos"> 11</span></a><span class="kn">import</span> <span class="nn">hassle.hassle_config</span> <span class="k">as</span> <span class="nn">hassle_config</span>
+</span><span id="L-12"><a href="#L-12"><span class="linenos"> 12</span></a><span class="kn">from</span> <span class="nn">hassle.generate_tests</span> <span class="kn">import</span> <span class="n">generate_test_files</span>
+</span><span id="L-13"><a href="#L-13"><span class="linenos"> 13</span></a>
+</span><span id="L-14"><a href="#L-14"><span class="linenos"> 14</span></a><span class="n">root</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="vm">__file__</span><span class="p">)</span><span class="o">.</span><span class="n">parent</span>
 </span><span id="L-15"><a href="#L-15"><span class="linenos"> 15</span></a>
-</span><span id="L-16"><a href="#L-16"><span class="linenos"> 16</span></a><span class="k">def</span> <span class="nf">get_args</span><span class="p">()</span> <span class="o">-&gt;</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span><span class="p">:</span>
-</span><span id="L-17"><a href="#L-17"><span class="linenos"> 17</span></a>    <span class="n">parser</span> <span class="o">=</span> <span class="n">argparse</span><span class="o">.</span><span class="n">ArgumentParser</span><span class="p">()</span>
-</span><span id="L-18"><a href="#L-18"><span class="linenos"> 18</span></a>
-</span><span id="L-19"><a href="#L-19"><span class="linenos"> 19</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="L-20"><a href="#L-20"><span class="linenos"> 20</span></a>        <span class="s2">&quot;name&quot;</span><span class="p">,</span>
-</span><span id="L-21"><a href="#L-21"><span class="linenos"> 21</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
-</span><span id="L-22"><a href="#L-22"><span class="linenos"> 22</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Name of the package to create in the current working directory. &quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="L-23"><a href="#L-23"><span class="linenos"> 23</span></a>    <span class="p">)</span>
-</span><span id="L-24"><a href="#L-24"><span class="linenos"> 24</span></a>
-</span><span id="L-25"><a href="#L-25"><span class="linenos"> 25</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="L-26"><a href="#L-26"><span class="linenos"> 26</span></a>        <span class="s2">&quot;-s&quot;</span><span class="p">,</span>
-</span><span id="L-27"><a href="#L-27"><span class="linenos"> 27</span></a>        <span class="s2">&quot;--source_files&quot;</span><span class="p">,</span>
-</span><span id="L-28"><a href="#L-28"><span class="linenos"> 28</span></a>        <span class="n">nargs</span><span class="o">=</span><span class="s2">&quot;*&quot;</span><span class="p">,</span>
-</span><span id="L-29"><a href="#L-29"><span class="linenos"> 29</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
-</span><span id="L-30"><a href="#L-30"><span class="linenos"> 30</span></a>        <span class="n">default</span><span class="o">=</span><span class="p">[],</span>
-</span><span id="L-31"><a href="#L-31"><span class="linenos"> 31</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; List of additional source files to create in addition to the default</span>
-</span><span id="L-32"><a href="#L-32"><span class="linenos"> 32</span></a><span class="s2">        __init__.py and </span><span class="si">{name}</span><span class="s2">.py files.&quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="L-33"><a href="#L-33"><span class="linenos"> 33</span></a>    <span class="p">)</span>
-</span><span id="L-34"><a href="#L-34"><span class="linenos"> 34</span></a>
-</span><span id="L-35"><a href="#L-35"><span class="linenos"> 35</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="L-36"><a href="#L-36"><span class="linenos"> 36</span></a>        <span class="s2">&quot;-d&quot;</span><span class="p">,</span>
-</span><span id="L-37"><a href="#L-37"><span class="linenos"> 37</span></a>        <span class="s2">&quot;--description&quot;</span><span class="p">,</span>
-</span><span id="L-38"><a href="#L-38"><span class="linenos"> 38</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
-</span><span id="L-39"><a href="#L-39"><span class="linenos"> 39</span></a>        <span class="n">default</span><span class="o">=</span><span class="s2">&quot;&quot;</span><span class="p">,</span>
-</span><span id="L-40"><a href="#L-40"><span class="linenos"> 40</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; The package description to be added to the pyproject.toml file. &quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="L-41"><a href="#L-41"><span class="linenos"> 41</span></a>    <span class="p">)</span>
-</span><span id="L-42"><a href="#L-42"><span class="linenos"> 42</span></a>
-</span><span id="L-43"><a href="#L-43"><span class="linenos"> 43</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="L-44"><a href="#L-44"><span class="linenos"> 44</span></a>        <span class="s2">&quot;-dp&quot;</span><span class="p">,</span>
-</span><span id="L-45"><a href="#L-45"><span class="linenos"> 45</span></a>        <span class="s2">&quot;--dependencies&quot;</span><span class="p">,</span>
-</span><span id="L-46"><a href="#L-46"><span class="linenos"> 46</span></a>        <span class="n">nargs</span><span class="o">=</span><span class="s2">&quot;*&quot;</span><span class="p">,</span>
-</span><span id="L-47"><a href="#L-47"><span class="linenos"> 47</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
-</span><span id="L-48"><a href="#L-48"><span class="linenos"> 48</span></a>        <span class="n">default</span><span class="o">=</span><span class="p">[],</span>
-</span><span id="L-49"><a href="#L-49"><span class="linenos"> 49</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; List of dependencies to add to pyproject.toml.</span>
-</span><span id="L-50"><a href="#L-50"><span class="linenos"> 50</span></a><span class="s2">        Note: hassle.py will automatically scan your project for 3rd party</span>
-</span><span id="L-51"><a href="#L-51"><span class="linenos"> 51</span></a><span class="s2">        imports and update pyproject.toml. This switch is largely useful</span>
-</span><span id="L-52"><a href="#L-52"><span class="linenos"> 52</span></a><span class="s2">        for adding dependencies your project might need, but doesn&#39;t</span>
-</span><span id="L-53"><a href="#L-53"><span class="linenos"> 53</span></a><span class="s2">        directly import in any source files,</span>
-</span><span id="L-54"><a href="#L-54"><span class="linenos"> 54</span></a><span class="s2">        like an os.system() call that invokes a 3rd party cli.&quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="L-55"><a href="#L-55"><span class="linenos"> 55</span></a>    <span class="p">)</span>
-</span><span id="L-56"><a href="#L-56"><span class="linenos"> 56</span></a>
-</span><span id="L-57"><a href="#L-57"><span class="linenos"> 57</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="L-58"><a href="#L-58"><span class="linenos"> 58</span></a>        <span class="s2">&quot;-k&quot;</span><span class="p">,</span>
-</span><span id="L-59"><a href="#L-59"><span class="linenos"> 59</span></a>        <span class="s2">&quot;--keywords&quot;</span><span class="p">,</span>
-</span><span id="L-60"><a href="#L-60"><span class="linenos"> 60</span></a>        <span class="n">nargs</span><span class="o">=</span><span class="s2">&quot;*&quot;</span><span class="p">,</span>
-</span><span id="L-61"><a href="#L-61"><span class="linenos"> 61</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
-</span><span id="L-62"><a href="#L-62"><span class="linenos"> 62</span></a>        <span class="n">default</span><span class="o">=</span><span class="p">[],</span>
-</span><span id="L-63"><a href="#L-63"><span class="linenos"> 63</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; List of keywords to be added to the keywords field in pyproject.toml. &quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="L-64"><a href="#L-64"><span class="linenos"> 64</span></a>    <span class="p">)</span>
-</span><span id="L-65"><a href="#L-65"><span class="linenos"> 65</span></a>
-</span><span id="L-66"><a href="#L-66"><span class="linenos"> 66</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="L-67"><a href="#L-67"><span class="linenos"> 67</span></a>        <span class="s2">&quot;-as&quot;</span><span class="p">,</span>
-</span><span id="L-68"><a href="#L-68"><span class="linenos"> 68</span></a>        <span class="s2">&quot;--add_script&quot;</span><span class="p">,</span>
-</span><span id="L-69"><a href="#L-69"><span class="linenos"> 69</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
-</span><span id="L-70"><a href="#L-70"><span class="linenos"> 70</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Add section to pyproject.toml declaring the package </span>
-</span><span id="L-71"><a href="#L-71"><span class="linenos"> 71</span></a><span class="s2">        should be installed with command line scripts added. </span>
-</span><span id="L-72"><a href="#L-72"><span class="linenos"> 72</span></a><span class="s2">        The default is &#39;</span><span class="si">{name}</span><span class="s2"> = &quot;</span><span class="si">{name}</span><span class="s2">.</span><span class="si">{name}</span><span class="s2">:main&quot;.</span>
-</span><span id="L-73"><a href="#L-73"><span class="linenos"> 73</span></a><span class="s2">        You will need to manually change this field.&quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="L-74"><a href="#L-74"><span class="linenos"> 74</span></a>    <span class="p">)</span>
-</span><span id="L-75"><a href="#L-75"><span class="linenos"> 75</span></a>
-</span><span id="L-76"><a href="#L-76"><span class="linenos"> 76</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="L-77"><a href="#L-77"><span class="linenos"> 77</span></a>        <span class="s2">&quot;-nl&quot;</span><span class="p">,</span>
-</span><span id="L-78"><a href="#L-78"><span class="linenos"> 78</span></a>        <span class="s2">&quot;--no_license&quot;</span><span class="p">,</span>
-</span><span id="L-79"><a href="#L-79"><span class="linenos"> 79</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
-</span><span id="L-80"><a href="#L-80"><span class="linenos"> 80</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; By default, projects are created with an MIT license.</span>
-</span><span id="L-81"><a href="#L-81"><span class="linenos"> 81</span></a><span class="s2">        Set this flag to avoid adding a license if you want to configure licensing</span>
-</span><span id="L-82"><a href="#L-82"><span class="linenos"> 82</span></a><span class="s2">        at another time.&quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="L-83"><a href="#L-83"><span class="linenos"> 83</span></a>    <span class="p">)</span>
-</span><span id="L-84"><a href="#L-84"><span class="linenos"> 84</span></a>
-</span><span id="L-85"><a href="#L-85"><span class="linenos"> 85</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="L-86"><a href="#L-86"><span class="linenos"> 86</span></a>        <span class="s2">&quot;-os&quot;</span><span class="p">,</span>
-</span><span id="L-87"><a href="#L-87"><span class="linenos"> 87</span></a>        <span class="s2">&quot;--operating_system&quot;</span><span class="p">,</span>
-</span><span id="L-88"><a href="#L-88"><span class="linenos"> 88</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
-</span><span id="L-89"><a href="#L-89"><span class="linenos"> 89</span></a>        <span class="n">default</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span>
-</span><span id="L-90"><a href="#L-90"><span class="linenos"> 90</span></a>        <span class="n">nargs</span><span class="o">=</span><span class="s2">&quot;*&quot;</span><span class="p">,</span>
-</span><span id="L-91"><a href="#L-91"><span class="linenos"> 91</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; List of operating systems this package will be compatible with.</span>
-</span><span id="L-92"><a href="#L-92"><span class="linenos"> 92</span></a><span class="s2">        The default is OS Independent.</span>
-</span><span id="L-93"><a href="#L-93"><span class="linenos"> 93</span></a><span class="s2">        This only affects the &#39;classifiers&#39; field of pyproject.toml .&quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="L-94"><a href="#L-94"><span class="linenos"> 94</span></a>    <span class="p">)</span>
-</span><span id="L-95"><a href="#L-95"><span class="linenos"> 95</span></a>
-</span><span id="L-96"><a href="#L-96"><span class="linenos"> 96</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="L-97"><a href="#L-97"><span class="linenos"> 97</span></a>        <span class="s2">&quot;-np&quot;</span><span class="p">,</span>
-</span><span id="L-98"><a href="#L-98"><span class="linenos"> 98</span></a>        <span class="s2">&quot;--not_package&quot;</span><span class="p">,</span>
-</span><span id="L-99"><a href="#L-99"><span class="linenos"> 99</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
-</span><span id="L-100"><a href="#L-100"><span class="linenos">100</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Put source files in top level directory and delete tests folder. &quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="L-101"><a href="#L-101"><span class="linenos">101</span></a>    <span class="p">)</span>
-</span><span id="L-102"><a href="#L-102"><span class="linenos">102</span></a>
-</span><span id="L-103"><a href="#L-103"><span class="linenos">103</span></a>    <span class="n">args</span> <span class="o">=</span> <span class="n">parser</span><span class="o">.</span><span class="n">parse_args</span><span class="p">()</span>
-</span><span id="L-104"><a href="#L-104"><span class="linenos">104</span></a>    <span class="n">args</span><span class="o">.</span><span class="n">source_files</span><span class="o">.</span><span class="n">extend</span><span class="p">([</span><span class="s2">&quot;__init__.py&quot;</span><span class="p">,</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="si">}</span><span class="s2">.py&quot;</span><span class="p">])</span>
-</span><span id="L-105"><a href="#L-105"><span class="linenos">105</span></a>
-</span><span id="L-106"><a href="#L-106"><span class="linenos">106</span></a>    <span class="k">return</span> <span class="n">args</span>
-</span><span id="L-107"><a href="#L-107"><span class="linenos">107</span></a>
+</span><span id="L-16"><a href="#L-16"><span class="linenos"> 16</span></a>
+</span><span id="L-17"><a href="#L-17"><span class="linenos"> 17</span></a><span class="k">def</span> <span class="nf">get_args</span><span class="p">()</span> <span class="o">-&gt;</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span><span class="p">:</span>
+</span><span id="L-18"><a href="#L-18"><span class="linenos"> 18</span></a>    <span class="n">parser</span> <span class="o">=</span> <span class="n">argparse</span><span class="o">.</span><span class="n">ArgumentParser</span><span class="p">()</span>
+</span><span id="L-19"><a href="#L-19"><span class="linenos"> 19</span></a>
+</span><span id="L-20"><a href="#L-20"><span class="linenos"> 20</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="L-21"><a href="#L-21"><span class="linenos"> 21</span></a>        <span class="s2">&quot;name&quot;</span><span class="p">,</span>
+</span><span id="L-22"><a href="#L-22"><span class="linenos"> 22</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
+</span><span id="L-23"><a href="#L-23"><span class="linenos"> 23</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Name of the package to create in the current working directory. &quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="L-24"><a href="#L-24"><span class="linenos"> 24</span></a>    <span class="p">)</span>
+</span><span id="L-25"><a href="#L-25"><span class="linenos"> 25</span></a>
+</span><span id="L-26"><a href="#L-26"><span class="linenos"> 26</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="L-27"><a href="#L-27"><span class="linenos"> 27</span></a>        <span class="s2">&quot;-s&quot;</span><span class="p">,</span>
+</span><span id="L-28"><a href="#L-28"><span class="linenos"> 28</span></a>        <span class="s2">&quot;--source_files&quot;</span><span class="p">,</span>
+</span><span id="L-29"><a href="#L-29"><span class="linenos"> 29</span></a>        <span class="n">nargs</span><span class="o">=</span><span class="s2">&quot;*&quot;</span><span class="p">,</span>
+</span><span id="L-30"><a href="#L-30"><span class="linenos"> 30</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
+</span><span id="L-31"><a href="#L-31"><span class="linenos"> 31</span></a>        <span class="n">default</span><span class="o">=</span><span class="p">[],</span>
+</span><span id="L-32"><a href="#L-32"><span class="linenos"> 32</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; List of additional source files to create in addition to the default</span>
+</span><span id="L-33"><a href="#L-33"><span class="linenos"> 33</span></a><span class="s2">        __init__.py and </span><span class="si">{name}</span><span class="s2">.py files.&quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="L-34"><a href="#L-34"><span class="linenos"> 34</span></a>    <span class="p">)</span>
+</span><span id="L-35"><a href="#L-35"><span class="linenos"> 35</span></a>
+</span><span id="L-36"><a href="#L-36"><span class="linenos"> 36</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="L-37"><a href="#L-37"><span class="linenos"> 37</span></a>        <span class="s2">&quot;-d&quot;</span><span class="p">,</span>
+</span><span id="L-38"><a href="#L-38"><span class="linenos"> 38</span></a>        <span class="s2">&quot;--description&quot;</span><span class="p">,</span>
+</span><span id="L-39"><a href="#L-39"><span class="linenos"> 39</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
+</span><span id="L-40"><a href="#L-40"><span class="linenos"> 40</span></a>        <span class="n">default</span><span class="o">=</span><span class="s2">&quot;&quot;</span><span class="p">,</span>
+</span><span id="L-41"><a href="#L-41"><span class="linenos"> 41</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; The package description to be added to the pyproject.toml file. &quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="L-42"><a href="#L-42"><span class="linenos"> 42</span></a>    <span class="p">)</span>
+</span><span id="L-43"><a href="#L-43"><span class="linenos"> 43</span></a>
+</span><span id="L-44"><a href="#L-44"><span class="linenos"> 44</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="L-45"><a href="#L-45"><span class="linenos"> 45</span></a>        <span class="s2">&quot;-dp&quot;</span><span class="p">,</span>
+</span><span id="L-46"><a href="#L-46"><span class="linenos"> 46</span></a>        <span class="s2">&quot;--dependencies&quot;</span><span class="p">,</span>
+</span><span id="L-47"><a href="#L-47"><span class="linenos"> 47</span></a>        <span class="n">nargs</span><span class="o">=</span><span class="s2">&quot;*&quot;</span><span class="p">,</span>
+</span><span id="L-48"><a href="#L-48"><span class="linenos"> 48</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
+</span><span id="L-49"><a href="#L-49"><span class="linenos"> 49</span></a>        <span class="n">default</span><span class="o">=</span><span class="p">[],</span>
+</span><span id="L-50"><a href="#L-50"><span class="linenos"> 50</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; List of dependencies to add to pyproject.toml.</span>
+</span><span id="L-51"><a href="#L-51"><span class="linenos"> 51</span></a><span class="s2">        Note: hassle.py will automatically scan your project for 3rd party</span>
+</span><span id="L-52"><a href="#L-52"><span class="linenos"> 52</span></a><span class="s2">        imports and update pyproject.toml. This switch is largely useful</span>
+</span><span id="L-53"><a href="#L-53"><span class="linenos"> 53</span></a><span class="s2">        for adding dependencies your project might need, but doesn&#39;t</span>
+</span><span id="L-54"><a href="#L-54"><span class="linenos"> 54</span></a><span class="s2">        directly import in any source files,</span>
+</span><span id="L-55"><a href="#L-55"><span class="linenos"> 55</span></a><span class="s2">        like an os.system() call that invokes a 3rd party cli.&quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="L-56"><a href="#L-56"><span class="linenos"> 56</span></a>    <span class="p">)</span>
+</span><span id="L-57"><a href="#L-57"><span class="linenos"> 57</span></a>
+</span><span id="L-58"><a href="#L-58"><span class="linenos"> 58</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="L-59"><a href="#L-59"><span class="linenos"> 59</span></a>        <span class="s2">&quot;-k&quot;</span><span class="p">,</span>
+</span><span id="L-60"><a href="#L-60"><span class="linenos"> 60</span></a>        <span class="s2">&quot;--keywords&quot;</span><span class="p">,</span>
+</span><span id="L-61"><a href="#L-61"><span class="linenos"> 61</span></a>        <span class="n">nargs</span><span class="o">=</span><span class="s2">&quot;*&quot;</span><span class="p">,</span>
+</span><span id="L-62"><a href="#L-62"><span class="linenos"> 62</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
+</span><span id="L-63"><a href="#L-63"><span class="linenos"> 63</span></a>        <span class="n">default</span><span class="o">=</span><span class="p">[],</span>
+</span><span id="L-64"><a href="#L-64"><span class="linenos"> 64</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; List of keywords to be added to the keywords field in pyproject.toml. &quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="L-65"><a href="#L-65"><span class="linenos"> 65</span></a>    <span class="p">)</span>
+</span><span id="L-66"><a href="#L-66"><span class="linenos"> 66</span></a>
+</span><span id="L-67"><a href="#L-67"><span class="linenos"> 67</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="L-68"><a href="#L-68"><span class="linenos"> 68</span></a>        <span class="s2">&quot;-as&quot;</span><span class="p">,</span>
+</span><span id="L-69"><a href="#L-69"><span class="linenos"> 69</span></a>        <span class="s2">&quot;--add_script&quot;</span><span class="p">,</span>
+</span><span id="L-70"><a href="#L-70"><span class="linenos"> 70</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
+</span><span id="L-71"><a href="#L-71"><span class="linenos"> 71</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Add section to pyproject.toml declaring the package </span>
+</span><span id="L-72"><a href="#L-72"><span class="linenos"> 72</span></a><span class="s2">        should be installed with command line scripts added. </span>
+</span><span id="L-73"><a href="#L-73"><span class="linenos"> 73</span></a><span class="s2">        The default is &#39;</span><span class="si">{name}</span><span class="s2"> = &quot;</span><span class="si">{name}</span><span class="s2">.</span><span class="si">{name}</span><span class="s2">:main&quot;.</span>
+</span><span id="L-74"><a href="#L-74"><span class="linenos"> 74</span></a><span class="s2">        You will need to manually change this field.&quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="L-75"><a href="#L-75"><span class="linenos"> 75</span></a>    <span class="p">)</span>
+</span><span id="L-76"><a href="#L-76"><span class="linenos"> 76</span></a>
+</span><span id="L-77"><a href="#L-77"><span class="linenos"> 77</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="L-78"><a href="#L-78"><span class="linenos"> 78</span></a>        <span class="s2">&quot;-nl&quot;</span><span class="p">,</span>
+</span><span id="L-79"><a href="#L-79"><span class="linenos"> 79</span></a>        <span class="s2">&quot;--no_license&quot;</span><span class="p">,</span>
+</span><span id="L-80"><a href="#L-80"><span class="linenos"> 80</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
+</span><span id="L-81"><a href="#L-81"><span class="linenos"> 81</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; By default, projects are created with an MIT license.</span>
+</span><span id="L-82"><a href="#L-82"><span class="linenos"> 82</span></a><span class="s2">        Set this flag to avoid adding a license if you want to configure licensing</span>
+</span><span id="L-83"><a href="#L-83"><span class="linenos"> 83</span></a><span class="s2">        at another time.&quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="L-84"><a href="#L-84"><span class="linenos"> 84</span></a>    <span class="p">)</span>
+</span><span id="L-85"><a href="#L-85"><span class="linenos"> 85</span></a>
+</span><span id="L-86"><a href="#L-86"><span class="linenos"> 86</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="L-87"><a href="#L-87"><span class="linenos"> 87</span></a>        <span class="s2">&quot;-os&quot;</span><span class="p">,</span>
+</span><span id="L-88"><a href="#L-88"><span class="linenos"> 88</span></a>        <span class="s2">&quot;--operating_system&quot;</span><span class="p">,</span>
+</span><span id="L-89"><a href="#L-89"><span class="linenos"> 89</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
+</span><span id="L-90"><a href="#L-90"><span class="linenos"> 90</span></a>        <span class="n">default</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span>
+</span><span id="L-91"><a href="#L-91"><span class="linenos"> 91</span></a>        <span class="n">nargs</span><span class="o">=</span><span class="s2">&quot;*&quot;</span><span class="p">,</span>
+</span><span id="L-92"><a href="#L-92"><span class="linenos"> 92</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; List of operating systems this package will be compatible with.</span>
+</span><span id="L-93"><a href="#L-93"><span class="linenos"> 93</span></a><span class="s2">        The default is OS Independent.</span>
+</span><span id="L-94"><a href="#L-94"><span class="linenos"> 94</span></a><span class="s2">        This only affects the &#39;classifiers&#39; field of pyproject.toml .&quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="L-95"><a href="#L-95"><span class="linenos"> 95</span></a>    <span class="p">)</span>
+</span><span id="L-96"><a href="#L-96"><span class="linenos"> 96</span></a>
+</span><span id="L-97"><a href="#L-97"><span class="linenos"> 97</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="L-98"><a href="#L-98"><span class="linenos"> 98</span></a>        <span class="s2">&quot;-np&quot;</span><span class="p">,</span>
+</span><span id="L-99"><a href="#L-99"><span class="linenos"> 99</span></a>        <span class="s2">&quot;--not_package&quot;</span><span class="p">,</span>
+</span><span id="L-100"><a href="#L-100"><span class="linenos">100</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
+</span><span id="L-101"><a href="#L-101"><span class="linenos">101</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Put source files in top level directory and delete tests folder. &quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="L-102"><a href="#L-102"><span class="linenos">102</span></a>    <span class="p">)</span>
+</span><span id="L-103"><a href="#L-103"><span class="linenos">103</span></a>
+</span><span id="L-104"><a href="#L-104"><span class="linenos">104</span></a>    <span class="n">args</span> <span class="o">=</span> <span class="n">parser</span><span class="o">.</span><span class="n">parse_args</span><span class="p">()</span>
+</span><span id="L-105"><a href="#L-105"><span class="linenos">105</span></a>    <span class="n">args</span><span class="o">.</span><span class="n">source_files</span><span class="o">.</span><span class="n">extend</span><span class="p">([</span><span class="s2">&quot;__init__.py&quot;</span><span class="p">,</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="si">}</span><span class="s2">.py&quot;</span><span class="p">])</span>
+</span><span id="L-106"><a href="#L-106"><span class="linenos">106</span></a>
+</span><span id="L-107"><a href="#L-107"><span class="linenos">107</span></a>    <span class="k">return</span> <span class="n">args</span>
 </span><span id="L-108"><a href="#L-108"><span class="linenos">108</span></a>
-</span><span id="L-109"><a href="#L-109"><span class="linenos">109</span></a><span class="k">def</span> <span class="nf">get_answer</span><span class="p">(</span><span class="n">question</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
-</span><span id="L-110"><a href="#L-110"><span class="linenos">110</span></a>    <span class="sd">&quot;&quot;&quot;Repeatedly ask the user a yes/no question until a &#39;y&#39; or a &#39;n&#39; is received.&quot;&quot;&quot;</span>
-</span><span id="L-111"><a href="#L-111"><span class="linenos">111</span></a>    <span class="n">ans</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
-</span><span id="L-112"><a href="#L-112"><span class="linenos">112</span></a>    <span class="n">question</span> <span class="o">=</span> <span class="n">question</span><span class="o">.</span><span class="n">strip</span><span class="p">()</span>
-</span><span id="L-113"><a href="#L-113"><span class="linenos">113</span></a>    <span class="k">if</span> <span class="s2">&quot;?&quot;</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">question</span><span class="p">:</span>
-</span><span id="L-114"><a href="#L-114"><span class="linenos">114</span></a>        <span class="n">question</span> <span class="o">+=</span> <span class="s2">&quot;?&quot;</span>
-</span><span id="L-115"><a href="#L-115"><span class="linenos">115</span></a>    <span class="n">question</span> <span class="o">+=</span> <span class="s2">&quot; (y/n): &quot;</span>
-</span><span id="L-116"><a href="#L-116"><span class="linenos">116</span></a>    <span class="k">while</span> <span class="n">ans</span> <span class="ow">not</span> <span class="ow">in</span> <span class="p">[</span><span class="s2">&quot;y&quot;</span><span class="p">,</span> <span class="s2">&quot;yes&quot;</span><span class="p">,</span> <span class="s2">&quot;no&quot;</span><span class="p">,</span> <span class="s2">&quot;n&quot;</span><span class="p">]:</span>
-</span><span id="L-117"><a href="#L-117"><span class="linenos">117</span></a>        <span class="n">ans</span> <span class="o">=</span> <span class="nb">input</span><span class="p">(</span><span class="n">question</span><span class="p">)</span><span class="o">.</span><span class="n">strip</span><span class="p">()</span><span class="o">.</span><span class="n">lower</span><span class="p">()</span>
-</span><span id="L-118"><a href="#L-118"><span class="linenos">118</span></a>        <span class="k">if</span> <span class="n">ans</span> <span class="ow">in</span> <span class="p">[</span><span class="s2">&quot;y&quot;</span><span class="p">,</span> <span class="s2">&quot;yes&quot;</span><span class="p">]:</span>
-</span><span id="L-119"><a href="#L-119"><span class="linenos">119</span></a>            <span class="k">return</span> <span class="kc">True</span>
-</span><span id="L-120"><a href="#L-120"><span class="linenos">120</span></a>        <span class="k">elif</span> <span class="n">ans</span> <span class="ow">in</span> <span class="p">[</span><span class="s2">&quot;n&quot;</span><span class="p">,</span> <span class="s2">&quot;no&quot;</span><span class="p">]:</span>
-</span><span id="L-121"><a href="#L-121"><span class="linenos">121</span></a>            <span class="k">return</span> <span class="kc">False</span>
-</span><span id="L-122"><a href="#L-122"><span class="linenos">122</span></a>        <span class="k">else</span><span class="p">:</span>
-</span><span id="L-123"><a href="#L-123"><span class="linenos">123</span></a>            <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Invalid answer.&quot;</span><span class="p">)</span>
-</span><span id="L-124"><a href="#L-124"><span class="linenos">124</span></a>
+</span><span id="L-109"><a href="#L-109"><span class="linenos">109</span></a>
+</span><span id="L-110"><a href="#L-110"><span class="linenos">110</span></a><span class="k">def</span> <span class="nf">get_answer</span><span class="p">(</span><span class="n">question</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
+</span><span id="L-111"><a href="#L-111"><span class="linenos">111</span></a>    <span class="sd">&quot;&quot;&quot;Repeatedly ask the user a yes/no question until a &#39;y&#39; or a &#39;n&#39; is received.&quot;&quot;&quot;</span>
+</span><span id="L-112"><a href="#L-112"><span class="linenos">112</span></a>    <span class="n">ans</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
+</span><span id="L-113"><a href="#L-113"><span class="linenos">113</span></a>    <span class="n">question</span> <span class="o">=</span> <span class="n">question</span><span class="o">.</span><span class="n">strip</span><span class="p">()</span>
+</span><span id="L-114"><a href="#L-114"><span class="linenos">114</span></a>    <span class="k">if</span> <span class="s2">&quot;?&quot;</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">question</span><span class="p">:</span>
+</span><span id="L-115"><a href="#L-115"><span class="linenos">115</span></a>        <span class="n">question</span> <span class="o">+=</span> <span class="s2">&quot;?&quot;</span>
+</span><span id="L-116"><a href="#L-116"><span class="linenos">116</span></a>    <span class="n">question</span> <span class="o">+=</span> <span class="s2">&quot; (y/n): &quot;</span>
+</span><span id="L-117"><a href="#L-117"><span class="linenos">117</span></a>    <span class="k">while</span> <span class="n">ans</span> <span class="ow">not</span> <span class="ow">in</span> <span class="p">[</span><span class="s2">&quot;y&quot;</span><span class="p">,</span> <span class="s2">&quot;yes&quot;</span><span class="p">,</span> <span class="s2">&quot;no&quot;</span><span class="p">,</span> <span class="s2">&quot;n&quot;</span><span class="p">]:</span>
+</span><span id="L-118"><a href="#L-118"><span class="linenos">118</span></a>        <span class="n">ans</span> <span class="o">=</span> <span class="nb">input</span><span class="p">(</span><span class="n">question</span><span class="p">)</span><span class="o">.</span><span class="n">strip</span><span class="p">()</span><span class="o">.</span><span class="n">lower</span><span class="p">()</span>
+</span><span id="L-119"><a href="#L-119"><span class="linenos">119</span></a>        <span class="k">if</span> <span class="n">ans</span> <span class="ow">in</span> <span class="p">[</span><span class="s2">&quot;y&quot;</span><span class="p">,</span> <span class="s2">&quot;yes&quot;</span><span class="p">]:</span>
+</span><span id="L-120"><a href="#L-120"><span class="linenos">120</span></a>            <span class="k">return</span> <span class="kc">True</span>
+</span><span id="L-121"><a href="#L-121"><span class="linenos">121</span></a>        <span class="k">elif</span> <span class="n">ans</span> <span class="ow">in</span> <span class="p">[</span><span class="s2">&quot;n&quot;</span><span class="p">,</span> <span class="s2">&quot;no&quot;</span><span class="p">]:</span>
+</span><span id="L-122"><a href="#L-122"><span class="linenos">122</span></a>            <span class="k">return</span> <span class="kc">False</span>
+</span><span id="L-123"><a href="#L-123"><span class="linenos">123</span></a>        <span class="k">else</span><span class="p">:</span>
+</span><span id="L-124"><a href="#L-124"><span class="linenos">124</span></a>            <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Invalid answer.&quot;</span><span class="p">)</span>
 </span><span id="L-125"><a href="#L-125"><span class="linenos">125</span></a>
-</span><span id="L-126"><a href="#L-126"><span class="linenos">126</span></a><span class="k">def</span> <span class="nf">check_pypi_for_name</span><span class="p">(</span><span class="n">package_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
-</span><span id="L-127"><a href="#L-127"><span class="linenos">127</span></a>    <span class="sd">&quot;&quot;&quot;Check if a package with package_name already exists on `pypi.org`.</span>
-</span><span id="L-128"><a href="#L-128"><span class="linenos">128</span></a><span class="sd">    Returns `True` if package name exists.</span>
-</span><span id="L-129"><a href="#L-129"><span class="linenos">129</span></a><span class="sd">    Only checks the first page of results.&quot;&quot;&quot;</span>
-</span><span id="L-130"><a href="#L-130"><span class="linenos">130</span></a>    <span class="n">url</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;https://pypi.org/search/?q=</span><span class="si">{</span><span class="n">package_name</span><span class="o">.</span><span class="n">lower</span><span class="p">()</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="L-131"><a href="#L-131"><span class="linenos">131</span></a>    <span class="n">response</span> <span class="o">=</span> <span class="n">requests</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="n">url</span><span class="p">)</span>
-</span><span id="L-132"><a href="#L-132"><span class="linenos">132</span></a>    <span class="k">if</span> <span class="n">response</span><span class="o">.</span><span class="n">status_code</span> <span class="o">!=</span> <span class="mi">200</span><span class="p">:</span>
-</span><span id="L-133"><a href="#L-133"><span class="linenos">133</span></a>        <span class="k">raise</span> <span class="ne">RuntimeError</span><span class="p">(</span>
-</span><span id="L-134"><a href="#L-134"><span class="linenos">134</span></a>            <span class="sa">f</span><span class="s2">&quot;Error: pypi.org returned status code: </span><span class="si">{</span><span class="n">response</span><span class="o">.</span><span class="n">status_code</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="L-135"><a href="#L-135"><span class="linenos">135</span></a>        <span class="p">)</span>
-</span><span id="L-136"><a href="#L-136"><span class="linenos">136</span></a>    <span class="n">soup</span> <span class="o">=</span> <span class="n">BeautifulSoup</span><span class="p">(</span><span class="n">response</span><span class="o">.</span><span class="n">text</span><span class="p">,</span> <span class="s2">&quot;html.parser&quot;</span><span class="p">)</span>
-</span><span id="L-137"><a href="#L-137"><span class="linenos">137</span></a>    <span class="n">pypi_packages</span> <span class="o">=</span> <span class="p">[</span>
-</span><span id="L-138"><a href="#L-138"><span class="linenos">138</span></a>        <span class="n">span</span><span class="o">.</span><span class="n">text</span><span class="o">.</span><span class="n">lower</span><span class="p">()</span>
-</span><span id="L-139"><a href="#L-139"><span class="linenos">139</span></a>        <span class="k">for</span> <span class="n">span</span> <span class="ow">in</span> <span class="n">soup</span><span class="o">.</span><span class="n">find_all</span><span class="p">(</span><span class="s2">&quot;span&quot;</span><span class="p">,</span> <span class="n">class_</span><span class="o">=</span><span class="s2">&quot;package-snippet__name&quot;</span><span class="p">)</span>
-</span><span id="L-140"><a href="#L-140"><span class="linenos">140</span></a>    <span class="p">]</span>
-</span><span id="L-141"><a href="#L-141"><span class="linenos">141</span></a>    <span class="k">return</span> <span class="n">package_name</span> <span class="ow">in</span> <span class="n">pypi_packages</span>
-</span><span id="L-142"><a href="#L-142"><span class="linenos">142</span></a>
+</span><span id="L-126"><a href="#L-126"><span class="linenos">126</span></a>
+</span><span id="L-127"><a href="#L-127"><span class="linenos">127</span></a><span class="k">def</span> <span class="nf">check_pypi_for_name</span><span class="p">(</span><span class="n">package_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
+</span><span id="L-128"><a href="#L-128"><span class="linenos">128</span></a>    <span class="sd">&quot;&quot;&quot;Check if a package with package_name already exists on `pypi.org`.</span>
+</span><span id="L-129"><a href="#L-129"><span class="linenos">129</span></a><span class="sd">    Returns `True` if package name exists.</span>
+</span><span id="L-130"><a href="#L-130"><span class="linenos">130</span></a><span class="sd">    Only checks the first page of results.&quot;&quot;&quot;</span>
+</span><span id="L-131"><a href="#L-131"><span class="linenos">131</span></a>    <span class="n">url</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;https://pypi.org/search/?q=</span><span class="si">{</span><span class="n">package_name</span><span class="o">.</span><span class="n">lower</span><span class="p">()</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="L-132"><a href="#L-132"><span class="linenos">132</span></a>    <span class="n">response</span> <span class="o">=</span> <span class="n">requests</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="n">url</span><span class="p">)</span>
+</span><span id="L-133"><a href="#L-133"><span class="linenos">133</span></a>    <span class="k">if</span> <span class="n">response</span><span class="o">.</span><span class="n">status_code</span> <span class="o">!=</span> <span class="mi">200</span><span class="p">:</span>
+</span><span id="L-134"><a href="#L-134"><span class="linenos">134</span></a>        <span class="k">raise</span> <span class="ne">RuntimeError</span><span class="p">(</span>
+</span><span id="L-135"><a href="#L-135"><span class="linenos">135</span></a>            <span class="sa">f</span><span class="s2">&quot;Error: pypi.org returned status code: </span><span class="si">{</span><span class="n">response</span><span class="o">.</span><span class="n">status_code</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="L-136"><a href="#L-136"><span class="linenos">136</span></a>        <span class="p">)</span>
+</span><span id="L-137"><a href="#L-137"><span class="linenos">137</span></a>    <span class="n">soup</span> <span class="o">=</span> <span class="n">BeautifulSoup</span><span class="p">(</span><span class="n">response</span><span class="o">.</span><span class="n">text</span><span class="p">,</span> <span class="s2">&quot;html.parser&quot;</span><span class="p">)</span>
+</span><span id="L-138"><a href="#L-138"><span class="linenos">138</span></a>    <span class="n">pypi_packages</span> <span class="o">=</span> <span class="p">[</span>
+</span><span id="L-139"><a href="#L-139"><span class="linenos">139</span></a>        <span class="n">span</span><span class="o">.</span><span class="n">text</span><span class="o">.</span><span class="n">lower</span><span class="p">()</span>
+</span><span id="L-140"><a href="#L-140"><span class="linenos">140</span></a>        <span class="k">for</span> <span class="n">span</span> <span class="ow">in</span> <span class="n">soup</span><span class="o">.</span><span class="n">find_all</span><span class="p">(</span><span class="s2">&quot;span&quot;</span><span class="p">,</span> <span class="n">class_</span><span class="o">=</span><span class="s2">&quot;package-snippet__name&quot;</span><span class="p">)</span>
+</span><span id="L-141"><a href="#L-141"><span class="linenos">141</span></a>    <span class="p">]</span>
+</span><span id="L-142"><a href="#L-142"><span class="linenos">142</span></a>    <span class="k">return</span> <span class="n">package_name</span> <span class="ow">in</span> <span class="n">pypi_packages</span>
 </span><span id="L-143"><a href="#L-143"><span class="linenos">143</span></a>
-</span><span id="L-144"><a href="#L-144"><span class="linenos">144</span></a><span class="k">def</span> <span class="nf">check_pypi_for_name_cli</span><span class="p">():</span>
-</span><span id="L-145"><a href="#L-145"><span class="linenos">145</span></a>    <span class="n">parser</span> <span class="o">=</span> <span class="n">argparse</span><span class="o">.</span><span class="n">ArgumentParser</span><span class="p">()</span>
-</span><span id="L-146"><a href="#L-146"><span class="linenos">146</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span><span class="s2">&quot;name&quot;</span><span class="p">,</span> <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">)</span>
-</span><span id="L-147"><a href="#L-147"><span class="linenos">147</span></a>    <span class="n">args</span> <span class="o">=</span> <span class="n">parser</span><span class="o">.</span><span class="n">parse_args</span><span class="p">()</span>
-</span><span id="L-148"><a href="#L-148"><span class="linenos">148</span></a>    <span class="k">if</span> <span class="n">check_pypi_for_name</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="p">):</span>
-</span><span id="L-149"><a href="#L-149"><span class="linenos">149</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="si">}</span><span class="s2"> is already taken.&quot;</span><span class="p">)</span>
-</span><span id="L-150"><a href="#L-150"><span class="linenos">150</span></a>    <span class="k">else</span><span class="p">:</span>
-</span><span id="L-151"><a href="#L-151"><span class="linenos">151</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="si">}</span><span class="s2"> is available.&quot;</span><span class="p">)</span>
-</span><span id="L-152"><a href="#L-152"><span class="linenos">152</span></a>
+</span><span id="L-144"><a href="#L-144"><span class="linenos">144</span></a>
+</span><span id="L-145"><a href="#L-145"><span class="linenos">145</span></a><span class="k">def</span> <span class="nf">check_pypi_for_name_cli</span><span class="p">():</span>
+</span><span id="L-146"><a href="#L-146"><span class="linenos">146</span></a>    <span class="n">parser</span> <span class="o">=</span> <span class="n">argparse</span><span class="o">.</span><span class="n">ArgumentParser</span><span class="p">()</span>
+</span><span id="L-147"><a href="#L-147"><span class="linenos">147</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span><span class="s2">&quot;name&quot;</span><span class="p">,</span> <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">)</span>
+</span><span id="L-148"><a href="#L-148"><span class="linenos">148</span></a>    <span class="n">args</span> <span class="o">=</span> <span class="n">parser</span><span class="o">.</span><span class="n">parse_args</span><span class="p">()</span>
+</span><span id="L-149"><a href="#L-149"><span class="linenos">149</span></a>    <span class="k">if</span> <span class="n">check_pypi_for_name</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="p">):</span>
+</span><span id="L-150"><a href="#L-150"><span class="linenos">150</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="si">}</span><span class="s2"> is already taken.&quot;</span><span class="p">)</span>
+</span><span id="L-151"><a href="#L-151"><span class="linenos">151</span></a>    <span class="k">else</span><span class="p">:</span>
+</span><span id="L-152"><a href="#L-152"><span class="linenos">152</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="si">}</span><span class="s2"> is available.&quot;</span><span class="p">)</span>
 </span><span id="L-153"><a href="#L-153"><span class="linenos">153</span></a>
-</span><span id="L-154"><a href="#L-154"><span class="linenos">154</span></a><span class="k">def</span> <span class="nf">create_pyproject_file</span><span class="p">(</span><span class="n">targetdir</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span><span class="p">):</span>
-</span><span id="L-155"><a href="#L-155"><span class="linenos">155</span></a>    <span class="sd">&quot;&quot;&quot;Create `pyproject.toml` in `./{project_name}` from args, pyproject_template, and hassle_config.&quot;&quot;&quot;</span>
-</span><span id="L-156"><a href="#L-156"><span class="linenos">156</span></a>    <span class="n">pyproject</span> <span class="o">=</span> <span class="p">(</span><span class="n">root</span> <span class="o">/</span> <span class="s2">&quot;pyproject_template.toml&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">loads</span><span class="p">()</span>
-</span><span id="L-157"><a href="#L-157"><span class="linenos">157</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">hassle_config</span><span class="o">.</span><span class="n">config_exists</span><span class="p">():</span>
-</span><span id="L-158"><a href="#L-158"><span class="linenos">158</span></a>        <span class="n">hassle_config</span><span class="o">.</span><span class="n">warn</span><span class="p">()</span>
-</span><span id="L-159"><a href="#L-159"><span class="linenos">159</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">get_answer</span><span class="p">(</span><span class="s2">&quot;Continue creating new package with blank config?&quot;</span><span class="p">):</span>
-</span><span id="L-160"><a href="#L-160"><span class="linenos">160</span></a>            <span class="k">raise</span> <span class="ne">Exception</span><span class="p">(</span><span class="s2">&quot;Aborting new package creation&quot;</span><span class="p">)</span>
-</span><span id="L-161"><a href="#L-161"><span class="linenos">161</span></a>        <span class="k">else</span><span class="p">:</span>
-</span><span id="L-162"><a href="#L-162"><span class="linenos">162</span></a>            <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Creating blank hassle_config.toml...&quot;</span><span class="p">)</span>
-</span><span id="L-163"><a href="#L-163"><span class="linenos">163</span></a>            <span class="n">hassle_config</span><span class="o">.</span><span class="n">create_config</span><span class="p">()</span>
-</span><span id="L-164"><a href="#L-164"><span class="linenos">164</span></a>    <span class="n">config</span> <span class="o">=</span> <span class="n">hassle_config</span><span class="o">.</span><span class="n">load_config</span><span class="p">()</span>
-</span><span id="L-165"><a href="#L-165"><span class="linenos">165</span></a>    <span class="n">pyproject</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;name&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">name</span>
-</span><span id="L-166"><a href="#L-166"><span class="linenos">166</span></a>    <span class="n">pyproject</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;authors&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="n">config</span><span class="p">[</span><span class="s2">&quot;authors&quot;</span><span class="p">]</span>
-</span><span id="L-167"><a href="#L-167"><span class="linenos">167</span></a>    <span class="n">pyproject</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;description&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">description</span>
-</span><span id="L-168"><a href="#L-168"><span class="linenos">168</span></a>    <span class="n">pyproject</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;dependencies&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">dependencies</span>
-</span><span id="L-169"><a href="#L-169"><span class="linenos">169</span></a>    <span class="n">pyproject</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;keywords&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">keywords</span>
-</span><span id="L-170"><a href="#L-170"><span class="linenos">170</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">operating_system</span><span class="p">:</span>
-</span><span id="L-171"><a href="#L-171"><span class="linenos">171</span></a>        <span class="n">pyproject</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;classifiers&quot;</span><span class="p">][</span><span class="mi">2</span><span class="p">]</span> <span class="o">=</span> <span class="s2">&quot;Operating System :: &quot;</span> <span class="o">+</span> <span class="s2">&quot; &quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span>
-</span><span id="L-172"><a href="#L-172"><span class="linenos">172</span></a>            <span class="n">args</span><span class="o">.</span><span class="n">operating_system</span>
-</span><span id="L-173"><a href="#L-173"><span class="linenos">173</span></a>        <span class="p">)</span>
-</span><span id="L-174"><a href="#L-174"><span class="linenos">174</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">no_license</span><span class="p">:</span>
-</span><span id="L-175"><a href="#L-175"><span class="linenos">175</span></a>        <span class="n">pyproject</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;classifiers&quot;</span><span class="p">]</span><span class="o">.</span><span class="n">pop</span><span class="p">(</span><span class="mi">1</span><span class="p">)</span>
-</span><span id="L-176"><a href="#L-176"><span class="linenos">176</span></a>    <span class="k">for</span> <span class="n">field</span> <span class="ow">in</span> <span class="n">config</span><span class="p">[</span><span class="s2">&quot;project_urls&quot;</span><span class="p">]:</span>
-</span><span id="L-177"><a href="#L-177"><span class="linenos">177</span></a>        <span class="n">pyproject</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;urls&quot;</span><span class="p">][</span><span class="n">field</span><span class="p">]</span> <span class="o">=</span> <span class="n">config</span><span class="p">[</span><span class="s2">&quot;project_urls&quot;</span><span class="p">][</span><span class="n">field</span><span class="p">]</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span>
-</span><span id="L-178"><a href="#L-178"><span class="linenos">178</span></a>            <span class="s2">&quot;$name&quot;</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">name</span>
-</span><span id="L-179"><a href="#L-179"><span class="linenos">179</span></a>        <span class="p">)</span>
-</span><span id="L-180"><a href="#L-180"><span class="linenos">180</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">add_script</span><span class="p">:</span>
-</span><span id="L-181"><a href="#L-181"><span class="linenos">181</span></a>        <span class="n">pyproject</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;scripts&quot;</span><span class="p">][</span><span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="p">]</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="si">}</span><span class="s2">.</span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="si">}</span><span class="s2">:main&quot;</span>
-</span><span id="L-182"><a href="#L-182"><span class="linenos">182</span></a>    <span class="p">(</span><span class="n">targetdir</span> <span class="o">/</span> <span class="s2">&quot;pyproject.toml&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">dumps</span><span class="p">(</span><span class="n">pyproject</span><span class="p">)</span>
-</span><span id="L-183"><a href="#L-183"><span class="linenos">183</span></a>
+</span><span id="L-154"><a href="#L-154"><span class="linenos">154</span></a>
+</span><span id="L-155"><a href="#L-155"><span class="linenos">155</span></a><span class="k">def</span> <span class="nf">create_pyproject_file</span><span class="p">(</span><span class="n">targetdir</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span><span class="p">):</span>
+</span><span id="L-156"><a href="#L-156"><span class="linenos">156</span></a>    <span class="sd">&quot;&quot;&quot;Create `pyproject.toml` in `./{project_name}` from args, pyproject_template, and hassle_config.&quot;&quot;&quot;</span>
+</span><span id="L-157"><a href="#L-157"><span class="linenos">157</span></a>    <span class="n">pyproject</span> <span class="o">=</span> <span class="p">(</span><span class="n">root</span> <span class="o">/</span> <span class="s2">&quot;pyproject_template.toml&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">loads</span><span class="p">()</span>
+</span><span id="L-158"><a href="#L-158"><span class="linenos">158</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">hassle_config</span><span class="o">.</span><span class="n">config_exists</span><span class="p">():</span>
+</span><span id="L-159"><a href="#L-159"><span class="linenos">159</span></a>        <span class="n">hassle_config</span><span class="o">.</span><span class="n">warn</span><span class="p">()</span>
+</span><span id="L-160"><a href="#L-160"><span class="linenos">160</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">get_answer</span><span class="p">(</span><span class="s2">&quot;Continue creating new package with blank config?&quot;</span><span class="p">):</span>
+</span><span id="L-161"><a href="#L-161"><span class="linenos">161</span></a>            <span class="k">raise</span> <span class="ne">Exception</span><span class="p">(</span><span class="s2">&quot;Aborting new package creation&quot;</span><span class="p">)</span>
+</span><span id="L-162"><a href="#L-162"><span class="linenos">162</span></a>        <span class="k">else</span><span class="p">:</span>
+</span><span id="L-163"><a href="#L-163"><span class="linenos">163</span></a>            <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Creating blank hassle_config.toml...&quot;</span><span class="p">)</span>
+</span><span id="L-164"><a href="#L-164"><span class="linenos">164</span></a>            <span class="n">hassle_config</span><span class="o">.</span><span class="n">create_config</span><span class="p">()</span>
+</span><span id="L-165"><a href="#L-165"><span class="linenos">165</span></a>    <span class="n">config</span> <span class="o">=</span> <span class="n">hassle_config</span><span class="o">.</span><span class="n">load_config</span><span class="p">()</span>
+</span><span id="L-166"><a href="#L-166"><span class="linenos">166</span></a>    <span class="n">pyproject</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;name&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">name</span>
+</span><span id="L-167"><a href="#L-167"><span class="linenos">167</span></a>    <span class="n">pyproject</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;authors&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="n">config</span><span class="p">[</span><span class="s2">&quot;authors&quot;</span><span class="p">]</span>
+</span><span id="L-168"><a href="#L-168"><span class="linenos">168</span></a>    <span class="n">pyproject</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;description&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">description</span>
+</span><span id="L-169"><a href="#L-169"><span class="linenos">169</span></a>    <span class="n">pyproject</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;dependencies&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">dependencies</span>
+</span><span id="L-170"><a href="#L-170"><span class="linenos">170</span></a>    <span class="n">pyproject</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;keywords&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">keywords</span>
+</span><span id="L-171"><a href="#L-171"><span class="linenos">171</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">operating_system</span><span class="p">:</span>
+</span><span id="L-172"><a href="#L-172"><span class="linenos">172</span></a>        <span class="n">pyproject</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;classifiers&quot;</span><span class="p">][</span><span class="mi">2</span><span class="p">]</span> <span class="o">=</span> <span class="s2">&quot;Operating System :: &quot;</span> <span class="o">+</span> <span class="s2">&quot; &quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span>
+</span><span id="L-173"><a href="#L-173"><span class="linenos">173</span></a>            <span class="n">args</span><span class="o">.</span><span class="n">operating_system</span>
+</span><span id="L-174"><a href="#L-174"><span class="linenos">174</span></a>        <span class="p">)</span>
+</span><span id="L-175"><a href="#L-175"><span class="linenos">175</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">no_license</span><span class="p">:</span>
+</span><span id="L-176"><a href="#L-176"><span class="linenos">176</span></a>        <span class="n">pyproject</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;classifiers&quot;</span><span class="p">]</span><span class="o">.</span><span class="n">pop</span><span class="p">(</span><span class="mi">1</span><span class="p">)</span>
+</span><span id="L-177"><a href="#L-177"><span class="linenos">177</span></a>    <span class="k">for</span> <span class="n">field</span> <span class="ow">in</span> <span class="n">config</span><span class="p">[</span><span class="s2">&quot;project_urls&quot;</span><span class="p">]:</span>
+</span><span id="L-178"><a href="#L-178"><span class="linenos">178</span></a>        <span class="n">pyproject</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;urls&quot;</span><span class="p">][</span><span class="n">field</span><span class="p">]</span> <span class="o">=</span> <span class="n">config</span><span class="p">[</span><span class="s2">&quot;project_urls&quot;</span><span class="p">][</span><span class="n">field</span><span class="p">]</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span>
+</span><span id="L-179"><a href="#L-179"><span class="linenos">179</span></a>            <span class="s2">&quot;$name&quot;</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">name</span>
+</span><span id="L-180"><a href="#L-180"><span class="linenos">180</span></a>        <span class="p">)</span>
+</span><span id="L-181"><a href="#L-181"><span class="linenos">181</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">add_script</span><span class="p">:</span>
+</span><span id="L-182"><a href="#L-182"><span class="linenos">182</span></a>        <span class="n">pyproject</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;scripts&quot;</span><span class="p">][</span><span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="p">]</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="si">}</span><span class="s2">.</span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="si">}</span><span class="s2">:main&quot;</span>
+</span><span id="L-183"><a href="#L-183"><span class="linenos">183</span></a>    <span class="p">(</span><span class="n">targetdir</span> <span class="o">/</span> <span class="s2">&quot;pyproject.toml&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">dumps</span><span class="p">(</span><span class="n">pyproject</span><span class="p">)</span>
 </span><span id="L-184"><a href="#L-184"><span class="linenos">184</span></a>
-</span><span id="L-185"><a href="#L-185"><span class="linenos">185</span></a><span class="k">def</span> <span class="nf">create_source_files</span><span class="p">(</span><span class="n">srcdir</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">,</span> <span class="n">filelist</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]):</span>
-</span><span id="L-186"><a href="#L-186"><span class="linenos">186</span></a>    <span class="sd">&quot;&quot;&quot;Generate empty source files in `./{package_name}/src/{package_name}/`&quot;&quot;&quot;</span>
-</span><span id="L-187"><a href="#L-187"><span class="linenos">187</span></a>    <span class="n">srcdir</span><span class="o">.</span><span class="n">mkdir</span><span class="p">(</span><span class="n">parents</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">exist_ok</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
-</span><span id="L-188"><a href="#L-188"><span class="linenos">188</span></a>    <span class="k">for</span> <span class="n">file</span> <span class="ow">in</span> <span class="n">filelist</span><span class="p">:</span>
-</span><span id="L-189"><a href="#L-189"><span class="linenos">189</span></a>        <span class="p">(</span><span class="n">srcdir</span> <span class="o">/</span> <span class="n">file</span><span class="p">)</span><span class="o">.</span><span class="n">touch</span><span class="p">()</span>
-</span><span id="L-190"><a href="#L-190"><span class="linenos">190</span></a>
+</span><span id="L-185"><a href="#L-185"><span class="linenos">185</span></a>
+</span><span id="L-186"><a href="#L-186"><span class="linenos">186</span></a><span class="k">def</span> <span class="nf">create_source_files</span><span class="p">(</span><span class="n">srcdir</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">,</span> <span class="n">filelist</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]):</span>
+</span><span id="L-187"><a href="#L-187"><span class="linenos">187</span></a>    <span class="sd">&quot;&quot;&quot;Generate empty source files in `./{package_name}/src/{package_name}/`&quot;&quot;&quot;</span>
+</span><span id="L-188"><a href="#L-188"><span class="linenos">188</span></a>    <span class="n">srcdir</span><span class="o">.</span><span class="n">mkdir</span><span class="p">(</span><span class="n">parents</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">exist_ok</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
+</span><span id="L-189"><a href="#L-189"><span class="linenos">189</span></a>    <span class="k">for</span> <span class="n">file</span> <span class="ow">in</span> <span class="n">filelist</span><span class="p">:</span>
+</span><span id="L-190"><a href="#L-190"><span class="linenos">190</span></a>        <span class="p">(</span><span class="n">srcdir</span> <span class="o">/</span> <span class="n">file</span><span class="p">)</span><span class="o">.</span><span class="n">touch</span><span class="p">()</span>
 </span><span id="L-191"><a href="#L-191"><span class="linenos">191</span></a>
-</span><span id="L-192"><a href="#L-192"><span class="linenos">192</span></a><span class="k">def</span> <span class="nf">create_readme</span><span class="p">(</span><span class="n">targetdir</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span><span class="p">):</span>
-</span><span id="L-193"><a href="#L-193"><span class="linenos">193</span></a>    <span class="sd">&quot;&quot;&quot;Create `README.md` in `./{package_name}` from readme_template and args.&quot;&quot;&quot;</span>
-</span><span id="L-194"><a href="#L-194"><span class="linenos">194</span></a>    <span class="n">readme</span> <span class="o">=</span> <span class="p">(</span><span class="n">root</span> <span class="o">/</span> <span class="s2">&quot;README_template.md&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">read_text</span><span class="p">()</span>
-</span><span id="L-195"><a href="#L-195"><span class="linenos">195</span></a>    <span class="n">readme</span> <span class="o">=</span> <span class="n">readme</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span><span class="s2">&quot;$name&quot;</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="p">)</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span>
-</span><span id="L-196"><a href="#L-196"><span class="linenos">196</span></a>        <span class="s2">&quot;$description&quot;</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">description</span>
-</span><span id="L-197"><a href="#L-197"><span class="linenos">197</span></a>    <span class="p">)</span>
-</span><span id="L-198"><a href="#L-198"><span class="linenos">198</span></a>    <span class="p">(</span><span class="n">targetdir</span> <span class="o">/</span> <span class="s2">&quot;README.md&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span><span class="n">readme</span><span class="p">)</span>
-</span><span id="L-199"><a href="#L-199"><span class="linenos">199</span></a>
+</span><span id="L-192"><a href="#L-192"><span class="linenos">192</span></a>
+</span><span id="L-193"><a href="#L-193"><span class="linenos">193</span></a><span class="k">def</span> <span class="nf">create_readme</span><span class="p">(</span><span class="n">targetdir</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span><span class="p">):</span>
+</span><span id="L-194"><a href="#L-194"><span class="linenos">194</span></a>    <span class="sd">&quot;&quot;&quot;Create `README.md` in `./{package_name}` from readme_template and args.&quot;&quot;&quot;</span>
+</span><span id="L-195"><a href="#L-195"><span class="linenos">195</span></a>    <span class="n">readme</span> <span class="o">=</span> <span class="p">(</span><span class="n">root</span> <span class="o">/</span> <span class="s2">&quot;README_template.md&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">read_text</span><span class="p">()</span>
+</span><span id="L-196"><a href="#L-196"><span class="linenos">196</span></a>    <span class="n">readme</span> <span class="o">=</span> <span class="n">readme</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span><span class="s2">&quot;$name&quot;</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="p">)</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span>
+</span><span id="L-197"><a href="#L-197"><span class="linenos">197</span></a>        <span class="s2">&quot;$description&quot;</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">description</span>
+</span><span id="L-198"><a href="#L-198"><span class="linenos">198</span></a>    <span class="p">)</span>
+</span><span id="L-199"><a href="#L-199"><span class="linenos">199</span></a>    <span class="p">(</span><span class="n">targetdir</span> <span class="o">/</span> <span class="s2">&quot;README.md&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span><span class="n">readme</span><span class="p">)</span>
 </span><span id="L-200"><a href="#L-200"><span class="linenos">200</span></a>
-</span><span id="L-201"><a href="#L-201"><span class="linenos">201</span></a><span class="k">def</span> <span class="nf">create_license</span><span class="p">(</span><span class="n">targetdir</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">):</span>
-</span><span id="L-202"><a href="#L-202"><span class="linenos">202</span></a>    <span class="sd">&quot;&quot;&quot;Add MIT license file to `./{package_name}`.&quot;&quot;&quot;</span>
-</span><span id="L-203"><a href="#L-203"><span class="linenos">203</span></a>    <span class="n">license_template</span> <span class="o">=</span> <span class="p">(</span><span class="n">root</span> <span class="o">/</span> <span class="s2">&quot;license_template.txt&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">read_text</span><span class="p">()</span>
-</span><span id="L-204"><a href="#L-204"><span class="linenos">204</span></a>    <span class="n">license_template</span> <span class="o">=</span> <span class="n">license_template</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span><span class="s2">&quot;$year&quot;</span><span class="p">,</span> <span class="nb">str</span><span class="p">(</span><span class="n">datetime</span><span class="o">.</span><span class="n">now</span><span class="p">()</span><span class="o">.</span><span class="n">year</span><span class="p">))</span>
-</span><span id="L-205"><a href="#L-205"><span class="linenos">205</span></a>    <span class="p">(</span><span class="n">targetdir</span> <span class="o">/</span> <span class="s2">&quot;LICENSE.txt&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span><span class="n">license_template</span><span class="p">)</span>
-</span><span id="L-206"><a href="#L-206"><span class="linenos">206</span></a>
+</span><span id="L-201"><a href="#L-201"><span class="linenos">201</span></a>
+</span><span id="L-202"><a href="#L-202"><span class="linenos">202</span></a><span class="k">def</span> <span class="nf">create_license</span><span class="p">(</span><span class="n">targetdir</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">):</span>
+</span><span id="L-203"><a href="#L-203"><span class="linenos">203</span></a>    <span class="sd">&quot;&quot;&quot;Add MIT license file to `./{package_name}`.&quot;&quot;&quot;</span>
+</span><span id="L-204"><a href="#L-204"><span class="linenos">204</span></a>    <span class="n">license_template</span> <span class="o">=</span> <span class="p">(</span><span class="n">root</span> <span class="o">/</span> <span class="s2">&quot;license_template.txt&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">read_text</span><span class="p">()</span>
+</span><span id="L-205"><a href="#L-205"><span class="linenos">205</span></a>    <span class="n">license_template</span> <span class="o">=</span> <span class="n">license_template</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span><span class="s2">&quot;$year&quot;</span><span class="p">,</span> <span class="nb">str</span><span class="p">(</span><span class="n">datetime</span><span class="o">.</span><span class="n">now</span><span class="p">()</span><span class="o">.</span><span class="n">year</span><span class="p">))</span>
+</span><span id="L-206"><a href="#L-206"><span class="linenos">206</span></a>    <span class="p">(</span><span class="n">targetdir</span> <span class="o">/</span> <span class="s2">&quot;LICENSE.txt&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span><span class="n">license_template</span><span class="p">)</span>
 </span><span id="L-207"><a href="#L-207"><span class="linenos">207</span></a>
-</span><span id="L-208"><a href="#L-208"><span class="linenos">208</span></a><span class="k">def</span> <span class="nf">create_gitignore</span><span class="p">(</span><span class="n">targetdir</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">):</span>
-</span><span id="L-209"><a href="#L-209"><span class="linenos">209</span></a>    <span class="sd">&quot;&quot;&quot;Add `.gitignore` to `./{package_name}`&quot;&quot;&quot;</span>
-</span><span id="L-210"><a href="#L-210"><span class="linenos">210</span></a>    <span class="p">(</span><span class="n">root</span> <span class="o">/</span> <span class="s2">&quot;.gitignore_template&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">copy</span><span class="p">(</span><span class="n">targetdir</span> <span class="o">/</span> <span class="s2">&quot;.gitignore&quot;</span><span class="p">,</span> <span class="kc">True</span><span class="p">)</span>
-</span><span id="L-211"><a href="#L-211"><span class="linenos">211</span></a>
+</span><span id="L-208"><a href="#L-208"><span class="linenos">208</span></a>
+</span><span id="L-209"><a href="#L-209"><span class="linenos">209</span></a><span class="k">def</span> <span class="nf">create_gitignore</span><span class="p">(</span><span class="n">targetdir</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">):</span>
+</span><span id="L-210"><a href="#L-210"><span class="linenos">210</span></a>    <span class="sd">&quot;&quot;&quot;Add `.gitignore` to `./{package_name}`&quot;&quot;&quot;</span>
+</span><span id="L-211"><a href="#L-211"><span class="linenos">211</span></a>    <span class="p">(</span><span class="n">root</span> <span class="o">/</span> <span class="s2">&quot;.gitignore_template&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">copy</span><span class="p">(</span><span class="n">targetdir</span> <span class="o">/</span> <span class="s2">&quot;.gitignore&quot;</span><span class="p">,</span> <span class="kc">True</span><span class="p">)</span>
 </span><span id="L-212"><a href="#L-212"><span class="linenos">212</span></a>
-</span><span id="L-213"><a href="#L-213"><span class="linenos">213</span></a><span class="k">def</span> <span class="nf">create_vscode_settings</span><span class="p">(</span><span class="n">targetdir</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">):</span>
-</span><span id="L-214"><a href="#L-214"><span class="linenos">214</span></a>    <span class="sd">&quot;&quot;&quot;Add `settings.json` to `./.vscode`&quot;&quot;&quot;</span>
-</span><span id="L-215"><a href="#L-215"><span class="linenos">215</span></a>    <span class="n">vsdir</span> <span class="o">=</span> <span class="n">targetdir</span> <span class="o">/</span> <span class="s2">&quot;.vscode&quot;</span>
-</span><span id="L-216"><a href="#L-216"><span class="linenos">216</span></a>    <span class="n">vsdir</span><span class="o">.</span><span class="n">mkdir</span><span class="p">(</span><span class="n">parents</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">exist_ok</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
-</span><span id="L-217"><a href="#L-217"><span class="linenos">217</span></a>    <span class="p">(</span><span class="n">root</span> <span class="o">/</span> <span class="s2">&quot;.vscode_template&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">copy</span><span class="p">(</span><span class="n">vsdir</span> <span class="o">/</span> <span class="s2">&quot;settings.json&quot;</span><span class="p">,</span> <span class="kc">True</span><span class="p">)</span>
-</span><span id="L-218"><a href="#L-218"><span class="linenos">218</span></a>
+</span><span id="L-213"><a href="#L-213"><span class="linenos">213</span></a>
+</span><span id="L-214"><a href="#L-214"><span class="linenos">214</span></a><span class="k">def</span> <span class="nf">create_vscode_settings</span><span class="p">(</span><span class="n">targetdir</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">):</span>
+</span><span id="L-215"><a href="#L-215"><span class="linenos">215</span></a>    <span class="sd">&quot;&quot;&quot;Add `settings.json` to `./.vscode`&quot;&quot;&quot;</span>
+</span><span id="L-216"><a href="#L-216"><span class="linenos">216</span></a>    <span class="n">vsdir</span> <span class="o">=</span> <span class="n">targetdir</span> <span class="o">/</span> <span class="s2">&quot;.vscode&quot;</span>
+</span><span id="L-217"><a href="#L-217"><span class="linenos">217</span></a>    <span class="n">vsdir</span><span class="o">.</span><span class="n">mkdir</span><span class="p">(</span><span class="n">parents</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">exist_ok</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
+</span><span id="L-218"><a href="#L-218"><span class="linenos">218</span></a>    <span class="p">(</span><span class="n">root</span> <span class="o">/</span> <span class="s2">&quot;.vscode_template&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">copy</span><span class="p">(</span><span class="n">vsdir</span> <span class="o">/</span> <span class="s2">&quot;settings.json&quot;</span><span class="p">,</span> <span class="kc">True</span><span class="p">)</span>
 </span><span id="L-219"><a href="#L-219"><span class="linenos">219</span></a>
-</span><span id="L-220"><a href="#L-220"><span class="linenos">220</span></a><span class="k">def</span> <span class="nf">main</span><span class="p">(</span><span class="n">args</span><span class="p">:</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span> <span class="o">=</span> <span class="kc">None</span><span class="p">):</span>
-</span><span id="L-221"><a href="#L-221"><span class="linenos">221</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="p">:</span>
-</span><span id="L-222"><a href="#L-222"><span class="linenos">222</span></a>        <span class="n">args</span> <span class="o">=</span> <span class="n">get_args</span><span class="p">()</span>
-</span><span id="L-223"><a href="#L-223"><span class="linenos">223</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">not_package</span><span class="p">:</span>
-</span><span id="L-224"><a href="#L-224"><span class="linenos">224</span></a>        <span class="k">try</span><span class="p">:</span>
-</span><span id="L-225"><a href="#L-225"><span class="linenos">225</span></a>            <span class="k">if</span> <span class="n">check_pypi_for_name</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="p">):</span>
-</span><span id="L-226"><a href="#L-226"><span class="linenos">226</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="si">}</span><span class="s2"> already exists on pypi.org&quot;</span><span class="p">)</span>
-</span><span id="L-227"><a href="#L-227"><span class="linenos">227</span></a>                <span class="k">if</span> <span class="ow">not</span> <span class="n">get_answer</span><span class="p">(</span><span class="s2">&quot;Continue anyway?&quot;</span><span class="p">):</span>
-</span><span id="L-228"><a href="#L-228"><span class="linenos">228</span></a>                    <span class="n">sys</span><span class="o">.</span><span class="n">exit</span><span class="p">(</span><span class="mi">0</span><span class="p">)</span>
-</span><span id="L-229"><a href="#L-229"><span class="linenos">229</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
-</span><span id="L-230"><a href="#L-230"><span class="linenos">230</span></a>            <span class="nb">print</span><span class="p">(</span><span class="n">e</span><span class="p">)</span>
-</span><span id="L-231"><a href="#L-231"><span class="linenos">231</span></a>            <span class="nb">print</span><span class="p">(</span>
-</span><span id="L-232"><a href="#L-232"><span class="linenos">232</span></a>                <span class="sa">f</span><span class="s2">&quot;Couldn&#39;t verify that </span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="si">}</span><span class="s2"> doesn&#39;t already exist on pypi.org .&quot;</span>
-</span><span id="L-233"><a href="#L-233"><span class="linenos">233</span></a>            <span class="p">)</span>
-</span><span id="L-234"><a href="#L-234"><span class="linenos">234</span></a>            <span class="k">if</span> <span class="ow">not</span> <span class="n">get_answer</span><span class="p">(</span><span class="s2">&quot;Continue anyway?&quot;</span><span class="p">):</span>
-</span><span id="L-235"><a href="#L-235"><span class="linenos">235</span></a>                <span class="n">sys</span><span class="o">.</span><span class="n">exit</span><span class="p">(</span><span class="mi">0</span><span class="p">)</span>
-</span><span id="L-236"><a href="#L-236"><span class="linenos">236</span></a>    <span class="k">try</span><span class="p">:</span>
-</span><span id="L-237"><a href="#L-237"><span class="linenos">237</span></a>        <span class="n">targetdir</span><span class="p">:</span> <span class="n">Pathier</span> <span class="o">=</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span> <span class="o">/</span> <span class="n">args</span><span class="o">.</span><span class="n">name</span>
-</span><span id="L-238"><a href="#L-238"><span class="linenos">238</span></a>        <span class="k">try</span><span class="p">:</span>
-</span><span id="L-239"><a href="#L-239"><span class="linenos">239</span></a>            <span class="n">targetdir</span><span class="o">.</span><span class="n">mkdir</span><span class="p">(</span><span class="n">parents</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">exist_ok</span><span class="o">=</span><span class="kc">False</span><span class="p">)</span>
-</span><span id="L-240"><a href="#L-240"><span class="linenos">240</span></a>        <span class="k">except</span><span class="p">:</span>
-</span><span id="L-241"><a href="#L-241"><span class="linenos">241</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">targetdir</span><span class="si">}</span><span class="s2"> already exists.&quot;</span><span class="p">)</span>
-</span><span id="L-242"><a href="#L-242"><span class="linenos">242</span></a>            <span class="k">if</span> <span class="ow">not</span> <span class="n">get_answer</span><span class="p">(</span><span class="s2">&quot;Overwrite?&quot;</span><span class="p">):</span>
-</span><span id="L-243"><a href="#L-243"><span class="linenos">243</span></a>                <span class="n">sys</span><span class="o">.</span><span class="n">exit</span><span class="p">(</span><span class="mi">0</span><span class="p">)</span>
-</span><span id="L-244"><a href="#L-244"><span class="linenos">244</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">not_package</span><span class="p">:</span>
-</span><span id="L-245"><a href="#L-245"><span class="linenos">245</span></a>            <span class="n">create_pyproject_file</span><span class="p">(</span><span class="n">targetdir</span><span class="p">,</span> <span class="n">args</span><span class="p">)</span>
-</span><span id="L-246"><a href="#L-246"><span class="linenos">246</span></a>        <span class="n">create_source_files</span><span class="p">(</span>
-</span><span id="L-247"><a href="#L-247"><span class="linenos">247</span></a>            <span class="n">targetdir</span> <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">not_package</span> <span class="k">else</span> <span class="p">(</span><span class="n">targetdir</span> <span class="o">/</span> <span class="s2">&quot;src&quot;</span> <span class="o">/</span> <span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="p">),</span>
-</span><span id="L-248"><a href="#L-248"><span class="linenos">248</span></a>            <span class="n">args</span><span class="o">.</span><span class="n">source_files</span><span class="p">[</span><span class="mi">1</span><span class="p">:]</span> <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">not_package</span> <span class="k">else</span> <span class="n">args</span><span class="o">.</span><span class="n">source_files</span><span class="p">,</span>
-</span><span id="L-249"><a href="#L-249"><span class="linenos">249</span></a>        <span class="p">)</span>
-</span><span id="L-250"><a href="#L-250"><span class="linenos">250</span></a>        <span class="n">create_readme</span><span class="p">(</span><span class="n">targetdir</span><span class="p">,</span> <span class="n">args</span><span class="p">)</span>
-</span><span id="L-251"><a href="#L-251"><span class="linenos">251</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">not_package</span><span class="p">:</span>
-</span><span id="L-252"><a href="#L-252"><span class="linenos">252</span></a>            <span class="n">generate_test_files</span><span class="p">(</span><span class="n">targetdir</span><span class="p">)</span>
-</span><span id="L-253"><a href="#L-253"><span class="linenos">253</span></a>            <span class="n">create_vscode_settings</span><span class="p">(</span><span class="n">targetdir</span><span class="p">)</span>
-</span><span id="L-254"><a href="#L-254"><span class="linenos">254</span></a>        <span class="n">create_gitignore</span><span class="p">(</span><span class="n">targetdir</span><span class="p">)</span>
-</span><span id="L-255"><a href="#L-255"><span class="linenos">255</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">no_license</span><span class="p">:</span>
-</span><span id="L-256"><a href="#L-256"><span class="linenos">256</span></a>            <span class="n">create_license</span><span class="p">(</span><span class="n">targetdir</span><span class="p">)</span>
-</span><span id="L-257"><a href="#L-257"><span class="linenos">257</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">chdir</span><span class="p">(</span><span class="n">targetdir</span><span class="p">)</span>
-</span><span id="L-258"><a href="#L-258"><span class="linenos">258</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="s2">&quot;git init -b main&quot;</span><span class="p">)</span>
-</span><span id="L-259"><a href="#L-259"><span class="linenos">259</span></a>
-</span><span id="L-260"><a href="#L-260"><span class="linenos">260</span></a>    <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
-</span><span id="L-261"><a href="#L-261"><span class="linenos">261</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="s2">&quot;Aborting new package creation&quot;</span> <span class="ow">in</span> <span class="nb">str</span><span class="p">(</span><span class="n">e</span><span class="p">):</span>
-</span><span id="L-262"><a href="#L-262"><span class="linenos">262</span></a>            <span class="nb">print</span><span class="p">(</span><span class="n">e</span><span class="p">)</span>
-</span><span id="L-263"><a href="#L-263"><span class="linenos">263</span></a>        <span class="k">if</span> <span class="n">get_answer</span><span class="p">(</span><span class="s2">&quot;Delete created files?&quot;</span><span class="p">):</span>
-</span><span id="L-264"><a href="#L-264"><span class="linenos">264</span></a>            <span class="n">targetdir</span><span class="o">.</span><span class="n">delete</span><span class="p">()</span>
-</span><span id="L-265"><a href="#L-265"><span class="linenos">265</span></a>
+</span><span id="L-220"><a href="#L-220"><span class="linenos">220</span></a>
+</span><span id="L-221"><a href="#L-221"><span class="linenos">221</span></a><span class="k">def</span> <span class="nf">main</span><span class="p">(</span><span class="n">args</span><span class="p">:</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span> <span class="o">=</span> <span class="kc">None</span><span class="p">):</span>
+</span><span id="L-222"><a href="#L-222"><span class="linenos">222</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="p">:</span>
+</span><span id="L-223"><a href="#L-223"><span class="linenos">223</span></a>        <span class="n">args</span> <span class="o">=</span> <span class="n">get_args</span><span class="p">()</span>
+</span><span id="L-224"><a href="#L-224"><span class="linenos">224</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">not_package</span><span class="p">:</span>
+</span><span id="L-225"><a href="#L-225"><span class="linenos">225</span></a>        <span class="k">try</span><span class="p">:</span>
+</span><span id="L-226"><a href="#L-226"><span class="linenos">226</span></a>            <span class="k">if</span> <span class="n">check_pypi_for_name</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="p">):</span>
+</span><span id="L-227"><a href="#L-227"><span class="linenos">227</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="si">}</span><span class="s2"> already exists on pypi.org&quot;</span><span class="p">)</span>
+</span><span id="L-228"><a href="#L-228"><span class="linenos">228</span></a>                <span class="k">if</span> <span class="ow">not</span> <span class="n">get_answer</span><span class="p">(</span><span class="s2">&quot;Continue anyway?&quot;</span><span class="p">):</span>
+</span><span id="L-229"><a href="#L-229"><span class="linenos">229</span></a>                    <span class="n">sys</span><span class="o">.</span><span class="n">exit</span><span class="p">(</span><span class="mi">0</span><span class="p">)</span>
+</span><span id="L-230"><a href="#L-230"><span class="linenos">230</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="L-231"><a href="#L-231"><span class="linenos">231</span></a>            <span class="nb">print</span><span class="p">(</span><span class="n">e</span><span class="p">)</span>
+</span><span id="L-232"><a href="#L-232"><span class="linenos">232</span></a>            <span class="nb">print</span><span class="p">(</span>
+</span><span id="L-233"><a href="#L-233"><span class="linenos">233</span></a>                <span class="sa">f</span><span class="s2">&quot;Couldn&#39;t verify that </span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="si">}</span><span class="s2"> doesn&#39;t already exist on pypi.org .&quot;</span>
+</span><span id="L-234"><a href="#L-234"><span class="linenos">234</span></a>            <span class="p">)</span>
+</span><span id="L-235"><a href="#L-235"><span class="linenos">235</span></a>            <span class="k">if</span> <span class="ow">not</span> <span class="n">get_answer</span><span class="p">(</span><span class="s2">&quot;Continue anyway?&quot;</span><span class="p">):</span>
+</span><span id="L-236"><a href="#L-236"><span class="linenos">236</span></a>                <span class="n">sys</span><span class="o">.</span><span class="n">exit</span><span class="p">(</span><span class="mi">0</span><span class="p">)</span>
+</span><span id="L-237"><a href="#L-237"><span class="linenos">237</span></a>    <span class="k">try</span><span class="p">:</span>
+</span><span id="L-238"><a href="#L-238"><span class="linenos">238</span></a>        <span class="n">targetdir</span><span class="p">:</span> <span class="n">Pathier</span> <span class="o">=</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span> <span class="o">/</span> <span class="n">args</span><span class="o">.</span><span class="n">name</span>
+</span><span id="L-239"><a href="#L-239"><span class="linenos">239</span></a>        <span class="k">try</span><span class="p">:</span>
+</span><span id="L-240"><a href="#L-240"><span class="linenos">240</span></a>            <span class="n">targetdir</span><span class="o">.</span><span class="n">mkdir</span><span class="p">(</span><span class="n">parents</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">exist_ok</span><span class="o">=</span><span class="kc">False</span><span class="p">)</span>
+</span><span id="L-241"><a href="#L-241"><span class="linenos">241</span></a>        <span class="k">except</span><span class="p">:</span>
+</span><span id="L-242"><a href="#L-242"><span class="linenos">242</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">targetdir</span><span class="si">}</span><span class="s2"> already exists.&quot;</span><span class="p">)</span>
+</span><span id="L-243"><a href="#L-243"><span class="linenos">243</span></a>            <span class="k">if</span> <span class="ow">not</span> <span class="n">get_answer</span><span class="p">(</span><span class="s2">&quot;Overwrite?&quot;</span><span class="p">):</span>
+</span><span id="L-244"><a href="#L-244"><span class="linenos">244</span></a>                <span class="n">sys</span><span class="o">.</span><span class="n">exit</span><span class="p">(</span><span class="mi">0</span><span class="p">)</span>
+</span><span id="L-245"><a href="#L-245"><span class="linenos">245</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">not_package</span><span class="p">:</span>
+</span><span id="L-246"><a href="#L-246"><span class="linenos">246</span></a>            <span class="n">create_pyproject_file</span><span class="p">(</span><span class="n">targetdir</span><span class="p">,</span> <span class="n">args</span><span class="p">)</span>
+</span><span id="L-247"><a href="#L-247"><span class="linenos">247</span></a>        <span class="n">create_source_files</span><span class="p">(</span>
+</span><span id="L-248"><a href="#L-248"><span class="linenos">248</span></a>            <span class="n">targetdir</span> <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">not_package</span> <span class="k">else</span> <span class="p">(</span><span class="n">targetdir</span> <span class="o">/</span> <span class="s2">&quot;src&quot;</span> <span class="o">/</span> <span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="p">),</span>
+</span><span id="L-249"><a href="#L-249"><span class="linenos">249</span></a>            <span class="n">args</span><span class="o">.</span><span class="n">source_files</span><span class="p">[</span><span class="mi">1</span><span class="p">:]</span> <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">not_package</span> <span class="k">else</span> <span class="n">args</span><span class="o">.</span><span class="n">source_files</span><span class="p">,</span>
+</span><span id="L-250"><a href="#L-250"><span class="linenos">250</span></a>        <span class="p">)</span>
+</span><span id="L-251"><a href="#L-251"><span class="linenos">251</span></a>        <span class="n">create_readme</span><span class="p">(</span><span class="n">targetdir</span><span class="p">,</span> <span class="n">args</span><span class="p">)</span>
+</span><span id="L-252"><a href="#L-252"><span class="linenos">252</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">not_package</span><span class="p">:</span>
+</span><span id="L-253"><a href="#L-253"><span class="linenos">253</span></a>            <span class="n">generate_test_files</span><span class="p">(</span><span class="n">targetdir</span><span class="p">)</span>
+</span><span id="L-254"><a href="#L-254"><span class="linenos">254</span></a>            <span class="n">create_vscode_settings</span><span class="p">(</span><span class="n">targetdir</span><span class="p">)</span>
+</span><span id="L-255"><a href="#L-255"><span class="linenos">255</span></a>        <span class="n">create_gitignore</span><span class="p">(</span><span class="n">targetdir</span><span class="p">)</span>
+</span><span id="L-256"><a href="#L-256"><span class="linenos">256</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">no_license</span><span class="p">:</span>
+</span><span id="L-257"><a href="#L-257"><span class="linenos">257</span></a>            <span class="n">create_license</span><span class="p">(</span><span class="n">targetdir</span><span class="p">)</span>
+</span><span id="L-258"><a href="#L-258"><span class="linenos">258</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">chdir</span><span class="p">(</span><span class="n">targetdir</span><span class="p">)</span>
+</span><span id="L-259"><a href="#L-259"><span class="linenos">259</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">new_repo</span><span class="p">()</span>
+</span><span id="L-260"><a href="#L-260"><span class="linenos">260</span></a>
+</span><span id="L-261"><a href="#L-261"><span class="linenos">261</span></a>    <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="L-262"><a href="#L-262"><span class="linenos">262</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="s2">&quot;Aborting new package creation&quot;</span> <span class="ow">in</span> <span class="nb">str</span><span class="p">(</span><span class="n">e</span><span class="p">):</span>
+</span><span id="L-263"><a href="#L-263"><span class="linenos">263</span></a>            <span class="nb">print</span><span class="p">(</span><span class="n">e</span><span class="p">)</span>
+</span><span id="L-264"><a href="#L-264"><span class="linenos">264</span></a>        <span class="k">if</span> <span class="n">get_answer</span><span class="p">(</span><span class="s2">&quot;Delete created files?&quot;</span><span class="p">):</span>
+</span><span id="L-265"><a href="#L-265"><span class="linenos">265</span></a>            <span class="n">targetdir</span><span class="o">.</span><span class="n">delete</span><span class="p">()</span>
 </span><span id="L-266"><a href="#L-266"><span class="linenos">266</span></a>
-</span><span id="L-267"><a href="#L-267"><span class="linenos">267</span></a><span class="k">if</span> <span class="vm">__name__</span> <span class="o">==</span> <span class="s2">&quot;__main__&quot;</span><span class="p">:</span>
-</span><span id="L-268"><a href="#L-268"><span class="linenos">268</span></a>    <span class="n">main</span><span class="p">(</span><span class="n">get_args</span><span class="p">())</span>
+</span><span id="L-267"><a href="#L-267"><span class="linenos">267</span></a>
+</span><span id="L-268"><a href="#L-268"><span class="linenos">268</span></a><span class="k">if</span> <span class="vm">__name__</span> <span class="o">==</span> <span class="s2">&quot;__main__&quot;</span><span class="p">:</span>
+</span><span id="L-269"><a href="#L-269"><span class="linenos">269</span></a>    <span class="n">main</span><span class="p">(</span><span class="n">get_args</span><span class="p">())</span>
 </span></pre></div>
 
 
             </section>
                 <section id="get_args">
                             <input id="get_args-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
@@ -363,105 +364,105 @@
         <span class="def">def</span>
         <span class="name">get_args</span><span class="signature pdoc-code condensed">(<span class="return-annotation">) -> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span>:</span></span>
 
                 <label class="view-source-button" for="get_args-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#get_args"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="get_args-17"><a href="#get_args-17"><span class="linenos"> 17</span></a><span class="k">def</span> <span class="nf">get_args</span><span class="p">()</span> <span class="o">-&gt;</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span><span class="p">:</span>
-</span><span id="get_args-18"><a href="#get_args-18"><span class="linenos"> 18</span></a>    <span class="n">parser</span> <span class="o">=</span> <span class="n">argparse</span><span class="o">.</span><span class="n">ArgumentParser</span><span class="p">()</span>
-</span><span id="get_args-19"><a href="#get_args-19"><span class="linenos"> 19</span></a>
-</span><span id="get_args-20"><a href="#get_args-20"><span class="linenos"> 20</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="get_args-21"><a href="#get_args-21"><span class="linenos"> 21</span></a>        <span class="s2">&quot;name&quot;</span><span class="p">,</span>
-</span><span id="get_args-22"><a href="#get_args-22"><span class="linenos"> 22</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
-</span><span id="get_args-23"><a href="#get_args-23"><span class="linenos"> 23</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Name of the package to create in the current working directory. &quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="get_args-24"><a href="#get_args-24"><span class="linenos"> 24</span></a>    <span class="p">)</span>
-</span><span id="get_args-25"><a href="#get_args-25"><span class="linenos"> 25</span></a>
-</span><span id="get_args-26"><a href="#get_args-26"><span class="linenos"> 26</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="get_args-27"><a href="#get_args-27"><span class="linenos"> 27</span></a>        <span class="s2">&quot;-s&quot;</span><span class="p">,</span>
-</span><span id="get_args-28"><a href="#get_args-28"><span class="linenos"> 28</span></a>        <span class="s2">&quot;--source_files&quot;</span><span class="p">,</span>
-</span><span id="get_args-29"><a href="#get_args-29"><span class="linenos"> 29</span></a>        <span class="n">nargs</span><span class="o">=</span><span class="s2">&quot;*&quot;</span><span class="p">,</span>
-</span><span id="get_args-30"><a href="#get_args-30"><span class="linenos"> 30</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
-</span><span id="get_args-31"><a href="#get_args-31"><span class="linenos"> 31</span></a>        <span class="n">default</span><span class="o">=</span><span class="p">[],</span>
-</span><span id="get_args-32"><a href="#get_args-32"><span class="linenos"> 32</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; List of additional source files to create in addition to the default</span>
-</span><span id="get_args-33"><a href="#get_args-33"><span class="linenos"> 33</span></a><span class="s2">        __init__.py and </span><span class="si">{name}</span><span class="s2">.py files.&quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="get_args-34"><a href="#get_args-34"><span class="linenos"> 34</span></a>    <span class="p">)</span>
-</span><span id="get_args-35"><a href="#get_args-35"><span class="linenos"> 35</span></a>
-</span><span id="get_args-36"><a href="#get_args-36"><span class="linenos"> 36</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="get_args-37"><a href="#get_args-37"><span class="linenos"> 37</span></a>        <span class="s2">&quot;-d&quot;</span><span class="p">,</span>
-</span><span id="get_args-38"><a href="#get_args-38"><span class="linenos"> 38</span></a>        <span class="s2">&quot;--description&quot;</span><span class="p">,</span>
-</span><span id="get_args-39"><a href="#get_args-39"><span class="linenos"> 39</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
-</span><span id="get_args-40"><a href="#get_args-40"><span class="linenos"> 40</span></a>        <span class="n">default</span><span class="o">=</span><span class="s2">&quot;&quot;</span><span class="p">,</span>
-</span><span id="get_args-41"><a href="#get_args-41"><span class="linenos"> 41</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; The package description to be added to the pyproject.toml file. &quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="get_args-42"><a href="#get_args-42"><span class="linenos"> 42</span></a>    <span class="p">)</span>
-</span><span id="get_args-43"><a href="#get_args-43"><span class="linenos"> 43</span></a>
-</span><span id="get_args-44"><a href="#get_args-44"><span class="linenos"> 44</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="get_args-45"><a href="#get_args-45"><span class="linenos"> 45</span></a>        <span class="s2">&quot;-dp&quot;</span><span class="p">,</span>
-</span><span id="get_args-46"><a href="#get_args-46"><span class="linenos"> 46</span></a>        <span class="s2">&quot;--dependencies&quot;</span><span class="p">,</span>
-</span><span id="get_args-47"><a href="#get_args-47"><span class="linenos"> 47</span></a>        <span class="n">nargs</span><span class="o">=</span><span class="s2">&quot;*&quot;</span><span class="p">,</span>
-</span><span id="get_args-48"><a href="#get_args-48"><span class="linenos"> 48</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
-</span><span id="get_args-49"><a href="#get_args-49"><span class="linenos"> 49</span></a>        <span class="n">default</span><span class="o">=</span><span class="p">[],</span>
-</span><span id="get_args-50"><a href="#get_args-50"><span class="linenos"> 50</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; List of dependencies to add to pyproject.toml.</span>
-</span><span id="get_args-51"><a href="#get_args-51"><span class="linenos"> 51</span></a><span class="s2">        Note: hassle.py will automatically scan your project for 3rd party</span>
-</span><span id="get_args-52"><a href="#get_args-52"><span class="linenos"> 52</span></a><span class="s2">        imports and update pyproject.toml. This switch is largely useful</span>
-</span><span id="get_args-53"><a href="#get_args-53"><span class="linenos"> 53</span></a><span class="s2">        for adding dependencies your project might need, but doesn&#39;t</span>
-</span><span id="get_args-54"><a href="#get_args-54"><span class="linenos"> 54</span></a><span class="s2">        directly import in any source files,</span>
-</span><span id="get_args-55"><a href="#get_args-55"><span class="linenos"> 55</span></a><span class="s2">        like an os.system() call that invokes a 3rd party cli.&quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="get_args-56"><a href="#get_args-56"><span class="linenos"> 56</span></a>    <span class="p">)</span>
-</span><span id="get_args-57"><a href="#get_args-57"><span class="linenos"> 57</span></a>
-</span><span id="get_args-58"><a href="#get_args-58"><span class="linenos"> 58</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="get_args-59"><a href="#get_args-59"><span class="linenos"> 59</span></a>        <span class="s2">&quot;-k&quot;</span><span class="p">,</span>
-</span><span id="get_args-60"><a href="#get_args-60"><span class="linenos"> 60</span></a>        <span class="s2">&quot;--keywords&quot;</span><span class="p">,</span>
-</span><span id="get_args-61"><a href="#get_args-61"><span class="linenos"> 61</span></a>        <span class="n">nargs</span><span class="o">=</span><span class="s2">&quot;*&quot;</span><span class="p">,</span>
-</span><span id="get_args-62"><a href="#get_args-62"><span class="linenos"> 62</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
-</span><span id="get_args-63"><a href="#get_args-63"><span class="linenos"> 63</span></a>        <span class="n">default</span><span class="o">=</span><span class="p">[],</span>
-</span><span id="get_args-64"><a href="#get_args-64"><span class="linenos"> 64</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; List of keywords to be added to the keywords field in pyproject.toml. &quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="get_args-65"><a href="#get_args-65"><span class="linenos"> 65</span></a>    <span class="p">)</span>
-</span><span id="get_args-66"><a href="#get_args-66"><span class="linenos"> 66</span></a>
-</span><span id="get_args-67"><a href="#get_args-67"><span class="linenos"> 67</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="get_args-68"><a href="#get_args-68"><span class="linenos"> 68</span></a>        <span class="s2">&quot;-as&quot;</span><span class="p">,</span>
-</span><span id="get_args-69"><a href="#get_args-69"><span class="linenos"> 69</span></a>        <span class="s2">&quot;--add_script&quot;</span><span class="p">,</span>
-</span><span id="get_args-70"><a href="#get_args-70"><span class="linenos"> 70</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
-</span><span id="get_args-71"><a href="#get_args-71"><span class="linenos"> 71</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Add section to pyproject.toml declaring the package </span>
-</span><span id="get_args-72"><a href="#get_args-72"><span class="linenos"> 72</span></a><span class="s2">        should be installed with command line scripts added. </span>
-</span><span id="get_args-73"><a href="#get_args-73"><span class="linenos"> 73</span></a><span class="s2">        The default is &#39;</span><span class="si">{name}</span><span class="s2"> = &quot;</span><span class="si">{name}</span><span class="s2">.</span><span class="si">{name}</span><span class="s2">:main&quot;.</span>
-</span><span id="get_args-74"><a href="#get_args-74"><span class="linenos"> 74</span></a><span class="s2">        You will need to manually change this field.&quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="get_args-75"><a href="#get_args-75"><span class="linenos"> 75</span></a>    <span class="p">)</span>
-</span><span id="get_args-76"><a href="#get_args-76"><span class="linenos"> 76</span></a>
-</span><span id="get_args-77"><a href="#get_args-77"><span class="linenos"> 77</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="get_args-78"><a href="#get_args-78"><span class="linenos"> 78</span></a>        <span class="s2">&quot;-nl&quot;</span><span class="p">,</span>
-</span><span id="get_args-79"><a href="#get_args-79"><span class="linenos"> 79</span></a>        <span class="s2">&quot;--no_license&quot;</span><span class="p">,</span>
-</span><span id="get_args-80"><a href="#get_args-80"><span class="linenos"> 80</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
-</span><span id="get_args-81"><a href="#get_args-81"><span class="linenos"> 81</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; By default, projects are created with an MIT license.</span>
-</span><span id="get_args-82"><a href="#get_args-82"><span class="linenos"> 82</span></a><span class="s2">        Set this flag to avoid adding a license if you want to configure licensing</span>
-</span><span id="get_args-83"><a href="#get_args-83"><span class="linenos"> 83</span></a><span class="s2">        at another time.&quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="get_args-84"><a href="#get_args-84"><span class="linenos"> 84</span></a>    <span class="p">)</span>
-</span><span id="get_args-85"><a href="#get_args-85"><span class="linenos"> 85</span></a>
-</span><span id="get_args-86"><a href="#get_args-86"><span class="linenos"> 86</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="get_args-87"><a href="#get_args-87"><span class="linenos"> 87</span></a>        <span class="s2">&quot;-os&quot;</span><span class="p">,</span>
-</span><span id="get_args-88"><a href="#get_args-88"><span class="linenos"> 88</span></a>        <span class="s2">&quot;--operating_system&quot;</span><span class="p">,</span>
-</span><span id="get_args-89"><a href="#get_args-89"><span class="linenos"> 89</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
-</span><span id="get_args-90"><a href="#get_args-90"><span class="linenos"> 90</span></a>        <span class="n">default</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span>
-</span><span id="get_args-91"><a href="#get_args-91"><span class="linenos"> 91</span></a>        <span class="n">nargs</span><span class="o">=</span><span class="s2">&quot;*&quot;</span><span class="p">,</span>
-</span><span id="get_args-92"><a href="#get_args-92"><span class="linenos"> 92</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; List of operating systems this package will be compatible with.</span>
-</span><span id="get_args-93"><a href="#get_args-93"><span class="linenos"> 93</span></a><span class="s2">        The default is OS Independent.</span>
-</span><span id="get_args-94"><a href="#get_args-94"><span class="linenos"> 94</span></a><span class="s2">        This only affects the &#39;classifiers&#39; field of pyproject.toml .&quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="get_args-95"><a href="#get_args-95"><span class="linenos"> 95</span></a>    <span class="p">)</span>
-</span><span id="get_args-96"><a href="#get_args-96"><span class="linenos"> 96</span></a>
-</span><span id="get_args-97"><a href="#get_args-97"><span class="linenos"> 97</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="get_args-98"><a href="#get_args-98"><span class="linenos"> 98</span></a>        <span class="s2">&quot;-np&quot;</span><span class="p">,</span>
-</span><span id="get_args-99"><a href="#get_args-99"><span class="linenos"> 99</span></a>        <span class="s2">&quot;--not_package&quot;</span><span class="p">,</span>
-</span><span id="get_args-100"><a href="#get_args-100"><span class="linenos">100</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
-</span><span id="get_args-101"><a href="#get_args-101"><span class="linenos">101</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Put source files in top level directory and delete tests folder. &quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="get_args-102"><a href="#get_args-102"><span class="linenos">102</span></a>    <span class="p">)</span>
-</span><span id="get_args-103"><a href="#get_args-103"><span class="linenos">103</span></a>
-</span><span id="get_args-104"><a href="#get_args-104"><span class="linenos">104</span></a>    <span class="n">args</span> <span class="o">=</span> <span class="n">parser</span><span class="o">.</span><span class="n">parse_args</span><span class="p">()</span>
-</span><span id="get_args-105"><a href="#get_args-105"><span class="linenos">105</span></a>    <span class="n">args</span><span class="o">.</span><span class="n">source_files</span><span class="o">.</span><span class="n">extend</span><span class="p">([</span><span class="s2">&quot;__init__.py&quot;</span><span class="p">,</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="si">}</span><span class="s2">.py&quot;</span><span class="p">])</span>
-</span><span id="get_args-106"><a href="#get_args-106"><span class="linenos">106</span></a>
-</span><span id="get_args-107"><a href="#get_args-107"><span class="linenos">107</span></a>    <span class="k">return</span> <span class="n">args</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="get_args-18"><a href="#get_args-18"><span class="linenos"> 18</span></a><span class="k">def</span> <span class="nf">get_args</span><span class="p">()</span> <span class="o">-&gt;</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span><span class="p">:</span>
+</span><span id="get_args-19"><a href="#get_args-19"><span class="linenos"> 19</span></a>    <span class="n">parser</span> <span class="o">=</span> <span class="n">argparse</span><span class="o">.</span><span class="n">ArgumentParser</span><span class="p">()</span>
+</span><span id="get_args-20"><a href="#get_args-20"><span class="linenos"> 20</span></a>
+</span><span id="get_args-21"><a href="#get_args-21"><span class="linenos"> 21</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="get_args-22"><a href="#get_args-22"><span class="linenos"> 22</span></a>        <span class="s2">&quot;name&quot;</span><span class="p">,</span>
+</span><span id="get_args-23"><a href="#get_args-23"><span class="linenos"> 23</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
+</span><span id="get_args-24"><a href="#get_args-24"><span class="linenos"> 24</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Name of the package to create in the current working directory. &quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="get_args-25"><a href="#get_args-25"><span class="linenos"> 25</span></a>    <span class="p">)</span>
+</span><span id="get_args-26"><a href="#get_args-26"><span class="linenos"> 26</span></a>
+</span><span id="get_args-27"><a href="#get_args-27"><span class="linenos"> 27</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="get_args-28"><a href="#get_args-28"><span class="linenos"> 28</span></a>        <span class="s2">&quot;-s&quot;</span><span class="p">,</span>
+</span><span id="get_args-29"><a href="#get_args-29"><span class="linenos"> 29</span></a>        <span class="s2">&quot;--source_files&quot;</span><span class="p">,</span>
+</span><span id="get_args-30"><a href="#get_args-30"><span class="linenos"> 30</span></a>        <span class="n">nargs</span><span class="o">=</span><span class="s2">&quot;*&quot;</span><span class="p">,</span>
+</span><span id="get_args-31"><a href="#get_args-31"><span class="linenos"> 31</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
+</span><span id="get_args-32"><a href="#get_args-32"><span class="linenos"> 32</span></a>        <span class="n">default</span><span class="o">=</span><span class="p">[],</span>
+</span><span id="get_args-33"><a href="#get_args-33"><span class="linenos"> 33</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; List of additional source files to create in addition to the default</span>
+</span><span id="get_args-34"><a href="#get_args-34"><span class="linenos"> 34</span></a><span class="s2">        __init__.py and </span><span class="si">{name}</span><span class="s2">.py files.&quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="get_args-35"><a href="#get_args-35"><span class="linenos"> 35</span></a>    <span class="p">)</span>
+</span><span id="get_args-36"><a href="#get_args-36"><span class="linenos"> 36</span></a>
+</span><span id="get_args-37"><a href="#get_args-37"><span class="linenos"> 37</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="get_args-38"><a href="#get_args-38"><span class="linenos"> 38</span></a>        <span class="s2">&quot;-d&quot;</span><span class="p">,</span>
+</span><span id="get_args-39"><a href="#get_args-39"><span class="linenos"> 39</span></a>        <span class="s2">&quot;--description&quot;</span><span class="p">,</span>
+</span><span id="get_args-40"><a href="#get_args-40"><span class="linenos"> 40</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
+</span><span id="get_args-41"><a href="#get_args-41"><span class="linenos"> 41</span></a>        <span class="n">default</span><span class="o">=</span><span class="s2">&quot;&quot;</span><span class="p">,</span>
+</span><span id="get_args-42"><a href="#get_args-42"><span class="linenos"> 42</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; The package description to be added to the pyproject.toml file. &quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="get_args-43"><a href="#get_args-43"><span class="linenos"> 43</span></a>    <span class="p">)</span>
+</span><span id="get_args-44"><a href="#get_args-44"><span class="linenos"> 44</span></a>
+</span><span id="get_args-45"><a href="#get_args-45"><span class="linenos"> 45</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="get_args-46"><a href="#get_args-46"><span class="linenos"> 46</span></a>        <span class="s2">&quot;-dp&quot;</span><span class="p">,</span>
+</span><span id="get_args-47"><a href="#get_args-47"><span class="linenos"> 47</span></a>        <span class="s2">&quot;--dependencies&quot;</span><span class="p">,</span>
+</span><span id="get_args-48"><a href="#get_args-48"><span class="linenos"> 48</span></a>        <span class="n">nargs</span><span class="o">=</span><span class="s2">&quot;*&quot;</span><span class="p">,</span>
+</span><span id="get_args-49"><a href="#get_args-49"><span class="linenos"> 49</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
+</span><span id="get_args-50"><a href="#get_args-50"><span class="linenos"> 50</span></a>        <span class="n">default</span><span class="o">=</span><span class="p">[],</span>
+</span><span id="get_args-51"><a href="#get_args-51"><span class="linenos"> 51</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; List of dependencies to add to pyproject.toml.</span>
+</span><span id="get_args-52"><a href="#get_args-52"><span class="linenos"> 52</span></a><span class="s2">        Note: hassle.py will automatically scan your project for 3rd party</span>
+</span><span id="get_args-53"><a href="#get_args-53"><span class="linenos"> 53</span></a><span class="s2">        imports and update pyproject.toml. This switch is largely useful</span>
+</span><span id="get_args-54"><a href="#get_args-54"><span class="linenos"> 54</span></a><span class="s2">        for adding dependencies your project might need, but doesn&#39;t</span>
+</span><span id="get_args-55"><a href="#get_args-55"><span class="linenos"> 55</span></a><span class="s2">        directly import in any source files,</span>
+</span><span id="get_args-56"><a href="#get_args-56"><span class="linenos"> 56</span></a><span class="s2">        like an os.system() call that invokes a 3rd party cli.&quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="get_args-57"><a href="#get_args-57"><span class="linenos"> 57</span></a>    <span class="p">)</span>
+</span><span id="get_args-58"><a href="#get_args-58"><span class="linenos"> 58</span></a>
+</span><span id="get_args-59"><a href="#get_args-59"><span class="linenos"> 59</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="get_args-60"><a href="#get_args-60"><span class="linenos"> 60</span></a>        <span class="s2">&quot;-k&quot;</span><span class="p">,</span>
+</span><span id="get_args-61"><a href="#get_args-61"><span class="linenos"> 61</span></a>        <span class="s2">&quot;--keywords&quot;</span><span class="p">,</span>
+</span><span id="get_args-62"><a href="#get_args-62"><span class="linenos"> 62</span></a>        <span class="n">nargs</span><span class="o">=</span><span class="s2">&quot;*&quot;</span><span class="p">,</span>
+</span><span id="get_args-63"><a href="#get_args-63"><span class="linenos"> 63</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
+</span><span id="get_args-64"><a href="#get_args-64"><span class="linenos"> 64</span></a>        <span class="n">default</span><span class="o">=</span><span class="p">[],</span>
+</span><span id="get_args-65"><a href="#get_args-65"><span class="linenos"> 65</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; List of keywords to be added to the keywords field in pyproject.toml. &quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="get_args-66"><a href="#get_args-66"><span class="linenos"> 66</span></a>    <span class="p">)</span>
+</span><span id="get_args-67"><a href="#get_args-67"><span class="linenos"> 67</span></a>
+</span><span id="get_args-68"><a href="#get_args-68"><span class="linenos"> 68</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="get_args-69"><a href="#get_args-69"><span class="linenos"> 69</span></a>        <span class="s2">&quot;-as&quot;</span><span class="p">,</span>
+</span><span id="get_args-70"><a href="#get_args-70"><span class="linenos"> 70</span></a>        <span class="s2">&quot;--add_script&quot;</span><span class="p">,</span>
+</span><span id="get_args-71"><a href="#get_args-71"><span class="linenos"> 71</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
+</span><span id="get_args-72"><a href="#get_args-72"><span class="linenos"> 72</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Add section to pyproject.toml declaring the package </span>
+</span><span id="get_args-73"><a href="#get_args-73"><span class="linenos"> 73</span></a><span class="s2">        should be installed with command line scripts added. </span>
+</span><span id="get_args-74"><a href="#get_args-74"><span class="linenos"> 74</span></a><span class="s2">        The default is &#39;</span><span class="si">{name}</span><span class="s2"> = &quot;</span><span class="si">{name}</span><span class="s2">.</span><span class="si">{name}</span><span class="s2">:main&quot;.</span>
+</span><span id="get_args-75"><a href="#get_args-75"><span class="linenos"> 75</span></a><span class="s2">        You will need to manually change this field.&quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="get_args-76"><a href="#get_args-76"><span class="linenos"> 76</span></a>    <span class="p">)</span>
+</span><span id="get_args-77"><a href="#get_args-77"><span class="linenos"> 77</span></a>
+</span><span id="get_args-78"><a href="#get_args-78"><span class="linenos"> 78</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="get_args-79"><a href="#get_args-79"><span class="linenos"> 79</span></a>        <span class="s2">&quot;-nl&quot;</span><span class="p">,</span>
+</span><span id="get_args-80"><a href="#get_args-80"><span class="linenos"> 80</span></a>        <span class="s2">&quot;--no_license&quot;</span><span class="p">,</span>
+</span><span id="get_args-81"><a href="#get_args-81"><span class="linenos"> 81</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
+</span><span id="get_args-82"><a href="#get_args-82"><span class="linenos"> 82</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; By default, projects are created with an MIT license.</span>
+</span><span id="get_args-83"><a href="#get_args-83"><span class="linenos"> 83</span></a><span class="s2">        Set this flag to avoid adding a license if you want to configure licensing</span>
+</span><span id="get_args-84"><a href="#get_args-84"><span class="linenos"> 84</span></a><span class="s2">        at another time.&quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="get_args-85"><a href="#get_args-85"><span class="linenos"> 85</span></a>    <span class="p">)</span>
+</span><span id="get_args-86"><a href="#get_args-86"><span class="linenos"> 86</span></a>
+</span><span id="get_args-87"><a href="#get_args-87"><span class="linenos"> 87</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="get_args-88"><a href="#get_args-88"><span class="linenos"> 88</span></a>        <span class="s2">&quot;-os&quot;</span><span class="p">,</span>
+</span><span id="get_args-89"><a href="#get_args-89"><span class="linenos"> 89</span></a>        <span class="s2">&quot;--operating_system&quot;</span><span class="p">,</span>
+</span><span id="get_args-90"><a href="#get_args-90"><span class="linenos"> 90</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
+</span><span id="get_args-91"><a href="#get_args-91"><span class="linenos"> 91</span></a>        <span class="n">default</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span>
+</span><span id="get_args-92"><a href="#get_args-92"><span class="linenos"> 92</span></a>        <span class="n">nargs</span><span class="o">=</span><span class="s2">&quot;*&quot;</span><span class="p">,</span>
+</span><span id="get_args-93"><a href="#get_args-93"><span class="linenos"> 93</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; List of operating systems this package will be compatible with.</span>
+</span><span id="get_args-94"><a href="#get_args-94"><span class="linenos"> 94</span></a><span class="s2">        The default is OS Independent.</span>
+</span><span id="get_args-95"><a href="#get_args-95"><span class="linenos"> 95</span></a><span class="s2">        This only affects the &#39;classifiers&#39; field of pyproject.toml .&quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="get_args-96"><a href="#get_args-96"><span class="linenos"> 96</span></a>    <span class="p">)</span>
+</span><span id="get_args-97"><a href="#get_args-97"><span class="linenos"> 97</span></a>
+</span><span id="get_args-98"><a href="#get_args-98"><span class="linenos"> 98</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="get_args-99"><a href="#get_args-99"><span class="linenos"> 99</span></a>        <span class="s2">&quot;-np&quot;</span><span class="p">,</span>
+</span><span id="get_args-100"><a href="#get_args-100"><span class="linenos">100</span></a>        <span class="s2">&quot;--not_package&quot;</span><span class="p">,</span>
+</span><span id="get_args-101"><a href="#get_args-101"><span class="linenos">101</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
+</span><span id="get_args-102"><a href="#get_args-102"><span class="linenos">102</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Put source files in top level directory and delete tests folder. &quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="get_args-103"><a href="#get_args-103"><span class="linenos">103</span></a>    <span class="p">)</span>
+</span><span id="get_args-104"><a href="#get_args-104"><span class="linenos">104</span></a>
+</span><span id="get_args-105"><a href="#get_args-105"><span class="linenos">105</span></a>    <span class="n">args</span> <span class="o">=</span> <span class="n">parser</span><span class="o">.</span><span class="n">parse_args</span><span class="p">()</span>
+</span><span id="get_args-106"><a href="#get_args-106"><span class="linenos">106</span></a>    <span class="n">args</span><span class="o">.</span><span class="n">source_files</span><span class="o">.</span><span class="n">extend</span><span class="p">([</span><span class="s2">&quot;__init__.py&quot;</span><span class="p">,</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="si">}</span><span class="s2">.py&quot;</span><span class="p">])</span>
+</span><span id="get_args-107"><a href="#get_args-107"><span class="linenos">107</span></a>
+</span><span id="get_args-108"><a href="#get_args-108"><span class="linenos">108</span></a>    <span class="k">return</span> <span class="n">args</span>
 </span></pre></div>
 
 
     
 
                 </section>
                 <section id="get_answer">
@@ -471,29 +472,29 @@
         <span class="def">def</span>
         <span class="name">get_answer</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">question</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">) -> <span class="nb">bool</span>:</span></span>
 
                 <label class="view-source-button" for="get_answer-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#get_answer"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="get_answer-110"><a href="#get_answer-110"><span class="linenos">110</span></a><span class="k">def</span> <span class="nf">get_answer</span><span class="p">(</span><span class="n">question</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
-</span><span id="get_answer-111"><a href="#get_answer-111"><span class="linenos">111</span></a>    <span class="sd">&quot;&quot;&quot;Repeatedly ask the user a yes/no question until a &#39;y&#39; or a &#39;n&#39; is received.&quot;&quot;&quot;</span>
-</span><span id="get_answer-112"><a href="#get_answer-112"><span class="linenos">112</span></a>    <span class="n">ans</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
-</span><span id="get_answer-113"><a href="#get_answer-113"><span class="linenos">113</span></a>    <span class="n">question</span> <span class="o">=</span> <span class="n">question</span><span class="o">.</span><span class="n">strip</span><span class="p">()</span>
-</span><span id="get_answer-114"><a href="#get_answer-114"><span class="linenos">114</span></a>    <span class="k">if</span> <span class="s2">&quot;?&quot;</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">question</span><span class="p">:</span>
-</span><span id="get_answer-115"><a href="#get_answer-115"><span class="linenos">115</span></a>        <span class="n">question</span> <span class="o">+=</span> <span class="s2">&quot;?&quot;</span>
-</span><span id="get_answer-116"><a href="#get_answer-116"><span class="linenos">116</span></a>    <span class="n">question</span> <span class="o">+=</span> <span class="s2">&quot; (y/n): &quot;</span>
-</span><span id="get_answer-117"><a href="#get_answer-117"><span class="linenos">117</span></a>    <span class="k">while</span> <span class="n">ans</span> <span class="ow">not</span> <span class="ow">in</span> <span class="p">[</span><span class="s2">&quot;y&quot;</span><span class="p">,</span> <span class="s2">&quot;yes&quot;</span><span class="p">,</span> <span class="s2">&quot;no&quot;</span><span class="p">,</span> <span class="s2">&quot;n&quot;</span><span class="p">]:</span>
-</span><span id="get_answer-118"><a href="#get_answer-118"><span class="linenos">118</span></a>        <span class="n">ans</span> <span class="o">=</span> <span class="nb">input</span><span class="p">(</span><span class="n">question</span><span class="p">)</span><span class="o">.</span><span class="n">strip</span><span class="p">()</span><span class="o">.</span><span class="n">lower</span><span class="p">()</span>
-</span><span id="get_answer-119"><a href="#get_answer-119"><span class="linenos">119</span></a>        <span class="k">if</span> <span class="n">ans</span> <span class="ow">in</span> <span class="p">[</span><span class="s2">&quot;y&quot;</span><span class="p">,</span> <span class="s2">&quot;yes&quot;</span><span class="p">]:</span>
-</span><span id="get_answer-120"><a href="#get_answer-120"><span class="linenos">120</span></a>            <span class="k">return</span> <span class="kc">True</span>
-</span><span id="get_answer-121"><a href="#get_answer-121"><span class="linenos">121</span></a>        <span class="k">elif</span> <span class="n">ans</span> <span class="ow">in</span> <span class="p">[</span><span class="s2">&quot;n&quot;</span><span class="p">,</span> <span class="s2">&quot;no&quot;</span><span class="p">]:</span>
-</span><span id="get_answer-122"><a href="#get_answer-122"><span class="linenos">122</span></a>            <span class="k">return</span> <span class="kc">False</span>
-</span><span id="get_answer-123"><a href="#get_answer-123"><span class="linenos">123</span></a>        <span class="k">else</span><span class="p">:</span>
-</span><span id="get_answer-124"><a href="#get_answer-124"><span class="linenos">124</span></a>            <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Invalid answer.&quot;</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="get_answer-111"><a href="#get_answer-111"><span class="linenos">111</span></a><span class="k">def</span> <span class="nf">get_answer</span><span class="p">(</span><span class="n">question</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
+</span><span id="get_answer-112"><a href="#get_answer-112"><span class="linenos">112</span></a>    <span class="sd">&quot;&quot;&quot;Repeatedly ask the user a yes/no question until a &#39;y&#39; or a &#39;n&#39; is received.&quot;&quot;&quot;</span>
+</span><span id="get_answer-113"><a href="#get_answer-113"><span class="linenos">113</span></a>    <span class="n">ans</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
+</span><span id="get_answer-114"><a href="#get_answer-114"><span class="linenos">114</span></a>    <span class="n">question</span> <span class="o">=</span> <span class="n">question</span><span class="o">.</span><span class="n">strip</span><span class="p">()</span>
+</span><span id="get_answer-115"><a href="#get_answer-115"><span class="linenos">115</span></a>    <span class="k">if</span> <span class="s2">&quot;?&quot;</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">question</span><span class="p">:</span>
+</span><span id="get_answer-116"><a href="#get_answer-116"><span class="linenos">116</span></a>        <span class="n">question</span> <span class="o">+=</span> <span class="s2">&quot;?&quot;</span>
+</span><span id="get_answer-117"><a href="#get_answer-117"><span class="linenos">117</span></a>    <span class="n">question</span> <span class="o">+=</span> <span class="s2">&quot; (y/n): &quot;</span>
+</span><span id="get_answer-118"><a href="#get_answer-118"><span class="linenos">118</span></a>    <span class="k">while</span> <span class="n">ans</span> <span class="ow">not</span> <span class="ow">in</span> <span class="p">[</span><span class="s2">&quot;y&quot;</span><span class="p">,</span> <span class="s2">&quot;yes&quot;</span><span class="p">,</span> <span class="s2">&quot;no&quot;</span><span class="p">,</span> <span class="s2">&quot;n&quot;</span><span class="p">]:</span>
+</span><span id="get_answer-119"><a href="#get_answer-119"><span class="linenos">119</span></a>        <span class="n">ans</span> <span class="o">=</span> <span class="nb">input</span><span class="p">(</span><span class="n">question</span><span class="p">)</span><span class="o">.</span><span class="n">strip</span><span class="p">()</span><span class="o">.</span><span class="n">lower</span><span class="p">()</span>
+</span><span id="get_answer-120"><a href="#get_answer-120"><span class="linenos">120</span></a>        <span class="k">if</span> <span class="n">ans</span> <span class="ow">in</span> <span class="p">[</span><span class="s2">&quot;y&quot;</span><span class="p">,</span> <span class="s2">&quot;yes&quot;</span><span class="p">]:</span>
+</span><span id="get_answer-121"><a href="#get_answer-121"><span class="linenos">121</span></a>            <span class="k">return</span> <span class="kc">True</span>
+</span><span id="get_answer-122"><a href="#get_answer-122"><span class="linenos">122</span></a>        <span class="k">elif</span> <span class="n">ans</span> <span class="ow">in</span> <span class="p">[</span><span class="s2">&quot;n&quot;</span><span class="p">,</span> <span class="s2">&quot;no&quot;</span><span class="p">]:</span>
+</span><span id="get_answer-123"><a href="#get_answer-123"><span class="linenos">123</span></a>            <span class="k">return</span> <span class="kc">False</span>
+</span><span id="get_answer-124"><a href="#get_answer-124"><span class="linenos">124</span></a>        <span class="k">else</span><span class="p">:</span>
+</span><span id="get_answer-125"><a href="#get_answer-125"><span class="linenos">125</span></a>            <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Invalid answer.&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Repeatedly ask the user a yes/no question until a 'y' or a 'n' is received.</p>
 </div>
 
 
@@ -505,30 +506,30 @@
         <span class="def">def</span>
         <span class="name">check_pypi_for_name</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">package_name</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">) -> <span class="nb">bool</span>:</span></span>
 
                 <label class="view-source-button" for="check_pypi_for_name-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#check_pypi_for_name"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="check_pypi_for_name-127"><a href="#check_pypi_for_name-127"><span class="linenos">127</span></a><span class="k">def</span> <span class="nf">check_pypi_for_name</span><span class="p">(</span><span class="n">package_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
-</span><span id="check_pypi_for_name-128"><a href="#check_pypi_for_name-128"><span class="linenos">128</span></a>    <span class="sd">&quot;&quot;&quot;Check if a package with package_name already exists on `pypi.org`.</span>
-</span><span id="check_pypi_for_name-129"><a href="#check_pypi_for_name-129"><span class="linenos">129</span></a><span class="sd">    Returns `True` if package name exists.</span>
-</span><span id="check_pypi_for_name-130"><a href="#check_pypi_for_name-130"><span class="linenos">130</span></a><span class="sd">    Only checks the first page of results.&quot;&quot;&quot;</span>
-</span><span id="check_pypi_for_name-131"><a href="#check_pypi_for_name-131"><span class="linenos">131</span></a>    <span class="n">url</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;https://pypi.org/search/?q=</span><span class="si">{</span><span class="n">package_name</span><span class="o">.</span><span class="n">lower</span><span class="p">()</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="check_pypi_for_name-132"><a href="#check_pypi_for_name-132"><span class="linenos">132</span></a>    <span class="n">response</span> <span class="o">=</span> <span class="n">requests</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="n">url</span><span class="p">)</span>
-</span><span id="check_pypi_for_name-133"><a href="#check_pypi_for_name-133"><span class="linenos">133</span></a>    <span class="k">if</span> <span class="n">response</span><span class="o">.</span><span class="n">status_code</span> <span class="o">!=</span> <span class="mi">200</span><span class="p">:</span>
-</span><span id="check_pypi_for_name-134"><a href="#check_pypi_for_name-134"><span class="linenos">134</span></a>        <span class="k">raise</span> <span class="ne">RuntimeError</span><span class="p">(</span>
-</span><span id="check_pypi_for_name-135"><a href="#check_pypi_for_name-135"><span class="linenos">135</span></a>            <span class="sa">f</span><span class="s2">&quot;Error: pypi.org returned status code: </span><span class="si">{</span><span class="n">response</span><span class="o">.</span><span class="n">status_code</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="check_pypi_for_name-136"><a href="#check_pypi_for_name-136"><span class="linenos">136</span></a>        <span class="p">)</span>
-</span><span id="check_pypi_for_name-137"><a href="#check_pypi_for_name-137"><span class="linenos">137</span></a>    <span class="n">soup</span> <span class="o">=</span> <span class="n">BeautifulSoup</span><span class="p">(</span><span class="n">response</span><span class="o">.</span><span class="n">text</span><span class="p">,</span> <span class="s2">&quot;html.parser&quot;</span><span class="p">)</span>
-</span><span id="check_pypi_for_name-138"><a href="#check_pypi_for_name-138"><span class="linenos">138</span></a>    <span class="n">pypi_packages</span> <span class="o">=</span> <span class="p">[</span>
-</span><span id="check_pypi_for_name-139"><a href="#check_pypi_for_name-139"><span class="linenos">139</span></a>        <span class="n">span</span><span class="o">.</span><span class="n">text</span><span class="o">.</span><span class="n">lower</span><span class="p">()</span>
-</span><span id="check_pypi_for_name-140"><a href="#check_pypi_for_name-140"><span class="linenos">140</span></a>        <span class="k">for</span> <span class="n">span</span> <span class="ow">in</span> <span class="n">soup</span><span class="o">.</span><span class="n">find_all</span><span class="p">(</span><span class="s2">&quot;span&quot;</span><span class="p">,</span> <span class="n">class_</span><span class="o">=</span><span class="s2">&quot;package-snippet__name&quot;</span><span class="p">)</span>
-</span><span id="check_pypi_for_name-141"><a href="#check_pypi_for_name-141"><span class="linenos">141</span></a>    <span class="p">]</span>
-</span><span id="check_pypi_for_name-142"><a href="#check_pypi_for_name-142"><span class="linenos">142</span></a>    <span class="k">return</span> <span class="n">package_name</span> <span class="ow">in</span> <span class="n">pypi_packages</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="check_pypi_for_name-128"><a href="#check_pypi_for_name-128"><span class="linenos">128</span></a><span class="k">def</span> <span class="nf">check_pypi_for_name</span><span class="p">(</span><span class="n">package_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
+</span><span id="check_pypi_for_name-129"><a href="#check_pypi_for_name-129"><span class="linenos">129</span></a>    <span class="sd">&quot;&quot;&quot;Check if a package with package_name already exists on `pypi.org`.</span>
+</span><span id="check_pypi_for_name-130"><a href="#check_pypi_for_name-130"><span class="linenos">130</span></a><span class="sd">    Returns `True` if package name exists.</span>
+</span><span id="check_pypi_for_name-131"><a href="#check_pypi_for_name-131"><span class="linenos">131</span></a><span class="sd">    Only checks the first page of results.&quot;&quot;&quot;</span>
+</span><span id="check_pypi_for_name-132"><a href="#check_pypi_for_name-132"><span class="linenos">132</span></a>    <span class="n">url</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;https://pypi.org/search/?q=</span><span class="si">{</span><span class="n">package_name</span><span class="o">.</span><span class="n">lower</span><span class="p">()</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="check_pypi_for_name-133"><a href="#check_pypi_for_name-133"><span class="linenos">133</span></a>    <span class="n">response</span> <span class="o">=</span> <span class="n">requests</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="n">url</span><span class="p">)</span>
+</span><span id="check_pypi_for_name-134"><a href="#check_pypi_for_name-134"><span class="linenos">134</span></a>    <span class="k">if</span> <span class="n">response</span><span class="o">.</span><span class="n">status_code</span> <span class="o">!=</span> <span class="mi">200</span><span class="p">:</span>
+</span><span id="check_pypi_for_name-135"><a href="#check_pypi_for_name-135"><span class="linenos">135</span></a>        <span class="k">raise</span> <span class="ne">RuntimeError</span><span class="p">(</span>
+</span><span id="check_pypi_for_name-136"><a href="#check_pypi_for_name-136"><span class="linenos">136</span></a>            <span class="sa">f</span><span class="s2">&quot;Error: pypi.org returned status code: </span><span class="si">{</span><span class="n">response</span><span class="o">.</span><span class="n">status_code</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="check_pypi_for_name-137"><a href="#check_pypi_for_name-137"><span class="linenos">137</span></a>        <span class="p">)</span>
+</span><span id="check_pypi_for_name-138"><a href="#check_pypi_for_name-138"><span class="linenos">138</span></a>    <span class="n">soup</span> <span class="o">=</span> <span class="n">BeautifulSoup</span><span class="p">(</span><span class="n">response</span><span class="o">.</span><span class="n">text</span><span class="p">,</span> <span class="s2">&quot;html.parser&quot;</span><span class="p">)</span>
+</span><span id="check_pypi_for_name-139"><a href="#check_pypi_for_name-139"><span class="linenos">139</span></a>    <span class="n">pypi_packages</span> <span class="o">=</span> <span class="p">[</span>
+</span><span id="check_pypi_for_name-140"><a href="#check_pypi_for_name-140"><span class="linenos">140</span></a>        <span class="n">span</span><span class="o">.</span><span class="n">text</span><span class="o">.</span><span class="n">lower</span><span class="p">()</span>
+</span><span id="check_pypi_for_name-141"><a href="#check_pypi_for_name-141"><span class="linenos">141</span></a>        <span class="k">for</span> <span class="n">span</span> <span class="ow">in</span> <span class="n">soup</span><span class="o">.</span><span class="n">find_all</span><span class="p">(</span><span class="s2">&quot;span&quot;</span><span class="p">,</span> <span class="n">class_</span><span class="o">=</span><span class="s2">&quot;package-snippet__name&quot;</span><span class="p">)</span>
+</span><span id="check_pypi_for_name-142"><a href="#check_pypi_for_name-142"><span class="linenos">142</span></a>    <span class="p">]</span>
+</span><span id="check_pypi_for_name-143"><a href="#check_pypi_for_name-143"><span class="linenos">143</span></a>    <span class="k">return</span> <span class="n">package_name</span> <span class="ow">in</span> <span class="n">pypi_packages</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Check if a package with package_name already exists on <code>pypi.org</code>.
 Returns <code>True</code> if package name exists.
 Only checks the first page of results.</p>
 </div>
@@ -542,22 +543,22 @@
         <span class="def">def</span>
         <span class="name">check_pypi_for_name_cli</span><span class="signature pdoc-code condensed">(<span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="check_pypi_for_name_cli-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#check_pypi_for_name_cli"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="check_pypi_for_name_cli-145"><a href="#check_pypi_for_name_cli-145"><span class="linenos">145</span></a><span class="k">def</span> <span class="nf">check_pypi_for_name_cli</span><span class="p">():</span>
-</span><span id="check_pypi_for_name_cli-146"><a href="#check_pypi_for_name_cli-146"><span class="linenos">146</span></a>    <span class="n">parser</span> <span class="o">=</span> <span class="n">argparse</span><span class="o">.</span><span class="n">ArgumentParser</span><span class="p">()</span>
-</span><span id="check_pypi_for_name_cli-147"><a href="#check_pypi_for_name_cli-147"><span class="linenos">147</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span><span class="s2">&quot;name&quot;</span><span class="p">,</span> <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">)</span>
-</span><span id="check_pypi_for_name_cli-148"><a href="#check_pypi_for_name_cli-148"><span class="linenos">148</span></a>    <span class="n">args</span> <span class="o">=</span> <span class="n">parser</span><span class="o">.</span><span class="n">parse_args</span><span class="p">()</span>
-</span><span id="check_pypi_for_name_cli-149"><a href="#check_pypi_for_name_cli-149"><span class="linenos">149</span></a>    <span class="k">if</span> <span class="n">check_pypi_for_name</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="p">):</span>
-</span><span id="check_pypi_for_name_cli-150"><a href="#check_pypi_for_name_cli-150"><span class="linenos">150</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="si">}</span><span class="s2"> is already taken.&quot;</span><span class="p">)</span>
-</span><span id="check_pypi_for_name_cli-151"><a href="#check_pypi_for_name_cli-151"><span class="linenos">151</span></a>    <span class="k">else</span><span class="p">:</span>
-</span><span id="check_pypi_for_name_cli-152"><a href="#check_pypi_for_name_cli-152"><span class="linenos">152</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="si">}</span><span class="s2"> is available.&quot;</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="check_pypi_for_name_cli-146"><a href="#check_pypi_for_name_cli-146"><span class="linenos">146</span></a><span class="k">def</span> <span class="nf">check_pypi_for_name_cli</span><span class="p">():</span>
+</span><span id="check_pypi_for_name_cli-147"><a href="#check_pypi_for_name_cli-147"><span class="linenos">147</span></a>    <span class="n">parser</span> <span class="o">=</span> <span class="n">argparse</span><span class="o">.</span><span class="n">ArgumentParser</span><span class="p">()</span>
+</span><span id="check_pypi_for_name_cli-148"><a href="#check_pypi_for_name_cli-148"><span class="linenos">148</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span><span class="s2">&quot;name&quot;</span><span class="p">,</span> <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">)</span>
+</span><span id="check_pypi_for_name_cli-149"><a href="#check_pypi_for_name_cli-149"><span class="linenos">149</span></a>    <span class="n">args</span> <span class="o">=</span> <span class="n">parser</span><span class="o">.</span><span class="n">parse_args</span><span class="p">()</span>
+</span><span id="check_pypi_for_name_cli-150"><a href="#check_pypi_for_name_cli-150"><span class="linenos">150</span></a>    <span class="k">if</span> <span class="n">check_pypi_for_name</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="p">):</span>
+</span><span id="check_pypi_for_name_cli-151"><a href="#check_pypi_for_name_cli-151"><span class="linenos">151</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="si">}</span><span class="s2"> is already taken.&quot;</span><span class="p">)</span>
+</span><span id="check_pypi_for_name_cli-152"><a href="#check_pypi_for_name_cli-152"><span class="linenos">152</span></a>    <span class="k">else</span><span class="p">:</span>
+</span><span id="check_pypi_for_name_cli-153"><a href="#check_pypi_for_name_cli-153"><span class="linenos">153</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="si">}</span><span class="s2"> is available.&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
     
 
                 </section>
                 <section id="create_pyproject_file">
@@ -567,43 +568,43 @@
         <span class="def">def</span>
         <span class="name">create_pyproject_file</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">targetdir</span><span class="p">:</span> <span class="n">pathier</span><span class="o">.</span><span class="n">pathier</span><span class="o">.</span><span class="n">Pathier</span>, </span><span class="param"><span class="n">args</span><span class="p">:</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="create_pyproject_file-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#create_pyproject_file"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="create_pyproject_file-155"><a href="#create_pyproject_file-155"><span class="linenos">155</span></a><span class="k">def</span> <span class="nf">create_pyproject_file</span><span class="p">(</span><span class="n">targetdir</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span><span class="p">):</span>
-</span><span id="create_pyproject_file-156"><a href="#create_pyproject_file-156"><span class="linenos">156</span></a>    <span class="sd">&quot;&quot;&quot;Create `pyproject.toml` in `./{project_name}` from args, pyproject_template, and hassle_config.&quot;&quot;&quot;</span>
-</span><span id="create_pyproject_file-157"><a href="#create_pyproject_file-157"><span class="linenos">157</span></a>    <span class="n">pyproject</span> <span class="o">=</span> <span class="p">(</span><span class="n">root</span> <span class="o">/</span> <span class="s2">&quot;pyproject_template.toml&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">loads</span><span class="p">()</span>
-</span><span id="create_pyproject_file-158"><a href="#create_pyproject_file-158"><span class="linenos">158</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">hassle_config</span><span class="o">.</span><span class="n">config_exists</span><span class="p">():</span>
-</span><span id="create_pyproject_file-159"><a href="#create_pyproject_file-159"><span class="linenos">159</span></a>        <span class="n">hassle_config</span><span class="o">.</span><span class="n">warn</span><span class="p">()</span>
-</span><span id="create_pyproject_file-160"><a href="#create_pyproject_file-160"><span class="linenos">160</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">get_answer</span><span class="p">(</span><span class="s2">&quot;Continue creating new package with blank config?&quot;</span><span class="p">):</span>
-</span><span id="create_pyproject_file-161"><a href="#create_pyproject_file-161"><span class="linenos">161</span></a>            <span class="k">raise</span> <span class="ne">Exception</span><span class="p">(</span><span class="s2">&quot;Aborting new package creation&quot;</span><span class="p">)</span>
-</span><span id="create_pyproject_file-162"><a href="#create_pyproject_file-162"><span class="linenos">162</span></a>        <span class="k">else</span><span class="p">:</span>
-</span><span id="create_pyproject_file-163"><a href="#create_pyproject_file-163"><span class="linenos">163</span></a>            <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Creating blank hassle_config.toml...&quot;</span><span class="p">)</span>
-</span><span id="create_pyproject_file-164"><a href="#create_pyproject_file-164"><span class="linenos">164</span></a>            <span class="n">hassle_config</span><span class="o">.</span><span class="n">create_config</span><span class="p">()</span>
-</span><span id="create_pyproject_file-165"><a href="#create_pyproject_file-165"><span class="linenos">165</span></a>    <span class="n">config</span> <span class="o">=</span> <span class="n">hassle_config</span><span class="o">.</span><span class="n">load_config</span><span class="p">()</span>
-</span><span id="create_pyproject_file-166"><a href="#create_pyproject_file-166"><span class="linenos">166</span></a>    <span class="n">pyproject</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;name&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">name</span>
-</span><span id="create_pyproject_file-167"><a href="#create_pyproject_file-167"><span class="linenos">167</span></a>    <span class="n">pyproject</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;authors&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="n">config</span><span class="p">[</span><span class="s2">&quot;authors&quot;</span><span class="p">]</span>
-</span><span id="create_pyproject_file-168"><a href="#create_pyproject_file-168"><span class="linenos">168</span></a>    <span class="n">pyproject</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;description&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">description</span>
-</span><span id="create_pyproject_file-169"><a href="#create_pyproject_file-169"><span class="linenos">169</span></a>    <span class="n">pyproject</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;dependencies&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">dependencies</span>
-</span><span id="create_pyproject_file-170"><a href="#create_pyproject_file-170"><span class="linenos">170</span></a>    <span class="n">pyproject</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;keywords&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">keywords</span>
-</span><span id="create_pyproject_file-171"><a href="#create_pyproject_file-171"><span class="linenos">171</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">operating_system</span><span class="p">:</span>
-</span><span id="create_pyproject_file-172"><a href="#create_pyproject_file-172"><span class="linenos">172</span></a>        <span class="n">pyproject</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;classifiers&quot;</span><span class="p">][</span><span class="mi">2</span><span class="p">]</span> <span class="o">=</span> <span class="s2">&quot;Operating System :: &quot;</span> <span class="o">+</span> <span class="s2">&quot; &quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span>
-</span><span id="create_pyproject_file-173"><a href="#create_pyproject_file-173"><span class="linenos">173</span></a>            <span class="n">args</span><span class="o">.</span><span class="n">operating_system</span>
-</span><span id="create_pyproject_file-174"><a href="#create_pyproject_file-174"><span class="linenos">174</span></a>        <span class="p">)</span>
-</span><span id="create_pyproject_file-175"><a href="#create_pyproject_file-175"><span class="linenos">175</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">no_license</span><span class="p">:</span>
-</span><span id="create_pyproject_file-176"><a href="#create_pyproject_file-176"><span class="linenos">176</span></a>        <span class="n">pyproject</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;classifiers&quot;</span><span class="p">]</span><span class="o">.</span><span class="n">pop</span><span class="p">(</span><span class="mi">1</span><span class="p">)</span>
-</span><span id="create_pyproject_file-177"><a href="#create_pyproject_file-177"><span class="linenos">177</span></a>    <span class="k">for</span> <span class="n">field</span> <span class="ow">in</span> <span class="n">config</span><span class="p">[</span><span class="s2">&quot;project_urls&quot;</span><span class="p">]:</span>
-</span><span id="create_pyproject_file-178"><a href="#create_pyproject_file-178"><span class="linenos">178</span></a>        <span class="n">pyproject</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;urls&quot;</span><span class="p">][</span><span class="n">field</span><span class="p">]</span> <span class="o">=</span> <span class="n">config</span><span class="p">[</span><span class="s2">&quot;project_urls&quot;</span><span class="p">][</span><span class="n">field</span><span class="p">]</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span>
-</span><span id="create_pyproject_file-179"><a href="#create_pyproject_file-179"><span class="linenos">179</span></a>            <span class="s2">&quot;$name&quot;</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">name</span>
-</span><span id="create_pyproject_file-180"><a href="#create_pyproject_file-180"><span class="linenos">180</span></a>        <span class="p">)</span>
-</span><span id="create_pyproject_file-181"><a href="#create_pyproject_file-181"><span class="linenos">181</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">add_script</span><span class="p">:</span>
-</span><span id="create_pyproject_file-182"><a href="#create_pyproject_file-182"><span class="linenos">182</span></a>        <span class="n">pyproject</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;scripts&quot;</span><span class="p">][</span><span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="p">]</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="si">}</span><span class="s2">.</span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="si">}</span><span class="s2">:main&quot;</span>
-</span><span id="create_pyproject_file-183"><a href="#create_pyproject_file-183"><span class="linenos">183</span></a>    <span class="p">(</span><span class="n">targetdir</span> <span class="o">/</span> <span class="s2">&quot;pyproject.toml&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">dumps</span><span class="p">(</span><span class="n">pyproject</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="create_pyproject_file-156"><a href="#create_pyproject_file-156"><span class="linenos">156</span></a><span class="k">def</span> <span class="nf">create_pyproject_file</span><span class="p">(</span><span class="n">targetdir</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span><span class="p">):</span>
+</span><span id="create_pyproject_file-157"><a href="#create_pyproject_file-157"><span class="linenos">157</span></a>    <span class="sd">&quot;&quot;&quot;Create `pyproject.toml` in `./{project_name}` from args, pyproject_template, and hassle_config.&quot;&quot;&quot;</span>
+</span><span id="create_pyproject_file-158"><a href="#create_pyproject_file-158"><span class="linenos">158</span></a>    <span class="n">pyproject</span> <span class="o">=</span> <span class="p">(</span><span class="n">root</span> <span class="o">/</span> <span class="s2">&quot;pyproject_template.toml&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">loads</span><span class="p">()</span>
+</span><span id="create_pyproject_file-159"><a href="#create_pyproject_file-159"><span class="linenos">159</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">hassle_config</span><span class="o">.</span><span class="n">config_exists</span><span class="p">():</span>
+</span><span id="create_pyproject_file-160"><a href="#create_pyproject_file-160"><span class="linenos">160</span></a>        <span class="n">hassle_config</span><span class="o">.</span><span class="n">warn</span><span class="p">()</span>
+</span><span id="create_pyproject_file-161"><a href="#create_pyproject_file-161"><span class="linenos">161</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">get_answer</span><span class="p">(</span><span class="s2">&quot;Continue creating new package with blank config?&quot;</span><span class="p">):</span>
+</span><span id="create_pyproject_file-162"><a href="#create_pyproject_file-162"><span class="linenos">162</span></a>            <span class="k">raise</span> <span class="ne">Exception</span><span class="p">(</span><span class="s2">&quot;Aborting new package creation&quot;</span><span class="p">)</span>
+</span><span id="create_pyproject_file-163"><a href="#create_pyproject_file-163"><span class="linenos">163</span></a>        <span class="k">else</span><span class="p">:</span>
+</span><span id="create_pyproject_file-164"><a href="#create_pyproject_file-164"><span class="linenos">164</span></a>            <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Creating blank hassle_config.toml...&quot;</span><span class="p">)</span>
+</span><span id="create_pyproject_file-165"><a href="#create_pyproject_file-165"><span class="linenos">165</span></a>            <span class="n">hassle_config</span><span class="o">.</span><span class="n">create_config</span><span class="p">()</span>
+</span><span id="create_pyproject_file-166"><a href="#create_pyproject_file-166"><span class="linenos">166</span></a>    <span class="n">config</span> <span class="o">=</span> <span class="n">hassle_config</span><span class="o">.</span><span class="n">load_config</span><span class="p">()</span>
+</span><span id="create_pyproject_file-167"><a href="#create_pyproject_file-167"><span class="linenos">167</span></a>    <span class="n">pyproject</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;name&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">name</span>
+</span><span id="create_pyproject_file-168"><a href="#create_pyproject_file-168"><span class="linenos">168</span></a>    <span class="n">pyproject</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;authors&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="n">config</span><span class="p">[</span><span class="s2">&quot;authors&quot;</span><span class="p">]</span>
+</span><span id="create_pyproject_file-169"><a href="#create_pyproject_file-169"><span class="linenos">169</span></a>    <span class="n">pyproject</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;description&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">description</span>
+</span><span id="create_pyproject_file-170"><a href="#create_pyproject_file-170"><span class="linenos">170</span></a>    <span class="n">pyproject</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;dependencies&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">dependencies</span>
+</span><span id="create_pyproject_file-171"><a href="#create_pyproject_file-171"><span class="linenos">171</span></a>    <span class="n">pyproject</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;keywords&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">keywords</span>
+</span><span id="create_pyproject_file-172"><a href="#create_pyproject_file-172"><span class="linenos">172</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">operating_system</span><span class="p">:</span>
+</span><span id="create_pyproject_file-173"><a href="#create_pyproject_file-173"><span class="linenos">173</span></a>        <span class="n">pyproject</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;classifiers&quot;</span><span class="p">][</span><span class="mi">2</span><span class="p">]</span> <span class="o">=</span> <span class="s2">&quot;Operating System :: &quot;</span> <span class="o">+</span> <span class="s2">&quot; &quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span>
+</span><span id="create_pyproject_file-174"><a href="#create_pyproject_file-174"><span class="linenos">174</span></a>            <span class="n">args</span><span class="o">.</span><span class="n">operating_system</span>
+</span><span id="create_pyproject_file-175"><a href="#create_pyproject_file-175"><span class="linenos">175</span></a>        <span class="p">)</span>
+</span><span id="create_pyproject_file-176"><a href="#create_pyproject_file-176"><span class="linenos">176</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">no_license</span><span class="p">:</span>
+</span><span id="create_pyproject_file-177"><a href="#create_pyproject_file-177"><span class="linenos">177</span></a>        <span class="n">pyproject</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;classifiers&quot;</span><span class="p">]</span><span class="o">.</span><span class="n">pop</span><span class="p">(</span><span class="mi">1</span><span class="p">)</span>
+</span><span id="create_pyproject_file-178"><a href="#create_pyproject_file-178"><span class="linenos">178</span></a>    <span class="k">for</span> <span class="n">field</span> <span class="ow">in</span> <span class="n">config</span><span class="p">[</span><span class="s2">&quot;project_urls&quot;</span><span class="p">]:</span>
+</span><span id="create_pyproject_file-179"><a href="#create_pyproject_file-179"><span class="linenos">179</span></a>        <span class="n">pyproject</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;urls&quot;</span><span class="p">][</span><span class="n">field</span><span class="p">]</span> <span class="o">=</span> <span class="n">config</span><span class="p">[</span><span class="s2">&quot;project_urls&quot;</span><span class="p">][</span><span class="n">field</span><span class="p">]</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span>
+</span><span id="create_pyproject_file-180"><a href="#create_pyproject_file-180"><span class="linenos">180</span></a>            <span class="s2">&quot;$name&quot;</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">name</span>
+</span><span id="create_pyproject_file-181"><a href="#create_pyproject_file-181"><span class="linenos">181</span></a>        <span class="p">)</span>
+</span><span id="create_pyproject_file-182"><a href="#create_pyproject_file-182"><span class="linenos">182</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">add_script</span><span class="p">:</span>
+</span><span id="create_pyproject_file-183"><a href="#create_pyproject_file-183"><span class="linenos">183</span></a>        <span class="n">pyproject</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;scripts&quot;</span><span class="p">][</span><span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="p">]</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="si">}</span><span class="s2">.</span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="si">}</span><span class="s2">:main&quot;</span>
+</span><span id="create_pyproject_file-184"><a href="#create_pyproject_file-184"><span class="linenos">184</span></a>    <span class="p">(</span><span class="n">targetdir</span> <span class="o">/</span> <span class="s2">&quot;pyproject.toml&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">dumps</span><span class="p">(</span><span class="n">pyproject</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Create <code>pyproject.toml</code> in <code>./{project_name}</code> from args, pyproject_template, and hassle_config.</p>
 </div>
 
 
@@ -615,19 +616,19 @@
         <span class="def">def</span>
         <span class="name">create_source_files</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">srcdir</span><span class="p">:</span> <span class="n">pathier</span><span class="o">.</span><span class="n">pathier</span><span class="o">.</span><span class="n">Pathier</span>, </span><span class="param"><span class="n">filelist</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="create_source_files-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#create_source_files"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="create_source_files-186"><a href="#create_source_files-186"><span class="linenos">186</span></a><span class="k">def</span> <span class="nf">create_source_files</span><span class="p">(</span><span class="n">srcdir</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">,</span> <span class="n">filelist</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]):</span>
-</span><span id="create_source_files-187"><a href="#create_source_files-187"><span class="linenos">187</span></a>    <span class="sd">&quot;&quot;&quot;Generate empty source files in `./{package_name}/src/{package_name}/`&quot;&quot;&quot;</span>
-</span><span id="create_source_files-188"><a href="#create_source_files-188"><span class="linenos">188</span></a>    <span class="n">srcdir</span><span class="o">.</span><span class="n">mkdir</span><span class="p">(</span><span class="n">parents</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">exist_ok</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
-</span><span id="create_source_files-189"><a href="#create_source_files-189"><span class="linenos">189</span></a>    <span class="k">for</span> <span class="n">file</span> <span class="ow">in</span> <span class="n">filelist</span><span class="p">:</span>
-</span><span id="create_source_files-190"><a href="#create_source_files-190"><span class="linenos">190</span></a>        <span class="p">(</span><span class="n">srcdir</span> <span class="o">/</span> <span class="n">file</span><span class="p">)</span><span class="o">.</span><span class="n">touch</span><span class="p">()</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="create_source_files-187"><a href="#create_source_files-187"><span class="linenos">187</span></a><span class="k">def</span> <span class="nf">create_source_files</span><span class="p">(</span><span class="n">srcdir</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">,</span> <span class="n">filelist</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]):</span>
+</span><span id="create_source_files-188"><a href="#create_source_files-188"><span class="linenos">188</span></a>    <span class="sd">&quot;&quot;&quot;Generate empty source files in `./{package_name}/src/{package_name}/`&quot;&quot;&quot;</span>
+</span><span id="create_source_files-189"><a href="#create_source_files-189"><span class="linenos">189</span></a>    <span class="n">srcdir</span><span class="o">.</span><span class="n">mkdir</span><span class="p">(</span><span class="n">parents</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">exist_ok</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
+</span><span id="create_source_files-190"><a href="#create_source_files-190"><span class="linenos">190</span></a>    <span class="k">for</span> <span class="n">file</span> <span class="ow">in</span> <span class="n">filelist</span><span class="p">:</span>
+</span><span id="create_source_files-191"><a href="#create_source_files-191"><span class="linenos">191</span></a>        <span class="p">(</span><span class="n">srcdir</span> <span class="o">/</span> <span class="n">file</span><span class="p">)</span><span class="o">.</span><span class="n">touch</span><span class="p">()</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Generate empty source files in <code>./{package_name}/src/{package_name}/</code></p>
 </div>
 
 
@@ -639,21 +640,21 @@
         <span class="def">def</span>
         <span class="name">create_readme</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">targetdir</span><span class="p">:</span> <span class="n">pathier</span><span class="o">.</span><span class="n">pathier</span><span class="o">.</span><span class="n">Pathier</span>, </span><span class="param"><span class="n">args</span><span class="p">:</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="create_readme-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#create_readme"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="create_readme-193"><a href="#create_readme-193"><span class="linenos">193</span></a><span class="k">def</span> <span class="nf">create_readme</span><span class="p">(</span><span class="n">targetdir</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span><span class="p">):</span>
-</span><span id="create_readme-194"><a href="#create_readme-194"><span class="linenos">194</span></a>    <span class="sd">&quot;&quot;&quot;Create `README.md` in `./{package_name}` from readme_template and args.&quot;&quot;&quot;</span>
-</span><span id="create_readme-195"><a href="#create_readme-195"><span class="linenos">195</span></a>    <span class="n">readme</span> <span class="o">=</span> <span class="p">(</span><span class="n">root</span> <span class="o">/</span> <span class="s2">&quot;README_template.md&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">read_text</span><span class="p">()</span>
-</span><span id="create_readme-196"><a href="#create_readme-196"><span class="linenos">196</span></a>    <span class="n">readme</span> <span class="o">=</span> <span class="n">readme</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span><span class="s2">&quot;$name&quot;</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="p">)</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span>
-</span><span id="create_readme-197"><a href="#create_readme-197"><span class="linenos">197</span></a>        <span class="s2">&quot;$description&quot;</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">description</span>
-</span><span id="create_readme-198"><a href="#create_readme-198"><span class="linenos">198</span></a>    <span class="p">)</span>
-</span><span id="create_readme-199"><a href="#create_readme-199"><span class="linenos">199</span></a>    <span class="p">(</span><span class="n">targetdir</span> <span class="o">/</span> <span class="s2">&quot;README.md&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span><span class="n">readme</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="create_readme-194"><a href="#create_readme-194"><span class="linenos">194</span></a><span class="k">def</span> <span class="nf">create_readme</span><span class="p">(</span><span class="n">targetdir</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span><span class="p">):</span>
+</span><span id="create_readme-195"><a href="#create_readme-195"><span class="linenos">195</span></a>    <span class="sd">&quot;&quot;&quot;Create `README.md` in `./{package_name}` from readme_template and args.&quot;&quot;&quot;</span>
+</span><span id="create_readme-196"><a href="#create_readme-196"><span class="linenos">196</span></a>    <span class="n">readme</span> <span class="o">=</span> <span class="p">(</span><span class="n">root</span> <span class="o">/</span> <span class="s2">&quot;README_template.md&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">read_text</span><span class="p">()</span>
+</span><span id="create_readme-197"><a href="#create_readme-197"><span class="linenos">197</span></a>    <span class="n">readme</span> <span class="o">=</span> <span class="n">readme</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span><span class="s2">&quot;$name&quot;</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="p">)</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span>
+</span><span id="create_readme-198"><a href="#create_readme-198"><span class="linenos">198</span></a>        <span class="s2">&quot;$description&quot;</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">description</span>
+</span><span id="create_readme-199"><a href="#create_readme-199"><span class="linenos">199</span></a>    <span class="p">)</span>
+</span><span id="create_readme-200"><a href="#create_readme-200"><span class="linenos">200</span></a>    <span class="p">(</span><span class="n">targetdir</span> <span class="o">/</span> <span class="s2">&quot;README.md&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span><span class="n">readme</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Create <code>README.md</code> in <code>./{package_name}</code> from readme_template and args.</p>
 </div>
 
 
@@ -665,19 +666,19 @@
         <span class="def">def</span>
         <span class="name">create_license</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">targetdir</span><span class="p">:</span> <span class="n">pathier</span><span class="o">.</span><span class="n">pathier</span><span class="o">.</span><span class="n">Pathier</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="create_license-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#create_license"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="create_license-202"><a href="#create_license-202"><span class="linenos">202</span></a><span class="k">def</span> <span class="nf">create_license</span><span class="p">(</span><span class="n">targetdir</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">):</span>
-</span><span id="create_license-203"><a href="#create_license-203"><span class="linenos">203</span></a>    <span class="sd">&quot;&quot;&quot;Add MIT license file to `./{package_name}`.&quot;&quot;&quot;</span>
-</span><span id="create_license-204"><a href="#create_license-204"><span class="linenos">204</span></a>    <span class="n">license_template</span> <span class="o">=</span> <span class="p">(</span><span class="n">root</span> <span class="o">/</span> <span class="s2">&quot;license_template.txt&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">read_text</span><span class="p">()</span>
-</span><span id="create_license-205"><a href="#create_license-205"><span class="linenos">205</span></a>    <span class="n">license_template</span> <span class="o">=</span> <span class="n">license_template</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span><span class="s2">&quot;$year&quot;</span><span class="p">,</span> <span class="nb">str</span><span class="p">(</span><span class="n">datetime</span><span class="o">.</span><span class="n">now</span><span class="p">()</span><span class="o">.</span><span class="n">year</span><span class="p">))</span>
-</span><span id="create_license-206"><a href="#create_license-206"><span class="linenos">206</span></a>    <span class="p">(</span><span class="n">targetdir</span> <span class="o">/</span> <span class="s2">&quot;LICENSE.txt&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span><span class="n">license_template</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="create_license-203"><a href="#create_license-203"><span class="linenos">203</span></a><span class="k">def</span> <span class="nf">create_license</span><span class="p">(</span><span class="n">targetdir</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">):</span>
+</span><span id="create_license-204"><a href="#create_license-204"><span class="linenos">204</span></a>    <span class="sd">&quot;&quot;&quot;Add MIT license file to `./{package_name}`.&quot;&quot;&quot;</span>
+</span><span id="create_license-205"><a href="#create_license-205"><span class="linenos">205</span></a>    <span class="n">license_template</span> <span class="o">=</span> <span class="p">(</span><span class="n">root</span> <span class="o">/</span> <span class="s2">&quot;license_template.txt&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">read_text</span><span class="p">()</span>
+</span><span id="create_license-206"><a href="#create_license-206"><span class="linenos">206</span></a>    <span class="n">license_template</span> <span class="o">=</span> <span class="n">license_template</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span><span class="s2">&quot;$year&quot;</span><span class="p">,</span> <span class="nb">str</span><span class="p">(</span><span class="n">datetime</span><span class="o">.</span><span class="n">now</span><span class="p">()</span><span class="o">.</span><span class="n">year</span><span class="p">))</span>
+</span><span id="create_license-207"><a href="#create_license-207"><span class="linenos">207</span></a>    <span class="p">(</span><span class="n">targetdir</span> <span class="o">/</span> <span class="s2">&quot;LICENSE.txt&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span><span class="n">license_template</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Add MIT license file to <code>./{package_name}</code>.</p>
 </div>
 
 
@@ -689,17 +690,17 @@
         <span class="def">def</span>
         <span class="name">create_gitignore</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">targetdir</span><span class="p">:</span> <span class="n">pathier</span><span class="o">.</span><span class="n">pathier</span><span class="o">.</span><span class="n">Pathier</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="create_gitignore-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#create_gitignore"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="create_gitignore-209"><a href="#create_gitignore-209"><span class="linenos">209</span></a><span class="k">def</span> <span class="nf">create_gitignore</span><span class="p">(</span><span class="n">targetdir</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">):</span>
-</span><span id="create_gitignore-210"><a href="#create_gitignore-210"><span class="linenos">210</span></a>    <span class="sd">&quot;&quot;&quot;Add `.gitignore` to `./{package_name}`&quot;&quot;&quot;</span>
-</span><span id="create_gitignore-211"><a href="#create_gitignore-211"><span class="linenos">211</span></a>    <span class="p">(</span><span class="n">root</span> <span class="o">/</span> <span class="s2">&quot;.gitignore_template&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">copy</span><span class="p">(</span><span class="n">targetdir</span> <span class="o">/</span> <span class="s2">&quot;.gitignore&quot;</span><span class="p">,</span> <span class="kc">True</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="create_gitignore-210"><a href="#create_gitignore-210"><span class="linenos">210</span></a><span class="k">def</span> <span class="nf">create_gitignore</span><span class="p">(</span><span class="n">targetdir</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">):</span>
+</span><span id="create_gitignore-211"><a href="#create_gitignore-211"><span class="linenos">211</span></a>    <span class="sd">&quot;&quot;&quot;Add `.gitignore` to `./{package_name}`&quot;&quot;&quot;</span>
+</span><span id="create_gitignore-212"><a href="#create_gitignore-212"><span class="linenos">212</span></a>    <span class="p">(</span><span class="n">root</span> <span class="o">/</span> <span class="s2">&quot;.gitignore_template&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">copy</span><span class="p">(</span><span class="n">targetdir</span> <span class="o">/</span> <span class="s2">&quot;.gitignore&quot;</span><span class="p">,</span> <span class="kc">True</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Add <code>.gitignore</code> to <code>./{package_name}</code></p>
 </div>
 
 
@@ -711,19 +712,19 @@
         <span class="def">def</span>
         <span class="name">create_vscode_settings</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">targetdir</span><span class="p">:</span> <span class="n">pathier</span><span class="o">.</span><span class="n">pathier</span><span class="o">.</span><span class="n">Pathier</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="create_vscode_settings-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#create_vscode_settings"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="create_vscode_settings-214"><a href="#create_vscode_settings-214"><span class="linenos">214</span></a><span class="k">def</span> <span class="nf">create_vscode_settings</span><span class="p">(</span><span class="n">targetdir</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">):</span>
-</span><span id="create_vscode_settings-215"><a href="#create_vscode_settings-215"><span class="linenos">215</span></a>    <span class="sd">&quot;&quot;&quot;Add `settings.json` to `./.vscode`&quot;&quot;&quot;</span>
-</span><span id="create_vscode_settings-216"><a href="#create_vscode_settings-216"><span class="linenos">216</span></a>    <span class="n">vsdir</span> <span class="o">=</span> <span class="n">targetdir</span> <span class="o">/</span> <span class="s2">&quot;.vscode&quot;</span>
-</span><span id="create_vscode_settings-217"><a href="#create_vscode_settings-217"><span class="linenos">217</span></a>    <span class="n">vsdir</span><span class="o">.</span><span class="n">mkdir</span><span class="p">(</span><span class="n">parents</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">exist_ok</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
-</span><span id="create_vscode_settings-218"><a href="#create_vscode_settings-218"><span class="linenos">218</span></a>    <span class="p">(</span><span class="n">root</span> <span class="o">/</span> <span class="s2">&quot;.vscode_template&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">copy</span><span class="p">(</span><span class="n">vsdir</span> <span class="o">/</span> <span class="s2">&quot;settings.json&quot;</span><span class="p">,</span> <span class="kc">True</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="create_vscode_settings-215"><a href="#create_vscode_settings-215"><span class="linenos">215</span></a><span class="k">def</span> <span class="nf">create_vscode_settings</span><span class="p">(</span><span class="n">targetdir</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">):</span>
+</span><span id="create_vscode_settings-216"><a href="#create_vscode_settings-216"><span class="linenos">216</span></a>    <span class="sd">&quot;&quot;&quot;Add `settings.json` to `./.vscode`&quot;&quot;&quot;</span>
+</span><span id="create_vscode_settings-217"><a href="#create_vscode_settings-217"><span class="linenos">217</span></a>    <span class="n">vsdir</span> <span class="o">=</span> <span class="n">targetdir</span> <span class="o">/</span> <span class="s2">&quot;.vscode&quot;</span>
+</span><span id="create_vscode_settings-218"><a href="#create_vscode_settings-218"><span class="linenos">218</span></a>    <span class="n">vsdir</span><span class="o">.</span><span class="n">mkdir</span><span class="p">(</span><span class="n">parents</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">exist_ok</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
+</span><span id="create_vscode_settings-219"><a href="#create_vscode_settings-219"><span class="linenos">219</span></a>    <span class="p">(</span><span class="n">root</span> <span class="o">/</span> <span class="s2">&quot;.vscode_template&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">copy</span><span class="p">(</span><span class="n">vsdir</span> <span class="o">/</span> <span class="s2">&quot;settings.json&quot;</span><span class="p">,</span> <span class="kc">True</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Add <code>settings.json</code> to <code>./.vscode</code></p>
 </div>
 
 
@@ -735,59 +736,59 @@
         <span class="def">def</span>
         <span class="name">main</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">args</span><span class="p">:</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span> <span class="o">=</span> <span class="kc">None</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="main-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#main"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="main-221"><a href="#main-221"><span class="linenos">221</span></a><span class="k">def</span> <span class="nf">main</span><span class="p">(</span><span class="n">args</span><span class="p">:</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span> <span class="o">=</span> <span class="kc">None</span><span class="p">):</span>
-</span><span id="main-222"><a href="#main-222"><span class="linenos">222</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="p">:</span>
-</span><span id="main-223"><a href="#main-223"><span class="linenos">223</span></a>        <span class="n">args</span> <span class="o">=</span> <span class="n">get_args</span><span class="p">()</span>
-</span><span id="main-224"><a href="#main-224"><span class="linenos">224</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">not_package</span><span class="p">:</span>
-</span><span id="main-225"><a href="#main-225"><span class="linenos">225</span></a>        <span class="k">try</span><span class="p">:</span>
-</span><span id="main-226"><a href="#main-226"><span class="linenos">226</span></a>            <span class="k">if</span> <span class="n">check_pypi_for_name</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="p">):</span>
-</span><span id="main-227"><a href="#main-227"><span class="linenos">227</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="si">}</span><span class="s2"> already exists on pypi.org&quot;</span><span class="p">)</span>
-</span><span id="main-228"><a href="#main-228"><span class="linenos">228</span></a>                <span class="k">if</span> <span class="ow">not</span> <span class="n">get_answer</span><span class="p">(</span><span class="s2">&quot;Continue anyway?&quot;</span><span class="p">):</span>
-</span><span id="main-229"><a href="#main-229"><span class="linenos">229</span></a>                    <span class="n">sys</span><span class="o">.</span><span class="n">exit</span><span class="p">(</span><span class="mi">0</span><span class="p">)</span>
-</span><span id="main-230"><a href="#main-230"><span class="linenos">230</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
-</span><span id="main-231"><a href="#main-231"><span class="linenos">231</span></a>            <span class="nb">print</span><span class="p">(</span><span class="n">e</span><span class="p">)</span>
-</span><span id="main-232"><a href="#main-232"><span class="linenos">232</span></a>            <span class="nb">print</span><span class="p">(</span>
-</span><span id="main-233"><a href="#main-233"><span class="linenos">233</span></a>                <span class="sa">f</span><span class="s2">&quot;Couldn&#39;t verify that </span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="si">}</span><span class="s2"> doesn&#39;t already exist on pypi.org .&quot;</span>
-</span><span id="main-234"><a href="#main-234"><span class="linenos">234</span></a>            <span class="p">)</span>
-</span><span id="main-235"><a href="#main-235"><span class="linenos">235</span></a>            <span class="k">if</span> <span class="ow">not</span> <span class="n">get_answer</span><span class="p">(</span><span class="s2">&quot;Continue anyway?&quot;</span><span class="p">):</span>
-</span><span id="main-236"><a href="#main-236"><span class="linenos">236</span></a>                <span class="n">sys</span><span class="o">.</span><span class="n">exit</span><span class="p">(</span><span class="mi">0</span><span class="p">)</span>
-</span><span id="main-237"><a href="#main-237"><span class="linenos">237</span></a>    <span class="k">try</span><span class="p">:</span>
-</span><span id="main-238"><a href="#main-238"><span class="linenos">238</span></a>        <span class="n">targetdir</span><span class="p">:</span> <span class="n">Pathier</span> <span class="o">=</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span> <span class="o">/</span> <span class="n">args</span><span class="o">.</span><span class="n">name</span>
-</span><span id="main-239"><a href="#main-239"><span class="linenos">239</span></a>        <span class="k">try</span><span class="p">:</span>
-</span><span id="main-240"><a href="#main-240"><span class="linenos">240</span></a>            <span class="n">targetdir</span><span class="o">.</span><span class="n">mkdir</span><span class="p">(</span><span class="n">parents</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">exist_ok</span><span class="o">=</span><span class="kc">False</span><span class="p">)</span>
-</span><span id="main-241"><a href="#main-241"><span class="linenos">241</span></a>        <span class="k">except</span><span class="p">:</span>
-</span><span id="main-242"><a href="#main-242"><span class="linenos">242</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">targetdir</span><span class="si">}</span><span class="s2"> already exists.&quot;</span><span class="p">)</span>
-</span><span id="main-243"><a href="#main-243"><span class="linenos">243</span></a>            <span class="k">if</span> <span class="ow">not</span> <span class="n">get_answer</span><span class="p">(</span><span class="s2">&quot;Overwrite?&quot;</span><span class="p">):</span>
-</span><span id="main-244"><a href="#main-244"><span class="linenos">244</span></a>                <span class="n">sys</span><span class="o">.</span><span class="n">exit</span><span class="p">(</span><span class="mi">0</span><span class="p">)</span>
-</span><span id="main-245"><a href="#main-245"><span class="linenos">245</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">not_package</span><span class="p">:</span>
-</span><span id="main-246"><a href="#main-246"><span class="linenos">246</span></a>            <span class="n">create_pyproject_file</span><span class="p">(</span><span class="n">targetdir</span><span class="p">,</span> <span class="n">args</span><span class="p">)</span>
-</span><span id="main-247"><a href="#main-247"><span class="linenos">247</span></a>        <span class="n">create_source_files</span><span class="p">(</span>
-</span><span id="main-248"><a href="#main-248"><span class="linenos">248</span></a>            <span class="n">targetdir</span> <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">not_package</span> <span class="k">else</span> <span class="p">(</span><span class="n">targetdir</span> <span class="o">/</span> <span class="s2">&quot;src&quot;</span> <span class="o">/</span> <span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="p">),</span>
-</span><span id="main-249"><a href="#main-249"><span class="linenos">249</span></a>            <span class="n">args</span><span class="o">.</span><span class="n">source_files</span><span class="p">[</span><span class="mi">1</span><span class="p">:]</span> <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">not_package</span> <span class="k">else</span> <span class="n">args</span><span class="o">.</span><span class="n">source_files</span><span class="p">,</span>
-</span><span id="main-250"><a href="#main-250"><span class="linenos">250</span></a>        <span class="p">)</span>
-</span><span id="main-251"><a href="#main-251"><span class="linenos">251</span></a>        <span class="n">create_readme</span><span class="p">(</span><span class="n">targetdir</span><span class="p">,</span> <span class="n">args</span><span class="p">)</span>
-</span><span id="main-252"><a href="#main-252"><span class="linenos">252</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">not_package</span><span class="p">:</span>
-</span><span id="main-253"><a href="#main-253"><span class="linenos">253</span></a>            <span class="n">generate_test_files</span><span class="p">(</span><span class="n">targetdir</span><span class="p">)</span>
-</span><span id="main-254"><a href="#main-254"><span class="linenos">254</span></a>            <span class="n">create_vscode_settings</span><span class="p">(</span><span class="n">targetdir</span><span class="p">)</span>
-</span><span id="main-255"><a href="#main-255"><span class="linenos">255</span></a>        <span class="n">create_gitignore</span><span class="p">(</span><span class="n">targetdir</span><span class="p">)</span>
-</span><span id="main-256"><a href="#main-256"><span class="linenos">256</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">no_license</span><span class="p">:</span>
-</span><span id="main-257"><a href="#main-257"><span class="linenos">257</span></a>            <span class="n">create_license</span><span class="p">(</span><span class="n">targetdir</span><span class="p">)</span>
-</span><span id="main-258"><a href="#main-258"><span class="linenos">258</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">chdir</span><span class="p">(</span><span class="n">targetdir</span><span class="p">)</span>
-</span><span id="main-259"><a href="#main-259"><span class="linenos">259</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="s2">&quot;git init -b main&quot;</span><span class="p">)</span>
-</span><span id="main-260"><a href="#main-260"><span class="linenos">260</span></a>
-</span><span id="main-261"><a href="#main-261"><span class="linenos">261</span></a>    <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
-</span><span id="main-262"><a href="#main-262"><span class="linenos">262</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="s2">&quot;Aborting new package creation&quot;</span> <span class="ow">in</span> <span class="nb">str</span><span class="p">(</span><span class="n">e</span><span class="p">):</span>
-</span><span id="main-263"><a href="#main-263"><span class="linenos">263</span></a>            <span class="nb">print</span><span class="p">(</span><span class="n">e</span><span class="p">)</span>
-</span><span id="main-264"><a href="#main-264"><span class="linenos">264</span></a>        <span class="k">if</span> <span class="n">get_answer</span><span class="p">(</span><span class="s2">&quot;Delete created files?&quot;</span><span class="p">):</span>
-</span><span id="main-265"><a href="#main-265"><span class="linenos">265</span></a>            <span class="n">targetdir</span><span class="o">.</span><span class="n">delete</span><span class="p">()</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="main-222"><a href="#main-222"><span class="linenos">222</span></a><span class="k">def</span> <span class="nf">main</span><span class="p">(</span><span class="n">args</span><span class="p">:</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span> <span class="o">=</span> <span class="kc">None</span><span class="p">):</span>
+</span><span id="main-223"><a href="#main-223"><span class="linenos">223</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="p">:</span>
+</span><span id="main-224"><a href="#main-224"><span class="linenos">224</span></a>        <span class="n">args</span> <span class="o">=</span> <span class="n">get_args</span><span class="p">()</span>
+</span><span id="main-225"><a href="#main-225"><span class="linenos">225</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">not_package</span><span class="p">:</span>
+</span><span id="main-226"><a href="#main-226"><span class="linenos">226</span></a>        <span class="k">try</span><span class="p">:</span>
+</span><span id="main-227"><a href="#main-227"><span class="linenos">227</span></a>            <span class="k">if</span> <span class="n">check_pypi_for_name</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="p">):</span>
+</span><span id="main-228"><a href="#main-228"><span class="linenos">228</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="si">}</span><span class="s2"> already exists on pypi.org&quot;</span><span class="p">)</span>
+</span><span id="main-229"><a href="#main-229"><span class="linenos">229</span></a>                <span class="k">if</span> <span class="ow">not</span> <span class="n">get_answer</span><span class="p">(</span><span class="s2">&quot;Continue anyway?&quot;</span><span class="p">):</span>
+</span><span id="main-230"><a href="#main-230"><span class="linenos">230</span></a>                    <span class="n">sys</span><span class="o">.</span><span class="n">exit</span><span class="p">(</span><span class="mi">0</span><span class="p">)</span>
+</span><span id="main-231"><a href="#main-231"><span class="linenos">231</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="main-232"><a href="#main-232"><span class="linenos">232</span></a>            <span class="nb">print</span><span class="p">(</span><span class="n">e</span><span class="p">)</span>
+</span><span id="main-233"><a href="#main-233"><span class="linenos">233</span></a>            <span class="nb">print</span><span class="p">(</span>
+</span><span id="main-234"><a href="#main-234"><span class="linenos">234</span></a>                <span class="sa">f</span><span class="s2">&quot;Couldn&#39;t verify that </span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="si">}</span><span class="s2"> doesn&#39;t already exist on pypi.org .&quot;</span>
+</span><span id="main-235"><a href="#main-235"><span class="linenos">235</span></a>            <span class="p">)</span>
+</span><span id="main-236"><a href="#main-236"><span class="linenos">236</span></a>            <span class="k">if</span> <span class="ow">not</span> <span class="n">get_answer</span><span class="p">(</span><span class="s2">&quot;Continue anyway?&quot;</span><span class="p">):</span>
+</span><span id="main-237"><a href="#main-237"><span class="linenos">237</span></a>                <span class="n">sys</span><span class="o">.</span><span class="n">exit</span><span class="p">(</span><span class="mi">0</span><span class="p">)</span>
+</span><span id="main-238"><a href="#main-238"><span class="linenos">238</span></a>    <span class="k">try</span><span class="p">:</span>
+</span><span id="main-239"><a href="#main-239"><span class="linenos">239</span></a>        <span class="n">targetdir</span><span class="p">:</span> <span class="n">Pathier</span> <span class="o">=</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span> <span class="o">/</span> <span class="n">args</span><span class="o">.</span><span class="n">name</span>
+</span><span id="main-240"><a href="#main-240"><span class="linenos">240</span></a>        <span class="k">try</span><span class="p">:</span>
+</span><span id="main-241"><a href="#main-241"><span class="linenos">241</span></a>            <span class="n">targetdir</span><span class="o">.</span><span class="n">mkdir</span><span class="p">(</span><span class="n">parents</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">exist_ok</span><span class="o">=</span><span class="kc">False</span><span class="p">)</span>
+</span><span id="main-242"><a href="#main-242"><span class="linenos">242</span></a>        <span class="k">except</span><span class="p">:</span>
+</span><span id="main-243"><a href="#main-243"><span class="linenos">243</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">targetdir</span><span class="si">}</span><span class="s2"> already exists.&quot;</span><span class="p">)</span>
+</span><span id="main-244"><a href="#main-244"><span class="linenos">244</span></a>            <span class="k">if</span> <span class="ow">not</span> <span class="n">get_answer</span><span class="p">(</span><span class="s2">&quot;Overwrite?&quot;</span><span class="p">):</span>
+</span><span id="main-245"><a href="#main-245"><span class="linenos">245</span></a>                <span class="n">sys</span><span class="o">.</span><span class="n">exit</span><span class="p">(</span><span class="mi">0</span><span class="p">)</span>
+</span><span id="main-246"><a href="#main-246"><span class="linenos">246</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">not_package</span><span class="p">:</span>
+</span><span id="main-247"><a href="#main-247"><span class="linenos">247</span></a>            <span class="n">create_pyproject_file</span><span class="p">(</span><span class="n">targetdir</span><span class="p">,</span> <span class="n">args</span><span class="p">)</span>
+</span><span id="main-248"><a href="#main-248"><span class="linenos">248</span></a>        <span class="n">create_source_files</span><span class="p">(</span>
+</span><span id="main-249"><a href="#main-249"><span class="linenos">249</span></a>            <span class="n">targetdir</span> <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">not_package</span> <span class="k">else</span> <span class="p">(</span><span class="n">targetdir</span> <span class="o">/</span> <span class="s2">&quot;src&quot;</span> <span class="o">/</span> <span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="p">),</span>
+</span><span id="main-250"><a href="#main-250"><span class="linenos">250</span></a>            <span class="n">args</span><span class="o">.</span><span class="n">source_files</span><span class="p">[</span><span class="mi">1</span><span class="p">:]</span> <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">not_package</span> <span class="k">else</span> <span class="n">args</span><span class="o">.</span><span class="n">source_files</span><span class="p">,</span>
+</span><span id="main-251"><a href="#main-251"><span class="linenos">251</span></a>        <span class="p">)</span>
+</span><span id="main-252"><a href="#main-252"><span class="linenos">252</span></a>        <span class="n">create_readme</span><span class="p">(</span><span class="n">targetdir</span><span class="p">,</span> <span class="n">args</span><span class="p">)</span>
+</span><span id="main-253"><a href="#main-253"><span class="linenos">253</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">not_package</span><span class="p">:</span>
+</span><span id="main-254"><a href="#main-254"><span class="linenos">254</span></a>            <span class="n">generate_test_files</span><span class="p">(</span><span class="n">targetdir</span><span class="p">)</span>
+</span><span id="main-255"><a href="#main-255"><span class="linenos">255</span></a>            <span class="n">create_vscode_settings</span><span class="p">(</span><span class="n">targetdir</span><span class="p">)</span>
+</span><span id="main-256"><a href="#main-256"><span class="linenos">256</span></a>        <span class="n">create_gitignore</span><span class="p">(</span><span class="n">targetdir</span><span class="p">)</span>
+</span><span id="main-257"><a href="#main-257"><span class="linenos">257</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">no_license</span><span class="p">:</span>
+</span><span id="main-258"><a href="#main-258"><span class="linenos">258</span></a>            <span class="n">create_license</span><span class="p">(</span><span class="n">targetdir</span><span class="p">)</span>
+</span><span id="main-259"><a href="#main-259"><span class="linenos">259</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">chdir</span><span class="p">(</span><span class="n">targetdir</span><span class="p">)</span>
+</span><span id="main-260"><a href="#main-260"><span class="linenos">260</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">new_repo</span><span class="p">()</span>
+</span><span id="main-261"><a href="#main-261"><span class="linenos">261</span></a>
+</span><span id="main-262"><a href="#main-262"><span class="linenos">262</span></a>    <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="main-263"><a href="#main-263"><span class="linenos">263</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="s2">&quot;Aborting new package creation&quot;</span> <span class="ow">in</span> <span class="nb">str</span><span class="p">(</span><span class="n">e</span><span class="p">):</span>
+</span><span id="main-264"><a href="#main-264"><span class="linenos">264</span></a>            <span class="nb">print</span><span class="p">(</span><span class="n">e</span><span class="p">)</span>
+</span><span id="main-265"><a href="#main-265"><span class="linenos">265</span></a>        <span class="k">if</span> <span class="n">get_answer</span><span class="p">(</span><span class="s2">&quot;Delete created files?&quot;</span><span class="p">):</span>
+</span><span id="main-266"><a href="#main-266"><span class="linenos">266</span></a>            <span class="n">targetdir</span><span class="o">.</span><span class="n">delete</span><span class="p">()</span>
 </span></pre></div>
 
 
     
 
                 </section>
     </main>
```

#### html2text {}

```diff
@@ -21,296 +21,23 @@
 __1import argparse
 __2import os
 __3import sys
 __4from datetime import datetime
 __5
 __6import requests
 __7from bs4 import BeautifulSoup
-__8from pathier import Pathier
-__9
-_10import hassle.hassle_config as hassle_config
-_11from hassle.generate_tests import generate_test_files
-_12
-_13root = Pathier(__file__).parent
-_14
+__8from gitbetter import git
+__9from pathier import Pathier
+_10
+_11import hassle.hassle_config as hassle_config
+_12from hassle.generate_tests import generate_test_files
+_13
+_14root = Pathier(__file__).parent
 _15
-_16def get_args() -> argparse.Namespace:
-_17    parser = argparse.ArgumentParser()
-_18
-_19    parser.add_argument(
-_20        "name",
-_21        type=str,
-_22        help=""" Name of the package to create in the current working
-directory. """,
-_23    )
-_24
-_25    parser.add_argument(
-_26        "-s",
-_27        "--source_files",
-_28        nargs="*",
-_29        type=str,
-_30        default=[],
-_31        help=""" List of additional source files to create in addition to
-the default
-_32        __init__.py and {name}.py files.""",
-_33    )
-_34
-_35    parser.add_argument(
-_36        "-d",
-_37        "--description",
-_38        type=str,
-_39        default="",
-_40        help=""" The package description to be added to the pyproject.toml
-file. """,
-_41    )
-_42
-_43    parser.add_argument(
-_44        "-dp",
-_45        "--dependencies",
-_46        nargs="*",
-_47        type=str,
-_48        default=[],
-_49        help=""" List of dependencies to add to pyproject.toml.
-_50        Note: hassle.py will automatically scan your project for 3rd party
-_51        imports and update pyproject.toml. This switch is largely useful
-_52        for adding dependencies your project might need, but doesn't
-_53        directly import in any source files,
-_54        like an os.system() call that invokes a 3rd party cli.""",
-_55    )
-_56
-_57    parser.add_argument(
-_58        "-k",
-_59        "--keywords",
-_60        nargs="*",
-_61        type=str,
-_62        default=[],
-_63        help=""" List of keywords to be added to the keywords field in
-pyproject.toml. """,
-_64    )
-_65
-_66    parser.add_argument(
-_67        "-as",
-_68        "--add_script",
-_69        action="store_true",
-_70        help=""" Add section to pyproject.toml declaring the package
-_71        should be installed with command line scripts added.
-_72        The default is '{name} = "{name}.{name}:main".
-_73        You will need to manually change this field.""",
-_74    )
-_75
-_76    parser.add_argument(
-_77        "-nl",
-_78        "--no_license",
-_79        action="store_true",
-_80        help=""" By default, projects are created with an MIT license.
-_81        Set this flag to avoid adding a license if you want to configure
-licensing
-_82        at another time.""",
-_83    )
-_84
-_85    parser.add_argument(
-_86        "-os",
-_87        "--operating_system",
-_88        type=str,
-_89        default=None,
-_90        nargs="*",
-_91        help=""" List of operating systems this package will be compatible
-with.
-_92        The default is OS Independent.
-_93        This only affects the 'classifiers' field of pyproject.toml .""",
-_94    )
-_95
-_96    parser.add_argument(
-_97        "-np",
-_98        "--not_package",
-_99        action="store_true",
-100        help=""" Put source files in top level directory and delete tests
-folder. """,
-101    )
-102
-103    args = parser.parse_args()
-104    args.source_files.extend(["__init__.py", f"{args.name}.py"])
-105
-106    return args
-107
-108
-109def get_answer(question: str) -> bool:
-110    """Repeatedly ask the user a yes/no question until a 'y' or a 'n' is
-received."""
-111    ans = ""
-112    question = question.strip()
-113    if "?" not in question:
-114        question += "?"
-115    question += " (y/n): "
-116    while ans not in ["y", "yes", "no", "n"]:
-117        ans = input(question).strip().lower()
-118        if ans in ["y", "yes"]:
-119            return True
-120        elif ans in ["n", "no"]:
-121            return False
-122        else:
-123            print("Invalid answer.")
-124
-125
-126def check_pypi_for_name(package_name: str) -> bool:
-127    """Check if a package with package_name already exists on `pypi.org`.
-128    Returns `True` if package name exists.
-129    Only checks the first page of results."""
-130    url = f"https://pypi.org/search/?q={package_name.lower()}"
-131    response = requests.get(url)
-132    if response.status_code != 200:
-133        raise RuntimeError(
-134            f"Error: pypi.org returned status code: {response.status_code}"
-135        )
-136    soup = BeautifulSoup(response.text, "html.parser")
-137    pypi_packages = [
-138        span.text.lower()
-139        for span in soup.find_all("span", class_="package-snippet__name")
-140    ]
-141    return package_name in pypi_packages
-142
-143
-144def check_pypi_for_name_cli():
-145    parser = argparse.ArgumentParser()
-146    parser.add_argument("name", type=str)
-147    args = parser.parse_args()
-148    if check_pypi_for_name(args.name):
-149        print(f"{args.name} is already taken.")
-150    else:
-151        print(f"{args.name} is available.")
-152
-153
-154def create_pyproject_file(targetdir: Pathier, args: argparse.Namespace):
-155    """Create `pyproject.toml` in `./{project_name}` from args,
-pyproject_template, and hassle_config."""
-156    pyproject = (root / "pyproject_template.toml").loads()
-157    if not hassle_config.config_exists():
-158        hassle_config.warn()
-159        if not get_answer("Continue creating new package with blank
-config?"):
-160            raise Exception("Aborting new package creation")
-161        else:
-162            print("Creating blank hassle_config.toml...")
-163            hassle_config.create_config()
-164    config = hassle_config.load_config()
-165    pyproject["project"]["name"] = args.name
-166    pyproject["project"]["authors"] = config["authors"]
-167    pyproject["project"]["description"] = args.description
-168    pyproject["project"]["dependencies"] = args.dependencies
-169    pyproject["project"]["keywords"] = args.keywords
-170    if args.operating_system:
-171        pyproject["project"]["classifiers"][2] = "Operating System :: " + "
-".join(
-172            args.operating_system
-173        )
-174    if args.no_license:
-175        pyproject["project"]["classifiers"].pop(1)
-176    for field in config["project_urls"]:
-177        pyproject["project"]["urls"][field] = config["project_urls"]
-[field].replace(
-178            "$name", args.name
-179        )
-180    if args.add_script:
-181        pyproject["project"]["scripts"][args.name] = f"{args.name}.
-{args.name}:main"
-182    (targetdir / "pyproject.toml").dumps(pyproject)
-183
-184
-185def create_source_files(srcdir: Pathier, filelist: list[str]):
-186    """Generate empty source files in `./{package_name}/src/{package_name}/
-`"""
-187    srcdir.mkdir(parents=True, exist_ok=True)
-188    for file in filelist:
-189        (srcdir / file).touch()
-190
-191
-192def create_readme(targetdir: Pathier, args: argparse.Namespace):
-193    """Create `README.md` in `./{package_name}` from readme_template and
-args."""
-194    readme = (root / "README_template.md").read_text()
-195    readme = readme.replace("$name", args.name).replace(
-196        "$description", args.description
-197    )
-198    (targetdir / "README.md").write_text(readme)
-199
-200
-201def create_license(targetdir: Pathier):
-202    """Add MIT license file to `./{package_name}`."""
-203    license_template = (root / "license_template.txt").read_text()
-204    license_template = license_template.replace("$year", str(datetime.now
-().year))
-205    (targetdir / "LICENSE.txt").write_text(license_template)
-206
-207
-208def create_gitignore(targetdir: Pathier):
-209    """Add `.gitignore` to `./{package_name}`"""
-210    (root / ".gitignore_template").copy(targetdir / ".gitignore", True)
-211
-212
-213def create_vscode_settings(targetdir: Pathier):
-214    """Add `settings.json` to `./.vscode`"""
-215    vsdir = targetdir / ".vscode"
-216    vsdir.mkdir(parents=True, exist_ok=True)
-217    (root / ".vscode_template").copy(vsdir / "settings.json", True)
-218
-219
-220def main(args: argparse.Namespace = None):
-221    if not args:
-222        args = get_args()
-223    if not args.not_package:
-224        try:
-225            if check_pypi_for_name(args.name):
-226                print(f"{args.name} already exists on pypi.org")
-227                if not get_answer("Continue anyway?"):
-228                    sys.exit(0)
-229        except Exception as e:
-230            print(e)
-231            print(
-232                f"Couldn't verify that {args.name} doesn't already exist on
-pypi.org ."
-233            )
-234            if not get_answer("Continue anyway?"):
-235                sys.exit(0)
-236    try:
-237        targetdir: Pathier = Pathier.cwd() / args.name
-238        try:
-239            targetdir.mkdir(parents=True, exist_ok=False)
-240        except:
-241            print(f"{targetdir} already exists.")
-242            if not get_answer("Overwrite?"):
-243                sys.exit(0)
-244        if not args.not_package:
-245            create_pyproject_file(targetdir, args)
-246        create_source_files(
-247            targetdir if args.not_package else (targetdir / "src" /
-args.name),
-248            args.source_files[1:] if args.not_package else
-args.source_files,
-249        )
-250        create_readme(targetdir, args)
-251        if not args.not_package:
-252            generate_test_files(targetdir)
-253            create_vscode_settings(targetdir)
-254        create_gitignore(targetdir)
-255        if not args.no_license:
-256            create_license(targetdir)
-257        os.chdir(targetdir)
-258        os.system("git init -b main")
-259
-260    except Exception as e:
-261        if not "Aborting new package creation" in str(e):
-262            print(e)
-263        if get_answer("Delete created files?"):
-264            targetdir.delete()
-265
-266
-267if __name__ == "__main__":
-268    main(get_args())
-  ⁰
-def get_args() -> argparse.Namespace: View Source
+_16
 _17def get_args() -> argparse.Namespace:
 _18    parser = argparse.ArgumentParser()
 _19
 _20    parser.add_argument(
 _21        "name",
 _22        type=str,
 _23        help=""" Name of the package to create in the current working
@@ -401,16 +128,16 @@
 folder. """,
 102    )
 103
 104    args = parser.parse_args()
 105    args.source_files.extend(["__init__.py", f"{args.name}.py"])
 106
 107    return args
-  ⁰
-def get_answer(question: str) -> bool: View Source
+108
+109
 110def get_answer(question: str) -> bool:
 111    """Repeatedly ask the user a yes/no question until a 'y' or a 'n' is
 received."""
 112    ans = ""
 113    question = question.strip()
 114    if "?" not in question:
 115        question += "?"
@@ -419,17 +146,16 @@
 118        ans = input(question).strip().lower()
 119        if ans in ["y", "yes"]:
 120            return True
 121        elif ans in ["n", "no"]:
 122            return False
 123        else:
 124            print("Invalid answer.")
-Repeatedly ask the user a yes/no question until a 'y' or a 'n' is received.
-  ⁰
-def check_pypi_for_name(package_name: str) -> bool: View Source
+125
+126
 127def check_pypi_for_name(package_name: str) -> bool:
 128    """Check if a package with package_name already exists on `pypi.org`.
 129    Returns `True` if package name exists.
 130    Only checks the first page of results."""
 131    url = f"https://pypi.org/search/?q={package_name.lower()}"
 132    response = requests.get(url)
 133    if response.status_code != 200:
@@ -438,29 +164,26 @@
 136        )
 137    soup = BeautifulSoup(response.text, "html.parser")
 138    pypi_packages = [
 139        span.text.lower()
 140        for span in soup.find_all("span", class_="package-snippet__name")
 141    ]
 142    return package_name in pypi_packages
-Check if a package with package_name already exists on pypi.org. Returns True
-if package name exists. Only checks the first page of results.
-  ⁰
-def check_pypi_for_name_cli(): View Source
+143
+144
 145def check_pypi_for_name_cli():
 146    parser = argparse.ArgumentParser()
 147    parser.add_argument("name", type=str)
 148    args = parser.parse_args()
 149    if check_pypi_for_name(args.name):
 150        print(f"{args.name} is already taken.")
 151    else:
 152        print(f"{args.name} is available.")
-  ⁰
-def create_pyproject_file(targetdir: pathier.pathier.Pathier, args:
-argparse.Namespace): View Source
+153
+154
 155def create_pyproject_file(targetdir: Pathier, args: argparse.Namespace):
 156    """Create `pyproject.toml` in `./{project_name}` from args,
 pyproject_template, and hassle_config."""
 157    pyproject = (root / "pyproject_template.toml").loads()
 158    if not hassle_config.config_exists():
 159        hassle_config.warn()
 160        if not get_answer("Continue creating new package with blank
@@ -487,63 +210,54 @@
 [field].replace(
 179            "$name", args.name
 180        )
 181    if args.add_script:
 182        pyproject["project"]["scripts"][args.name] = f"{args.name}.
 {args.name}:main"
 183    (targetdir / "pyproject.toml").dumps(pyproject)
-Create pyproject.toml in ./{project_name} from args, pyproject_template, and
-hassle_config.
-  ⁰
-def create_source_files(srcdir: pathier.pathier.Pathier, filelist: list[str]):
-View Source
+184
+185
 186def create_source_files(srcdir: Pathier, filelist: list[str]):
 187    """Generate empty source files in `./{package_name}/src/{package_name}/
 `"""
 188    srcdir.mkdir(parents=True, exist_ok=True)
 189    for file in filelist:
 190        (srcdir / file).touch()
-Generate empty source files in ./{package_name}/src/{package_name}/
-  ⁰
-def create_readme(targetdir: pathier.pathier.Pathier, args:
-argparse.Namespace): View Source
+191
+192
 193def create_readme(targetdir: Pathier, args: argparse.Namespace):
 194    """Create `README.md` in `./{package_name}` from readme_template and
 args."""
 195    readme = (root / "README_template.md").read_text()
 196    readme = readme.replace("$name", args.name).replace(
 197        "$description", args.description
 198    )
 199    (targetdir / "README.md").write_text(readme)
-Create README.md in ./{package_name} from readme_template and args.
-  ⁰
-def create_license(targetdir: pathier.pathier.Pathier): View Source
+200
+201
 202def create_license(targetdir: Pathier):
 203    """Add MIT license file to `./{package_name}`."""
 204    license_template = (root / "license_template.txt").read_text()
 205    license_template = license_template.replace("$year", str(datetime.now
 ().year))
 206    (targetdir / "LICENSE.txt").write_text(license_template)
-Add MIT license file to ./{package_name}.
-  ⁰
-def create_gitignore(targetdir: pathier.pathier.Pathier): View Source
+207
+208
 209def create_gitignore(targetdir: Pathier):
 210    """Add `.gitignore` to `./{package_name}`"""
 211    (root / ".gitignore_template").copy(targetdir / ".gitignore", True)
-Add .gitignore to ./{package_name}
-  ⁰
-def create_vscode_settings(targetdir: pathier.pathier.Pathier): View Source
+212
+213
 214def create_vscode_settings(targetdir: Pathier):
 215    """Add `settings.json` to `./.vscode`"""
 216    vsdir = targetdir / ".vscode"
 217    vsdir.mkdir(parents=True, exist_ok=True)
 218    (root / ".vscode_template").copy(vsdir / "settings.json", True)
-Add settings.json to ./.vscode
-  ⁰
-def main(args: argparse.Namespace = None): View Source
+219
+220
 221def main(args: argparse.Namespace = None):
 222    if not args:
 223        args = get_args()
 224    if not args.not_package:
 225        try:
 226            if check_pypi_for_name(args.name):
 227                print(f"{args.name} already exists on pypi.org")
@@ -577,15 +291,302 @@
 252        if not args.not_package:
 253            generate_test_files(targetdir)
 254            create_vscode_settings(targetdir)
 255        create_gitignore(targetdir)
 256        if not args.no_license:
 257            create_license(targetdir)
 258        os.chdir(targetdir)
-259        os.system("git init -b main")
+259        git.new_repo()
 260
 261    except Exception as e:
 262        if not "Aborting new package creation" in str(e):
 263            print(e)
 264        if get_answer("Delete created files?"):
 265            targetdir.delete()
+266
+267
+268if __name__ == "__main__":
+269    main(get_args())
+  ⁰
+def get_args() -> argparse.Namespace: View Source
+_18def get_args() -> argparse.Namespace:
+_19    parser = argparse.ArgumentParser()
+_20
+_21    parser.add_argument(
+_22        "name",
+_23        type=str,
+_24        help=""" Name of the package to create in the current working
+directory. """,
+_25    )
+_26
+_27    parser.add_argument(
+_28        "-s",
+_29        "--source_files",
+_30        nargs="*",
+_31        type=str,
+_32        default=[],
+_33        help=""" List of additional source files to create in addition to
+the default
+_34        __init__.py and {name}.py files.""",
+_35    )
+_36
+_37    parser.add_argument(
+_38        "-d",
+_39        "--description",
+_40        type=str,
+_41        default="",
+_42        help=""" The package description to be added to the pyproject.toml
+file. """,
+_43    )
+_44
+_45    parser.add_argument(
+_46        "-dp",
+_47        "--dependencies",
+_48        nargs="*",
+_49        type=str,
+_50        default=[],
+_51        help=""" List of dependencies to add to pyproject.toml.
+_52        Note: hassle.py will automatically scan your project for 3rd party
+_53        imports and update pyproject.toml. This switch is largely useful
+_54        for adding dependencies your project might need, but doesn't
+_55        directly import in any source files,
+_56        like an os.system() call that invokes a 3rd party cli.""",
+_57    )
+_58
+_59    parser.add_argument(
+_60        "-k",
+_61        "--keywords",
+_62        nargs="*",
+_63        type=str,
+_64        default=[],
+_65        help=""" List of keywords to be added to the keywords field in
+pyproject.toml. """,
+_66    )
+_67
+_68    parser.add_argument(
+_69        "-as",
+_70        "--add_script",
+_71        action="store_true",
+_72        help=""" Add section to pyproject.toml declaring the package
+_73        should be installed with command line scripts added.
+_74        The default is '{name} = "{name}.{name}:main".
+_75        You will need to manually change this field.""",
+_76    )
+_77
+_78    parser.add_argument(
+_79        "-nl",
+_80        "--no_license",
+_81        action="store_true",
+_82        help=""" By default, projects are created with an MIT license.
+_83        Set this flag to avoid adding a license if you want to configure
+licensing
+_84        at another time.""",
+_85    )
+_86
+_87    parser.add_argument(
+_88        "-os",
+_89        "--operating_system",
+_90        type=str,
+_91        default=None,
+_92        nargs="*",
+_93        help=""" List of operating systems this package will be compatible
+with.
+_94        The default is OS Independent.
+_95        This only affects the 'classifiers' field of pyproject.toml .""",
+_96    )
+_97
+_98    parser.add_argument(
+_99        "-np",
+100        "--not_package",
+101        action="store_true",
+102        help=""" Put source files in top level directory and delete tests
+folder. """,
+103    )
+104
+105    args = parser.parse_args()
+106    args.source_files.extend(["__init__.py", f"{args.name}.py"])
+107
+108    return args
+  ⁰
+def get_answer(question: str) -> bool: View Source
+111def get_answer(question: str) -> bool:
+112    """Repeatedly ask the user a yes/no question until a 'y' or a 'n' is
+received."""
+113    ans = ""
+114    question = question.strip()
+115    if "?" not in question:
+116        question += "?"
+117    question += " (y/n): "
+118    while ans not in ["y", "yes", "no", "n"]:
+119        ans = input(question).strip().lower()
+120        if ans in ["y", "yes"]:
+121            return True
+122        elif ans in ["n", "no"]:
+123            return False
+124        else:
+125            print("Invalid answer.")
+Repeatedly ask the user a yes/no question until a 'y' or a 'n' is received.
+  ⁰
+def check_pypi_for_name(package_name: str) -> bool: View Source
+128def check_pypi_for_name(package_name: str) -> bool:
+129    """Check if a package with package_name already exists on `pypi.org`.
+130    Returns `True` if package name exists.
+131    Only checks the first page of results."""
+132    url = f"https://pypi.org/search/?q={package_name.lower()}"
+133    response = requests.get(url)
+134    if response.status_code != 200:
+135        raise RuntimeError(
+136            f"Error: pypi.org returned status code: {response.status_code}"
+137        )
+138    soup = BeautifulSoup(response.text, "html.parser")
+139    pypi_packages = [
+140        span.text.lower()
+141        for span in soup.find_all("span", class_="package-snippet__name")
+142    ]
+143    return package_name in pypi_packages
+Check if a package with package_name already exists on pypi.org. Returns True
+if package name exists. Only checks the first page of results.
+  ⁰
+def check_pypi_for_name_cli(): View Source
+146def check_pypi_for_name_cli():
+147    parser = argparse.ArgumentParser()
+148    parser.add_argument("name", type=str)
+149    args = parser.parse_args()
+150    if check_pypi_for_name(args.name):
+151        print(f"{args.name} is already taken.")
+152    else:
+153        print(f"{args.name} is available.")
+  ⁰
+def create_pyproject_file(targetdir: pathier.pathier.Pathier, args:
+argparse.Namespace): View Source
+156def create_pyproject_file(targetdir: Pathier, args: argparse.Namespace):
+157    """Create `pyproject.toml` in `./{project_name}` from args,
+pyproject_template, and hassle_config."""
+158    pyproject = (root / "pyproject_template.toml").loads()
+159    if not hassle_config.config_exists():
+160        hassle_config.warn()
+161        if not get_answer("Continue creating new package with blank
+config?"):
+162            raise Exception("Aborting new package creation")
+163        else:
+164            print("Creating blank hassle_config.toml...")
+165            hassle_config.create_config()
+166    config = hassle_config.load_config()
+167    pyproject["project"]["name"] = args.name
+168    pyproject["project"]["authors"] = config["authors"]
+169    pyproject["project"]["description"] = args.description
+170    pyproject["project"]["dependencies"] = args.dependencies
+171    pyproject["project"]["keywords"] = args.keywords
+172    if args.operating_system:
+173        pyproject["project"]["classifiers"][2] = "Operating System :: " + "
+".join(
+174            args.operating_system
+175        )
+176    if args.no_license:
+177        pyproject["project"]["classifiers"].pop(1)
+178    for field in config["project_urls"]:
+179        pyproject["project"]["urls"][field] = config["project_urls"]
+[field].replace(
+180            "$name", args.name
+181        )
+182    if args.add_script:
+183        pyproject["project"]["scripts"][args.name] = f"{args.name}.
+{args.name}:main"
+184    (targetdir / "pyproject.toml").dumps(pyproject)
+Create pyproject.toml in ./{project_name} from args, pyproject_template, and
+hassle_config.
+  ⁰
+def create_source_files(srcdir: pathier.pathier.Pathier, filelist: list[str]):
+View Source
+187def create_source_files(srcdir: Pathier, filelist: list[str]):
+188    """Generate empty source files in `./{package_name}/src/{package_name}/
+`"""
+189    srcdir.mkdir(parents=True, exist_ok=True)
+190    for file in filelist:
+191        (srcdir / file).touch()
+Generate empty source files in ./{package_name}/src/{package_name}/
+  ⁰
+def create_readme(targetdir: pathier.pathier.Pathier, args:
+argparse.Namespace): View Source
+194def create_readme(targetdir: Pathier, args: argparse.Namespace):
+195    """Create `README.md` in `./{package_name}` from readme_template and
+args."""
+196    readme = (root / "README_template.md").read_text()
+197    readme = readme.replace("$name", args.name).replace(
+198        "$description", args.description
+199    )
+200    (targetdir / "README.md").write_text(readme)
+Create README.md in ./{package_name} from readme_template and args.
+  ⁰
+def create_license(targetdir: pathier.pathier.Pathier): View Source
+203def create_license(targetdir: Pathier):
+204    """Add MIT license file to `./{package_name}`."""
+205    license_template = (root / "license_template.txt").read_text()
+206    license_template = license_template.replace("$year", str(datetime.now
+().year))
+207    (targetdir / "LICENSE.txt").write_text(license_template)
+Add MIT license file to ./{package_name}.
+  ⁰
+def create_gitignore(targetdir: pathier.pathier.Pathier): View Source
+210def create_gitignore(targetdir: Pathier):
+211    """Add `.gitignore` to `./{package_name}`"""
+212    (root / ".gitignore_template").copy(targetdir / ".gitignore", True)
+Add .gitignore to ./{package_name}
+  ⁰
+def create_vscode_settings(targetdir: pathier.pathier.Pathier): View Source
+215def create_vscode_settings(targetdir: Pathier):
+216    """Add `settings.json` to `./.vscode`"""
+217    vsdir = targetdir / ".vscode"
+218    vsdir.mkdir(parents=True, exist_ok=True)
+219    (root / ".vscode_template").copy(vsdir / "settings.json", True)
+Add settings.json to ./.vscode
+  ⁰
+def main(args: argparse.Namespace = None): View Source
+222def main(args: argparse.Namespace = None):
+223    if not args:
+224        args = get_args()
+225    if not args.not_package:
+226        try:
+227            if check_pypi_for_name(args.name):
+228                print(f"{args.name} already exists on pypi.org")
+229                if not get_answer("Continue anyway?"):
+230                    sys.exit(0)
+231        except Exception as e:
+232            print(e)
+233            print(
+234                f"Couldn't verify that {args.name} doesn't already exist on
+pypi.org ."
+235            )
+236            if not get_answer("Continue anyway?"):
+237                sys.exit(0)
+238    try:
+239        targetdir: Pathier = Pathier.cwd() / args.name
+240        try:
+241            targetdir.mkdir(parents=True, exist_ok=False)
+242        except:
+243            print(f"{targetdir} already exists.")
+244            if not get_answer("Overwrite?"):
+245                sys.exit(0)
+246        if not args.not_package:
+247            create_pyproject_file(targetdir, args)
+248        create_source_files(
+249            targetdir if args.not_package else (targetdir / "src" /
+args.name),
+250            args.source_files[1:] if args.not_package else
+args.source_files,
+251        )
+252        create_readme(targetdir, args)
+253        if not args.not_package:
+254            generate_test_files(targetdir)
+255            create_vscode_settings(targetdir)
+256        create_gitignore(targetdir)
+257        if not args.no_license:
+258            create_license(targetdir)
+259        os.chdir(targetdir)
+260        git.new_repo()
+261
+262    except Exception as e:
+263        if not "Aborting new package creation" in str(e):
+264            print(e)
+265        if get_answer("Delete created files?"):
+266            targetdir.delete()
```

### Comparing `hassle-2.7.1/docs/hassle/run_tests.html` & `hassle-2.8.0/docs/hassle/run_tests.html`

 * *Files 6% similar despite different names*

```diff
@@ -59,55 +59,62 @@
                         <input id="mod-run_tests-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 
                         <label class="view-source-button" for="mod-run_tests-view-source"><span>View Source</span></label>
 
                         <div class="pdoc-code codehilite"><pre><span></span><span id="L-1"><a href="#L-1"><span class="linenos"> 1</span></a><span class="kn">import</span> <span class="nn">argparse</span>
 </span><span id="L-2"><a href="#L-2"><span class="linenos"> 2</span></a><span class="kn">import</span> <span class="nn">os</span>
 </span><span id="L-3"><a href="#L-3"><span class="linenos"> 3</span></a>
-</span><span id="L-4"><a href="#L-4"><span class="linenos"> 4</span></a><span class="kn">from</span> <span class="nn">pathier</span> <span class="kn">import</span> <span class="n">Pathier</span>
-</span><span id="L-5"><a href="#L-5"><span class="linenos"> 5</span></a>
-</span><span id="L-6"><a href="#L-6"><span class="linenos"> 6</span></a>
-</span><span id="L-7"><a href="#L-7"><span class="linenos"> 7</span></a><span class="k">def</span> <span class="nf">get_args</span><span class="p">()</span> <span class="o">-&gt;</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span><span class="p">:</span>
-</span><span id="L-8"><a href="#L-8"><span class="linenos"> 8</span></a>    <span class="n">parser</span> <span class="o">=</span> <span class="n">argparse</span><span class="o">.</span><span class="n">ArgumentParser</span><span class="p">()</span>
-</span><span id="L-9"><a href="#L-9"><span class="linenos"> 9</span></a>
-</span><span id="L-10"><a href="#L-10"><span class="linenos">10</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="L-11"><a href="#L-11"><span class="linenos">11</span></a>        <span class="s2">&quot;package_name&quot;</span><span class="p">,</span>
-</span><span id="L-12"><a href="#L-12"><span class="linenos">12</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
-</span><span id="L-13"><a href="#L-13"><span class="linenos">13</span></a>        <span class="n">default</span><span class="o">=</span><span class="s2">&quot;.&quot;</span><span class="p">,</span>
-</span><span id="L-14"><a href="#L-14"><span class="linenos">14</span></a>        <span class="n">nargs</span><span class="o">=</span><span class="s2">&quot;?&quot;</span><span class="p">,</span>
-</span><span id="L-15"><a href="#L-15"><span class="linenos">15</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; The name of the package or project to run tests for,</span>
-</span><span id="L-16"><a href="#L-16"><span class="linenos">16</span></a><span class="s2">        assuming it&#39;s a subfolder of your current working directory.</span>
-</span><span id="L-17"><a href="#L-17"><span class="linenos">17</span></a><span class="s2">        Can also be a full path to the package. If nothing is given,</span>
-</span><span id="L-18"><a href="#L-18"><span class="linenos">18</span></a><span class="s2">        the current working directory will be used.&quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="L-19"><a href="#L-19"><span class="linenos">19</span></a>    <span class="p">)</span>
-</span><span id="L-20"><a href="#L-20"><span class="linenos">20</span></a>
-</span><span id="L-21"><a href="#L-21"><span class="linenos">21</span></a>    <span class="n">args</span> <span class="o">=</span> <span class="n">parser</span><span class="o">.</span><span class="n">parse_args</span><span class="p">()</span>
+</span><span id="L-4"><a href="#L-4"><span class="linenos"> 4</span></a><span class="kn">import</span> <span class="nn">coverage</span>
+</span><span id="L-5"><a href="#L-5"><span class="linenos"> 5</span></a><span class="kn">import</span> <span class="nn">pytest</span>
+</span><span id="L-6"><a href="#L-6"><span class="linenos"> 6</span></a><span class="kn">from</span> <span class="nn">pathier</span> <span class="kn">import</span> <span class="n">Pathier</span>
+</span><span id="L-7"><a href="#L-7"><span class="linenos"> 7</span></a>
+</span><span id="L-8"><a href="#L-8"><span class="linenos"> 8</span></a>
+</span><span id="L-9"><a href="#L-9"><span class="linenos"> 9</span></a><span class="k">def</span> <span class="nf">get_args</span><span class="p">()</span> <span class="o">-&gt;</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span><span class="p">:</span>
+</span><span id="L-10"><a href="#L-10"><span class="linenos">10</span></a>    <span class="n">parser</span> <span class="o">=</span> <span class="n">argparse</span><span class="o">.</span><span class="n">ArgumentParser</span><span class="p">()</span>
+</span><span id="L-11"><a href="#L-11"><span class="linenos">11</span></a>
+</span><span id="L-12"><a href="#L-12"><span class="linenos">12</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="L-13"><a href="#L-13"><span class="linenos">13</span></a>        <span class="s2">&quot;package_name&quot;</span><span class="p">,</span>
+</span><span id="L-14"><a href="#L-14"><span class="linenos">14</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
+</span><span id="L-15"><a href="#L-15"><span class="linenos">15</span></a>        <span class="n">default</span><span class="o">=</span><span class="s2">&quot;.&quot;</span><span class="p">,</span>
+</span><span id="L-16"><a href="#L-16"><span class="linenos">16</span></a>        <span class="n">nargs</span><span class="o">=</span><span class="s2">&quot;?&quot;</span><span class="p">,</span>
+</span><span id="L-17"><a href="#L-17"><span class="linenos">17</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; The name of the package or project to run tests for,</span>
+</span><span id="L-18"><a href="#L-18"><span class="linenos">18</span></a><span class="s2">        assuming it&#39;s a subfolder of your current working directory.</span>
+</span><span id="L-19"><a href="#L-19"><span class="linenos">19</span></a><span class="s2">        Can also be a full path to the package. If nothing is given,</span>
+</span><span id="L-20"><a href="#L-20"><span class="linenos">20</span></a><span class="s2">        the current working directory will be used.&quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="L-21"><a href="#L-21"><span class="linenos">21</span></a>    <span class="p">)</span>
 </span><span id="L-22"><a href="#L-22"><span class="linenos">22</span></a>
-</span><span id="L-23"><a href="#L-23"><span class="linenos">23</span></a>    <span class="k">return</span> <span class="n">args</span>
+</span><span id="L-23"><a href="#L-23"><span class="linenos">23</span></a>    <span class="n">args</span> <span class="o">=</span> <span class="n">parser</span><span class="o">.</span><span class="n">parse_args</span><span class="p">()</span>
 </span><span id="L-24"><a href="#L-24"><span class="linenos">24</span></a>
-</span><span id="L-25"><a href="#L-25"><span class="linenos">25</span></a>
-</span><span id="L-26"><a href="#L-26"><span class="linenos">26</span></a><span class="k">def</span> <span class="nf">run_tests</span><span class="p">(</span><span class="n">package_path</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">):</span>
-</span><span id="L-27"><a href="#L-27"><span class="linenos">27</span></a>    <span class="sd">&quot;&quot;&quot;Run tests with coverage and pytest.&quot;&quot;&quot;</span>
-</span><span id="L-28"><a href="#L-28"><span class="linenos">28</span></a>    <span class="n">startdir</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">()</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span>
-</span><span id="L-29"><a href="#L-29"><span class="linenos">29</span></a>    <span class="n">os</span><span class="o">.</span><span class="n">chdir</span><span class="p">(</span><span class="n">package_path</span><span class="p">)</span>
-</span><span id="L-30"><a href="#L-30"><span class="linenos">30</span></a>    <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;pip install -e .&quot;</span><span class="p">)</span>
-</span><span id="L-31"><a href="#L-31"><span class="linenos">31</span></a>    <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;coverage run -m pytest -s&quot;</span><span class="p">)</span>
-</span><span id="L-32"><a href="#L-32"><span class="linenos">32</span></a>    <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;coverage report -m&quot;</span><span class="p">)</span>
-</span><span id="L-33"><a href="#L-33"><span class="linenos">33</span></a>    <span class="n">os</span><span class="o">.</span><span class="n">chdir</span><span class="p">(</span><span class="n">startdir</span><span class="p">)</span>
-</span><span id="L-34"><a href="#L-34"><span class="linenos">34</span></a>
-</span><span id="L-35"><a href="#L-35"><span class="linenos">35</span></a>
-</span><span id="L-36"><a href="#L-36"><span class="linenos">36</span></a><span class="k">def</span> <span class="nf">main</span><span class="p">(</span><span class="n">args</span><span class="p">:</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span> <span class="o">=</span> <span class="kc">None</span><span class="p">):</span>
-</span><span id="L-37"><a href="#L-37"><span class="linenos">37</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="p">:</span>
-</span><span id="L-38"><a href="#L-38"><span class="linenos">38</span></a>        <span class="n">args</span> <span class="o">=</span> <span class="n">get_args</span><span class="p">()</span>
-</span><span id="L-39"><a href="#L-39"><span class="linenos">39</span></a>    <span class="n">package_path</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">package_name</span><span class="p">)</span><span class="o">.</span><span class="n">resolve</span><span class="p">()</span>
-</span><span id="L-40"><a href="#L-40"><span class="linenos">40</span></a>    <span class="n">run_tests</span><span class="p">(</span><span class="n">package_path</span><span class="p">)</span>
+</span><span id="L-25"><a href="#L-25"><span class="linenos">25</span></a>    <span class="k">return</span> <span class="n">args</span>
+</span><span id="L-26"><a href="#L-26"><span class="linenos">26</span></a>
+</span><span id="L-27"><a href="#L-27"><span class="linenos">27</span></a>
+</span><span id="L-28"><a href="#L-28"><span class="linenos">28</span></a><span class="k">def</span> <span class="nf">run_tests</span><span class="p">(</span><span class="n">package_path</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
+</span><span id="L-29"><a href="#L-29"><span class="linenos">29</span></a>    <span class="sd">&quot;&quot;&quot;Run tests with coverage and pytest.</span>
+</span><span id="L-30"><a href="#L-30"><span class="linenos">30</span></a>
+</span><span id="L-31"><a href="#L-31"><span class="linenos">31</span></a><span class="sd">    Returns True if all tests passed.&quot;&quot;&quot;</span>
+</span><span id="L-32"><a href="#L-32"><span class="linenos">32</span></a>    <span class="n">startdir</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">()</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span>
+</span><span id="L-33"><a href="#L-33"><span class="linenos">33</span></a>    <span class="n">package_path</span><span class="o">.</span><span class="n">mkcwd</span><span class="p">()</span>
+</span><span id="L-34"><a href="#L-34"><span class="linenos">34</span></a>    <span class="n">cover</span> <span class="o">=</span> <span class="n">coverage</span><span class="o">.</span><span class="n">Coverage</span><span class="p">()</span>
+</span><span id="L-35"><a href="#L-35"><span class="linenos">35</span></a>    <span class="n">cover</span><span class="o">.</span><span class="n">start</span><span class="p">()</span>
+</span><span id="L-36"><a href="#L-36"><span class="linenos">36</span></a>    <span class="n">results</span> <span class="o">=</span> <span class="n">pytest</span><span class="o">.</span><span class="n">main</span><span class="p">([</span><span class="s2">&quot;-s&quot;</span><span class="p">])</span>
+</span><span id="L-37"><a href="#L-37"><span class="linenos">37</span></a>    <span class="n">cover</span><span class="o">.</span><span class="n">stop</span><span class="p">()</span>
+</span><span id="L-38"><a href="#L-38"><span class="linenos">38</span></a>    <span class="n">cover</span><span class="o">.</span><span class="n">report</span><span class="p">()</span>
+</span><span id="L-39"><a href="#L-39"><span class="linenos">39</span></a>    <span class="n">startdir</span><span class="o">.</span><span class="n">mkcwd</span><span class="p">()</span>
+</span><span id="L-40"><a href="#L-40"><span class="linenos">40</span></a>    <span class="k">return</span> <span class="n">results</span> <span class="o">==</span> <span class="mi">0</span>
 </span><span id="L-41"><a href="#L-41"><span class="linenos">41</span></a>
 </span><span id="L-42"><a href="#L-42"><span class="linenos">42</span></a>
-</span><span id="L-43"><a href="#L-43"><span class="linenos">43</span></a><span class="k">if</span> <span class="vm">__name__</span> <span class="o">==</span> <span class="s2">&quot;__main__&quot;</span><span class="p">:</span>
-</span><span id="L-44"><a href="#L-44"><span class="linenos">44</span></a>    <span class="n">main</span><span class="p">(</span><span class="n">get_args</span><span class="p">())</span>
+</span><span id="L-43"><a href="#L-43"><span class="linenos">43</span></a><span class="k">def</span> <span class="nf">main</span><span class="p">(</span><span class="n">args</span><span class="p">:</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span> <span class="o">=</span> <span class="kc">None</span><span class="p">):</span>
+</span><span id="L-44"><a href="#L-44"><span class="linenos">44</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="p">:</span>
+</span><span id="L-45"><a href="#L-45"><span class="linenos">45</span></a>        <span class="n">args</span> <span class="o">=</span> <span class="n">get_args</span><span class="p">()</span>
+</span><span id="L-46"><a href="#L-46"><span class="linenos">46</span></a>    <span class="n">package_path</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">package_name</span><span class="p">)</span><span class="o">.</span><span class="n">resolve</span><span class="p">()</span>
+</span><span id="L-47"><a href="#L-47"><span class="linenos">47</span></a>    <span class="n">run_tests</span><span class="p">(</span><span class="n">package_path</span><span class="p">)</span>
+</span><span id="L-48"><a href="#L-48"><span class="linenos">48</span></a>
+</span><span id="L-49"><a href="#L-49"><span class="linenos">49</span></a>
+</span><span id="L-50"><a href="#L-50"><span class="linenos">50</span></a><span class="k">if</span> <span class="vm">__name__</span> <span class="o">==</span> <span class="s2">&quot;__main__&quot;</span><span class="p">:</span>
+</span><span id="L-51"><a href="#L-51"><span class="linenos">51</span></a>    <span class="n">main</span><span class="p">(</span><span class="n">get_args</span><span class="p">())</span>
 </span></pre></div>
 
 
             </section>
                 <section id="get_args">
                             <input id="get_args-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
@@ -115,60 +122,67 @@
         <span class="def">def</span>
         <span class="name">get_args</span><span class="signature pdoc-code condensed">(<span class="return-annotation">) -> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span>:</span></span>
 
                 <label class="view-source-button" for="get_args-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#get_args"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="get_args-8"><a href="#get_args-8"><span class="linenos"> 8</span></a><span class="k">def</span> <span class="nf">get_args</span><span class="p">()</span> <span class="o">-&gt;</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span><span class="p">:</span>
-</span><span id="get_args-9"><a href="#get_args-9"><span class="linenos"> 9</span></a>    <span class="n">parser</span> <span class="o">=</span> <span class="n">argparse</span><span class="o">.</span><span class="n">ArgumentParser</span><span class="p">()</span>
-</span><span id="get_args-10"><a href="#get_args-10"><span class="linenos">10</span></a>
-</span><span id="get_args-11"><a href="#get_args-11"><span class="linenos">11</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="get_args-12"><a href="#get_args-12"><span class="linenos">12</span></a>        <span class="s2">&quot;package_name&quot;</span><span class="p">,</span>
-</span><span id="get_args-13"><a href="#get_args-13"><span class="linenos">13</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
-</span><span id="get_args-14"><a href="#get_args-14"><span class="linenos">14</span></a>        <span class="n">default</span><span class="o">=</span><span class="s2">&quot;.&quot;</span><span class="p">,</span>
-</span><span id="get_args-15"><a href="#get_args-15"><span class="linenos">15</span></a>        <span class="n">nargs</span><span class="o">=</span><span class="s2">&quot;?&quot;</span><span class="p">,</span>
-</span><span id="get_args-16"><a href="#get_args-16"><span class="linenos">16</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; The name of the package or project to run tests for,</span>
-</span><span id="get_args-17"><a href="#get_args-17"><span class="linenos">17</span></a><span class="s2">        assuming it&#39;s a subfolder of your current working directory.</span>
-</span><span id="get_args-18"><a href="#get_args-18"><span class="linenos">18</span></a><span class="s2">        Can also be a full path to the package. If nothing is given,</span>
-</span><span id="get_args-19"><a href="#get_args-19"><span class="linenos">19</span></a><span class="s2">        the current working directory will be used.&quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="get_args-20"><a href="#get_args-20"><span class="linenos">20</span></a>    <span class="p">)</span>
-</span><span id="get_args-21"><a href="#get_args-21"><span class="linenos">21</span></a>
-</span><span id="get_args-22"><a href="#get_args-22"><span class="linenos">22</span></a>    <span class="n">args</span> <span class="o">=</span> <span class="n">parser</span><span class="o">.</span><span class="n">parse_args</span><span class="p">()</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="get_args-10"><a href="#get_args-10"><span class="linenos">10</span></a><span class="k">def</span> <span class="nf">get_args</span><span class="p">()</span> <span class="o">-&gt;</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span><span class="p">:</span>
+</span><span id="get_args-11"><a href="#get_args-11"><span class="linenos">11</span></a>    <span class="n">parser</span> <span class="o">=</span> <span class="n">argparse</span><span class="o">.</span><span class="n">ArgumentParser</span><span class="p">()</span>
+</span><span id="get_args-12"><a href="#get_args-12"><span class="linenos">12</span></a>
+</span><span id="get_args-13"><a href="#get_args-13"><span class="linenos">13</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="get_args-14"><a href="#get_args-14"><span class="linenos">14</span></a>        <span class="s2">&quot;package_name&quot;</span><span class="p">,</span>
+</span><span id="get_args-15"><a href="#get_args-15"><span class="linenos">15</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
+</span><span id="get_args-16"><a href="#get_args-16"><span class="linenos">16</span></a>        <span class="n">default</span><span class="o">=</span><span class="s2">&quot;.&quot;</span><span class="p">,</span>
+</span><span id="get_args-17"><a href="#get_args-17"><span class="linenos">17</span></a>        <span class="n">nargs</span><span class="o">=</span><span class="s2">&quot;?&quot;</span><span class="p">,</span>
+</span><span id="get_args-18"><a href="#get_args-18"><span class="linenos">18</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; The name of the package or project to run tests for,</span>
+</span><span id="get_args-19"><a href="#get_args-19"><span class="linenos">19</span></a><span class="s2">        assuming it&#39;s a subfolder of your current working directory.</span>
+</span><span id="get_args-20"><a href="#get_args-20"><span class="linenos">20</span></a><span class="s2">        Can also be a full path to the package. If nothing is given,</span>
+</span><span id="get_args-21"><a href="#get_args-21"><span class="linenos">21</span></a><span class="s2">        the current working directory will be used.&quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="get_args-22"><a href="#get_args-22"><span class="linenos">22</span></a>    <span class="p">)</span>
 </span><span id="get_args-23"><a href="#get_args-23"><span class="linenos">23</span></a>
-</span><span id="get_args-24"><a href="#get_args-24"><span class="linenos">24</span></a>    <span class="k">return</span> <span class="n">args</span>
+</span><span id="get_args-24"><a href="#get_args-24"><span class="linenos">24</span></a>    <span class="n">args</span> <span class="o">=</span> <span class="n">parser</span><span class="o">.</span><span class="n">parse_args</span><span class="p">()</span>
+</span><span id="get_args-25"><a href="#get_args-25"><span class="linenos">25</span></a>
+</span><span id="get_args-26"><a href="#get_args-26"><span class="linenos">26</span></a>    <span class="k">return</span> <span class="n">args</span>
 </span></pre></div>
 
 
     
 
                 </section>
                 <section id="run_tests">
                             <input id="run_tests-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
             
         <span class="def">def</span>
-        <span class="name">run_tests</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">package_path</span><span class="p">:</span> <span class="n">pathier</span><span class="o">.</span><span class="n">pathier</span><span class="o">.</span><span class="n">Pathier</span></span><span class="return-annotation">):</span></span>
+        <span class="name">run_tests</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">package_path</span><span class="p">:</span> <span class="n">pathier</span><span class="o">.</span><span class="n">pathier</span><span class="o">.</span><span class="n">Pathier</span></span><span class="return-annotation">) -> <span class="nb">bool</span>:</span></span>
 
                 <label class="view-source-button" for="run_tests-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#run_tests"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="run_tests-27"><a href="#run_tests-27"><span class="linenos">27</span></a><span class="k">def</span> <span class="nf">run_tests</span><span class="p">(</span><span class="n">package_path</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">):</span>
-</span><span id="run_tests-28"><a href="#run_tests-28"><span class="linenos">28</span></a>    <span class="sd">&quot;&quot;&quot;Run tests with coverage and pytest.&quot;&quot;&quot;</span>
-</span><span id="run_tests-29"><a href="#run_tests-29"><span class="linenos">29</span></a>    <span class="n">startdir</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">()</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span>
-</span><span id="run_tests-30"><a href="#run_tests-30"><span class="linenos">30</span></a>    <span class="n">os</span><span class="o">.</span><span class="n">chdir</span><span class="p">(</span><span class="n">package_path</span><span class="p">)</span>
-</span><span id="run_tests-31"><a href="#run_tests-31"><span class="linenos">31</span></a>    <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;pip install -e .&quot;</span><span class="p">)</span>
-</span><span id="run_tests-32"><a href="#run_tests-32"><span class="linenos">32</span></a>    <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;coverage run -m pytest -s&quot;</span><span class="p">)</span>
-</span><span id="run_tests-33"><a href="#run_tests-33"><span class="linenos">33</span></a>    <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;coverage report -m&quot;</span><span class="p">)</span>
-</span><span id="run_tests-34"><a href="#run_tests-34"><span class="linenos">34</span></a>    <span class="n">os</span><span class="o">.</span><span class="n">chdir</span><span class="p">(</span><span class="n">startdir</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="run_tests-29"><a href="#run_tests-29"><span class="linenos">29</span></a><span class="k">def</span> <span class="nf">run_tests</span><span class="p">(</span><span class="n">package_path</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
+</span><span id="run_tests-30"><a href="#run_tests-30"><span class="linenos">30</span></a>    <span class="sd">&quot;&quot;&quot;Run tests with coverage and pytest.</span>
+</span><span id="run_tests-31"><a href="#run_tests-31"><span class="linenos">31</span></a>
+</span><span id="run_tests-32"><a href="#run_tests-32"><span class="linenos">32</span></a><span class="sd">    Returns True if all tests passed.&quot;&quot;&quot;</span>
+</span><span id="run_tests-33"><a href="#run_tests-33"><span class="linenos">33</span></a>    <span class="n">startdir</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">()</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span>
+</span><span id="run_tests-34"><a href="#run_tests-34"><span class="linenos">34</span></a>    <span class="n">package_path</span><span class="o">.</span><span class="n">mkcwd</span><span class="p">()</span>
+</span><span id="run_tests-35"><a href="#run_tests-35"><span class="linenos">35</span></a>    <span class="n">cover</span> <span class="o">=</span> <span class="n">coverage</span><span class="o">.</span><span class="n">Coverage</span><span class="p">()</span>
+</span><span id="run_tests-36"><a href="#run_tests-36"><span class="linenos">36</span></a>    <span class="n">cover</span><span class="o">.</span><span class="n">start</span><span class="p">()</span>
+</span><span id="run_tests-37"><a href="#run_tests-37"><span class="linenos">37</span></a>    <span class="n">results</span> <span class="o">=</span> <span class="n">pytest</span><span class="o">.</span><span class="n">main</span><span class="p">([</span><span class="s2">&quot;-s&quot;</span><span class="p">])</span>
+</span><span id="run_tests-38"><a href="#run_tests-38"><span class="linenos">38</span></a>    <span class="n">cover</span><span class="o">.</span><span class="n">stop</span><span class="p">()</span>
+</span><span id="run_tests-39"><a href="#run_tests-39"><span class="linenos">39</span></a>    <span class="n">cover</span><span class="o">.</span><span class="n">report</span><span class="p">()</span>
+</span><span id="run_tests-40"><a href="#run_tests-40"><span class="linenos">40</span></a>    <span class="n">startdir</span><span class="o">.</span><span class="n">mkcwd</span><span class="p">()</span>
+</span><span id="run_tests-41"><a href="#run_tests-41"><span class="linenos">41</span></a>    <span class="k">return</span> <span class="n">results</span> <span class="o">==</span> <span class="mi">0</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Run tests with coverage and pytest.</p>
+
+<p>Returns True if all tests passed.</p>
 </div>
 
 
                 </section>
                 <section id="main">
                             <input id="main-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
@@ -176,19 +190,19 @@
         <span class="def">def</span>
         <span class="name">main</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">args</span><span class="p">:</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span> <span class="o">=</span> <span class="kc">None</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="main-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#main"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="main-37"><a href="#main-37"><span class="linenos">37</span></a><span class="k">def</span> <span class="nf">main</span><span class="p">(</span><span class="n">args</span><span class="p">:</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span> <span class="o">=</span> <span class="kc">None</span><span class="p">):</span>
-</span><span id="main-38"><a href="#main-38"><span class="linenos">38</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="p">:</span>
-</span><span id="main-39"><a href="#main-39"><span class="linenos">39</span></a>        <span class="n">args</span> <span class="o">=</span> <span class="n">get_args</span><span class="p">()</span>
-</span><span id="main-40"><a href="#main-40"><span class="linenos">40</span></a>    <span class="n">package_path</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">package_name</span><span class="p">)</span><span class="o">.</span><span class="n">resolve</span><span class="p">()</span>
-</span><span id="main-41"><a href="#main-41"><span class="linenos">41</span></a>    <span class="n">run_tests</span><span class="p">(</span><span class="n">package_path</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="main-44"><a href="#main-44"><span class="linenos">44</span></a><span class="k">def</span> <span class="nf">main</span><span class="p">(</span><span class="n">args</span><span class="p">:</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span> <span class="o">=</span> <span class="kc">None</span><span class="p">):</span>
+</span><span id="main-45"><a href="#main-45"><span class="linenos">45</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="p">:</span>
+</span><span id="main-46"><a href="#main-46"><span class="linenos">46</span></a>        <span class="n">args</span> <span class="o">=</span> <span class="n">get_args</span><span class="p">()</span>
+</span><span id="main-47"><a href="#main-47"><span class="linenos">47</span></a>    <span class="n">package_path</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">package_name</span><span class="p">)</span><span class="o">.</span><span class="n">resolve</span><span class="p">()</span>
+</span><span id="main-48"><a href="#main-48"><span class="linenos">48</span></a>    <span class="n">run_tests</span><span class="p">(</span><span class="n">package_path</span><span class="p">)</span>
 </span></pre></div>
 
 
     
 
                 </section>
     </main>
```

#### html2text {}

```diff
@@ -9,86 +9,99 @@
 built_with_pdoc[pdoc_logo]
 
 ****** hassle.run_tests ******
 ⁰ View Source
 _1import argparse
 _2import os
 _3
-_4from pathier import Pathier
-_5
-_6
-_7def get_args() -> argparse.Namespace:
-_8    parser = argparse.ArgumentParser()
-_9
-10    parser.add_argument(
-11        "package_name",
-12        type=str,
-13        default=".",
-14        nargs="?",
-15        help=""" The name of the package or project to run tests for,
-16        assuming it's a subfolder of your current working directory.
-17        Can also be a full path to the package. If nothing is given,
-18        the current working directory will be used.""",
-19    )
-20
-21    args = parser.parse_args()
+_4import coverage
+_5import pytest
+_6from pathier import Pathier
+_7
+_8
+_9def get_args() -> argparse.Namespace:
+10    parser = argparse.ArgumentParser()
+11
+12    parser.add_argument(
+13        "package_name",
+14        type=str,
+15        default=".",
+16        nargs="?",
+17        help=""" The name of the package or project to run tests for,
+18        assuming it's a subfolder of your current working directory.
+19        Can also be a full path to the package. If nothing is given,
+20        the current working directory will be used.""",
+21    )
 22
-23    return args
+23    args = parser.parse_args()
 24
-25
-26def run_tests(package_path: Pathier):
-27    """Run tests with coverage and pytest."""
-28    startdir = Pathier().cwd()
-29    os.chdir(package_path)
-30    os.system(f"pip install -e .")
-31    os.system(f"coverage run -m pytest -s")
-32    os.system(f"coverage report -m")
-33    os.chdir(startdir)
-34
-35
-36def main(args: argparse.Namespace = None):
-37    if not args:
-38        args = get_args()
-39    package_path = Pathier(args.package_name).resolve()
-40    run_tests(package_path)
+25    return args
+26
+27
+28def run_tests(package_path: Pathier) -> bool:
+29    """Run tests with coverage and pytest.
+30
+31    Returns True if all tests passed."""
+32    startdir = Pathier().cwd()
+33    package_path.mkcwd()
+34    cover = coverage.Coverage()
+35    cover.start()
+36    results = pytest.main(["-s"])
+37    cover.stop()
+38    cover.report()
+39    startdir.mkcwd()
+40    return results == 0
 41
 42
-43if __name__ == "__main__":
-44    main(get_args())
+43def main(args: argparse.Namespace = None):
+44    if not args:
+45        args = get_args()
+46    package_path = Pathier(args.package_name).resolve()
+47    run_tests(package_path)
+48
+49
+50if __name__ == "__main__":
+51    main(get_args())
   ⁰
 def get_args() -> argparse.Namespace: View Source
-_8def get_args() -> argparse.Namespace:
-_9    parser = argparse.ArgumentParser()
-10
-11    parser.add_argument(
-12        "package_name",
-13        type=str,
-14        default=".",
-15        nargs="?",
-16        help=""" The name of the package or project to run tests for,
-17        assuming it's a subfolder of your current working directory.
-18        Can also be a full path to the package. If nothing is given,
-19        the current working directory will be used.""",
-20    )
-21
-22    args = parser.parse_args()
+10def get_args() -> argparse.Namespace:
+11    parser = argparse.ArgumentParser()
+12
+13    parser.add_argument(
+14        "package_name",
+15        type=str,
+16        default=".",
+17        nargs="?",
+18        help=""" The name of the package or project to run tests for,
+19        assuming it's a subfolder of your current working directory.
+20        Can also be a full path to the package. If nothing is given,
+21        the current working directory will be used.""",
+22    )
 23
-24    return args
+24    args = parser.parse_args()
+25
+26    return args
   ⁰
-def run_tests(package_path: pathier.pathier.Pathier): View Source
-27def run_tests(package_path: Pathier):
-28    """Run tests with coverage and pytest."""
-29    startdir = Pathier().cwd()
-30    os.chdir(package_path)
-31    os.system(f"pip install -e .")
-32    os.system(f"coverage run -m pytest -s")
-33    os.system(f"coverage report -m")
-34    os.chdir(startdir)
+def run_tests(package_path: pathier.pathier.Pathier) -> bool: View Source
+29def run_tests(package_path: Pathier) -> bool:
+30    """Run tests with coverage and pytest.
+31
+32    Returns True if all tests passed."""
+33    startdir = Pathier().cwd()
+34    package_path.mkcwd()
+35    cover = coverage.Coverage()
+36    cover.start()
+37    results = pytest.main(["-s"])
+38    cover.stop()
+39    cover.report()
+40    startdir.mkcwd()
+41    return results == 0
 Run tests with coverage and pytest.
+Returns True if all tests passed.
   ⁰
 def main(args: argparse.Namespace = None): View Source
-37def main(args: argparse.Namespace = None):
-38    if not args:
-39        args = get_args()
-40    package_path = Pathier(args.package_name).resolve()
-41    run_tests(package_path)
+44def main(args: argparse.Namespace = None):
+45    if not args:
+46        args = get_args()
+47    package_path = Pathier(args.package_name).resolve()
+48    run_tests(package_path)
```

### Comparing `hassle-2.7.1/src/hassle/generate_tests.py` & `hassle-2.8.0/src/hassle/generate_tests.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import argparse
-import os
 import tokenize
 
+import isort
 from pathier import Pathier
 
+from hassle import hassle_utilities
+
 root = Pathier(__file__).parent
 
 
 def get_args() -> argparse.Namespace:
     parser = argparse.ArgumentParser()
 
     parser.add_argument(
@@ -86,16 +88,16 @@
     else:
         content = f"import pytest\nfrom {package_name} import {pyfile.stem}\n\n\n"
     for function in functions:
         test_function = f"def test_{function}"
         if test_function not in content and function != "__init__":
             content += f"{test_function}():\n    ...\n\n\n"
     test_file.write_text(content)
-    os.system(f"black {tests_dir}")
-    os.system(f"isort {tests_dir}")
+    hassle_utilities.format_files(tests_dir)
+    [isort.file(path) for path in tests_dir.rglob("*.py")]
 
 
 def generate_test_files(package_path: Pathier, tests_dir: Pathier = None):
     """Generate test files for all .py files in 'src'
     directory of 'package_path'."""
     pyfiles = [
         file
```

### Comparing `hassle-2.7.1/src/hassle/hassle.py` & `hassle-2.8.0/src/hassle/hassle.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 import argparse
 import os
+import sys
 
+import isort
+from gitbetter import git
 from pathier import Pathier
 
 from hassle import hassle_utilities
 from hassle.generate_tests import generate_test_files
 from hassle.run_tests import run_tests
 
 root = Pathier(__file__).parent
@@ -127,14 +130,21 @@
         type=str,
         default=None,
         help=""" Excpects one argument: "major", "minor", or "patch".
         Passing "-up minor" is equivalent to passing the cli string: "-b -t -i -iv minor -uc -ca build -s".
         To publish the updated package, the -p/--publish switch needs to be added to the cli input.""",
     )
 
+    parser.add_argument(
+        "-st",
+        "--skip_tests",
+        action="store_true",
+        help=""" Don't run tests when using the -b/--build command. """,
+    )
+
     args = parser.parse_args()
 
     args.package = Pathier(args.package).resolve()
 
     if args.update:
         args.build = True
         args.tag_version = True
@@ -155,75 +165,95 @@
 
     if args.commit_all == "":
         raise ValueError("Commit message for args.commit_all cannot be empty.")
 
     return args
 
 
+def build(
+    package_dir: Pathier, skip_tests: bool = False, overwrite_dependencies: bool = False
+):
+    """Perform the build process.
+
+    Steps:
+    * Run tests (unless `skip_tests` is `True`)
+    * Raise error and abandon build if tests fail
+    * Format source code with `Black`
+    * Sort source code imports with `isort`
+    * Update project dependencies in `pyproject.toml`
+    * Generate docs
+    * Delete previous `dist` folder contents
+    * Invoke build module"""
+    if not skip_tests and not run_tests(package_dir):
+        raise RuntimeError(
+            f"ERROR: {package_dir.stem} failed testing.\nAbandoning build."
+        )
+    hassle_utilities.format_files(package_dir)
+    [isort.file(path) for path in package_dir.rglob("*.py")]
+    hassle_utilities.update_dependencies(
+        package_dir / "pyproject.toml", overwrite_dependencies
+    )
+    # Vermin isn't taking into account the minimum version of dependencies.
+    # Removing from now and defaulting to >=3.10
+    # hassle_utilities.update_minimum_python_version(pyproject_path)
+    hassle_utilities.generate_docs(package_dir)
+    (package_dir / "dist").delete()
+    os.system(f"{sys.executable} -m build {package_dir}")
+
+
 def main(args: argparse.Namespace = None):
     if not args:
         args = get_args()
 
     pyproject_path = args.package / "pyproject.toml"
+    args.package.mkcwd()
 
     if not pyproject_path.exists():
         raise FileNotFoundError(f"Could not locate pyproject.toml for {args.package}")
 
     if args.generate_tests:
         generate_test_files(args.package)
 
     if args.run_tests:
         run_tests(args.package)
 
     if args.increment_version:
         hassle_utilities.increment_version(pyproject_path, args.increment_version)
 
     if args.build:
-        (args.package / "dist").delete()
-        os.system(f"black {args.package}")
-        os.system(f"isort {args.package}")
-        hassle_utilities.update_dependencies(
-            pyproject_path, args.overwrite_dependencies
-        )
-        # Vermin isn't taking into account the minimum version of dependencies.
-        # Removing from now and defaulting to >=3.10
-        # hassle_utilities.update_minimum_python_version(pyproject_path)
-        hassle_utilities.generate_docs(args.package)
-        os.system(f"py -m build {args.package}")
+        build(args.package, args.skip_tests, args.overwrite_dependencies)
 
     if args.update_changelog:
         hassle_utilities.update_changelog(pyproject_path)
         # If we're going to add tag for current version
         # commit changelog first
         if args.tag_version:
             input(
                 "Press enter to continue after optionally pruning the updated changelog..."
             )
-            os.chdir(args.package)
-            os.system("git add CHANGELOG.md")
-            os.system('git commit CHANGELOG.md -m "chore: update changelog"')
+            git.commit_files(
+                [str(args.package / "CHANGELOG.md")], "chore: update changelog"
+            )
 
     if args.commit_all:
-        os.chdir(args.package)
         if args.commit_all == "build":
             version = pyproject_path.loads()["project"]["version"]
             args.commit_all = f"chore: build v{version}"
-        os.system("git add .")
-        os.system(f'git commit -m "{args.commit_all}"')
+        git.add()
+        git.commit(f'-m "{args.commit_all}"')
 
     if args.tag_version:
         hassle_utilities.tag_version(args.package)
 
     if args.publish:
         os.system(f"twine upload {args.package / 'dist' / '*'}")
 
     if args.install:
         os.system(f"pip install {args.package} --no-deps --upgrade --no-cache-dir")
 
     if args.sync:
-        os.chdir(args.package)
-        os.system(f"git pull --tags origin main")
-        os.system(f"git push origin main:main --tags")
+        git.pull("--tags")
+        git.push("--tags")
 
 
 if __name__ == "__main__":
     main(get_args())
```

### Comparing `hassle-2.7.1/src/hassle/hassle_config.py` & `hassle-2.8.0/src/hassle/hassle_config.py`

 * *Files identical despite different names*

### Comparing `hassle-2.7.1/src/hassle/hassle_utilities.py` & `hassle-2.8.0/src/hassle/hassle_utilities.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import os
 
+import black
 import packagelister
 import vermin
+from gitbetter import git
 from pathier import Pathier
 
 from hassle import hassle_config
 
 root = Pathier(__file__).parent
 
 
@@ -136,8 +138,16 @@
     if hassle_config.config_exists():
         tag_prefix = hassle_config.load_config()["git"]["tag_prefix"]
     else:
         hassle_config.warn()
         tag_prefix = ""
     version = (package_path / "pyproject.toml").loads()["project"]["version"]
     os.chdir(package_path)
-    os.system(f"git tag {tag_prefix}{version}")
+    git.tag(f"{tag_prefix}{version}")
+
+
+def format_files(path: Pathier):
+    """Use `Black` to format file(s)."""
+    try:
+        black.main([str(path)])
+    except SystemExit:
+        ...
```

### Comparing `hassle-2.7.1/src/hassle/license_template.txt` & `hassle-2.8.0/src/hassle/license_template.txt`

 * *Files identical despite different names*

### Comparing `hassle-2.7.1/src/hassle/new_project.py` & `hassle-2.8.0/src/hassle/new_project.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import argparse
 import os
 import sys
 from datetime import datetime
 
 import requests
 from bs4 import BeautifulSoup
+from gitbetter import git
 from pathier import Pathier
 
 import hassle.hassle_config as hassle_config
 from hassle.generate_tests import generate_test_files
 
 root = Pathier(__file__).parent
 
@@ -251,15 +252,15 @@
         if not args.not_package:
             generate_test_files(targetdir)
             create_vscode_settings(targetdir)
         create_gitignore(targetdir)
         if not args.no_license:
             create_license(targetdir)
         os.chdir(targetdir)
-        os.system("git init -b main")
+        git.new_repo()
 
     except Exception as e:
         if not "Aborting new package creation" in str(e):
             print(e)
         if get_answer("Delete created files?"):
             targetdir.delete()
```

### Comparing `hassle-2.7.1/src/hassle/pyproject_template.toml` & `hassle-2.8.0/src/hassle/pyproject_template.toml`

 * *Files identical despite different names*

### Comparing `hassle-2.7.1/src/hassle/run_tests.py` & `hassle-2.8.0/src/hassle/run_tests.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import argparse
 import os
 
+import coverage
+import pytest
 from pathier import Pathier
 
 
 def get_args() -> argparse.Namespace:
     parser = argparse.ArgumentParser()
 
     parser.add_argument(
@@ -19,22 +21,27 @@
     )
 
     args = parser.parse_args()
 
     return args
 
 
-def run_tests(package_path: Pathier):
-    """Run tests with coverage and pytest."""
+def run_tests(package_path: Pathier) -> bool:
+    """Run tests with coverage and pytest.
+
+    Returns True if all tests passed."""
     startdir = Pathier().cwd()
-    os.chdir(package_path)
-    os.system(f"pip install -e .")
-    os.system(f"coverage run -m pytest -s")
-    os.system(f"coverage report -m")
-    os.chdir(startdir)
+    package_path.mkcwd()
+    cover = coverage.Coverage()
+    cover.start()
+    results = pytest.main(["-s"])
+    cover.stop()
+    cover.report()
+    startdir.mkcwd()
+    return results == 0
 
 
 def main(args: argparse.Namespace = None):
     if not args:
         args = get_args()
     package_path = Pathier(args.package_name).resolve()
     run_tests(package_path)
```

### Comparing `hassle-2.7.1/LICENSE.txt` & `hassle-2.8.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hassle-2.7.1/README.md` & `hassle-2.8.0/README.md`

 * *Files identical despite different names*

### Comparing `hassle-2.7.1/pyproject.toml` & `hassle-2.8.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 00000090: 226d 6174 746d 616e 6573 4070 6d2e 6d65  "mattmanes@pm.me
 000000a0: 227d 5d0d 0a64 6573 6372 6970 7469 6f6e  "}]..description
 000000b0: 203d 2022 4372 6561 7465 2c20 6275 696c   = "Create, buil
 000000c0: 642c 2074 6573 742c 2061 6e64 2070 7562  d, test, and pub
 000000d0: 6c69 7368 2050 7974 686f 6e20 7072 6f6a  lish Python proj
 000000e0: 6563 7473 2061 6e64 2070 6163 6b61 6765  ects and package
 000000f0: 732e 220d 0a76 6572 7369 6f6e 203d 2022  s."..version = "
-00000100: 322e 372e 3122 0d0a 7265 7175 6972 6573  2.7.1"..requires
+00000100: 322e 382e 3022 0d0a 7265 7175 6972 6573  2.8.0"..requires
 00000110: 2d70 7974 686f 6e20 3d20 223e 3d33 2e31  -python = ">=3.1
 00000120: 3022 0d0a 6465 7065 6e64 656e 6369 6573  0"..dependencies
 00000130: 203d 205b 0d0a 2020 2020 2262 6c61 636b   = [..    "black
 00000140: 222c 200d 0a20 2020 2022 6973 6f72 7422  ", ..    "isort"
 00000150: 2c20 0d0a 2020 2020 2270 7974 6573 747e  , ..    "pytest~
 00000160: 3d37 2e32 2e31 222c 200d 0a20 2020 2022  =7.2.1", ..    "
 00000170: 636f 7665 7261 6765 222c 0d0a 2020 2020  coverage",..    
@@ -27,73 +27,74 @@
 000001a0: 2e35 2e31 222c 0d0a 2020 2020 2270 646f  .5.1",..    "pdo
 000001b0: 6322 2c0d 0a20 2020 2022 7477 696e 6522  c",..    "twine"
 000001c0: 2c0d 0a20 2020 2022 6175 746f 2d63 6861  ,..    "auto-cha
 000001d0: 6e67 656c 6f67 222c 0d0a 2020 2020 2262  ngelog",..    "b
 000001e0: 7334 222c 0d0a 2020 2020 2272 6571 7565  s4",..    "reque
 000001f0: 7374 7322 2c0d 0a20 2020 2022 6275 696c  sts",..    "buil
 00000200: 6422 2c0d 0a20 2020 2022 7061 7468 6965  d",..    "pathie
-00000210: 7222 0d0a 2020 2020 5d0d 0a72 6561 646d  r"..    ]..readm
-00000220: 6520 3d20 2252 4541 444d 452e 6d64 220d  e = "README.md".
-00000230: 0a6b 6579 776f 7264 7320 3d20 5b22 6465  .keywords = ["de
-00000240: 766f 7073 222c 2022 7061 636b 6167 696e  vops", "packagin
-00000250: 6722 2c20 2262 7569 6c64 222c 2022 7465  g", "build", "te
-00000260: 7374 222c 2022 6175 746f 6d61 7469 6f6e  st", "automation
-00000270: 225d 0d0a 636c 6173 7369 6669 6572 7320  "]..classifiers 
-00000280: 3d20 5b0d 0a20 2020 2022 5072 6f67 7261  = [..    "Progra
-00000290: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
-000002a0: 3a20 5079 7468 6f6e 203a 3a20 3322 2c0d  : Python :: 3",.
-000002b0: 0a20 2020 2022 4c69 6365 6e73 6520 3a3a  .    "License ::
-000002c0: 204f 5349 2041 7070 726f 7665 6420 3a3a   OSI Approved ::
-000002d0: 204d 4954 204c 6963 656e 7365 222c 0d0a   MIT License",..
-000002e0: 2020 2020 224f 7065 7261 7469 6e67 2053      "Operating S
-000002f0: 7973 7465 6d20 3a3a 204f 5320 496e 6465  ystem :: OS Inde
-00000300: 7065 6e64 656e 7422 2c0d 0a20 2020 205d  pendent",..    ]
-00000310: 0d0a 0d0a 5b70 726f 6a65 6374 2e75 726c  ....[project.url
-00000320: 735d 0d0a 2248 6f6d 6570 6167 6522 203d  s].."Homepage" =
-00000330: 2022 6874 7470 733a 2f2f 6769 7468 7562   "https://github
-00000340: 2e63 6f6d 2f6d 6174 742d 6d61 6e65 732f  .com/matt-manes/
-00000350: 6861 7373 6c65 220d 0a22 446f 6375 6d65  hassle".."Docume
-00000360: 6e74 6174 696f 6e22 203d 2022 6874 7470  ntation" = "http
-00000370: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6d  s://github.com/m
-00000380: 6174 742d 6d61 6e65 732f 6861 7373 6c65  att-manes/hassle
-00000390: 2f74 7265 652f 6d61 696e 2f64 6f63 7322  /tree/main/docs"
-000003a0: 0d0a 2253 6f75 7263 6520 636f 6465 2220  .."Source code" 
-000003b0: 3d20 2268 7474 7073 3a2f 2f67 6974 6875  = "https://githu
-000003c0: 622e 636f 6d2f 6d61 7474 2d6d 616e 6573  b.com/matt-manes
-000003d0: 2f68 6173 736c 652f 7472 6565 2f6d 6169  /hassle/tree/mai
-000003e0: 6e2f 7372 632f 6861 7373 6c65 220d 0a0d  n/src/hassle"...
-000003f0: 0a5b 746f 6f6c 2e70 7974 6573 742e 696e  .[tool.pytest.in
-00000400: 695f 6f70 7469 6f6e 735d 0d0a 6164 646f  i_options]..addo
-00000410: 7074 7320 3d20 5b0d 0a20 2020 2022 2d2d  pts = [..    "--
-00000420: 696d 706f 7274 2d6d 6f64 653d 696d 706f  import-mode=impo
-00000430: 7274 6c69 6222 2c0d 0a20 2020 205d 0d0a  rtlib",..    ]..
-00000440: 7079 7468 6f6e 7061 7468 203d 2022 7372  pythonpath = "sr
-00000450: 6322 0d0a 0d0a 5b74 6f6f 6c2e 6861 7463  c"....[tool.hatc
-00000460: 682e 6275 696c 642e 7461 7267 6574 732e  h.build.targets.
-00000470: 7364 6973 745d 0d0a 6578 636c 7564 6520  sdist]..exclude 
-00000480: 3d20 5b0d 0a20 2020 2022 2e63 6f76 6572  = [..    ".cover
-00000490: 6167 6522 2c0d 0a20 2020 2022 2e70 7974  age",..    ".pyt
-000004a0: 6573 745f 6361 6368 6522 2c0d 0a20 2020  est_cache",..   
-000004b0: 2022 2e76 7363 6f64 6522 2c0d 0a20 2020   ".vscode",..   
-000004c0: 2022 7465 7374 7322 2c0d 0a20 2020 2022   "tests",..    "
-000004d0: 6e6f 7465 732e 7478 7422 2c0d 0a20 2020  notes.txt",..   
-000004e0: 2022 2e67 6974 6967 6e6f 7265 222c 0d0a   ".gitignore",..
-000004f0: 2020 2020 2268 6173 736c 655f 636f 6e66      "hassle_conf
-00000500: 6967 2e74 6f6d 6c22 0d0a 2020 2020 5d0d  ig.toml"..    ].
-00000510: 0a5b 7072 6f6a 6563 742e 7363 7269 7074  .[project.script
-00000520: 735d 0d0a 6861 7373 6c65 203d 2022 6861  s]..hassle = "ha
-00000530: 7373 6c65 2e68 6173 736c 653a 6d61 696e  ssle.hassle:main
-00000540: 220d 0a6e 6577 5f70 726f 6a65 6374 203d  "..new_project =
-00000550: 2022 6861 7373 6c65 2e6e 6577 5f70 726f   "hassle.new_pro
-00000560: 6a65 6374 3a6d 6169 6e22 0d0a 6765 6e65  ject:main"..gene
-00000570: 7261 7465 5f74 6573 7473 203d 2022 6861  rate_tests = "ha
-00000580: 7373 6c65 2e67 656e 6572 6174 655f 7465  ssle.generate_te
-00000590: 7374 733a 6d61 696e 220d 0a72 756e 5f74  sts:main"..run_t
-000005a0: 6573 7473 203d 2022 6861 7373 6c65 2e72  ests = "hassle.r
-000005b0: 756e 5f74 6573 7473 3a6d 6169 6e22 0d0a  un_tests:main"..
-000005c0: 6861 7373 6c65 5f63 6f6e 6669 6720 3d20  hassle_config = 
-000005d0: 2268 6173 736c 652e 6861 7373 6c65 5f63  "hassle.hassle_c
-000005e0: 6f6e 6669 673a 6d61 696e 220d 0a63 6865  onfig:main"..che
-000005f0: 636b 5f70 7970 6920 3d20 2268 6173 736c  ck_pypi = "hassl
-00000600: 652e 6e65 775f 7072 6f6a 6563 743a 6368  e.new_project:ch
-00000610: 6563 6b5f 7079 7069 5f66 6f72 5f6e 616d  eck_pypi_for_nam
-00000620: 655f 636c 6922                           e_cli"
+00000210: 7222 2c0d 0a20 2020 2022 6769 7462 6574  r",..    "gitbet
+00000220: 7465 7222 0d0a 2020 2020 5d0d 0a72 6561  ter"..    ]..rea
+00000230: 646d 6520 3d20 2252 4541 444d 452e 6d64  dme = "README.md
+00000240: 220d 0a6b 6579 776f 7264 7320 3d20 5b22  "..keywords = ["
+00000250: 6465 766f 7073 222c 2022 7061 636b 6167  devops", "packag
+00000260: 696e 6722 2c20 2262 7569 6c64 222c 2022  ing", "build", "
+00000270: 7465 7374 222c 2022 6175 746f 6d61 7469  test", "automati
+00000280: 6f6e 225d 0d0a 636c 6173 7369 6669 6572  on"]..classifier
+00000290: 7320 3d20 5b0d 0a20 2020 2022 5072 6f67  s = [..    "Prog
+000002a0: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
+000002b0: 203a 3a20 5079 7468 6f6e 203a 3a20 3322   :: Python :: 3"
+000002c0: 2c0d 0a20 2020 2022 4c69 6365 6e73 6520  ,..    "License 
+000002d0: 3a3a 204f 5349 2041 7070 726f 7665 6420  :: OSI Approved 
+000002e0: 3a3a 204d 4954 204c 6963 656e 7365 222c  :: MIT License",
+000002f0: 0d0a 2020 2020 224f 7065 7261 7469 6e67  ..    "Operating
+00000300: 2053 7973 7465 6d20 3a3a 204f 5320 496e   System :: OS In
+00000310: 6465 7065 6e64 656e 7422 2c0d 0a20 2020  dependent",..   
+00000320: 205d 0d0a 0d0a 5b70 726f 6a65 6374 2e75   ]....[project.u
+00000330: 726c 735d 0d0a 2248 6f6d 6570 6167 6522  rls].."Homepage"
+00000340: 203d 2022 6874 7470 733a 2f2f 6769 7468   = "https://gith
+00000350: 7562 2e63 6f6d 2f6d 6174 742d 6d61 6e65  ub.com/matt-mane
+00000360: 732f 6861 7373 6c65 220d 0a22 446f 6375  s/hassle".."Docu
+00000370: 6d65 6e74 6174 696f 6e22 203d 2022 6874  mentation" = "ht
+00000380: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000390: 2f6d 6174 742d 6d61 6e65 732f 6861 7373  /matt-manes/hass
+000003a0: 6c65 2f74 7265 652f 6d61 696e 2f64 6f63  le/tree/main/doc
+000003b0: 7322 0d0a 2253 6f75 7263 6520 636f 6465  s".."Source code
+000003c0: 2220 3d20 2268 7474 7073 3a2f 2f67 6974  " = "https://git
+000003d0: 6875 622e 636f 6d2f 6d61 7474 2d6d 616e  hub.com/matt-man
+000003e0: 6573 2f68 6173 736c 652f 7472 6565 2f6d  es/hassle/tree/m
+000003f0: 6169 6e2f 7372 632f 6861 7373 6c65 220d  ain/src/hassle".
+00000400: 0a0d 0a5b 746f 6f6c 2e70 7974 6573 742e  ...[tool.pytest.
+00000410: 696e 695f 6f70 7469 6f6e 735d 0d0a 6164  ini_options]..ad
+00000420: 646f 7074 7320 3d20 5b0d 0a20 2020 2022  dopts = [..    "
+00000430: 2d2d 696d 706f 7274 2d6d 6f64 653d 696d  --import-mode=im
+00000440: 706f 7274 6c69 6222 2c0d 0a20 2020 205d  portlib",..    ]
+00000450: 0d0a 7079 7468 6f6e 7061 7468 203d 2022  ..pythonpath = "
+00000460: 7372 6322 0d0a 0d0a 5b74 6f6f 6c2e 6861  src"....[tool.ha
+00000470: 7463 682e 6275 696c 642e 7461 7267 6574  tch.build.target
+00000480: 732e 7364 6973 745d 0d0a 6578 636c 7564  s.sdist]..exclud
+00000490: 6520 3d20 5b0d 0a20 2020 2022 2e63 6f76  e = [..    ".cov
+000004a0: 6572 6167 6522 2c0d 0a20 2020 2022 2e70  erage",..    ".p
+000004b0: 7974 6573 745f 6361 6368 6522 2c0d 0a20  ytest_cache",.. 
+000004c0: 2020 2022 2e76 7363 6f64 6522 2c0d 0a20     ".vscode",.. 
+000004d0: 2020 2022 7465 7374 7322 2c0d 0a20 2020     "tests",..   
+000004e0: 2022 6e6f 7465 732e 7478 7422 2c0d 0a20   "notes.txt",.. 
+000004f0: 2020 2022 2e67 6974 6967 6e6f 7265 222c     ".gitignore",
+00000500: 0d0a 2020 2020 2268 6173 736c 655f 636f  ..    "hassle_co
+00000510: 6e66 6967 2e74 6f6d 6c22 0d0a 2020 2020  nfig.toml"..    
+00000520: 5d0d 0a5b 7072 6f6a 6563 742e 7363 7269  ]..[project.scri
+00000530: 7074 735d 0d0a 6861 7373 6c65 203d 2022  pts]..hassle = "
+00000540: 6861 7373 6c65 2e68 6173 736c 653a 6d61  hassle.hassle:ma
+00000550: 696e 220d 0a6e 6577 5f70 726f 6a65 6374  in"..new_project
+00000560: 203d 2022 6861 7373 6c65 2e6e 6577 5f70   = "hassle.new_p
+00000570: 726f 6a65 6374 3a6d 6169 6e22 0d0a 6765  roject:main"..ge
+00000580: 6e65 7261 7465 5f74 6573 7473 203d 2022  nerate_tests = "
+00000590: 6861 7373 6c65 2e67 656e 6572 6174 655f  hassle.generate_
+000005a0: 7465 7374 733a 6d61 696e 220d 0a72 756e  tests:main"..run
+000005b0: 5f74 6573 7473 203d 2022 6861 7373 6c65  _tests = "hassle
+000005c0: 2e72 756e 5f74 6573 7473 3a6d 6169 6e22  .run_tests:main"
+000005d0: 0d0a 6861 7373 6c65 5f63 6f6e 6669 6720  ..hassle_config 
+000005e0: 3d20 2268 6173 736c 652e 6861 7373 6c65  = "hassle.hassle
+000005f0: 5f63 6f6e 6669 673a 6d61 696e 220d 0a63  _config:main"..c
+00000600: 6865 636b 5f70 7970 6920 3d20 2268 6173  heck_pypi = "has
+00000610: 736c 652e 6e65 775f 7072 6f6a 6563 743a  sle.new_project:
+00000620: 6368 6563 6b5f 7079 7069 5f66 6f72 5f6e  check_pypi_for_n
+00000630: 616d 655f 636c 6922                      ame_cli"
```

### Comparing `hassle-2.7.1/PKG-INFO` & `hassle-2.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hassle
-Version: 2.7.1
+Version: 2.8.0
 Summary: Create, build, test, and publish Python projects and packages.
 Project-URL: Homepage, https://github.com/matt-manes/hassle
 Project-URL: Documentation, https://github.com/matt-manes/hassle/tree/main/docs
 Project-URL: Source code, https://github.com/matt-manes/hassle/tree/main/src/hassle
 Author-email: Matt Manes <mattmanes@pm.me>
 License-File: LICENSE.txt
 Keywords: automation,build,devops,packaging,test
@@ -13,14 +13,15 @@
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Requires-Dist: auto-changelog
 Requires-Dist: black
 Requires-Dist: bs4
 Requires-Dist: build
 Requires-Dist: coverage
+Requires-Dist: gitbetter
 Requires-Dist: isort
 Requires-Dist: packagelister
 Requires-Dist: pathier
 Requires-Dist: pdoc
 Requires-Dist: pytest~=7.2.1
 Requires-Dist: requests
 Requires-Dist: twine
```

