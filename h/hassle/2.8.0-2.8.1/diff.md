# Comparing `tmp/hassle-2.8.0.tar.gz` & `tmp/hassle-2.8.1.tar.gz`

## Comparing `hassle-2.8.0.tar` & `hassle-2.8.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     2706 2020-02-02 00:00:00.000000 hassle-2.8.0/CHANGELOG.md
--rw-r--r--   0        0        0    33936 2020-02-02 00:00:00.000000 hassle-2.8.0/docs/hassle.html
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 hassle-2.8.0/docs/index.html
--rw-r--r--   0        0        0    44738 2020-02-02 00:00:00.000000 hassle-2.8.0/docs/search.js
--rw-r--r--   0        0        0    93372 2020-02-02 00:00:00.000000 hassle-2.8.0/docs/hassle/generate_tests.html
--rw-r--r--   0        0        0   134014 2020-02-02 00:00:00.000000 hassle-2.8.0/docs/hassle/hassle.html
--rw-r--r--   0        0        0   107599 2020-02-02 00:00:00.000000 hassle-2.8.0/docs/hassle/hassle_config.html
--rw-r--r--   0        0        0   116364 2020-02-02 00:00:00.000000 hassle-2.8.0/docs/hassle/hassle_utilities.html
--rw-r--r--   0        0        0   165062 2020-02-02 00:00:00.000000 hassle-2.8.0/docs/hassle/new_project.html
--rw-r--r--   0        0        0    53742 2020-02-02 00:00:00.000000 hassle-2.8.0/docs/hassle/run_tests.html
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 hassle-2.8.0/src/hassle/.gitignore_template
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 hassle-2.8.0/src/hassle/.vscode_template
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 hassle-2.8.0/src/hassle/README_template.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hassle-2.8.0/src/hassle/__init__.py
--rw-r--r--   0        0        0     4156 2020-02-02 00:00:00.000000 hassle-2.8.0/src/hassle/generate_tests.py
--rw-r--r--   0        0        0     7838 2020-02-02 00:00:00.000000 hassle-2.8.0/src/hassle/hassle.py
--rw-r--r--   0        0        0     5456 2020-02-02 00:00:00.000000 hassle-2.8.0/src/hassle/hassle_config.py
--rw-r--r--   0        0        0     5246 2020-02-02 00:00:00.000000 hassle-2.8.0/src/hassle/hassle_utilities.py
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 hassle-2.8.0/src/hassle/license_template.txt
--rw-r--r--   0        0        0     9187 2020-02-02 00:00:00.000000 hassle-2.8.0/src/hassle/new_project.py
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 hassle-2.8.0/src/hassle/pyproject_template.toml
--rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 hassle-2.8.0/src/hassle/run_tests.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 hassle-2.8.0/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 hassle-2.8.0/LICENSE.txt
--rw-r--r--   0        0        0    22059 2020-02-02 00:00:00.000000 hassle-2.8.0/README.md
--rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 hassle-2.8.0/pyproject.toml
--rw-r--r--   0        0        0    22533 2020-02-02 00:00:00.000000 hassle-2.8.0/PKG-INFO
+-rw-r--r--   0        0        0     3343 2020-02-02 00:00:00.000000 hassle-2.8.1/CHANGELOG.md
+-rw-r--r--   0        0        0    33936 2020-02-02 00:00:00.000000 hassle-2.8.1/docs/hassle.html
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 hassle-2.8.1/docs/index.html
+-rw-r--r--   0        0        0    44738 2020-02-02 00:00:00.000000 hassle-2.8.1/docs/search.js
+-rw-r--r--   0        0        0    93372 2020-02-02 00:00:00.000000 hassle-2.8.1/docs/hassle/generate_tests.html
+-rw-r--r--   0        0        0   134700 2020-02-02 00:00:00.000000 hassle-2.8.1/docs/hassle/hassle.html
+-rw-r--r--   0        0        0   107599 2020-02-02 00:00:00.000000 hassle-2.8.1/docs/hassle/hassle_config.html
+-rw-r--r--   0        0        0   116364 2020-02-02 00:00:00.000000 hassle-2.8.1/docs/hassle/hassle_utilities.html
+-rw-r--r--   0        0        0   165062 2020-02-02 00:00:00.000000 hassle-2.8.1/docs/hassle/new_project.html
+-rw-r--r--   0        0        0    53608 2020-02-02 00:00:00.000000 hassle-2.8.1/docs/hassle/run_tests.html
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 hassle-2.8.1/src/hassle/.gitignore_template
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 hassle-2.8.1/src/hassle/.vscode_template
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 hassle-2.8.1/src/hassle/README_template.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hassle-2.8.1/src/hassle/__init__.py
+-rw-r--r--   0        0        0     4156 2020-02-02 00:00:00.000000 hassle-2.8.1/src/hassle/generate_tests.py
+-rw-r--r--   0        0        0     7882 2020-02-02 00:00:00.000000 hassle-2.8.1/src/hassle/hassle.py
+-rw-r--r--   0        0        0     5456 2020-02-02 00:00:00.000000 hassle-2.8.1/src/hassle/hassle_config.py
+-rw-r--r--   0        0        0     5246 2020-02-02 00:00:00.000000 hassle-2.8.1/src/hassle/hassle_utilities.py
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 hassle-2.8.1/src/hassle/license_template.txt
+-rw-r--r--   0        0        0     9187 2020-02-02 00:00:00.000000 hassle-2.8.1/src/hassle/new_project.py
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 hassle-2.8.1/src/hassle/pyproject_template.toml
+-rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 hassle-2.8.1/src/hassle/run_tests.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 hassle-2.8.1/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 hassle-2.8.1/LICENSE.txt
+-rw-r--r--   0        0        0    22059 2020-02-02 00:00:00.000000 hassle-2.8.1/README.md
+-rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 hassle-2.8.1/pyproject.toml
+-rw-r--r--   0        0        0    22533 2020-02-02 00:00:00.000000 hassle-2.8.1/PKG-INFO
```

### Comparing `hassle-2.8.0/CHANGELOG.md` & `hassle-2.8.1/CHANGELOG.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,46 @@
 # Changelog
 
-## 2.7.1 (2023-05-02)
+## 2.8.0 (2023-05-09)
+
+#### New Features
+
+* add tests execution to build command
+* add -st/--skip_tests flag to hassle parser
+#### Fixes
+
+* catch Black.main()'s SystemExit
+* fix Pathier.mkcwd() usage
+* invoke build with sys.executable instead of py
+#### Refactorings
+
+* replace os.system calls to git with gitbetter.git methods
+* replace os.system calls for black and isort with direct invocations
+* extract build process into it's own function
+* make run_tests() invoke pytest and coverage directly and return pytest result
+#### Others
+
+* remove unused import
+
+
+## v2.7.1 (2023-05-02)
 
 #### Fixes
 
 * remove update_minimum_python_version from build process since vermin is incorrectly reporting min versions
 #### Refactorings
 
 * set requires-python to >=3.10 in pyproject_template
 #### Docs
 
 * modify doc string formatting
+#### Others
+
+* build v2.7.1
+* update changelog
 
 
 ## v2.7.0 (2023-04-28)
 
 #### Refactorings
 
 * add a pause to manually prune the changelog before committing the autoupdate
```

### Comparing `hassle-2.8.0/docs/hassle.html` & `hassle-2.8.1/docs/hassle.html`

 * *Files identical despite different names*

### Comparing `hassle-2.8.0/docs/search.js` & `hassle-2.8.1/docs/search.js`

 * *Files identical despite different names*

### Comparing `hassle-2.8.0/docs/hassle/generate_tests.html` & `hassle-2.8.1/docs/hassle/generate_tests.html`

 * *Files identical despite different names*

### Comparing `hassle-2.8.0/docs/hassle/hassle.html` & `hassle-2.8.1/docs/hassle/hassle.html`

 * *Files 0% similar despite different names*

```diff
@@ -306,23 +306,25 @@
 </span><span id="L-244"><a href="#L-244"><span class="linenos">244</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">tag_version</span><span class="p">:</span>
 </span><span id="L-245"><a href="#L-245"><span class="linenos">245</span></a>        <span class="n">hassle_utilities</span><span class="o">.</span><span class="n">tag_version</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="p">)</span>
 </span><span id="L-246"><a href="#L-246"><span class="linenos">246</span></a>
 </span><span id="L-247"><a href="#L-247"><span class="linenos">247</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">publish</span><span class="p">:</span>
 </span><span id="L-248"><a href="#L-248"><span class="linenos">248</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;twine upload </span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">package</span> <span class="o">/</span> <span class="s1">&#39;dist&#39;</span> <span class="o">/</span> <span class="s1">&#39;*&#39;</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
 </span><span id="L-249"><a href="#L-249"><span class="linenos">249</span></a>
 </span><span id="L-250"><a href="#L-250"><span class="linenos">250</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">install</span><span class="p">:</span>
-</span><span id="L-251"><a href="#L-251"><span class="linenos">251</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;pip install </span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="si">}</span><span class="s2"> --no-deps --upgrade --no-cache-dir&quot;</span><span class="p">)</span>
-</span><span id="L-252"><a href="#L-252"><span class="linenos">252</span></a>
-</span><span id="L-253"><a href="#L-253"><span class="linenos">253</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">sync</span><span class="p">:</span>
-</span><span id="L-254"><a href="#L-254"><span class="linenos">254</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">pull</span><span class="p">(</span><span class="s2">&quot;--tags&quot;</span><span class="p">)</span>
-</span><span id="L-255"><a href="#L-255"><span class="linenos">255</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">push</span><span class="p">(</span><span class="s2">&quot;--tags&quot;</span><span class="p">)</span>
-</span><span id="L-256"><a href="#L-256"><span class="linenos">256</span></a>
-</span><span id="L-257"><a href="#L-257"><span class="linenos">257</span></a>
-</span><span id="L-258"><a href="#L-258"><span class="linenos">258</span></a><span class="k">if</span> <span class="vm">__name__</span> <span class="o">==</span> <span class="s2">&quot;__main__&quot;</span><span class="p">:</span>
-</span><span id="L-259"><a href="#L-259"><span class="linenos">259</span></a>    <span class="n">main</span><span class="p">(</span><span class="n">get_args</span><span class="p">())</span>
+</span><span id="L-251"><a href="#L-251"><span class="linenos">251</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span>
+</span><span id="L-252"><a href="#L-252"><span class="linenos">252</span></a>            <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">sys</span><span class="o">.</span><span class="n">executable</span><span class="si">}</span><span class="s2"> -m pip install </span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="si">}</span><span class="s2"> --no-deps --upgrade --no-cache-dir&quot;</span>
+</span><span id="L-253"><a href="#L-253"><span class="linenos">253</span></a>        <span class="p">)</span>
+</span><span id="L-254"><a href="#L-254"><span class="linenos">254</span></a>
+</span><span id="L-255"><a href="#L-255"><span class="linenos">255</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">sync</span><span class="p">:</span>
+</span><span id="L-256"><a href="#L-256"><span class="linenos">256</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">pull</span><span class="p">(</span><span class="s2">&quot;--tags&quot;</span><span class="p">)</span>
+</span><span id="L-257"><a href="#L-257"><span class="linenos">257</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">push</span><span class="p">(</span><span class="s2">&quot;--tags&quot;</span><span class="p">)</span>
+</span><span id="L-258"><a href="#L-258"><span class="linenos">258</span></a>
+</span><span id="L-259"><a href="#L-259"><span class="linenos">259</span></a>
+</span><span id="L-260"><a href="#L-260"><span class="linenos">260</span></a><span class="k">if</span> <span class="vm">__name__</span> <span class="o">==</span> <span class="s2">&quot;__main__&quot;</span><span class="p">:</span>
+</span><span id="L-261"><a href="#L-261"><span class="linenos">261</span></a>    <span class="n">main</span><span class="p">(</span><span class="n">get_args</span><span class="p">())</span>
 </span></pre></div>
 
 
             </section>
                 <section id="get_args">
                             <input id="get_args-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
@@ -610,19 +612,21 @@
 </span><span id="main-245"><a href="#main-245"><span class="linenos">245</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">tag_version</span><span class="p">:</span>
 </span><span id="main-246"><a href="#main-246"><span class="linenos">246</span></a>        <span class="n">hassle_utilities</span><span class="o">.</span><span class="n">tag_version</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="p">)</span>
 </span><span id="main-247"><a href="#main-247"><span class="linenos">247</span></a>
 </span><span id="main-248"><a href="#main-248"><span class="linenos">248</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">publish</span><span class="p">:</span>
 </span><span id="main-249"><a href="#main-249"><span class="linenos">249</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;twine upload </span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">package</span> <span class="o">/</span> <span class="s1">&#39;dist&#39;</span> <span class="o">/</span> <span class="s1">&#39;*&#39;</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
 </span><span id="main-250"><a href="#main-250"><span class="linenos">250</span></a>
 </span><span id="main-251"><a href="#main-251"><span class="linenos">251</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">install</span><span class="p">:</span>
-</span><span id="main-252"><a href="#main-252"><span class="linenos">252</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;pip install </span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="si">}</span><span class="s2"> --no-deps --upgrade --no-cache-dir&quot;</span><span class="p">)</span>
-</span><span id="main-253"><a href="#main-253"><span class="linenos">253</span></a>
-</span><span id="main-254"><a href="#main-254"><span class="linenos">254</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">sync</span><span class="p">:</span>
-</span><span id="main-255"><a href="#main-255"><span class="linenos">255</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">pull</span><span class="p">(</span><span class="s2">&quot;--tags&quot;</span><span class="p">)</span>
-</span><span id="main-256"><a href="#main-256"><span class="linenos">256</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">push</span><span class="p">(</span><span class="s2">&quot;--tags&quot;</span><span class="p">)</span>
+</span><span id="main-252"><a href="#main-252"><span class="linenos">252</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span>
+</span><span id="main-253"><a href="#main-253"><span class="linenos">253</span></a>            <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">sys</span><span class="o">.</span><span class="n">executable</span><span class="si">}</span><span class="s2"> -m pip install </span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="si">}</span><span class="s2"> --no-deps --upgrade --no-cache-dir&quot;</span>
+</span><span id="main-254"><a href="#main-254"><span class="linenos">254</span></a>        <span class="p">)</span>
+</span><span id="main-255"><a href="#main-255"><span class="linenos">255</span></a>
+</span><span id="main-256"><a href="#main-256"><span class="linenos">256</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">sync</span><span class="p">:</span>
+</span><span id="main-257"><a href="#main-257"><span class="linenos">257</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">pull</span><span class="p">(</span><span class="s2">&quot;--tags&quot;</span><span class="p">)</span>
+</span><span id="main-258"><a href="#main-258"><span class="linenos">258</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">push</span><span class="p">(</span><span class="s2">&quot;--tags&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
     
 
                 </section>
     </main>
```

#### html2text {}

```diff
@@ -267,24 +267,26 @@
 244    if args.tag_version:
 245        hassle_utilities.tag_version(args.package)
 246
 247    if args.publish:
 248        os.system(f"twine upload {args.package / 'dist' / '*'}")
 249
 250    if args.install:
-251        os.system(f"pip install {args.package} --no-deps --upgrade --no-
-cache-dir")
-252
-253    if args.sync:
-254        git.pull("--tags")
-255        git.push("--tags")
-256
-257
-258if __name__ == "__main__":
-259    main(get_args())
+251        os.system(
+252            f"{sys.executable} -m pip install {args.package} --no-deps --
+upgrade --no-cache-dir"
+253        )
+254
+255    if args.sync:
+256        git.pull("--tags")
+257        git.push("--tags")
+258
+259
+260if __name__ == "__main__":
+261    main(get_args())
   ⁰
 def get_args() -> argparse.Namespace: View Source
 _17def get_args() -> argparse.Namespace:
 _18    parser = argparse.ArgumentParser()
 _19
 _20    parser.add_argument(
 _21        "package",
@@ -538,14 +540,16 @@
 245    if args.tag_version:
 246        hassle_utilities.tag_version(args.package)
 247
 248    if args.publish:
 249        os.system(f"twine upload {args.package / 'dist' / '*'}")
 250
 251    if args.install:
-252        os.system(f"pip install {args.package} --no-deps --upgrade --no-
-cache-dir")
-253
-254    if args.sync:
-255        git.pull("--tags")
-256        git.push("--tags")
+252        os.system(
+253            f"{sys.executable} -m pip install {args.package} --no-deps --
+upgrade --no-cache-dir"
+254        )
+255
+256    if args.sync:
+257        git.pull("--tags")
+258        git.push("--tags")
```

### Comparing `hassle-2.8.0/docs/hassle/hassle_config.html` & `hassle-2.8.1/docs/hassle/hassle_config.html`

 * *Files identical despite different names*

### Comparing `hassle-2.8.0/docs/hassle/hassle_utilities.html` & `hassle-2.8.1/docs/hassle/hassle_utilities.html`

 * *Files identical despite different names*

### Comparing `hassle-2.8.0/docs/hassle/new_project.html` & `hassle-2.8.1/docs/hassle/new_project.html`

 * *Files identical despite different names*

### Comparing `hassle-2.8.0/docs/hassle/run_tests.html` & `hassle-2.8.1/docs/hassle/run_tests.html`

 * *Files 0% similar despite different names*

```diff
@@ -57,64 +57,63 @@
 
                 
                         <input id="mod-run_tests-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 
                         <label class="view-source-button" for="mod-run_tests-view-source"><span>View Source</span></label>
 
                         <div class="pdoc-code codehilite"><pre><span></span><span id="L-1"><a href="#L-1"><span class="linenos"> 1</span></a><span class="kn">import</span> <span class="nn">argparse</span>
-</span><span id="L-2"><a href="#L-2"><span class="linenos"> 2</span></a><span class="kn">import</span> <span class="nn">os</span>
-</span><span id="L-3"><a href="#L-3"><span class="linenos"> 3</span></a>
-</span><span id="L-4"><a href="#L-4"><span class="linenos"> 4</span></a><span class="kn">import</span> <span class="nn">coverage</span>
-</span><span id="L-5"><a href="#L-5"><span class="linenos"> 5</span></a><span class="kn">import</span> <span class="nn">pytest</span>
-</span><span id="L-6"><a href="#L-6"><span class="linenos"> 6</span></a><span class="kn">from</span> <span class="nn">pathier</span> <span class="kn">import</span> <span class="n">Pathier</span>
+</span><span id="L-2"><a href="#L-2"><span class="linenos"> 2</span></a>
+</span><span id="L-3"><a href="#L-3"><span class="linenos"> 3</span></a><span class="kn">import</span> <span class="nn">coverage</span>
+</span><span id="L-4"><a href="#L-4"><span class="linenos"> 4</span></a><span class="kn">import</span> <span class="nn">pytest</span>
+</span><span id="L-5"><a href="#L-5"><span class="linenos"> 5</span></a><span class="kn">from</span> <span class="nn">pathier</span> <span class="kn">import</span> <span class="n">Pathier</span>
+</span><span id="L-6"><a href="#L-6"><span class="linenos"> 6</span></a>
 </span><span id="L-7"><a href="#L-7"><span class="linenos"> 7</span></a>
-</span><span id="L-8"><a href="#L-8"><span class="linenos"> 8</span></a>
-</span><span id="L-9"><a href="#L-9"><span class="linenos"> 9</span></a><span class="k">def</span> <span class="nf">get_args</span><span class="p">()</span> <span class="o">-&gt;</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span><span class="p">:</span>
-</span><span id="L-10"><a href="#L-10"><span class="linenos">10</span></a>    <span class="n">parser</span> <span class="o">=</span> <span class="n">argparse</span><span class="o">.</span><span class="n">ArgumentParser</span><span class="p">()</span>
-</span><span id="L-11"><a href="#L-11"><span class="linenos">11</span></a>
-</span><span id="L-12"><a href="#L-12"><span class="linenos">12</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="L-13"><a href="#L-13"><span class="linenos">13</span></a>        <span class="s2">&quot;package_name&quot;</span><span class="p">,</span>
-</span><span id="L-14"><a href="#L-14"><span class="linenos">14</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
-</span><span id="L-15"><a href="#L-15"><span class="linenos">15</span></a>        <span class="n">default</span><span class="o">=</span><span class="s2">&quot;.&quot;</span><span class="p">,</span>
-</span><span id="L-16"><a href="#L-16"><span class="linenos">16</span></a>        <span class="n">nargs</span><span class="o">=</span><span class="s2">&quot;?&quot;</span><span class="p">,</span>
-</span><span id="L-17"><a href="#L-17"><span class="linenos">17</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; The name of the package or project to run tests for,</span>
-</span><span id="L-18"><a href="#L-18"><span class="linenos">18</span></a><span class="s2">        assuming it&#39;s a subfolder of your current working directory.</span>
-</span><span id="L-19"><a href="#L-19"><span class="linenos">19</span></a><span class="s2">        Can also be a full path to the package. If nothing is given,</span>
-</span><span id="L-20"><a href="#L-20"><span class="linenos">20</span></a><span class="s2">        the current working directory will be used.&quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="L-21"><a href="#L-21"><span class="linenos">21</span></a>    <span class="p">)</span>
-</span><span id="L-22"><a href="#L-22"><span class="linenos">22</span></a>
-</span><span id="L-23"><a href="#L-23"><span class="linenos">23</span></a>    <span class="n">args</span> <span class="o">=</span> <span class="n">parser</span><span class="o">.</span><span class="n">parse_args</span><span class="p">()</span>
-</span><span id="L-24"><a href="#L-24"><span class="linenos">24</span></a>
-</span><span id="L-25"><a href="#L-25"><span class="linenos">25</span></a>    <span class="k">return</span> <span class="n">args</span>
+</span><span id="L-8"><a href="#L-8"><span class="linenos"> 8</span></a><span class="k">def</span> <span class="nf">get_args</span><span class="p">()</span> <span class="o">-&gt;</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span><span class="p">:</span>
+</span><span id="L-9"><a href="#L-9"><span class="linenos"> 9</span></a>    <span class="n">parser</span> <span class="o">=</span> <span class="n">argparse</span><span class="o">.</span><span class="n">ArgumentParser</span><span class="p">()</span>
+</span><span id="L-10"><a href="#L-10"><span class="linenos">10</span></a>
+</span><span id="L-11"><a href="#L-11"><span class="linenos">11</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="L-12"><a href="#L-12"><span class="linenos">12</span></a>        <span class="s2">&quot;package_name&quot;</span><span class="p">,</span>
+</span><span id="L-13"><a href="#L-13"><span class="linenos">13</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
+</span><span id="L-14"><a href="#L-14"><span class="linenos">14</span></a>        <span class="n">default</span><span class="o">=</span><span class="s2">&quot;.&quot;</span><span class="p">,</span>
+</span><span id="L-15"><a href="#L-15"><span class="linenos">15</span></a>        <span class="n">nargs</span><span class="o">=</span><span class="s2">&quot;?&quot;</span><span class="p">,</span>
+</span><span id="L-16"><a href="#L-16"><span class="linenos">16</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; The name of the package or project to run tests for,</span>
+</span><span id="L-17"><a href="#L-17"><span class="linenos">17</span></a><span class="s2">        assuming it&#39;s a subfolder of your current working directory.</span>
+</span><span id="L-18"><a href="#L-18"><span class="linenos">18</span></a><span class="s2">        Can also be a full path to the package. If nothing is given,</span>
+</span><span id="L-19"><a href="#L-19"><span class="linenos">19</span></a><span class="s2">        the current working directory will be used.&quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="L-20"><a href="#L-20"><span class="linenos">20</span></a>    <span class="p">)</span>
+</span><span id="L-21"><a href="#L-21"><span class="linenos">21</span></a>
+</span><span id="L-22"><a href="#L-22"><span class="linenos">22</span></a>    <span class="n">args</span> <span class="o">=</span> <span class="n">parser</span><span class="o">.</span><span class="n">parse_args</span><span class="p">()</span>
+</span><span id="L-23"><a href="#L-23"><span class="linenos">23</span></a>
+</span><span id="L-24"><a href="#L-24"><span class="linenos">24</span></a>    <span class="k">return</span> <span class="n">args</span>
+</span><span id="L-25"><a href="#L-25"><span class="linenos">25</span></a>
 </span><span id="L-26"><a href="#L-26"><span class="linenos">26</span></a>
-</span><span id="L-27"><a href="#L-27"><span class="linenos">27</span></a>
-</span><span id="L-28"><a href="#L-28"><span class="linenos">28</span></a><span class="k">def</span> <span class="nf">run_tests</span><span class="p">(</span><span class="n">package_path</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
-</span><span id="L-29"><a href="#L-29"><span class="linenos">29</span></a>    <span class="sd">&quot;&quot;&quot;Run tests with coverage and pytest.</span>
-</span><span id="L-30"><a href="#L-30"><span class="linenos">30</span></a>
-</span><span id="L-31"><a href="#L-31"><span class="linenos">31</span></a><span class="sd">    Returns True if all tests passed.&quot;&quot;&quot;</span>
-</span><span id="L-32"><a href="#L-32"><span class="linenos">32</span></a>    <span class="n">startdir</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">()</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span>
-</span><span id="L-33"><a href="#L-33"><span class="linenos">33</span></a>    <span class="n">package_path</span><span class="o">.</span><span class="n">mkcwd</span><span class="p">()</span>
-</span><span id="L-34"><a href="#L-34"><span class="linenos">34</span></a>    <span class="n">cover</span> <span class="o">=</span> <span class="n">coverage</span><span class="o">.</span><span class="n">Coverage</span><span class="p">()</span>
-</span><span id="L-35"><a href="#L-35"><span class="linenos">35</span></a>    <span class="n">cover</span><span class="o">.</span><span class="n">start</span><span class="p">()</span>
-</span><span id="L-36"><a href="#L-36"><span class="linenos">36</span></a>    <span class="n">results</span> <span class="o">=</span> <span class="n">pytest</span><span class="o">.</span><span class="n">main</span><span class="p">([</span><span class="s2">&quot;-s&quot;</span><span class="p">])</span>
-</span><span id="L-37"><a href="#L-37"><span class="linenos">37</span></a>    <span class="n">cover</span><span class="o">.</span><span class="n">stop</span><span class="p">()</span>
-</span><span id="L-38"><a href="#L-38"><span class="linenos">38</span></a>    <span class="n">cover</span><span class="o">.</span><span class="n">report</span><span class="p">()</span>
-</span><span id="L-39"><a href="#L-39"><span class="linenos">39</span></a>    <span class="n">startdir</span><span class="o">.</span><span class="n">mkcwd</span><span class="p">()</span>
-</span><span id="L-40"><a href="#L-40"><span class="linenos">40</span></a>    <span class="k">return</span> <span class="n">results</span> <span class="o">==</span> <span class="mi">0</span>
+</span><span id="L-27"><a href="#L-27"><span class="linenos">27</span></a><span class="k">def</span> <span class="nf">run_tests</span><span class="p">(</span><span class="n">package_path</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
+</span><span id="L-28"><a href="#L-28"><span class="linenos">28</span></a>    <span class="sd">&quot;&quot;&quot;Run tests with coverage and pytest.</span>
+</span><span id="L-29"><a href="#L-29"><span class="linenos">29</span></a>
+</span><span id="L-30"><a href="#L-30"><span class="linenos">30</span></a><span class="sd">    Returns True if all tests passed.&quot;&quot;&quot;</span>
+</span><span id="L-31"><a href="#L-31"><span class="linenos">31</span></a>    <span class="n">startdir</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">()</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span>
+</span><span id="L-32"><a href="#L-32"><span class="linenos">32</span></a>    <span class="n">package_path</span><span class="o">.</span><span class="n">mkcwd</span><span class="p">()</span>
+</span><span id="L-33"><a href="#L-33"><span class="linenos">33</span></a>    <span class="n">cover</span> <span class="o">=</span> <span class="n">coverage</span><span class="o">.</span><span class="n">Coverage</span><span class="p">()</span>
+</span><span id="L-34"><a href="#L-34"><span class="linenos">34</span></a>    <span class="n">cover</span><span class="o">.</span><span class="n">start</span><span class="p">()</span>
+</span><span id="L-35"><a href="#L-35"><span class="linenos">35</span></a>    <span class="n">results</span> <span class="o">=</span> <span class="n">pytest</span><span class="o">.</span><span class="n">main</span><span class="p">([</span><span class="s2">&quot;-s&quot;</span><span class="p">])</span>
+</span><span id="L-36"><a href="#L-36"><span class="linenos">36</span></a>    <span class="n">cover</span><span class="o">.</span><span class="n">stop</span><span class="p">()</span>
+</span><span id="L-37"><a href="#L-37"><span class="linenos">37</span></a>    <span class="n">cover</span><span class="o">.</span><span class="n">report</span><span class="p">()</span>
+</span><span id="L-38"><a href="#L-38"><span class="linenos">38</span></a>    <span class="n">startdir</span><span class="o">.</span><span class="n">mkcwd</span><span class="p">()</span>
+</span><span id="L-39"><a href="#L-39"><span class="linenos">39</span></a>    <span class="k">return</span> <span class="n">results</span> <span class="o">==</span> <span class="mi">0</span>
+</span><span id="L-40"><a href="#L-40"><span class="linenos">40</span></a>
 </span><span id="L-41"><a href="#L-41"><span class="linenos">41</span></a>
-</span><span id="L-42"><a href="#L-42"><span class="linenos">42</span></a>
-</span><span id="L-43"><a href="#L-43"><span class="linenos">43</span></a><span class="k">def</span> <span class="nf">main</span><span class="p">(</span><span class="n">args</span><span class="p">:</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span> <span class="o">=</span> <span class="kc">None</span><span class="p">):</span>
-</span><span id="L-44"><a href="#L-44"><span class="linenos">44</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="p">:</span>
-</span><span id="L-45"><a href="#L-45"><span class="linenos">45</span></a>        <span class="n">args</span> <span class="o">=</span> <span class="n">get_args</span><span class="p">()</span>
-</span><span id="L-46"><a href="#L-46"><span class="linenos">46</span></a>    <span class="n">package_path</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">package_name</span><span class="p">)</span><span class="o">.</span><span class="n">resolve</span><span class="p">()</span>
-</span><span id="L-47"><a href="#L-47"><span class="linenos">47</span></a>    <span class="n">run_tests</span><span class="p">(</span><span class="n">package_path</span><span class="p">)</span>
+</span><span id="L-42"><a href="#L-42"><span class="linenos">42</span></a><span class="k">def</span> <span class="nf">main</span><span class="p">(</span><span class="n">args</span><span class="p">:</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span> <span class="o">=</span> <span class="kc">None</span><span class="p">):</span>
+</span><span id="L-43"><a href="#L-43"><span class="linenos">43</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="p">:</span>
+</span><span id="L-44"><a href="#L-44"><span class="linenos">44</span></a>        <span class="n">args</span> <span class="o">=</span> <span class="n">get_args</span><span class="p">()</span>
+</span><span id="L-45"><a href="#L-45"><span class="linenos">45</span></a>    <span class="n">package_path</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">package_name</span><span class="p">)</span><span class="o">.</span><span class="n">resolve</span><span class="p">()</span>
+</span><span id="L-46"><a href="#L-46"><span class="linenos">46</span></a>    <span class="n">run_tests</span><span class="p">(</span><span class="n">package_path</span><span class="p">)</span>
+</span><span id="L-47"><a href="#L-47"><span class="linenos">47</span></a>
 </span><span id="L-48"><a href="#L-48"><span class="linenos">48</span></a>
-</span><span id="L-49"><a href="#L-49"><span class="linenos">49</span></a>
-</span><span id="L-50"><a href="#L-50"><span class="linenos">50</span></a><span class="k">if</span> <span class="vm">__name__</span> <span class="o">==</span> <span class="s2">&quot;__main__&quot;</span><span class="p">:</span>
-</span><span id="L-51"><a href="#L-51"><span class="linenos">51</span></a>    <span class="n">main</span><span class="p">(</span><span class="n">get_args</span><span class="p">())</span>
+</span><span id="L-49"><a href="#L-49"><span class="linenos">49</span></a><span class="k">if</span> <span class="vm">__name__</span> <span class="o">==</span> <span class="s2">&quot;__main__&quot;</span><span class="p">:</span>
+</span><span id="L-50"><a href="#L-50"><span class="linenos">50</span></a>    <span class="n">main</span><span class="p">(</span><span class="n">get_args</span><span class="p">())</span>
 </span></pre></div>
 
 
             </section>
                 <section id="get_args">
                             <input id="get_args-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
@@ -122,31 +121,31 @@
         <span class="def">def</span>
         <span class="name">get_args</span><span class="signature pdoc-code condensed">(<span class="return-annotation">) -> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span>:</span></span>
 
                 <label class="view-source-button" for="get_args-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#get_args"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="get_args-10"><a href="#get_args-10"><span class="linenos">10</span></a><span class="k">def</span> <span class="nf">get_args</span><span class="p">()</span> <span class="o">-&gt;</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span><span class="p">:</span>
-</span><span id="get_args-11"><a href="#get_args-11"><span class="linenos">11</span></a>    <span class="n">parser</span> <span class="o">=</span> <span class="n">argparse</span><span class="o">.</span><span class="n">ArgumentParser</span><span class="p">()</span>
-</span><span id="get_args-12"><a href="#get_args-12"><span class="linenos">12</span></a>
-</span><span id="get_args-13"><a href="#get_args-13"><span class="linenos">13</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="get_args-14"><a href="#get_args-14"><span class="linenos">14</span></a>        <span class="s2">&quot;package_name&quot;</span><span class="p">,</span>
-</span><span id="get_args-15"><a href="#get_args-15"><span class="linenos">15</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
-</span><span id="get_args-16"><a href="#get_args-16"><span class="linenos">16</span></a>        <span class="n">default</span><span class="o">=</span><span class="s2">&quot;.&quot;</span><span class="p">,</span>
-</span><span id="get_args-17"><a href="#get_args-17"><span class="linenos">17</span></a>        <span class="n">nargs</span><span class="o">=</span><span class="s2">&quot;?&quot;</span><span class="p">,</span>
-</span><span id="get_args-18"><a href="#get_args-18"><span class="linenos">18</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; The name of the package or project to run tests for,</span>
-</span><span id="get_args-19"><a href="#get_args-19"><span class="linenos">19</span></a><span class="s2">        assuming it&#39;s a subfolder of your current working directory.</span>
-</span><span id="get_args-20"><a href="#get_args-20"><span class="linenos">20</span></a><span class="s2">        Can also be a full path to the package. If nothing is given,</span>
-</span><span id="get_args-21"><a href="#get_args-21"><span class="linenos">21</span></a><span class="s2">        the current working directory will be used.&quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="get_args-22"><a href="#get_args-22"><span class="linenos">22</span></a>    <span class="p">)</span>
-</span><span id="get_args-23"><a href="#get_args-23"><span class="linenos">23</span></a>
-</span><span id="get_args-24"><a href="#get_args-24"><span class="linenos">24</span></a>    <span class="n">args</span> <span class="o">=</span> <span class="n">parser</span><span class="o">.</span><span class="n">parse_args</span><span class="p">()</span>
-</span><span id="get_args-25"><a href="#get_args-25"><span class="linenos">25</span></a>
-</span><span id="get_args-26"><a href="#get_args-26"><span class="linenos">26</span></a>    <span class="k">return</span> <span class="n">args</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="get_args-9"><a href="#get_args-9"><span class="linenos"> 9</span></a><span class="k">def</span> <span class="nf">get_args</span><span class="p">()</span> <span class="o">-&gt;</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span><span class="p">:</span>
+</span><span id="get_args-10"><a href="#get_args-10"><span class="linenos">10</span></a>    <span class="n">parser</span> <span class="o">=</span> <span class="n">argparse</span><span class="o">.</span><span class="n">ArgumentParser</span><span class="p">()</span>
+</span><span id="get_args-11"><a href="#get_args-11"><span class="linenos">11</span></a>
+</span><span id="get_args-12"><a href="#get_args-12"><span class="linenos">12</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="get_args-13"><a href="#get_args-13"><span class="linenos">13</span></a>        <span class="s2">&quot;package_name&quot;</span><span class="p">,</span>
+</span><span id="get_args-14"><a href="#get_args-14"><span class="linenos">14</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
+</span><span id="get_args-15"><a href="#get_args-15"><span class="linenos">15</span></a>        <span class="n">default</span><span class="o">=</span><span class="s2">&quot;.&quot;</span><span class="p">,</span>
+</span><span id="get_args-16"><a href="#get_args-16"><span class="linenos">16</span></a>        <span class="n">nargs</span><span class="o">=</span><span class="s2">&quot;?&quot;</span><span class="p">,</span>
+</span><span id="get_args-17"><a href="#get_args-17"><span class="linenos">17</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; The name of the package or project to run tests for,</span>
+</span><span id="get_args-18"><a href="#get_args-18"><span class="linenos">18</span></a><span class="s2">        assuming it&#39;s a subfolder of your current working directory.</span>
+</span><span id="get_args-19"><a href="#get_args-19"><span class="linenos">19</span></a><span class="s2">        Can also be a full path to the package. If nothing is given,</span>
+</span><span id="get_args-20"><a href="#get_args-20"><span class="linenos">20</span></a><span class="s2">        the current working directory will be used.&quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="get_args-21"><a href="#get_args-21"><span class="linenos">21</span></a>    <span class="p">)</span>
+</span><span id="get_args-22"><a href="#get_args-22"><span class="linenos">22</span></a>
+</span><span id="get_args-23"><a href="#get_args-23"><span class="linenos">23</span></a>    <span class="n">args</span> <span class="o">=</span> <span class="n">parser</span><span class="o">.</span><span class="n">parse_args</span><span class="p">()</span>
+</span><span id="get_args-24"><a href="#get_args-24"><span class="linenos">24</span></a>
+</span><span id="get_args-25"><a href="#get_args-25"><span class="linenos">25</span></a>    <span class="k">return</span> <span class="n">args</span>
 </span></pre></div>
 
 
     
 
                 </section>
                 <section id="run_tests">
@@ -156,27 +155,27 @@
         <span class="def">def</span>
         <span class="name">run_tests</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">package_path</span><span class="p">:</span> <span class="n">pathier</span><span class="o">.</span><span class="n">pathier</span><span class="o">.</span><span class="n">Pathier</span></span><span class="return-annotation">) -> <span class="nb">bool</span>:</span></span>
 
                 <label class="view-source-button" for="run_tests-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#run_tests"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="run_tests-29"><a href="#run_tests-29"><span class="linenos">29</span></a><span class="k">def</span> <span class="nf">run_tests</span><span class="p">(</span><span class="n">package_path</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
-</span><span id="run_tests-30"><a href="#run_tests-30"><span class="linenos">30</span></a>    <span class="sd">&quot;&quot;&quot;Run tests with coverage and pytest.</span>
-</span><span id="run_tests-31"><a href="#run_tests-31"><span class="linenos">31</span></a>
-</span><span id="run_tests-32"><a href="#run_tests-32"><span class="linenos">32</span></a><span class="sd">    Returns True if all tests passed.&quot;&quot;&quot;</span>
-</span><span id="run_tests-33"><a href="#run_tests-33"><span class="linenos">33</span></a>    <span class="n">startdir</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">()</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span>
-</span><span id="run_tests-34"><a href="#run_tests-34"><span class="linenos">34</span></a>    <span class="n">package_path</span><span class="o">.</span><span class="n">mkcwd</span><span class="p">()</span>
-</span><span id="run_tests-35"><a href="#run_tests-35"><span class="linenos">35</span></a>    <span class="n">cover</span> <span class="o">=</span> <span class="n">coverage</span><span class="o">.</span><span class="n">Coverage</span><span class="p">()</span>
-</span><span id="run_tests-36"><a href="#run_tests-36"><span class="linenos">36</span></a>    <span class="n">cover</span><span class="o">.</span><span class="n">start</span><span class="p">()</span>
-</span><span id="run_tests-37"><a href="#run_tests-37"><span class="linenos">37</span></a>    <span class="n">results</span> <span class="o">=</span> <span class="n">pytest</span><span class="o">.</span><span class="n">main</span><span class="p">([</span><span class="s2">&quot;-s&quot;</span><span class="p">])</span>
-</span><span id="run_tests-38"><a href="#run_tests-38"><span class="linenos">38</span></a>    <span class="n">cover</span><span class="o">.</span><span class="n">stop</span><span class="p">()</span>
-</span><span id="run_tests-39"><a href="#run_tests-39"><span class="linenos">39</span></a>    <span class="n">cover</span><span class="o">.</span><span class="n">report</span><span class="p">()</span>
-</span><span id="run_tests-40"><a href="#run_tests-40"><span class="linenos">40</span></a>    <span class="n">startdir</span><span class="o">.</span><span class="n">mkcwd</span><span class="p">()</span>
-</span><span id="run_tests-41"><a href="#run_tests-41"><span class="linenos">41</span></a>    <span class="k">return</span> <span class="n">results</span> <span class="o">==</span> <span class="mi">0</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="run_tests-28"><a href="#run_tests-28"><span class="linenos">28</span></a><span class="k">def</span> <span class="nf">run_tests</span><span class="p">(</span><span class="n">package_path</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
+</span><span id="run_tests-29"><a href="#run_tests-29"><span class="linenos">29</span></a>    <span class="sd">&quot;&quot;&quot;Run tests with coverage and pytest.</span>
+</span><span id="run_tests-30"><a href="#run_tests-30"><span class="linenos">30</span></a>
+</span><span id="run_tests-31"><a href="#run_tests-31"><span class="linenos">31</span></a><span class="sd">    Returns True if all tests passed.&quot;&quot;&quot;</span>
+</span><span id="run_tests-32"><a href="#run_tests-32"><span class="linenos">32</span></a>    <span class="n">startdir</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">()</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span>
+</span><span id="run_tests-33"><a href="#run_tests-33"><span class="linenos">33</span></a>    <span class="n">package_path</span><span class="o">.</span><span class="n">mkcwd</span><span class="p">()</span>
+</span><span id="run_tests-34"><a href="#run_tests-34"><span class="linenos">34</span></a>    <span class="n">cover</span> <span class="o">=</span> <span class="n">coverage</span><span class="o">.</span><span class="n">Coverage</span><span class="p">()</span>
+</span><span id="run_tests-35"><a href="#run_tests-35"><span class="linenos">35</span></a>    <span class="n">cover</span><span class="o">.</span><span class="n">start</span><span class="p">()</span>
+</span><span id="run_tests-36"><a href="#run_tests-36"><span class="linenos">36</span></a>    <span class="n">results</span> <span class="o">=</span> <span class="n">pytest</span><span class="o">.</span><span class="n">main</span><span class="p">([</span><span class="s2">&quot;-s&quot;</span><span class="p">])</span>
+</span><span id="run_tests-37"><a href="#run_tests-37"><span class="linenos">37</span></a>    <span class="n">cover</span><span class="o">.</span><span class="n">stop</span><span class="p">()</span>
+</span><span id="run_tests-38"><a href="#run_tests-38"><span class="linenos">38</span></a>    <span class="n">cover</span><span class="o">.</span><span class="n">report</span><span class="p">()</span>
+</span><span id="run_tests-39"><a href="#run_tests-39"><span class="linenos">39</span></a>    <span class="n">startdir</span><span class="o">.</span><span class="n">mkcwd</span><span class="p">()</span>
+</span><span id="run_tests-40"><a href="#run_tests-40"><span class="linenos">40</span></a>    <span class="k">return</span> <span class="n">results</span> <span class="o">==</span> <span class="mi">0</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Run tests with coverage and pytest.</p>
 
 <p>Returns True if all tests passed.</p>
 </div>
@@ -190,19 +189,19 @@
         <span class="def">def</span>
         <span class="name">main</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">args</span><span class="p">:</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span> <span class="o">=</span> <span class="kc">None</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="main-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#main"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="main-44"><a href="#main-44"><span class="linenos">44</span></a><span class="k">def</span> <span class="nf">main</span><span class="p">(</span><span class="n">args</span><span class="p">:</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span> <span class="o">=</span> <span class="kc">None</span><span class="p">):</span>
-</span><span id="main-45"><a href="#main-45"><span class="linenos">45</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="p">:</span>
-</span><span id="main-46"><a href="#main-46"><span class="linenos">46</span></a>        <span class="n">args</span> <span class="o">=</span> <span class="n">get_args</span><span class="p">()</span>
-</span><span id="main-47"><a href="#main-47"><span class="linenos">47</span></a>    <span class="n">package_path</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">package_name</span><span class="p">)</span><span class="o">.</span><span class="n">resolve</span><span class="p">()</span>
-</span><span id="main-48"><a href="#main-48"><span class="linenos">48</span></a>    <span class="n">run_tests</span><span class="p">(</span><span class="n">package_path</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="main-43"><a href="#main-43"><span class="linenos">43</span></a><span class="k">def</span> <span class="nf">main</span><span class="p">(</span><span class="n">args</span><span class="p">:</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span> <span class="o">=</span> <span class="kc">None</span><span class="p">):</span>
+</span><span id="main-44"><a href="#main-44"><span class="linenos">44</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="p">:</span>
+</span><span id="main-45"><a href="#main-45"><span class="linenos">45</span></a>        <span class="n">args</span> <span class="o">=</span> <span class="n">get_args</span><span class="p">()</span>
+</span><span id="main-46"><a href="#main-46"><span class="linenos">46</span></a>    <span class="n">package_path</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">package_name</span><span class="p">)</span><span class="o">.</span><span class="n">resolve</span><span class="p">()</span>
+</span><span id="main-47"><a href="#main-47"><span class="linenos">47</span></a>    <span class="n">run_tests</span><span class="p">(</span><span class="n">package_path</span><span class="p">)</span>
 </span></pre></div>
 
 
     
 
                 </section>
     </main>
```

#### html2text {}

```diff
@@ -7,21 +7,65 @@
     * run_tests
     * main
 built_with_pdoc[pdoc_logo]
 
 ****** hassle.run_tests ******
 ⁰ View Source
 _1import argparse
-_2import os
-_3
-_4import coverage
-_5import pytest
-_6from pathier import Pathier
+_2
+_3import coverage
+_4import pytest
+_5from pathier import Pathier
+_6
 _7
-_8
+_8def get_args() -> argparse.Namespace:
+_9    parser = argparse.ArgumentParser()
+10
+11    parser.add_argument(
+12        "package_name",
+13        type=str,
+14        default=".",
+15        nargs="?",
+16        help=""" The name of the package or project to run tests for,
+17        assuming it's a subfolder of your current working directory.
+18        Can also be a full path to the package. If nothing is given,
+19        the current working directory will be used.""",
+20    )
+21
+22    args = parser.parse_args()
+23
+24    return args
+25
+26
+27def run_tests(package_path: Pathier) -> bool:
+28    """Run tests with coverage and pytest.
+29
+30    Returns True if all tests passed."""
+31    startdir = Pathier().cwd()
+32    package_path.mkcwd()
+33    cover = coverage.Coverage()
+34    cover.start()
+35    results = pytest.main(["-s"])
+36    cover.stop()
+37    cover.report()
+38    startdir.mkcwd()
+39    return results == 0
+40
+41
+42def main(args: argparse.Namespace = None):
+43    if not args:
+44        args = get_args()
+45    package_path = Pathier(args.package_name).resolve()
+46    run_tests(package_path)
+47
+48
+49if __name__ == "__main__":
+50    main(get_args())
+  ⁰
+def get_args() -> argparse.Namespace: View Source
 _9def get_args() -> argparse.Namespace:
 10    parser = argparse.ArgumentParser()
 11
 12    parser.add_argument(
 13        "package_name",
 14        type=str,
 15        default=".",
@@ -31,77 +75,32 @@
 19        Can also be a full path to the package. If nothing is given,
 20        the current working directory will be used.""",
 21    )
 22
 23    args = parser.parse_args()
 24
 25    return args
-26
-27
+  ⁰
+def run_tests(package_path: pathier.pathier.Pathier) -> bool: View Source
 28def run_tests(package_path: Pathier) -> bool:
 29    """Run tests with coverage and pytest.
 30
 31    Returns True if all tests passed."""
 32    startdir = Pathier().cwd()
 33    package_path.mkcwd()
 34    cover = coverage.Coverage()
 35    cover.start()
 36    results = pytest.main(["-s"])
 37    cover.stop()
 38    cover.report()
 39    startdir.mkcwd()
 40    return results == 0
-41
-42
+Run tests with coverage and pytest.
+Returns True if all tests passed.
+  ⁰
+def main(args: argparse.Namespace = None): View Source
 43def main(args: argparse.Namespace = None):
 44    if not args:
 45        args = get_args()
 46    package_path = Pathier(args.package_name).resolve()
 47    run_tests(package_path)
-48
-49
-50if __name__ == "__main__":
-51    main(get_args())
-  ⁰
-def get_args() -> argparse.Namespace: View Source
-10def get_args() -> argparse.Namespace:
-11    parser = argparse.ArgumentParser()
-12
-13    parser.add_argument(
-14        "package_name",
-15        type=str,
-16        default=".",
-17        nargs="?",
-18        help=""" The name of the package or project to run tests for,
-19        assuming it's a subfolder of your current working directory.
-20        Can also be a full path to the package. If nothing is given,
-21        the current working directory will be used.""",
-22    )
-23
-24    args = parser.parse_args()
-25
-26    return args
-  ⁰
-def run_tests(package_path: pathier.pathier.Pathier) -> bool: View Source
-29def run_tests(package_path: Pathier) -> bool:
-30    """Run tests with coverage and pytest.
-31
-32    Returns True if all tests passed."""
-33    startdir = Pathier().cwd()
-34    package_path.mkcwd()
-35    cover = coverage.Coverage()
-36    cover.start()
-37    results = pytest.main(["-s"])
-38    cover.stop()
-39    cover.report()
-40    startdir.mkcwd()
-41    return results == 0
-Run tests with coverage and pytest.
-Returns True if all tests passed.
-  ⁰
-def main(args: argparse.Namespace = None): View Source
-44def main(args: argparse.Namespace = None):
-45    if not args:
-46        args = get_args()
-47    package_path = Pathier(args.package_name).resolve()
-48    run_tests(package_path)
```

### Comparing `hassle-2.8.0/src/hassle/generate_tests.py` & `hassle-2.8.1/src/hassle/generate_tests.py`

 * *Files identical despite different names*

### Comparing `hassle-2.8.0/src/hassle/hassle.py` & `hassle-2.8.1/src/hassle/hassle.py`

 * *Files 2% similar despite different names*

```diff
@@ -244,15 +244,17 @@
     if args.tag_version:
         hassle_utilities.tag_version(args.package)
 
     if args.publish:
         os.system(f"twine upload {args.package / 'dist' / '*'}")
 
     if args.install:
-        os.system(f"pip install {args.package} --no-deps --upgrade --no-cache-dir")
+        os.system(
+            f"{sys.executable} -m pip install {args.package} --no-deps --upgrade --no-cache-dir"
+        )
 
     if args.sync:
         git.pull("--tags")
         git.push("--tags")
 
 
 if __name__ == "__main__":
```

### Comparing `hassle-2.8.0/src/hassle/hassle_config.py` & `hassle-2.8.1/src/hassle/hassle_config.py`

 * *Files identical despite different names*

### Comparing `hassle-2.8.0/src/hassle/hassle_utilities.py` & `hassle-2.8.1/src/hassle/hassle_utilities.py`

 * *Files identical despite different names*

### Comparing `hassle-2.8.0/src/hassle/license_template.txt` & `hassle-2.8.1/src/hassle/license_template.txt`

 * *Files identical despite different names*

### Comparing `hassle-2.8.0/src/hassle/new_project.py` & `hassle-2.8.1/src/hassle/new_project.py`

 * *Files identical despite different names*

### Comparing `hassle-2.8.0/src/hassle/pyproject_template.toml` & `hassle-2.8.1/src/hassle/pyproject_template.toml`

 * *Files identical despite different names*

### Comparing `hassle-2.8.0/src/hassle/run_tests.py` & `hassle-2.8.1/src/hassle/run_tests.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import argparse
-import os
 
 import coverage
 import pytest
 from pathier import Pathier
 
 
 def get_args() -> argparse.Namespace:
```

### Comparing `hassle-2.8.0/LICENSE.txt` & `hassle-2.8.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hassle-2.8.0/README.md` & `hassle-2.8.1/README.md`

 * *Files identical despite different names*

### Comparing `hassle-2.8.0/pyproject.toml` & `hassle-2.8.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 00000090: 226d 6174 746d 616e 6573 4070 6d2e 6d65  "mattmanes@pm.me
 000000a0: 227d 5d0d 0a64 6573 6372 6970 7469 6f6e  "}]..description
 000000b0: 203d 2022 4372 6561 7465 2c20 6275 696c   = "Create, buil
 000000c0: 642c 2074 6573 742c 2061 6e64 2070 7562  d, test, and pub
 000000d0: 6c69 7368 2050 7974 686f 6e20 7072 6f6a  lish Python proj
 000000e0: 6563 7473 2061 6e64 2070 6163 6b61 6765  ects and package
 000000f0: 732e 220d 0a76 6572 7369 6f6e 203d 2022  s."..version = "
-00000100: 322e 382e 3022 0d0a 7265 7175 6972 6573  2.8.0"..requires
+00000100: 322e 382e 3122 0d0a 7265 7175 6972 6573  2.8.1"..requires
 00000110: 2d70 7974 686f 6e20 3d20 223e 3d33 2e31  -python = ">=3.1
 00000120: 3022 0d0a 6465 7065 6e64 656e 6369 6573  0"..dependencies
 00000130: 203d 205b 0d0a 2020 2020 2262 6c61 636b   = [..    "black
 00000140: 222c 200d 0a20 2020 2022 6973 6f72 7422  ", ..    "isort"
 00000150: 2c20 0d0a 2020 2020 2270 7974 6573 747e  , ..    "pytest~
 00000160: 3d37 2e32 2e31 222c 200d 0a20 2020 2022  =7.2.1", ..    "
 00000170: 636f 7665 7261 6765 222c 0d0a 2020 2020  coverage",..
```

### Comparing `hassle-2.8.0/PKG-INFO` & `hassle-2.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hassle
-Version: 2.8.0
+Version: 2.8.1
 Summary: Create, build, test, and publish Python projects and packages.
 Project-URL: Homepage, https://github.com/matt-manes/hassle
 Project-URL: Documentation, https://github.com/matt-manes/hassle/tree/main/docs
 Project-URL: Source code, https://github.com/matt-manes/hassle/tree/main/src/hassle
 Author-email: Matt Manes <mattmanes@pm.me>
 License-File: LICENSE.txt
 Keywords: automation,build,devops,packaging,test
```

