# Comparing `tmp/jupyterlab_celltagsclasses-0.1.2.tar.gz` & `tmp/jupyterlab_celltagsclasses-0.2.0.tar.gz`

## Comparing `jupyterlab_celltagsclasses-0.1.2.tar` & `jupyterlab_celltagsclasses-0.2.0.tar`

### file list

```diff
@@ -1,117 +1,48 @@
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/.editorconfig
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/.eslintignore
--rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/.eslintrc.js
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/.gitattributes
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/.prettierignore
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/.prettierrc
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/.stylelintrc
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/.yarnrc.yml
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/CHANGELOG.md
--rw-r--r--   0        0        0     2134 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/RELEASE.md
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/install.json
--rw-r--r--   0        0        0     3536 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/package.json
--rwxr-xr-x   0        0        0      854 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/release.sh
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/requirements.txt
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/setup.py
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/tsconfig.json
--rw-r--r--   0        0        0   208796 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/yarn.lock
--rw-r--r--   0        0        0     2484 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/examples/test.ipynb
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/__init__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/_version.py
--rw-r--r--   0        0        0    21236 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/build_log.json
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/install.json
--rw-r--r--   0        0        0     3678 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/package.json
--rw-r--r--   0        0        0     6367 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/lib_index_js.69027069f0720bba2d30.js
--rw-r--r--   0        0        0     6331 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/lib_index_js.69027069f0720bba2d30.js.map
--rw-r--r--   0        0        0     6367 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/lib_index_js.745b7b07e91b136d36b8.js
--rw-r--r--   0        0        0     8238 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/lib_index_js.745b7b07e91b136d36b8.js.map
--rw-r--r--   0        0        0     6351 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/lib_index_js.e0bf585461963e3d1e28.js
--rw-r--r--   0        0        0     6314 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/lib_index_js.e0bf585461963e3d1e28.js.map
--rw-r--r--   0        0        0    27528 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/remoteEntry.09eb75b8b35017dd61cc.js
--rw-r--r--   0        0        0    26437 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/remoteEntry.09eb75b8b35017dd61cc.js.map
--rw-r--r--   0        0        0    26437 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/remoteEntry.0a4c39b501971c60ffd2.js.map
--rw-r--r--   0        0        0    27528 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/remoteEntry.121544801bc433e00240.js
--rw-r--r--   0        0        0    26437 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/remoteEntry.121544801bc433e00240.js.map
--rw-r--r--   0        0        0    26437 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/remoteEntry.170c8a935f39cb9518d6.js.map
--rw-r--r--   0        0        0    26437 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/remoteEntry.17f7467f156319c755c0.js.map
--rw-r--r--   0        0        0    26437 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/remoteEntry.1849839b62edee24aec8.js.map
--rw-r--r--   0        0        0    26437 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/remoteEntry.22ac66fc46652f220c02.js.map
--rw-r--r--   0        0        0    26437 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/remoteEntry.4fc7106cb22143a5fce6.js.map
--rw-r--r--   0        0        0    26437 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/remoteEntry.586ed0a7209176557f21.js.map
--rw-r--r--   0        0        0    26437 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/remoteEntry.666f3bf51bf09fc5bf7f.js.map
--rw-r--r--   0        0        0    26437 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/remoteEntry.6cbab8277822394dfb29.js.map
--rw-r--r--   0        0        0    26437 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/remoteEntry.933bc9f561b8ebc92287.js.map
--rw-r--r--   0        0        0    26437 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/remoteEntry.9728aad82475f1fe62ea.js.map
--rw-r--r--   0        0        0    26437 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/remoteEntry.a58905825d751323be61.js.map
--rw-r--r--   0        0        0    26437 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/remoteEntry.b24f4403982fe69ad690.js.map
--rw-r--r--   0        0        0    26437 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/remoteEntry.b3482340b7d50da9319c.js.map
--rw-r--r--   0        0        0    26437 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/remoteEntry.bdfe1655a685cae2eb10.js.map
--rw-r--r--   0        0        0    26437 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/remoteEntry.c07b230f1f57c9e89481.js.map
--rw-r--r--   0        0        0    26446 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/remoteEntry.c33d2bfa2fdbc5139570.js.map
--rw-r--r--   0        0        0    26437 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/remoteEntry.c848fd19f30b6f3af7d6.js.map
--rw-r--r--   0        0        0    26437 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/remoteEntry.d1d5567cd1ed4013c60b.js.map
--rw-r--r--   0        0        0    26437 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/remoteEntry.d347944507729fb1c1d2.js.map
--rw-r--r--   0        0        0    26437 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/remoteEntry.db28ad9a76e4c9f2ecb5.js.map
--rw-r--r--   0        0        0    26437 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/remoteEntry.dc9b6438cba1062a18bd.js.map
--rw-r--r--   0        0        0    26437 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/remoteEntry.e631040c6c782fc048c3.js.map
--rw-r--r--   0        0        0    26437 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/remoteEntry.e6d891cc83354cb06c15.js.map
--rw-r--r--   0        0        0    26437 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/remoteEntry.fb379948d6ce49efaa3b.js.map
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/style.js
--rw-r--r--   0        0        0    20480 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/style_index_js.012e4d3162293b291168.js
--rw-r--r--   0        0        0    16223 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/style_index_js.012e4d3162293b291168.js.map
--rw-r--r--   0        0        0    20499 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/style_index_js.0e23ae348872f42dfa7e.js
--rw-r--r--   0        0        0    16245 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/style_index_js.0e23ae348872f42dfa7e.js.map
--rw-r--r--   0        0        0    20292 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/style_index_js.1db0f3b8d794741b4cb4.js
--rw-r--r--   0        0        0    16022 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/style_index_js.1db0f3b8d794741b4cb4.js.map
--rw-r--r--   0        0        0    20495 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/style_index_js.2d159db83d8284e0cf12.js
--rw-r--r--   0        0        0    16239 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/style_index_js.2d159db83d8284e0cf12.js.map
--rw-r--r--   0        0        0    20485 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/style_index_js.33fc960cbf5aa7e756d6.js
--rw-r--r--   0        0        0    16233 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/style_index_js.33fc960cbf5aa7e756d6.js.map
--rw-r--r--   0        0        0    20542 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/style_index_js.447299cd6bd7a4db7267.js
--rw-r--r--   0        0        0    16284 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/style_index_js.447299cd6bd7a4db7267.js.map
--rw-r--r--   0        0        0    20494 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/style_index_js.4784725fff15b54ffe3d.js
--rw-r--r--   0        0        0    16237 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/style_index_js.4784725fff15b54ffe3d.js.map
--rw-r--r--   0        0        0    20485 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/style_index_js.50300ed39417ed24f985.js
--rw-r--r--   0        0        0    16229 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/style_index_js.50300ed39417ed24f985.js.map
--rw-r--r--   0        0        0    20290 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/style_index_js.52cce799d0432472b152.js
--rw-r--r--   0        0        0    16020 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/style_index_js.52cce799d0432472b152.js.map
--rw-r--r--   0        0        0    14877 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/style_index_js.64ac856d9dbfdba5f5c7.js
--rw-r--r--   0        0        0     9957 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/style_index_js.64ac856d9dbfdba5f5c7.js.map
--rw-r--r--   0        0        0    20486 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/style_index_js.6d05dad2bd11f4949416.js
--rw-r--r--   0        0        0    16224 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/style_index_js.6d05dad2bd11f4949416.js.map
--rw-r--r--   0        0        0    20490 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/style_index_js.8484ad0db61e328da5f5.js
--rw-r--r--   0        0        0    16236 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/style_index_js.8484ad0db61e328da5f5.js.map
--rw-r--r--   0        0        0    20484 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/style_index_js.951d4f88d7f9cc18fa51.js
--rw-r--r--   0        0        0    16227 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/style_index_js.951d4f88d7f9cc18fa51.js.map
--rw-r--r--   0        0        0    20418 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/style_index_js.a23abff9382042ed82e8.js
--rw-r--r--   0        0        0    16154 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/style_index_js.a23abff9382042ed82e8.js.map
--rw-r--r--   0        0        0    20312 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/style_index_js.af71ef0579110bcfe1ab.js
--rw-r--r--   0        0        0    16042 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/style_index_js.af71ef0579110bcfe1ab.js.map
--rw-r--r--   0        0        0    20541 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/style_index_js.b48473261159e6e27fea.js
--rw-r--r--   0        0        0    16281 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/style_index_js.b48473261159e6e27fea.js.map
--rw-r--r--   0        0        0    20378 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/style_index_js.c13f242cce861218e3cf.js
--rw-r--r--   0        0        0    16115 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/style_index_js.c13f242cce861218e3cf.js.map
--rw-r--r--   0        0        0    20440 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/style_index_js.c59e15e049f3a009d4a2.js
--rw-r--r--   0        0        0    16176 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/style_index_js.c59e15e049f3a009d4a2.js.map
--rw-r--r--   0        0        0    20491 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/style_index_js.c804bc222706d3cf7bec.js
--rw-r--r--   0        0        0    16235 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/style_index_js.c804bc222706d3cf7bec.js.map
--rw-r--r--   0        0        0    20494 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/style_index_js.d3e9571212d458ccc458.js
--rw-r--r--   0        0        0    16240 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/style_index_js.d3e9571212d458ccc458.js.map
--rw-r--r--   0        0        0    20546 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/style_index_js.dcf32fced0a182594cc6.js
--rw-r--r--   0        0        0    16288 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/style_index_js.dcf32fced0a182594cc6.js.map
--rw-r--r--   0        0        0    20494 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/style_index_js.df6561a0531b63f9a29b.js
--rw-r--r--   0        0        0    16238 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/style_index_js.df6561a0531b63f9a29b.js.map
--rw-r--r--   0        0        0    20490 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/style_index_js.ee239d110f5f639974dc.js
--rw-r--r--   0        0        0    16232 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/style_index_js.ee239d110f5f639974dc.js.map
--rw-r--r--   0        0        0    20474 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/style_index_js.f7b2683e356c1be8a8ed.js
--rw-r--r--   0        0        0    16212 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/style_index_js.f7b2683e356c1be8a8ed.js.map
--rw-r--r--   0        0        0    54944 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/media/screenshot.png
--rw-r--r--   0        0        0     4491 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/src/index.ts
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/style/base.css
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/style/index.css
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/style/index.js
--rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/.gitignore
--rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/LICENSE
--rw-r--r--   0        0        0     2177 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/README.md
--rw-r--r--   0        0        0     2405 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     5095 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.2.0/.editorconfig
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.2.0/.eslintignore
+-rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.2.0/.eslintrc.js
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.2.0/.gitattributes
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.2.0/.prettierignore
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.2.0/.prettierrc
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.2.0/.stylelintrc
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.2.0/.yarnrc.yml
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.2.0/CHANGELOG.md
+-rw-r--r--   0        0        0     2134 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.2.0/RELEASE.md
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.2.0/install.json
+-rw-r--r--   0        0        0     3536 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.2.0/package.json
+-rw-r--r--   0        0        0     3536 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.2.0/package.json.version
+-rwxr-xr-x   0        0        0      813 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.2.0/release.sh
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.2.0/requirements.txt
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.2.0/setup.py
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.2.0/tsconfig.json
+-rw-r--r--   0        0        0   208796 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.2.0/yarn.lock
+-rw-r--r--   0        0        0     2483 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.2.0/examples/test.ipynb
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.2.0/jupyterlab_celltagsclasses/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.2.0/jupyterlab_celltagsclasses/_version.py
+-rw-r--r--   0        0        0    21418 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.2.0/jupyterlab_celltagsclasses/labextension/build_log.json
+-rw-r--r--   0        0        0     3678 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.2.0/jupyterlab_celltagsclasses/labextension/package.json
+-rw-r--r--   0        0        0    22882 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.2.0/jupyterlab_celltagsclasses/labextension/static/lib_index_js.cddacca2ba0e6c761c6d.js
+-rw-r--r--   0        0        0    22193 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.2.0/jupyterlab_celltagsclasses/labextension/static/lib_index_js.cddacca2ba0e6c761c6d.js.map
+-rw-r--r--   0        0        0     6351 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.2.0/jupyterlab_celltagsclasses/labextension/static/lib_index_js.e0bf585461963e3d1e28.js
+-rw-r--r--   0        0        0     6314 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.2.0/jupyterlab_celltagsclasses/labextension/static/lib_index_js.e0bf585461963e3d1e28.js.map
+-rw-r--r--   0        0        0    26439 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.2.0/jupyterlab_celltagsclasses/labextension/static/remoteEntry.cc30540db9a44cea877f.js.map
+-rw-r--r--   0        0        0    27740 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.2.0/jupyterlab_celltagsclasses/labextension/static/remoteEntry.e8bcb578ed91b775bd99.js
+-rw-r--r--   0        0        0    26652 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.2.0/jupyterlab_celltagsclasses/labextension/static/remoteEntry.e8bcb578ed91b775bd99.js.map
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.2.0/jupyterlab_celltagsclasses/labextension/static/style.js
+-rw-r--r--   0        0        0    20494 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.2.0/jupyterlab_celltagsclasses/labextension/static/style_index_js.4784725fff15b54ffe3d.js
+-rw-r--r--   0        0        0    16237 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.2.0/jupyterlab_celltagsclasses/labextension/static/style_index_js.4784725fff15b54ffe3d.js.map
+-rw-r--r--   0        0        0    54944 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.2.0/media/screenshot.png
+-rw-r--r--   0        0        0     4636 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.2.0/src/index.ts
+-rw-r--r--   0        0        0     5897 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.2.0/src/metadata.ts
+-rw-r--r--   0        0        0     5491 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.2.0/src/xpath-test.js
+-rw-r--r--   0        0        0     4774 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.2.0/src/xpath-test.ts
+-rw-r--r--   0        0        0     7428 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.2.0/src/xpath.js
+-rw-r--r--   0        0        0     5991 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.2.0/src/xpath.ts
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.2.0/style/base.css
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.2.0/style/index.css
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.2.0/style/index.js
+-rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2791 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.2.0/README.md
+-rw-r--r--   0        0        0     2405 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     5709 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.2.0/PKG-INFO
```

### Comparing `jupyterlab_celltagsclasses-0.1.2/.eslintrc.js` & `jupyterlab_celltagsclasses-0.2.0/.eslintrc.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_celltagsclasses-0.1.2/RELEASE.md` & `jupyterlab_celltagsclasses-0.2.0/RELEASE.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_celltagsclasses-0.1.2/package.json` & `jupyterlab_celltagsclasses-0.2.0/package.json.version`

 * *Files identical despite different names*

### Comparing `jupyterlab_celltagsclasses-0.1.2/tsconfig.json` & `jupyterlab_celltagsclasses-0.2.0/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_celltagsclasses-0.1.2/yarn.lock` & `jupyterlab_celltagsclasses-0.2.0/yarn.lock`

 * *Files identical despite different names*

### Comparing `jupyterlab_celltagsclasses-0.1.2/examples/test.ipynb` & `jupyterlab_celltagsclasses-0.2.0/examples/test.ipynb`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9985119047619048%*

 * *Differences: {"'metadata'": "{'language_info': {'version': '3.11.3'}}"}*

```diff
@@ -117,15 +117,15 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.10"
+            "version": "3.11.3"
         },
         "toc": {
             "base_numbering": 1
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
```

### Comparing `jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/build_log.json` & `jupyterlab_celltagsclasses-0.2.0/jupyterlab_celltagsclasses/labextension/build_log.json`

 * *Files 17% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999211907776723%*

 * *Differences: {'0': "{'plugins': {1: {'_options': {'shared': {'@jupyterlab/application': {'requiredVersion': "*

 * *      "'^4.0.0-beta.2'}, '@jupyterlab/application-extension': {'requiredVersion': "*

 * *      "'^4.0.0-beta.2'}, '@jupyterlab/apputils-extension': {'requiredVersion': '^4.0.0-beta.2'}, "*

 * *      "'@jupyterlab/cell-toolbar-extension': {'requiredVersion': '^4.0.0-beta.2'}, "*

 * *      "'@jupyterlab/celltags-extension': {'requiredVersion': '^4.0.0-beta.2'}, "*

 * *      "'@jupyterlab/codemirror-extension': {'requiredVersion': '^4 […]*

```diff
@@ -136,415 +136,415 @@
                         "@jupyter/ydoc": {
                             "import": false,
                             "requiredVersion": "^1.0.2",
                             "singleton": true
                         },
                         "@jupyterlab/application": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-rc.0",
+                            "requiredVersion": "^4.0.0-beta.2",
                             "singleton": true
                         },
                         "@jupyterlab/application-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-rc.0"
+                            "requiredVersion": "^4.0.0-beta.2"
                         },
                         "@jupyterlab/apputils": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-rc.0",
+                            "requiredVersion": "^4.0.0-beta.2",
                             "singleton": true
                         },
                         "@jupyterlab/apputils-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-rc.0"
+                            "requiredVersion": "^4.0.0-beta.2"
                         },
                         "@jupyterlab/attachments": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-rc.0"
+                            "requiredVersion": "^4.0.0-beta.2"
                         },
                         "@jupyterlab/cell-toolbar": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-rc.0",
+                            "requiredVersion": "^4.0.0-beta.2",
                             "singleton": true
                         },
                         "@jupyterlab/cell-toolbar-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-rc.0"
+                            "requiredVersion": "^4.0.0-beta.2"
                         },
                         "@jupyterlab/cells": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-rc.0"
+                            "requiredVersion": "^4.0.0-beta.2"
                         },
                         "@jupyterlab/celltags": {
                             "import": false,
                             "requiredVersion": "^4.0.0-alpha.20"
                         },
                         "@jupyterlab/celltags-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-rc.0"
+                            "requiredVersion": "^4.0.0-beta.2"
                         },
                         "@jupyterlab/codeeditor": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-rc.0",
+                            "requiredVersion": "^4.0.0-beta.2",
                             "singleton": true
                         },
                         "@jupyterlab/codemirror": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-rc.0",
+                            "requiredVersion": "^4.0.0-beta.2",
                             "singleton": true
                         },
                         "@jupyterlab/codemirror-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-rc.0"
+                            "requiredVersion": "^4.0.0-beta.2"
                         },
                         "@jupyterlab/completer": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-rc.0",
+                            "requiredVersion": "^4.0.0-beta.2",
                             "singleton": true
                         },
                         "@jupyterlab/completer-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-rc.0"
+                            "requiredVersion": "^4.0.0-beta.2"
                         },
                         "@jupyterlab/console": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-rc.0",
+                            "requiredVersion": "^4.0.0-beta.2",
                             "singleton": true
                         },
                         "@jupyterlab/console-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-rc.0"
+                            "requiredVersion": "^4.0.0-beta.2"
                         },
                         "@jupyterlab/coreutils": {
                             "import": false,
-                            "requiredVersion": "^6.0.0-rc.0",
+                            "requiredVersion": "^6.0.0-beta.2",
                             "singleton": true
                         },
                         "@jupyterlab/csvviewer": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-rc.0"
+                            "requiredVersion": "^4.0.0-beta.2"
                         },
                         "@jupyterlab/csvviewer-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-rc.0"
+                            "requiredVersion": "^4.0.0-beta.2"
                         },
                         "@jupyterlab/debugger": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-rc.0",
+                            "requiredVersion": "^4.0.0-beta.2",
                             "singleton": true
                         },
                         "@jupyterlab/debugger-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-rc.0"
+                            "requiredVersion": "^4.0.0-beta.2"
                         },
                         "@jupyterlab/docmanager": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-rc.0",
+                            "requiredVersion": "^4.0.0-beta.2",
                             "singleton": true
                         },
                         "@jupyterlab/docmanager-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-rc.0"
+                            "requiredVersion": "^4.0.0-beta.2"
                         },
                         "@jupyterlab/docregistry": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-rc.0"
+                            "requiredVersion": "^4.0.0-beta.2"
                         },
                         "@jupyterlab/documentsearch": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-rc.0",
+                            "requiredVersion": "^4.0.0-beta.2",
                             "singleton": true
                         },
                         "@jupyterlab/documentsearch-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-rc.0"
+                            "requiredVersion": "^4.0.0-beta.2"
                         },
                         "@jupyterlab/extensionmanager": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-rc.0",
+                            "requiredVersion": "^4.0.0-beta.2",
                             "singleton": true
                         },
                         "@jupyterlab/extensionmanager-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-rc.0"
+                            "requiredVersion": "^4.0.0-beta.2"
                         },
                         "@jupyterlab/filebrowser": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-rc.0",
+                            "requiredVersion": "^4.0.0-beta.2",
                             "singleton": true
                         },
                         "@jupyterlab/filebrowser-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-rc.0"
+                            "requiredVersion": "^4.0.0-beta.2"
                         },
                         "@jupyterlab/fileeditor": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-rc.0",
+                            "requiredVersion": "^4.0.0-beta.2",
                             "singleton": true
                         },
                         "@jupyterlab/fileeditor-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-rc.0"
+                            "requiredVersion": "^4.0.0-beta.2"
                         },
                         "@jupyterlab/help-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-rc.0"
+                            "requiredVersion": "^4.0.0-beta.2"
                         },
                         "@jupyterlab/htmlviewer": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-rc.0",
+                            "requiredVersion": "^4.0.0-beta.2",
                             "singleton": true
                         },
                         "@jupyterlab/htmlviewer-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-rc.0"
+                            "requiredVersion": "^4.0.0-beta.2"
                         },
                         "@jupyterlab/hub-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-rc.0"
+                            "requiredVersion": "^4.0.0-beta.2"
                         },
                         "@jupyterlab/imageviewer": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-rc.0",
+                            "requiredVersion": "^4.0.0-beta.2",
                             "singleton": true
                         },
                         "@jupyterlab/imageviewer-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-rc.0"
+                            "requiredVersion": "^4.0.0-beta.2"
                         },
                         "@jupyterlab/inspector": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-rc.0",
+                            "requiredVersion": "^4.0.0-beta.2",
                             "singleton": true
                         },
                         "@jupyterlab/inspector-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-rc.0"
+                            "requiredVersion": "^4.0.0-beta.2"
                         },
                         "@jupyterlab/javascript-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-rc.0"
+                            "requiredVersion": "^4.0.0-beta.2"
                         },
                         "@jupyterlab/json-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-rc.0"
+                            "requiredVersion": "^4.0.0-beta.2"
                         },
                         "@jupyterlab/launcher": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-rc.0",
+                            "requiredVersion": "^4.0.0-beta.2",
                             "singleton": true
                         },
                         "@jupyterlab/launcher-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-rc.0"
+                            "requiredVersion": "^4.0.0-beta.2"
                         },
                         "@jupyterlab/logconsole": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-rc.0",
+                            "requiredVersion": "^4.0.0-beta.2",
                             "singleton": true
                         },
                         "@jupyterlab/logconsole-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-rc.0"
+                            "requiredVersion": "^4.0.0-beta.2"
                         },
                         "@jupyterlab/lsp": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-rc.0",
+                            "requiredVersion": "^4.0.0-beta.2",
                             "singleton": true
                         },
                         "@jupyterlab/lsp-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-rc.0"
+                            "requiredVersion": "^4.0.0-beta.2"
                         },
                         "@jupyterlab/mainmenu": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-rc.0",
+                            "requiredVersion": "^4.0.0-beta.2",
                             "singleton": true
                         },
                         "@jupyterlab/mainmenu-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-rc.0"
+                            "requiredVersion": "^4.0.0-beta.2"
                         },
                         "@jupyterlab/markdownviewer": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-rc.0",
+                            "requiredVersion": "^4.0.0-beta.2",
                             "singleton": true
                         },
                         "@jupyterlab/markdownviewer-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-rc.0"
+                            "requiredVersion": "^4.0.0-beta.2"
                         },
                         "@jupyterlab/markedparser-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-rc.0"
+                            "requiredVersion": "^4.0.0-beta.2"
                         },
                         "@jupyterlab/mathjax-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-rc.0"
+                            "requiredVersion": "^4.0.0-beta.2"
                         },
                         "@jupyterlab/metadataform": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-rc.0",
+                            "requiredVersion": "^4.0.0-beta.2",
                             "singleton": true
                         },
                         "@jupyterlab/metadataform-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-rc.0"
+                            "requiredVersion": "^4.0.0-beta.2"
                         },
                         "@jupyterlab/metapackage": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-rc.0"
+                            "requiredVersion": "^4.0.0-beta.2"
                         },
                         "@jupyterlab/nbconvert-css": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-rc.0"
+                            "requiredVersion": "^4.0.0-beta.2"
                         },
                         "@jupyterlab/nbformat": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-rc.0"
+                            "requiredVersion": "^4.0.0-beta.2"
                         },
                         "@jupyterlab/notebook": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-rc.0",
+                            "requiredVersion": "^4.0.0-beta.2",
                             "singleton": true
                         },
                         "@jupyterlab/notebook-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-rc.0"
+                            "requiredVersion": "^4.0.0-beta.2"
                         },
                         "@jupyterlab/observables": {
                             "import": false,
-                            "requiredVersion": "^5.0.0-rc.0"
+                            "requiredVersion": "^5.0.0-beta.2"
                         },
                         "@jupyterlab/outputarea": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-rc.0"
+                            "requiredVersion": "^4.0.0-beta.2"
                         },
                         "@jupyterlab/pdf-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-rc.0"
+                            "requiredVersion": "^4.0.0-beta.2"
                         },
                         "@jupyterlab/property-inspector": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-rc.0"
+                            "requiredVersion": "^4.0.0-beta.2"
                         },
                         "@jupyterlab/rendermime": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-rc.0",
+                            "requiredVersion": "^4.0.0-beta.2",
                             "singleton": true
                         },
                         "@jupyterlab/rendermime-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-rc.0"
+                            "requiredVersion": "^4.0.0-beta.2"
                         },
                         "@jupyterlab/rendermime-interfaces": {
                             "import": false,
-                            "requiredVersion": "^3.8.0-rc.0",
+                            "requiredVersion": "^3.8.0-beta.2",
                             "singleton": true
                         },
                         "@jupyterlab/running": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-rc.0"
+                            "requiredVersion": "^4.0.0-beta.2"
                         },
                         "@jupyterlab/running-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-rc.0"
+                            "requiredVersion": "^4.0.0-beta.2"
                         },
                         "@jupyterlab/services": {
                             "import": false,
-                            "requiredVersion": "^7.0.0-rc.0",
+                            "requiredVersion": "^7.0.0-beta.2",
                             "singleton": true
                         },
                         "@jupyterlab/settingeditor": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-rc.0",
+                            "requiredVersion": "^4.0.0-beta.2",
                             "singleton": true
                         },
                         "@jupyterlab/settingeditor-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-rc.0"
+                            "requiredVersion": "^4.0.0-beta.2"
                         },
                         "@jupyterlab/settingregistry": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-rc.0",
+                            "requiredVersion": "^4.0.0-beta.2",
                             "singleton": true
                         },
                         "@jupyterlab/shortcuts-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-rc.0"
+                            "requiredVersion": "^4.0.0-beta.2"
                         },
                         "@jupyterlab/statedb": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-rc.0",
+                            "requiredVersion": "^4.0.0-beta.2",
                             "singleton": true
                         },
                         "@jupyterlab/statusbar": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-rc.0",
+                            "requiredVersion": "^4.0.0-beta.2",
                             "singleton": true
                         },
                         "@jupyterlab/statusbar-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-rc.0"
+                            "requiredVersion": "^4.0.0-beta.2"
                         },
                         "@jupyterlab/terminal": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-rc.0",
+                            "requiredVersion": "^4.0.0-beta.2",
                             "singleton": true
                         },
                         "@jupyterlab/terminal-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-rc.0"
+                            "requiredVersion": "^4.0.0-beta.2"
                         },
                         "@jupyterlab/theme-dark-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-rc.0"
+                            "requiredVersion": "^4.0.0-beta.2"
                         },
                         "@jupyterlab/theme-light-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-rc.0"
+                            "requiredVersion": "^4.0.0-beta.2"
                         },
                         "@jupyterlab/toc": {
                             "import": false,
-                            "requiredVersion": "^6.0.0-rc.0",
+                            "requiredVersion": "^6.0.0-beta.2",
                             "singleton": true
                         },
                         "@jupyterlab/toc-extension": {
                             "import": false,
-                            "requiredVersion": "^6.0.0-rc.0"
+                            "requiredVersion": "^6.0.0-beta.2"
                         },
                         "@jupyterlab/tooltip": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-rc.0",
+                            "requiredVersion": "^4.0.0-beta.2",
                             "singleton": true
                         },
                         "@jupyterlab/tooltip-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-rc.0"
+                            "requiredVersion": "^4.0.0-beta.2"
                         },
                         "@jupyterlab/translation": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-rc.0",
+                            "requiredVersion": "^4.0.0-beta.2",
                             "singleton": true
                         },
                         "@jupyterlab/translation-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-rc.0"
+                            "requiredVersion": "^4.0.0-beta.2"
                         },
                         "@jupyterlab/ui-components": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-rc.0",
+                            "requiredVersion": "^4.0.0-beta.2",
                             "singleton": true
                         },
                         "@jupyterlab/ui-components-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-rc.0"
+                            "requiredVersion": "^4.0.0-beta.2"
                         },
                         "@jupyterlab/vega5-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-rc.0"
+                            "requiredVersion": "^4.0.0-beta.2"
                         },
                         "@lezer/common": {
                             "import": false,
                             "requiredVersion": "^1.0.0",
                             "singleton": true
                         },
                         "@lezer/highlight": {
@@ -626,15 +626,15 @@
                             "import": false,
                             "requiredVersion": "^2.0.1",
                             "singleton": true
                         },
                         "jupyterlab-celltagsclasses": {
                             "import": "/Users/tparment/git/jupyterlab-celltagsclasses/lib/index.js",
                             "singleton": true,
-                            "version": "0.1.0"
+                            "version": "0.2.0"
                         },
                         "react": {
                             "import": false,
                             "requiredVersion": "^18.2.0",
                             "singleton": true
                         },
                         "react-dom": {
```

### Comparing `jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/package.json` & `jupyterlab_celltagsclasses-0.2.0/package.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666666%*

 * *Differences: {"'jupyterlab'": "{delete: ['_build']}", "'version'": "'0.2.0'"}*

```diff
@@ -39,19 +39,14 @@
     "files": [
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
         "style/index.js"
     ],
     "homepage": "https://github.com/parmentelat/jupyterlab-celltagsclasses",
     "jupyterlab": {
-        "_build": {
-            "extension": "./extension",
-            "load": "static/remoteEntry.09eb75b8b35017dd61cc.js",
-            "style": "./style"
-        },
         "extension": true,
         "outputDir": "jupyterlab_celltagsclasses/labextension"
     },
     "keywords": [
         "jupyter",
         "jupyterlab",
         "jupyterlab-extension"
@@ -95,9 +90,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.1.0"
+    "version": "0.2.0"
 }
```

### Comparing `jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/lib_index_js.69027069f0720bba2d30.js` & `jupyterlab_celltagsclasses-0.2.0/jupyterlab_celltagsclasses/labextension/static/lib_index_js.e0bf585461963e3d1e28.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -41,19 +41,19 @@
                             if (notebookModel === null) {
                                 return;
                             }
                             notebookModel.cells.changed.connect((cellList, change) => {
                                 if (change.type !== 'add') {
                                     return;
                                 }
-                                change.newValues.forEach((cellModel) => {
+                                change.newValues.forEach(cellModel => {
                                     var _a, _b;
                                     // compute widgets attached to cellModel
-                                    const cellWidgets = (_a = notebookTracker.currentWidget) === null || _a === void 0 ? void 0 : _a.content.widgets.filter((cell, index) => (cell.model.id === cellModel.id));
-                                    if ((cellWidgets === undefined) || ((cellWidgets === null || cellWidgets === void 0 ? void 0 : cellWidgets.length) === 0)) {
+                                    const cellWidgets = (_a = notebookTracker.currentWidget) === null || _a === void 0 ? void 0 : _a.content.widgets.filter((cell, index) => cell.model.id === cellModel.id);
+                                    if (cellWidgets === undefined || (cellWidgets === null || cellWidgets === void 0 ? void 0 : cellWidgets.length) === 0) {
                                         console.warn('could not find cell widget for cell model', cellModel);
                                         return;
                                     }
                                     console.debug(`found ${cellWidgets === null || cellWidgets === void 0 ? void 0 : cellWidgets.length} cell widgets`, cellWidgets[0]);
                                     // add classes for pre-existing tags
                                     (_b = cellModel.getMetadata('tags')) === null || _b === void 0 ? void 0 : _b.forEach((tag) => cellWidgets === null || cellWidgets === void 0 ? void 0 : cellWidgets.forEach(cellWidget => {
                                         console.debug(`adding initial class for tag ${class_for_tag(tag)}`);
@@ -71,39 +71,39 @@
                                         //   (cell: Cell, index: number) => (cell.model.id === cellModel.id)
                                         // )
                                         if (change.type === 'change') {
                                             console.debug('change', change, change.newValue);
                                             // compute difference between old and new tags
                                             const oldTags = change.oldValue;
                                             const newTags = change.newValue;
-                                            const addedTags = newTags.filter((tag) => !oldTags.includes(tag));
-                                            const removedTags = oldTags.filter((tag) => !newTags.includes(tag));
+                                            const addedTags = newTags.filter(tag => !oldTags.includes(tag));
+                                            const removedTags = oldTags.filter(tag => !newTags.includes(tag));
                                             console.log('addedTags', addedTags);
                                             console.log('removedTags', removedTags);
                                             cellWidgets.forEach(cellWidget => {
                                                 addedTags.forEach(tag => {
                                                     console.debug(`adding class for tag ${class_for_tag(tag)}`);
                                                     cellWidget.addClass(class_for_tag(tag));
                                                 });
                                                 removedTags.forEach(tag => {
                                                     console.debug(`removing class for tag ${class_for_tag(tag)}`);
                                                     cellWidget.removeClass(class_for_tag(tag));
                                                 });
                                             });
                                         } else if (change.type === 'add') {
                                             console.log('add', change, change.newValue);
-                                            cellWidgets.forEach((cellWidget) => {
+                                            cellWidgets.forEach(cellWidget => {
                                                 for (const tag of change.newValue) {
                                                     console.debug(`adding class for tag ${class_for_tag(tag)}`);
                                                     cellWidget.addClass(class_for_tag(tag));
                                                 }
                                             });
                                         } else if (change.type === 'remove') {
                                             console.log('remove', change, change.newValue);
-                                            cellWidgets.forEach((cellWidget) => {
+                                            cellWidgets.forEach(cellWidget => {
                                                 for (const tag of change.newValue) {
                                                     console.debug(`removing class for tag ${class_for_tag(tag)}`);
                                                     cellWidget.removeClass(class_for_tag(tag));
                                                 }
                                             });
                                         }
                                     });
@@ -117,8 +117,8 @@
 
 
                 /***/
             })
 
     }
 ]);
-//# sourceMappingURL=lib_index_js.69027069f0720bba2d30.js.map
+//# sourceMappingURL=lib_index_js.e0bf585461963e3d1e28.js.map
```

### Comparing `jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/lib_index_js.69027069f0720bba2d30.js.map` & `jupyterlab_celltagsclasses-0.2.0/jupyterlab_celltagsclasses/labextension/static/lib_index_js.e0bf585461963e3d1e28.js.map`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7857142857142857%*

 * *Differences: {"'file'": "'lib_index_js.e0bf585461963e3d1e28.js'",*

 * * "'mappings'": "';;;;;;;;;;;;;;;AAAA;AACA;AACA;AACA;AACwD;AACxD;AACA;AACA;AACA;AACA;AACA;AACA,eAAe,kEAAgB;AAC/B;AACA;AACA,mDAAmD,IAAI;AACvD;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,2CAA2C,8EAA8E;AACzH;AACA;AACA,sEAAsE,mBAAmB;AACzF;AACA,qBAAqB;AACrB;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,0EAA0E,mBAAmB;AAC7F;AACA,iCAAiC;AACjC;AACA,4EAA4E,mBAAmB […]*

```diff
@@ -1,13 +1,13 @@
 {
-    "file": "lib_index_js.69027069f0720bba2d30.js",
-    "mappings": ";;;;;;;;;;;;;;;AAAA;AACA;AACA;AACA;AACyD;AACzD;AACA;AACA;AACA;AACA;AACA;AACA,eAAe,kEAAgB;AAC/B;AACA;AACA,mDAAmD,IAAI;AACvD;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,2CAA2C,8EAA8E;AACzH;AACA;AACA,sEAAsE,mBAAmB;AACzF;AACA,qBAAqB;AACrB;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,0EAA0E,mBAAmB;AAC7F;AACA,iCAAiC;AACjC;AACA,4EAA4E,mBAAmB;AAC/F;AACA,iCAAiC;AACjC,6BAA6B;AAC7B;AACA;AACA;AACA;AACA;AACA,0EAA0E,mBAAmB;AAC7F;AACA;AACA,6BAA6B;AAC7B;AACA;AACA;AACA;AACA;AACA,4EAA4E,mBAAmB;AAC/F;AACA;AACA,6BAA6B;AAC7B;AACA,qBAAqB;AACrB,iBAAiB;AACjB,aAAa;AACb,SAAS;AACT;AACA;AACA,iEAAe,MAAM,EAAC",
+    "file": "lib_index_js.e0bf585461963e3d1e28.js",
+    "mappings": ";;;;;;;;;;;;;;;AAAA;AACA;AACA;AACA;AACwD;AACxD;AACA;AACA;AACA;AACA;AACA;AACA,eAAe,kEAAgB;AAC/B;AACA;AACA,mDAAmD,IAAI;AACvD;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,2CAA2C,8EAA8E;AACzH;AACA;AACA,sEAAsE,mBAAmB;AACzF;AACA,qBAAqB;AACrB;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,0EAA0E,mBAAmB;AAC7F;AACA,iCAAiC;AACjC;AACA,4EAA4E,mBAAmB;AAC/F;AACA,iCAAiC;AACjC,6BAA6B;AAC7B;AACA;AACA;AACA;AACA;AACA,0EAA0E,mBAAmB;AAC7F;AACA;AACA,6BAA6B;AAC7B;AACA;AACA;AACA;AACA;AACA,4EAA4E,mBAAmB;AAC/F;AACA;AACA,6BAA6B;AAC7B;AACA,qBAAqB;AACrB,iBAAiB;AACjB,aAAa;AACb,SAAS;AACT;AACA;AACA,iEAAe,MAAM,EAAC",
     "names": [],
     "sourceRoot": "",
     "sources": [
         "webpack://jupyterlab-celltagsclasses/./lib/index.js"
     ],
     "sourcesContent": [
-        "/*\n * for attaching keybindings later on, see\n * https://towardsdatascience.com/how-to-customize-jupyterlab-keyboard-shortcuts-72321f73753d\n */\nimport { INotebookTracker, } from '@jupyterlab/notebook';\n/**\n * Initialization data for the jupyterlab-celltagsclasses extension.\n */\nconst plugin = {\n    id: 'jupyterlab-celltagsclasses:plugin',\n    autoStart: true,\n    requires: [INotebookTracker],\n    activate: (app, notebookTracker) => {\n        console.log('extension jupyterlab-celltagsclasses is activating');\n        const class_for_tag = (tag) => `cell-tag-${tag}`;\n        notebookTracker.widgetAdded.connect((_, panel) => {\n            const notebookModel = panel.content.model;\n            if (notebookModel === null) {\n                return;\n            }\n            notebookModel.cells.changed.connect((cellList, change) => {\n                if (change.type !== 'add') {\n                    return;\n                }\n                change.newValues.forEach((cellModel) => {\n                    var _a, _b;\n                    // compute widgets attached to cellModel\n                    const cellWidgets = (_a = notebookTracker.currentWidget) === null || _a === void 0 ? void 0 : _a.content.widgets.filter((cell, index) => (cell.model.id === cellModel.id));\n                    if ((cellWidgets === undefined) || ((cellWidgets === null || cellWidgets === void 0 ? void 0 : cellWidgets.length) === 0)) {\n                        console.warn('could not find cell widget for cell model', cellModel);\n                        return;\n                    }\n                    console.debug(`found ${cellWidgets === null || cellWidgets === void 0 ? void 0 : cellWidgets.length} cell widgets`, cellWidgets[0]);\n                    // add classes for pre-existing tags\n                    (_b = cellModel.getMetadata('tags')) === null || _b === void 0 ? void 0 : _b.forEach((tag) => cellWidgets === null || cellWidgets === void 0 ? void 0 : cellWidgets.forEach(cellWidget => {\n                        console.debug(`adding initial class for tag ${class_for_tag(tag)}`);\n                        cellWidget.addClass(class_for_tag(tag));\n                    }));\n                    // react to changes in tags\n                    cellModel.metadataChanged.connect((sender, change) => {\n                        console.debug('metadata changed', sender, change);\n                        if (change.key !== 'tags') {\n                            // console.debug(\"ignoring non-tags metadata change\")\n                            return;\n                        }\n                        // does not seem useful to recompute this\n                        // const cellWidgets = notebookTracker.currentWidget?.content.widgets.filter(\n                        //   (cell: Cell, index: number) => (cell.model.id === cellModel.id)\n                        // )\n                        if (change.type === 'change') {\n                            console.debug('change', change, change.newValue);\n                            // compute difference between old and new tags\n                            const oldTags = change.oldValue;\n                            const newTags = change.newValue;\n                            const addedTags = newTags.filter((tag) => !oldTags.includes(tag));\n                            const removedTags = oldTags.filter((tag) => !newTags.includes(tag));\n                            console.log('addedTags', addedTags);\n                            console.log('removedTags', removedTags);\n                            cellWidgets.forEach(cellWidget => {\n                                addedTags.forEach(tag => {\n                                    console.debug(`adding class for tag ${class_for_tag(tag)}`);\n                                    cellWidget.addClass(class_for_tag(tag));\n                                });\n                                removedTags.forEach(tag => {\n                                    console.debug(`removing class for tag ${class_for_tag(tag)}`);\n                                    cellWidget.removeClass(class_for_tag(tag));\n                                });\n                            });\n                        }\n                        else if (change.type === 'add') {\n                            console.log('add', change, change.newValue);\n                            cellWidgets.forEach((cellWidget) => {\n                                for (const tag of change.newValue) {\n                                    console.debug(`adding class for tag ${class_for_tag(tag)}`);\n                                    cellWidget.addClass(class_for_tag(tag));\n                                }\n                            });\n                        }\n                        else if (change.type === 'remove') {\n                            console.log('remove', change, change.newValue);\n                            cellWidgets.forEach((cellWidget) => {\n                                for (const tag of change.newValue) {\n                                    console.debug(`removing class for tag ${class_for_tag(tag)}`);\n                                    cellWidget.removeClass(class_for_tag(tag));\n                                }\n                            });\n                        }\n                    });\n                });\n            });\n        });\n    }\n};\nexport default plugin;\n"
+        "/*\n * for attaching keybindings later on, see\n * https://towardsdatascience.com/how-to-customize-jupyterlab-keyboard-shortcuts-72321f73753d\n */\nimport { INotebookTracker } from '@jupyterlab/notebook';\n/**\n * Initialization data for the jupyterlab-celltagsclasses extension.\n */\nconst plugin = {\n    id: 'jupyterlab-celltagsclasses:plugin',\n    autoStart: true,\n    requires: [INotebookTracker],\n    activate: (app, notebookTracker) => {\n        console.log('extension jupyterlab-celltagsclasses is activating');\n        const class_for_tag = (tag) => `cell-tag-${tag}`;\n        notebookTracker.widgetAdded.connect((_, panel) => {\n            const notebookModel = panel.content.model;\n            if (notebookModel === null) {\n                return;\n            }\n            notebookModel.cells.changed.connect((cellList, change) => {\n                if (change.type !== 'add') {\n                    return;\n                }\n                change.newValues.forEach(cellModel => {\n                    var _a, _b;\n                    // compute widgets attached to cellModel\n                    const cellWidgets = (_a = notebookTracker.currentWidget) === null || _a === void 0 ? void 0 : _a.content.widgets.filter((cell, index) => cell.model.id === cellModel.id);\n                    if (cellWidgets === undefined || (cellWidgets === null || cellWidgets === void 0 ? void 0 : cellWidgets.length) === 0) {\n                        console.warn('could not find cell widget for cell model', cellModel);\n                        return;\n                    }\n                    console.debug(`found ${cellWidgets === null || cellWidgets === void 0 ? void 0 : cellWidgets.length} cell widgets`, cellWidgets[0]);\n                    // add classes for pre-existing tags\n                    (_b = cellModel.getMetadata('tags')) === null || _b === void 0 ? void 0 : _b.forEach((tag) => cellWidgets === null || cellWidgets === void 0 ? void 0 : cellWidgets.forEach(cellWidget => {\n                        console.debug(`adding initial class for tag ${class_for_tag(tag)}`);\n                        cellWidget.addClass(class_for_tag(tag));\n                    }));\n                    // react to changes in tags\n                    cellModel.metadataChanged.connect((sender, change) => {\n                        console.debug('metadata changed', sender, change);\n                        if (change.key !== 'tags') {\n                            // console.debug(\"ignoring non-tags metadata change\")\n                            return;\n                        }\n                        // does not seem useful to recompute this\n                        // const cellWidgets = notebookTracker.currentWidget?.content.widgets.filter(\n                        //   (cell: Cell, index: number) => (cell.model.id === cellModel.id)\n                        // )\n                        if (change.type === 'change') {\n                            console.debug('change', change, change.newValue);\n                            // compute difference between old and new tags\n                            const oldTags = change.oldValue;\n                            const newTags = change.newValue;\n                            const addedTags = newTags.filter(tag => !oldTags.includes(tag));\n                            const removedTags = oldTags.filter(tag => !newTags.includes(tag));\n                            console.log('addedTags', addedTags);\n                            console.log('removedTags', removedTags);\n                            cellWidgets.forEach(cellWidget => {\n                                addedTags.forEach(tag => {\n                                    console.debug(`adding class for tag ${class_for_tag(tag)}`);\n                                    cellWidget.addClass(class_for_tag(tag));\n                                });\n                                removedTags.forEach(tag => {\n                                    console.debug(`removing class for tag ${class_for_tag(tag)}`);\n                                    cellWidget.removeClass(class_for_tag(tag));\n                                });\n                            });\n                        }\n                        else if (change.type === 'add') {\n                            console.log('add', change, change.newValue);\n                            cellWidgets.forEach(cellWidget => {\n                                for (const tag of change.newValue) {\n                                    console.debug(`adding class for tag ${class_for_tag(tag)}`);\n                                    cellWidget.addClass(class_for_tag(tag));\n                                }\n                            });\n                        }\n                        else if (change.type === 'remove') {\n                            console.log('remove', change, change.newValue);\n                            cellWidgets.forEach(cellWidget => {\n                                for (const tag of change.newValue) {\n                                    console.debug(`removing class for tag ${class_for_tag(tag)}`);\n                                    cellWidget.removeClass(class_for_tag(tag));\n                                }\n                            });\n                        }\n                    });\n                });\n            });\n        });\n    }\n};\nexport default plugin;\n"
     ],
     "version": 3
 }
```

### Comparing `jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/lib_index_js.745b7b07e91b136d36b8.js` & `jupyterlab_celltagsclasses-0.2.0/src/index.ts`

 * *Files 25% similar despite different names*

```diff
@@ -1,398 +1,290 @@
-00000000: 2275 7365 2073 7472 6963 7422 3b0a 2873  "use strict";.(s
-00000010: 656c 665b 2277 6562 7061 636b 4368 756e  elf["webpackChun
-00000020: 6b6a 7570 7974 6572 6c61 625f 6365 6c6c  kjupyterlab_cell
-00000030: 7461 6773 636c 6173 7365 7322 5d20 3d20  tagsclasses"] = 
-00000040: 7365 6c66 5b22 7765 6270 6163 6b43 6875  self["webpackChu
-00000050: 6e6b 6a75 7079 7465 726c 6162 5f63 656c  nkjupyterlab_cel
-00000060: 6c74 6167 7363 6c61 7373 6573 225d 207c  ltagsclasses"] |
-00000070: 7c20 5b5d 292e 7075 7368 285b 5b22 6c69  | []).push([["li
-00000080: 625f 696e 6465 785f 6a73 225d 2c7b 0a0a  b_index_js"],{..
-00000090: 2f2a 2a2a 2f20 222e 2f6c 6962 2f69 6e64  /***/ "./lib/ind
-000000a0: 6578 2e6a 7322 3a0a 2f2a 212a 2a2a 2a2a  ex.js":./*!*****
-000000b0: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
-000000c0: 2a21 2a5c 0a20 2021 2a2a 2a20 2e2f 6c69  *!*\.  !*** ./li
-000000d0: 622f 696e 6465 782e 6a73 202a 2a2a 210a  b/index.js ***!.
-000000e0: 2020 5c2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a    \*************
-000000f0: 2a2a 2a2a 2a2a 2a2a 2a2f 0a2f 2a2a 2a2f  *********/./***/
-00000100: 2028 285f 5f75 6e75 7365 645f 7765 6270   ((__unused_webp
-00000110: 6163 6b5f 6d6f 6475 6c65 2c20 5f5f 7765  ack_module, __we
-00000120: 6270 6163 6b5f 6578 706f 7274 735f 5f2c  bpack_exports__,
-00000130: 205f 5f77 6562 7061 636b 5f72 6571 7569   __webpack_requi
-00000140: 7265 5f5f 2920 3d3e 207b 0a0a 5f5f 7765  re__) => {..__we
-00000150: 6270 6163 6b5f 7265 7175 6972 655f 5f2e  bpack_require__.
-00000160: 7228 5f5f 7765 6270 6163 6b5f 6578 706f  r(__webpack_expo
-00000170: 7274 735f 5f29 3b0a 2f2a 2068 6172 6d6f  rts__);./* harmo
-00000180: 6e79 2065 7870 6f72 7420 2a2f 205f 5f77  ny export */ __w
-00000190: 6562 7061 636b 5f72 6571 7569 7265 5f5f  ebpack_require__
-000001a0: 2e64 285f 5f77 6562 7061 636b 5f65 7870  .d(__webpack_exp
-000001b0: 6f72 7473 5f5f 2c20 7b0a 2f2a 2068 6172  orts__, {./* har
-000001c0: 6d6f 6e79 2065 7870 6f72 7420 2a2f 2020  mony export */  
-000001d0: 2022 6465 6661 756c 7422 3a20 2829 203d   "default": () =
-000001e0: 3e20 285f 5f57 4542 5041 434b 5f44 4546  > (__WEBPACK_DEF
-000001f0: 4155 4c54 5f45 5850 4f52 545f 5f29 0a2f  AULT_EXPORT__)./
-00000200: 2a20 6861 726d 6f6e 7920 6578 706f 7274  * harmony export
-00000210: 202a 2f20 7d29 3b0a 2f2a 2068 6172 6d6f   */ });./* harmo
-00000220: 6e79 2069 6d70 6f72 7420 2a2f 2076 6172  ny import */ var
-00000230: 205f 6a75 7079 7465 726c 6162 5f6e 6f74   _jupyterlab_not
-00000240: 6562 6f6f 6b5f 5f57 4542 5041 434b 5f49  ebook__WEBPACK_I
-00000250: 4d50 4f52 5445 445f 4d4f 4455 4c45 5f30  MPORTED_MODULE_0
-00000260: 5f5f 203d 205f 5f77 6562 7061 636b 5f72  __ = __webpack_r
-00000270: 6571 7569 7265 5f5f 282f 2a21 2040 6a75  equire__(/*! @ju
-00000280: 7079 7465 726c 6162 2f6e 6f74 6562 6f6f  pyterlab/noteboo
-00000290: 6b20 2a2f 2022 7765 6270 6163 6b2f 7368  k */ "webpack/sh
-000002a0: 6172 696e 672f 636f 6e73 756d 652f 6465  aring/consume/de
-000002b0: 6661 756c 742f 406a 7570 7974 6572 6c61  fault/@jupyterla
-000002c0: 622f 6e6f 7465 626f 6f6b 2229 3b0a 2f2a  b/notebook");./*
-000002d0: 2068 6172 6d6f 6e79 2069 6d70 6f72 7420   harmony import 
-000002e0: 2a2f 2076 6172 205f 6a75 7079 7465 726c  */ var _jupyterl
-000002f0: 6162 5f6e 6f74 6562 6f6f 6b5f 5f57 4542  ab_notebook__WEB
-00000300: 5041 434b 5f49 4d50 4f52 5445 445f 4d4f  PACK_IMPORTED_MO
-00000310: 4455 4c45 5f30 5f5f 5f64 6566 6175 6c74  DULE_0___default
-00000320: 203d 202f 2a23 5f5f 5055 5245 5f5f 2a2f   = /*#__PURE__*/
-00000330: 5f5f 7765 6270 6163 6b5f 7265 7175 6972  __webpack_requir
-00000340: 655f 5f2e 6e28 5f6a 7570 7974 6572 6c61  e__.n(_jupyterla
-00000350: 625f 6e6f 7465 626f 6f6b 5f5f 5745 4250  b_notebook__WEBP
-00000360: 4143 4b5f 494d 504f 5254 4544 5f4d 4f44  ACK_IMPORTED_MOD
-00000370: 554c 455f 305f 5f29 3b0a 2f2a 0a20 2a20  ULE_0__);./*. * 
-00000380: 666f 7220 6174 7461 6368 696e 6720 6b65  for attaching ke
-00000390: 7962 696e 6469 6e67 7320 6c61 7465 7220  ybindings later 
-000003a0: 6f6e 2c20 7365 650a 202a 2068 7474 7073  on, see. * https
-000003b0: 3a2f 2f74 6f77 6172 6473 6461 7461 7363  ://towardsdatasc
-000003c0: 6965 6e63 652e 636f 6d2f 686f 772d 746f  ience.com/how-to
-000003d0: 2d63 7573 746f 6d69 7a65 2d6a 7570 7974  -customize-jupyt
-000003e0: 6572 6c61 622d 6b65 7962 6f61 7264 2d73  erlab-keyboard-s
-000003f0: 686f 7274 6375 7473 2d37 3233 3231 6637  hortcuts-72321f7
-00000400: 3337 3533 640a 202a 2f0a 0a2f 2a2a 0a20  3753d. */../**. 
-00000410: 2a20 496e 6974 6961 6c69 7a61 7469 6f6e  * Initialization
-00000420: 2064 6174 6120 666f 7220 7468 6520 6a75   data for the ju
-00000430: 7079 7465 726c 6162 2d63 656c 6c74 6167  pyterlab-celltag
-00000440: 7363 6c61 7373 6573 2065 7874 656e 7369  sclasses extensi
-00000450: 6f6e 2e0a 202a 2f0a 636f 6e73 7420 706c  on.. */.const pl
-00000460: 7567 696e 203d 207b 0a20 2020 2069 643a  ugin = {.    id:
-00000470: 2027 6a75 7079 7465 726c 6162 2d63 656c   'jupyterlab-cel
-00000480: 6c74 6167 7363 6c61 7373 6573 3a70 6c75  ltagsclasses:plu
-00000490: 6769 6e27 2c0a 2020 2020 6175 746f 5374  gin',.    autoSt
-000004a0: 6172 743a 2074 7275 652c 0a20 2020 2072  art: true,.    r
-000004b0: 6571 7569 7265 733a 205b 5f6a 7570 7974  equires: [_jupyt
-000004c0: 6572 6c61 625f 6e6f 7465 626f 6f6b 5f5f  erlab_notebook__
-000004d0: 5745 4250 4143 4b5f 494d 504f 5254 4544  WEBPACK_IMPORTED
-000004e0: 5f4d 4f44 554c 455f 305f 5f2e 494e 6f74  _MODULE_0__.INot
-000004f0: 6562 6f6f 6b54 7261 636b 6572 5d2c 0a20  ebookTracker],. 
-00000500: 2020 2061 6374 6976 6174 653a 2028 6170     activate: (ap
-00000510: 702c 206e 6f74 6562 6f6f 6b54 7261 636b  p, notebookTrack
-00000520: 6572 2920 3d3e 207b 0a20 2020 2020 2020  er) => {.       
-00000530: 2063 6f6e 736f 6c65 2e6c 6f67 2827 6578   console.log('ex
-00000540: 7465 6e73 696f 6e20 6a75 7079 7465 726c  tension jupyterl
-00000550: 6162 2d63 656c 6c74 6167 7363 6c61 7373  ab-celltagsclass
-00000560: 6573 2069 7320 6163 7469 7661 7469 6e67  es is activating
-00000570: 2729 3b0a 2020 2020 2020 2020 636f 6e73  ');.        cons
-00000580: 7420 636c 6173 735f 666f 725f 7461 6720  t class_for_tag 
-00000590: 3d20 2874 6167 2920 3d3e 2060 6365 6c6c  = (tag) => `cell
-000005a0: 2d74 6167 2d24 7b74 6167 7d60 3b0a 2020  -tag-${tag}`;.  
-000005b0: 2020 2020 2020 6e6f 7465 626f 6f6b 5472        notebookTr
-000005c0: 6163 6b65 722e 7769 6467 6574 4164 6465  acker.widgetAdde
-000005d0: 642e 636f 6e6e 6563 7428 285f 2c20 7061  d.connect((_, pa
-000005e0: 6e65 6c29 203d 3e20 7b0a 2020 2020 2020  nel) => {.      
-000005f0: 2020 2020 2020 636f 6e73 7420 6e6f 7465        const note
-00000600: 626f 6f6b 4d6f 6465 6c20 3d20 7061 6e65  bookModel = pane
-00000610: 6c2e 636f 6e74 656e 742e 6d6f 6465 6c3b  l.content.model;
-00000620: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00000630: 286e 6f74 6562 6f6f 6b4d 6f64 656c 203d  (notebookModel =
-00000640: 3d3d 206e 756c 6c29 207b 0a20 2020 2020  == null) {.     
-00000650: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00000660: 6e3b 0a20 2020 2020 2020 2020 2020 207d  n;.            }
-00000670: 0a20 2020 2020 2020 2020 2020 206e 6f74  .            not
-00000680: 6562 6f6f 6b4d 6f64 656c 2e63 656c 6c73  ebookModel.cells
-00000690: 2e63 6861 6e67 6564 2e63 6f6e 6e65 6374  .changed.connect
-000006a0: 2828 6365 6c6c 4c69 7374 2c20 6368 616e  ((cellList, chan
-000006b0: 6765 2920 3d3e 207b 0a20 2020 2020 2020  ge) => {.       
-000006c0: 2020 2020 2020 2020 2069 6620 2863 6861           if (cha
-000006d0: 6e67 652e 7479 7065 2021 3d3d 2027 6164  nge.type !== 'ad
-000006e0: 6427 2920 7b0a 2020 2020 2020 2020 2020  d') {.          
-000006f0: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00000700: 3b0a 2020 2020 2020 2020 2020 2020 2020  ;.              
-00000710: 2020 7d0a 2020 2020 2020 2020 2020 2020    }.            
-00000720: 2020 2020 6368 616e 6765 2e6e 6577 5661      change.newVa
-00000730: 6c75 6573 2e66 6f72 4561 6368 2828 6365  lues.forEach((ce
-00000740: 6c6c 4d6f 6465 6c29 203d 3e20 7b0a 2020  llModel) => {.  
-00000750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000760: 2020 7661 7220 5f61 2c20 5f62 3b0a 2020    var _a, _b;.  
-00000770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000780: 2020 2f2f 2063 6f6d 7075 7465 2077 6964    // compute wid
-00000790: 6765 7473 2061 7474 6163 6865 6420 746f  gets attached to
-000007a0: 2063 656c 6c4d 6f64 656c 0a20 2020 2020   cellModel.     
-000007b0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-000007c0: 6f6e 7374 2063 656c 6c57 6964 6765 7473  onst cellWidgets
-000007d0: 203d 2028 5f61 203d 206e 6f74 6562 6f6f   = (_a = noteboo
-000007e0: 6b54 7261 636b 6572 2e63 7572 7265 6e74  kTracker.current
-000007f0: 5769 6467 6574 2920 3d3d 3d20 6e75 6c6c  Widget) === null
-00000800: 207c 7c20 5f61 203d 3d3d 2076 6f69 6420   || _a === void 
-00000810: 3020 3f20 766f 6964 2030 203a 205f 612e  0 ? void 0 : _a.
-00000820: 636f 6e74 656e 742e 7769 6467 6574 732e  content.widgets.
-00000830: 6669 6c74 6572 2828 6365 6c6c 2c20 696e  filter((cell, in
-00000840: 6465 7829 203d 3e20 2863 656c 6c2e 6d6f  dex) => (cell.mo
-00000850: 6465 6c2e 6964 203d 3d3d 2063 656c 6c4d  del.id === cellM
-00000860: 6f64 656c 2e69 6429 293b 0a20 2020 2020  odel.id));.     
-00000870: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00000880: 6620 2828 6365 6c6c 5769 6467 6574 7320  f ((cellWidgets 
-00000890: 3d3d 3d20 756e 6465 6669 6e65 6429 207c  === undefined) |
-000008a0: 7c20 2828 6365 6c6c 5769 6467 6574 7320  | ((cellWidgets 
-000008b0: 3d3d 3d20 6e75 6c6c 207c 7c20 6365 6c6c  === null || cell
-000008c0: 5769 6467 6574 7320 3d3d 3d20 766f 6964  Widgets === void
-000008d0: 2030 203f 2076 6f69 6420 3020 3a20 6365   0 ? void 0 : ce
-000008e0: 6c6c 5769 6467 6574 732e 6c65 6e67 7468  llWidgets.length
-000008f0: 2920 3d3d 3d20 3029 2920 7b0a 2020 2020  ) === 0)) {.    
-00000900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000910: 2020 2020 636f 6e73 6f6c 652e 7761 726e      console.warn
-00000920: 2827 636f 756c 6420 6e6f 7420 6669 6e64  ('could not find
-00000930: 2063 656c 6c20 7769 6467 6574 2066 6f72   cell widget for
-00000940: 2063 656c 6c20 6d6f 6465 6c27 2c20 6365   cell model', ce
-00000950: 6c6c 4d6f 6465 6c29 3b0a 2020 2020 2020  llModel);.      
-00000960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000970: 2020 7265 7475 726e 3b0a 2020 2020 2020    return;.      
-00000980: 2020 2020 2020 2020 2020 2020 2020 7d0a                }.
-00000990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000009a0: 2020 2020 636f 6e73 6f6c 652e 6465 6275      console.debu
-000009b0: 6728 6066 6f75 6e64 2024 7b63 656c 6c57  g(`found ${cellW
-000009c0: 6964 6765 7473 203d 3d3d 206e 756c 6c20  idgets === null 
-000009d0: 7c7c 2063 656c 6c57 6964 6765 7473 203d  || cellWidgets =
-000009e0: 3d3d 2076 6f69 6420 3020 3f20 766f 6964  == void 0 ? void
-000009f0: 2030 203a 2063 656c 6c57 6964 6765 7473   0 : cellWidgets
-00000a00: 2e6c 656e 6774 687d 2063 656c 6c20 7769  .length} cell wi
-00000a10: 6467 6574 7360 2c20 6365 6c6c 5769 6467  dgets`, cellWidg
-00000a20: 6574 735b 305d 293b 0a20 2020 2020 2020  ets[0]);.       
-00000a30: 2020 2020 2020 2020 2020 2020 202f 2f20               // 
-00000a40: 6164 6420 636c 6173 7365 7320 666f 7220  add classes for 
-00000a50: 7072 652d 6578 6973 7469 6e67 2074 6167  pre-existing tag
-00000a60: 730a 2020 2020 2020 2020 2020 2020 2020  s.              
-00000a70: 2020 2020 2020 285f 6220 3d20 6365 6c6c        (_b = cell
-00000a80: 4d6f 6465 6c2e 6765 744d 6574 6164 6174  Model.getMetadat
-00000a90: 6128 2774 6167 7327 2929 203d 3d3d 206e  a('tags')) === n
-00000aa0: 756c 6c20 7c7c 205f 6220 3d3d 3d20 766f  ull || _b === vo
-00000ab0: 6964 2030 203f 2076 6f69 6420 3020 3a20  id 0 ? void 0 : 
-00000ac0: 5f62 2e66 6f72 4561 6368 2828 7461 6729  _b.forEach((tag)
-00000ad0: 203d 3e20 6365 6c6c 5769 6467 6574 7320   => cellWidgets 
-00000ae0: 3d3d 3d20 6e75 6c6c 207c 7c20 6365 6c6c  === null || cell
-00000af0: 5769 6467 6574 7320 3d3d 3d20 766f 6964  Widgets === void
-00000b00: 2030 203f 2076 6f69 6420 3020 3a20 6365   0 ? void 0 : ce
-00000b10: 6c6c 5769 6467 6574 732e 666f 7245 6163  llWidgets.forEac
-00000b20: 6828 6365 6c6c 5769 6467 6574 203d 3e20  h(cellWidget => 
-00000b30: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
-00000b40: 2020 2020 2020 2020 2020 636f 6e73 6f6c            consol
-00000b50: 652e 6465 6275 6728 6061 6464 696e 6720  e.debug(`adding 
-00000b60: 696e 6974 6961 6c20 636c 6173 7320 666f  initial class fo
-00000b70: 7220 7461 6720 247b 636c 6173 735f 666f  r tag ${class_fo
-00000b80: 725f 7461 6728 7461 6729 7d60 293b 0a20  r_tag(tag)}`);. 
-00000b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000ba0: 2020 2020 2020 2063 656c 6c57 6964 6765         cellWidge
-00000bb0: 742e 6164 6443 6c61 7373 2863 6c61 7373  t.addClass(class
-00000bc0: 5f66 6f72 5f74 6167 2874 6167 2929 3b0a  _for_tag(tag));.
-00000bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000be0: 2020 2020 7d29 293b 0a20 2020 2020 2020      }));.       
-00000bf0: 2020 2020 2020 2020 2020 2020 202f 2f20               // 
-00000c00: 7265 6163 7420 746f 2063 6861 6e67 6573  react to changes
-00000c10: 2069 6e20 7461 6773 0a20 2020 2020 2020   in tags.       
-00000c20: 2020 2020 2020 2020 2020 2020 2063 656c               cel
-00000c30: 6c4d 6f64 656c 2e6d 6574 6164 6174 6143  lModel.metadataC
-00000c40: 6861 6e67 6564 2e63 6f6e 6e65 6374 2828  hanged.connect((
-00000c50: 7365 6e64 6572 2c20 6368 616e 6765 2920  sender, change) 
-00000c60: 3d3e 207b 0a20 2020 2020 2020 2020 2020  => {.           
-00000c70: 2020 2020 2020 2020 2020 2020 2063 6f6e               con
-00000c80: 736f 6c65 2e64 6562 7567 2827 6d65 7461  sole.debug('meta
-00000c90: 6461 7461 2063 6861 6e67 6564 272c 2073  data changed', s
-00000ca0: 656e 6465 722c 2063 6861 6e67 6529 3b0a  ender, change);.
-00000cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000cc0: 2020 2020 2020 2020 6966 2028 6368 616e          if (chan
-00000cd0: 6765 2e6b 6579 2021 3d3d 2027 7461 6773  ge.key !== 'tags
-00000ce0: 2729 207b 0a20 2020 2020 2020 2020 2020  ') {.           
-00000cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000d00: 202f 2f20 636f 6e73 6f6c 652e 6465 6275   // console.debu
-00000d10: 6728 2269 676e 6f72 696e 6720 6e6f 6e2d  g("ignoring non-
-00000d20: 7461 6773 206d 6574 6164 6174 6120 6368  tags metadata ch
-00000d30: 616e 6765 2229 0a20 2020 2020 2020 2020  ange").         
-00000d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000d50: 2020 2072 6574 7572 6e3b 0a20 2020 2020     return;.     
-00000d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000d70: 2020 207d 0a20 2020 2020 2020 2020 2020     }.           
-00000d80: 2020 2020 2020 2020 2020 2020 202f 2f20               // 
-00000d90: 646f 6573 206e 6f74 2073 6565 6d20 7573  does not seem us
-00000da0: 6566 756c 2074 6f20 7265 636f 6d70 7574  eful to recomput
-00000db0: 6520 7468 6973 0a20 2020 2020 2020 2020  e this.         
-00000dc0: 2020 2020 2020 2020 2020 2020 2020 202f                 /
-00000dd0: 2f20 636f 6e73 7420 6365 6c6c 5769 6467  / const cellWidg
-00000de0: 6574 7320 3d20 6e6f 7465 626f 6f6b 5472  ets = notebookTr
-00000df0: 6163 6b65 722e 6375 7272 656e 7457 6964  acker.currentWid
-00000e00: 6765 743f 2e63 6f6e 7465 6e74 2e77 6964  get?.content.wid
-00000e10: 6765 7473 2e66 696c 7465 7228 0a20 2020  gets.filter(.   
-00000e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000e30: 2020 2020 202f 2f20 2020 2863 656c 6c3a       //   (cell:
-00000e40: 2043 656c 6c2c 2069 6e64 6578 3a20 6e75   Cell, index: nu
-00000e50: 6d62 6572 2920 3d3e 2028 6365 6c6c 2e6d  mber) => (cell.m
-00000e60: 6f64 656c 2e69 6420 3d3d 3d20 6365 6c6c  odel.id === cell
-00000e70: 4d6f 6465 6c2e 6964 290a 2020 2020 2020  Model.id).      
-00000e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000e90: 2020 2f2f 2029 0a20 2020 2020 2020 2020    // ).         
-00000ea0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00000eb0: 6620 2863 6861 6e67 652e 7479 7065 203d  f (change.type =
-00000ec0: 3d3d 2027 6368 616e 6765 2729 207b 0a20  == 'change') {. 
-00000ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000ee0: 2020 2020 2020 2020 2020 2063 6f6e 736f             conso
-00000ef0: 6c65 2e64 6562 7567 2827 6368 616e 6765  le.debug('change
-00000f00: 272c 2063 6861 6e67 652c 2063 6861 6e67  ', change, chang
-00000f10: 652e 6e65 7756 616c 7565 293b 0a20 2020  e.newValue);.   
-00000f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000f30: 2020 2020 2020 2020 202f 2f20 636f 6d70           // comp
-00000f40: 7574 6520 6469 6666 6572 656e 6365 2062  ute difference b
-00000f50: 6574 7765 656e 206f 6c64 2061 6e64 206e  etween old and n
-00000f60: 6577 2074 6167 730a 2020 2020 2020 2020  ew tags.        
-00000f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000f80: 2020 2020 636f 6e73 7420 6f6c 6454 6167      const oldTag
-00000f90: 7320 3d20 6368 616e 6765 2e6f 6c64 5661  s = change.oldVa
-00000fa0: 6c75 653b 0a20 2020 2020 2020 2020 2020  lue;.           
-00000fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000fc0: 2063 6f6e 7374 206e 6577 5461 6773 203d   const newTags =
-00000fd0: 2063 6861 6e67 652e 6e65 7756 616c 7565   change.newValue
-00000fe0: 3b0a 2020 2020 2020 2020 2020 2020 2020  ;.              
-00000ff0: 2020 2020 2020 2020 2020 2020 2020 636f                co
-00001000: 6e73 7420 6164 6465 6454 6167 7320 3d20  nst addedTags = 
-00001010: 6e65 7754 6167 732e 6669 6c74 6572 2828  newTags.filter((
-00001020: 7461 6729 203d 3e20 216f 6c64 5461 6773  tag) => !oldTags
-00001030: 2e69 6e63 6c75 6465 7328 7461 6729 293b  .includes(tag));
-00001040: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001050: 2020 2020 2020 2020 2020 2020 2063 6f6e               con
-00001060: 7374 2072 656d 6f76 6564 5461 6773 203d  st removedTags =
-00001070: 206f 6c64 5461 6773 2e66 696c 7465 7228   oldTags.filter(
-00001080: 2874 6167 2920 3d3e 2021 6e65 7754 6167  (tag) => !newTag
-00001090: 732e 696e 636c 7564 6573 2874 6167 2929  s.includes(tag))
-000010a0: 3b0a 2020 2020 2020 2020 2020 2020 2020  ;.              
-000010b0: 2020 2020 2020 2020 2020 2020 2020 636f                co
-000010c0: 6e73 6f6c 652e 6c6f 6728 2761 6464 6564  nsole.log('added
-000010d0: 5461 6773 272c 2061 6464 6564 5461 6773  Tags', addedTags
-000010e0: 293b 0a20 2020 2020 2020 2020 2020 2020  );.             
-000010f0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00001100: 6f6e 736f 6c65 2e6c 6f67 2827 7265 6d6f  onsole.log('remo
-00001110: 7665 6454 6167 7327 2c20 7265 6d6f 7665  vedTags', remove
-00001120: 6454 6167 7329 3b0a 2020 2020 2020 2020  dTags);.        
-00001130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001140: 2020 2020 6365 6c6c 5769 6467 6574 732e      cellWidgets.
-00001150: 666f 7245 6163 6828 6365 6c6c 5769 6467  forEach(cellWidg
-00001160: 6574 203d 3e20 7b0a 2020 2020 2020 2020  et => {.        
-00001170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001180: 2020 2020 2020 2020 6164 6465 6454 6167          addedTag
-00001190: 732e 666f 7245 6163 6828 7461 6720 3d3e  s.forEach(tag =>
-000011a0: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
-000011b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000011c0: 2020 2020 2020 2063 6f6e 736f 6c65 2e64         console.d
-000011d0: 6562 7567 2860 6164 6469 6e67 2063 6c61  ebug(`adding cla
-000011e0: 7373 2066 6f72 2074 6167 2024 7b63 6c61  ss for tag ${cla
-000011f0: 7373 5f66 6f72 5f74 6167 2874 6167 297d  ss_for_tag(tag)}
-00001200: 6029 3b0a 2020 2020 2020 2020 2020 2020  `);.            
-00001210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001220: 2020 2020 2020 2020 6365 6c6c 5769 6467          cellWidg
-00001230: 6574 2e61 6464 436c 6173 7328 636c 6173  et.addClass(clas
-00001240: 735f 666f 725f 7461 6728 7461 6729 293b  s_for_tag(tag));
-00001250: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001270: 207d 293b 0a20 2020 2020 2020 2020 2020   });.           
-00001280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001290: 2020 2020 2072 656d 6f76 6564 5461 6773       removedTags
-000012a0: 2e66 6f72 4561 6368 2874 6167 203d 3e20  .forEach(tag => 
-000012b0: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
-000012c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000012d0: 2020 2020 2020 636f 6e73 6f6c 652e 6465        console.de
-000012e0: 6275 6728 6072 656d 6f76 696e 6720 636c  bug(`removing cl
-000012f0: 6173 7320 666f 7220 7461 6720 247b 636c  ass for tag ${cl
-00001300: 6173 735f 666f 725f 7461 6728 7461 6729  ass_for_tag(tag)
-00001310: 7d60 293b 0a20 2020 2020 2020 2020 2020  }`);.           
-00001320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001330: 2020 2020 2020 2020 2063 656c 6c57 6964           cellWid
-00001340: 6765 742e 7265 6d6f 7665 436c 6173 7328  get.removeClass(
-00001350: 636c 6173 735f 666f 725f 7461 6728 7461  class_for_tag(ta
-00001360: 6729 293b 0a20 2020 2020 2020 2020 2020  g));.           
-00001370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001380: 2020 2020 207d 293b 0a20 2020 2020 2020       });.       
-00001390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000013a0: 2020 2020 207d 293b 0a20 2020 2020 2020       });.       
-000013b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000013c0: 207d 0a20 2020 2020 2020 2020 2020 2020   }.             
-000013d0: 2020 2020 2020 2020 2020 2065 6c73 6520             else 
-000013e0: 6966 2028 6368 616e 6765 2e74 7970 6520  if (change.type 
-000013f0: 3d3d 3d20 2761 6464 2729 207b 0a20 2020  === 'add') {.   
-00001400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001410: 2020 2020 2020 2020 2063 6f6e 736f 6c65           console
-00001420: 2e6c 6f67 2827 6164 6427 2c20 6368 616e  .log('add', chan
-00001430: 6765 2c20 6368 616e 6765 2e6e 6577 5661  ge, change.newVa
-00001440: 6c75 6529 3b0a 2020 2020 2020 2020 2020  lue);.          
-00001450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001460: 2020 6365 6c6c 5769 6467 6574 732e 666f    cellWidgets.fo
-00001470: 7245 6163 6828 2863 656c 6c57 6964 6765  rEach((cellWidge
-00001480: 7429 203d 3e20 7b0a 2020 2020 2020 2020  t) => {.        
-00001490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000014a0: 2020 2020 2020 2020 666f 7220 2863 6f6e          for (con
-000014b0: 7374 2074 6167 206f 6620 6368 616e 6765  st tag of change
-000014c0: 2e6e 6577 5661 6c75 6529 207b 0a20 2020  .newValue) {.   
-000014d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000014e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000014f0: 2063 6f6e 736f 6c65 2e64 6562 7567 2860   console.debug(`
-00001500: 6164 6469 6e67 2063 6c61 7373 2066 6f72  adding class for
-00001510: 2074 6167 2024 7b63 6c61 7373 5f66 6f72   tag ${class_for
-00001520: 5f74 6167 2874 6167 297d 6029 3b0a 2020  _tag(tag)}`);.  
-00001530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001550: 2020 6365 6c6c 5769 6467 6574 2e61 6464    cellWidget.add
-00001560: 436c 6173 7328 636c 6173 735f 666f 725f  Class(class_for_
-00001570: 7461 6728 7461 6729 293b 0a20 2020 2020  tag(tag));.     
-00001580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001590: 2020 2020 2020 2020 2020 207d 0a20 2020             }.   
-000015a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000015b0: 2020 2020 2020 2020 207d 293b 0a20 2020           });.   
-000015c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000015d0: 2020 2020 207d 0a20 2020 2020 2020 2020       }.         
-000015e0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-000015f0: 6c73 6520 6966 2028 6368 616e 6765 2e74  lse if (change.t
-00001600: 7970 6520 3d3d 3d20 2772 656d 6f76 6527  ype === 'remove'
-00001610: 2920 7b0a 2020 2020 2020 2020 2020 2020  ) {.            
-00001620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001630: 636f 6e73 6f6c 652e 6c6f 6728 2772 656d  console.log('rem
-00001640: 6f76 6527 2c20 6368 616e 6765 2c20 6368  ove', change, ch
-00001650: 616e 6765 2e6e 6577 5661 6c75 6529 3b0a  ange.newValue);.
-00001660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001670: 2020 2020 2020 2020 2020 2020 6365 6c6c              cell
-00001680: 5769 6467 6574 732e 666f 7245 6163 6828  Widgets.forEach(
-00001690: 2863 656c 6c57 6964 6765 7429 203d 3e20  (cellWidget) => 
-000016a0: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
-000016b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000016c0: 2020 666f 7220 2863 6f6e 7374 2074 6167    for (const tag
-000016d0: 206f 6620 6368 616e 6765 2e6e 6577 5661   of change.newVa
-000016e0: 6c75 6529 207b 0a20 2020 2020 2020 2020  lue) {.         
-000016f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001700: 2020 2020 2020 2020 2020 2063 6f6e 736f             conso
-00001710: 6c65 2e64 6562 7567 2860 7265 6d6f 7669  le.debug(`removi
-00001720: 6e67 2063 6c61 7373 2066 6f72 2074 6167  ng class for tag
-00001730: 2024 7b63 6c61 7373 5f66 6f72 5f74 6167   ${class_for_tag
-00001740: 2874 6167 297d 6029 3b0a 2020 2020 2020  (tag)}`);.      
-00001750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001760: 2020 2020 2020 2020 2020 2020 2020 6365                ce
-00001770: 6c6c 5769 6467 6574 2e72 656d 6f76 6543  llWidget.removeC
-00001780: 6c61 7373 2863 6c61 7373 5f66 6f72 5f74  lass(class_for_t
-00001790: 6167 2874 6167 2929 3b0a 2020 2020 2020  ag(tag));.      
-000017a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000017b0: 2020 2020 2020 2020 2020 7d0a 2020 2020            }.    
-000017c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000017d0: 2020 2020 2020 2020 7d29 3b0a 2020 2020          });.    
-000017e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000017f0: 2020 2020 7d0a 2020 2020 2020 2020 2020      }.          
-00001800: 2020 2020 2020 2020 2020 7d29 3b0a 2020            });.  
-00001810: 2020 2020 2020 2020 2020 2020 2020 7d29                })
-00001820: 3b0a 2020 2020 2020 2020 2020 2020 7d29  ;.            })
-00001830: 3b0a 2020 2020 2020 2020 7d29 3b0a 2020  ;.        });.  
-00001840: 2020 7d0a 7d3b 0a2f 2a20 6861 726d 6f6e    }.};./* harmon
-00001850: 7920 6465 6661 756c 7420 6578 706f 7274  y default export
-00001860: 202a 2f20 636f 6e73 7420 5f5f 5745 4250   */ const __WEBP
-00001870: 4143 4b5f 4445 4641 554c 545f 4558 504f  ACK_DEFAULT_EXPO
-00001880: 5254 5f5f 203d 2028 706c 7567 696e 293b  RT__ = (plugin);
-00001890: 0a0a 0a2f 2a2a 2a2f 207d 290a 0a7d 5d29  .../***/ })..}])
-000018a0: 3b0a 2f2f 2320 736f 7572 6365 4d61 7070  ;.//# sourceMapp
-000018b0: 696e 6755 524c 3d6c 6962 5f69 6e64 6578  ingURL=lib_index
-000018c0: 5f6a 732e 3734 3562 3762 3037 6539 3162  _js.745b7b07e91b
-000018d0: 3133 3664 3336 6238 2e6a 732e 6d61 70    136d36b8.js.map
+00000000: 2f2a 0a20 2a20 666f 7220 6174 7461 6368  /*. * for attach
+00000010: 696e 6720 6b65 7962 696e 6469 6e67 7320  ing keybindings 
+00000020: 6c61 7465 7220 6f6e 2c20 7365 650a 202a  later on, see. *
+00000030: 2068 7474 7073 3a2f 2f74 6f77 6172 6473   https://towards
+00000040: 6461 7461 7363 6965 6e63 652e 636f 6d2f  datascience.com/
+00000050: 686f 772d 746f 2d63 7573 746f 6d69 7a65  how-to-customize
+00000060: 2d6a 7570 7974 6572 6c61 622d 6b65 7962  -jupyterlab-keyb
+00000070: 6f61 7264 2d73 686f 7274 6375 7473 2d37  oard-shortcuts-7
+00000080: 3233 3231 6637 3337 3533 640a 202a 2f0a  2321f73753d. */.
+00000090: 0a2f 2a20 6573 6c69 6e74 2d64 6973 6162  ./* eslint-disab
+000000a0: 6c65 2070 7265 7474 6965 722f 7072 6574  le prettier/pret
+000000b0: 7469 6572 202a 2f0a 0a69 6d70 6f72 7420  tier */..import 
+000000c0: 7b20 4a75 7079 7465 7246 726f 6e74 456e  { JupyterFrontEn
+000000d0: 642c 204a 7570 7974 6572 4672 6f6e 7445  d, JupyterFrontE
+000000e0: 6e64 506c 7567 696e 207d 2066 726f 6d20  ndPlugin } from 
+000000f0: 2740 6a75 7079 7465 726c 6162 2f61 7070  '@jupyterlab/app
+00000100: 6c69 6361 7469 6f6e 270a 0a69 6d70 6f72  lication'..impor
+00000110: 7420 7b20 494e 6f74 6562 6f6f 6b54 7261  t { INotebookTra
+00000120: 636b 6572 207d 2066 726f 6d20 2740 6a75  cker } from '@ju
+00000130: 7079 7465 726c 6162 2f6e 6f74 6562 6f6f  pyterlab/noteboo
+00000140: 6b27 0a0a 696d 706f 7274 207b 2049 4365  k'..import { ICe
+00000150: 6c6c 4d6f 6465 6c2c 2043 656c 6c20 7d20  llModel, Cell } 
+00000160: 6672 6f6d 2027 406a 7570 7974 6572 6c61  from '@jupyterla
+00000170: 622f 6365 6c6c 7327 0a0a 2f2a 2a0a 202a  b/cells'../**. *
+00000180: 2049 6e69 7469 616c 697a 6174 696f 6e20   Initialization 
+00000190: 6461 7461 2066 6f72 2074 6865 206a 7570  data for the jup
+000001a0: 7974 6572 6c61 622d 6365 6c6c 7461 6773  yterlab-celltags
+000001b0: 636c 6173 7365 7320 6578 7465 6e73 696f  classes extensio
+000001c0: 6e2e 0a20 2a2f 0a63 6f6e 7374 2070 6c75  n.. */.const plu
+000001d0: 6769 6e3a 204a 7570 7974 6572 4672 6f6e  gin: JupyterFron
+000001e0: 7445 6e64 506c 7567 696e 3c76 6f69 643e  tEndPlugin<void>
+000001f0: 203d 207b 0a20 2069 643a 2027 6a75 7079   = {.  id: 'jupy
+00000200: 7465 726c 6162 2d63 656c 6c74 6167 7363  terlab-celltagsc
+00000210: 6c61 7373 6573 3a70 6c75 6769 6e27 2c0a  lasses:plugin',.
+00000220: 2020 6175 746f 5374 6172 743a 2074 7275    autoStart: tru
+00000230: 652c 0a20 2072 6571 7569 7265 733a 205b  e,.  requires: [
+00000240: 494e 6f74 6562 6f6f 6b54 7261 636b 6572  INotebookTracker
+00000250: 5d2c 0a20 2061 6374 6976 6174 653a 2028  ],.  activate: (
+00000260: 6170 703a 204a 7570 7974 6572 4672 6f6e  app: JupyterFron
+00000270: 7445 6e64 2c20 6e6f 7465 626f 6f6b 5472  tEnd, notebookTr
+00000280: 6163 6b65 723a 2049 4e6f 7465 626f 6f6b  acker: INotebook
+00000290: 5472 6163 6b65 7229 203d 3e20 7b0a 2020  Tracker) => {.  
+000002a0: 2020 636f 6e73 6f6c 652e 6c6f 6728 2765    console.log('e
+000002b0: 7874 656e 7369 6f6e 206a 7570 7974 6572  xtension jupyter
+000002c0: 6c61 622d 6365 6c6c 7461 6773 636c 6173  lab-celltagsclas
+000002d0: 7365 7320 6973 2061 6374 6976 6174 696e  ses is activatin
+000002e0: 6727 290a 0a20 2020 2063 6f6e 7374 2063  g')..    const c
+000002f0: 6c61 7373 5f66 6f72 5f74 6167 203d 2028  lass_for_tag = (
+00000300: 7461 673a 2073 7472 696e 6729 203d 3e20  tag: string) => 
+00000310: 6063 656c 6c2d 7461 672d 247b 7461 677d  `cell-tag-${tag}
+00000320: 600a 0a20 2020 206e 6f74 6562 6f6f 6b54  `..    notebookT
+00000330: 7261 636b 6572 2e77 6964 6765 7441 6464  racker.widgetAdd
+00000340: 6564 2e63 6f6e 6e65 6374 2828 5f2c 2070  ed.connect((_, p
+00000350: 616e 656c 2920 3d3e 207b 0a20 2020 2020  anel) => {.     
+00000360: 2063 6f6e 7374 206e 6f74 6562 6f6f 6b4d   const notebookM
+00000370: 6f64 656c 203d 2070 616e 656c 2e63 6f6e  odel = panel.con
+00000380: 7465 6e74 2e6d 6f64 656c 0a20 2020 2020  tent.model.     
+00000390: 2069 6620 286e 6f74 6562 6f6f 6b4d 6f64   if (notebookMod
+000003a0: 656c 203d 3d3d 206e 756c 6c29 207b 0a20  el === null) {. 
+000003b0: 2020 2020 2020 2072 6574 7572 6e0a 2020         return.  
+000003c0: 2020 2020 7d0a 0a20 2020 2020 206e 6f74      }..      not
+000003d0: 6562 6f6f 6b4d 6f64 656c 2e63 656c 6c73  ebookModel.cells
+000003e0: 2e63 6861 6e67 6564 2e63 6f6e 6e65 6374  .changed.connect
+000003f0: 2828 6365 6c6c 4c69 7374 2c20 6368 616e  ((cellList, chan
+00000400: 6765 2920 3d3e 207b 0a20 2020 2020 2020  ge) => {.       
+00000410: 2069 6620 2863 6861 6e67 652e 7479 7065   if (change.type
+00000420: 2021 3d3d 2027 6164 6427 2920 7b0a 2020   !== 'add') {.  
+00000430: 2020 2020 2020 2020 7265 7475 726e 0a20          return. 
+00000440: 2020 2020 2020 207d 0a20 2020 2020 2020         }.       
+00000450: 2063 6861 6e67 652e 6e65 7756 616c 7565   change.newValue
+00000460: 732e 666f 7245 6163 6828 6365 6c6c 4d6f  s.forEach(cellMo
+00000470: 6465 6c20 3d3e 207b 0a20 2020 2020 2020  del => {.       
+00000480: 2020 202f 2f20 636f 6d70 7574 6520 7769     // compute wi
+00000490: 6467 6574 7320 6174 7461 6368 6564 2074  dgets attached t
+000004a0: 6f20 6365 6c6c 4d6f 6465 6c0a 2020 2020  o cellModel.    
+000004b0: 2020 2020 2020 636f 6e73 7420 6365 6c6c        const cell
+000004c0: 5769 6467 6574 7320 3d0a 2020 2020 2020  Widgets =.      
+000004d0: 2020 2020 2020 6e6f 7465 626f 6f6b 5472        notebookTr
+000004e0: 6163 6b65 722e 6375 7272 656e 7457 6964  acker.currentWid
+000004f0: 6765 743f 2e63 6f6e 7465 6e74 2e77 6964  get?.content.wid
+00000500: 6765 7473 2e66 696c 7465 7228 0a20 2020  gets.filter(.   
+00000510: 2020 2020 2020 2020 2020 2028 6365 6c6c             (cell
+00000520: 3a20 4365 6c6c 2c20 696e 6465 783a 206e  : Cell, index: n
+00000530: 756d 6265 7229 203d 3e20 6365 6c6c 2e6d  umber) => cell.m
+00000540: 6f64 656c 2e69 6420 3d3d 3d20 6365 6c6c  odel.id === cell
+00000550: 4d6f 6465 6c2e 6964 0a20 2020 2020 2020  Model.id.       
+00000560: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
+00000570: 2069 6620 2863 656c 6c57 6964 6765 7473   if (cellWidgets
+00000580: 203d 3d3d 2075 6e64 6566 696e 6564 207c   === undefined |
+00000590: 7c20 6365 6c6c 5769 6467 6574 733f 2e6c  | cellWidgets?.l
+000005a0: 656e 6774 6820 3d3d 3d20 3029 207b 0a20  ength === 0) {. 
+000005b0: 2020 2020 2020 2020 2020 2063 6f6e 736f             conso
+000005c0: 6c65 2e77 6172 6e28 2763 6f75 6c64 206e  le.warn('could n
+000005d0: 6f74 2066 696e 6420 6365 6c6c 2077 6964  ot find cell wid
+000005e0: 6765 7420 666f 7220 6365 6c6c 206d 6f64  get for cell mod
+000005f0: 656c 272c 2063 656c 6c4d 6f64 656c 290a  el', cellModel).
+00000600: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00000610: 726e 0a20 2020 2020 2020 2020 207d 0a20  rn.          }. 
+00000620: 2020 2020 2020 2020 2063 6f6e 736f 6c65           console
+00000630: 2e64 6562 7567 280a 2020 2020 2020 2020  .debug(.        
+00000640: 2020 2020 6066 6f75 6e64 2024 7b63 656c      `found ${cel
+00000650: 6c57 6964 6765 7473 3f2e 6c65 6e67 7468  lWidgets?.length
+00000660: 7d20 6365 6c6c 2077 6964 6765 7473 602c  } cell widgets`,
+00000670: 0a20 2020 2020 2020 2020 2020 2063 656c  .            cel
+00000680: 6c57 6964 6765 7473 5b30 5d0a 2020 2020  lWidgets[0].    
+00000690: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
+000006a0: 2020 202f 2f20 6164 6420 636c 6173 7365     // add classe
+000006b0: 7320 666f 7220 7072 652d 6578 6973 7469  s for pre-existi
+000006c0: 6e67 2074 6167 730a 2020 2020 2020 2020  ng tags.        
+000006d0: 2020 6365 6c6c 4d6f 6465 6c2e 6765 744d    cellModel.getM
+000006e0: 6574 6164 6174 6128 2774 6167 7327 293f  etadata('tags')?
+000006f0: 2e66 6f72 4561 6368 2828 7461 673a 2073  .forEach((tag: s
+00000700: 7472 696e 6729 203d 3e0a 2020 2020 2020  tring) =>.      
+00000710: 2020 2020 2020 6365 6c6c 5769 6467 6574        cellWidget
+00000720: 733f 2e66 6f72 4561 6368 2863 656c 6c57  s?.forEach(cellW
+00000730: 6964 6765 7420 3d3e 207b 0a20 2020 2020  idget => {.     
+00000740: 2020 2020 2020 2020 2063 6f6e 736f 6c65           console
+00000750: 2e64 6562 7567 280a 2020 2020 2020 2020  .debug(.        
+00000760: 2020 2020 2020 2020 6061 6464 696e 6720          `adding 
+00000770: 696e 6974 6961 6c20 636c 6173 7320 666f  initial class fo
+00000780: 7220 7461 6720 247b 636c 6173 735f 666f  r tag ${class_fo
+00000790: 725f 7461 6728 7461 6729 7d60 0a20 2020  r_tag(tag)}`.   
+000007a0: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+000007b0: 2020 2020 2020 2020 2020 2063 656c 6c57             cellW
+000007c0: 6964 6765 742e 6164 6443 6c61 7373 2863  idget.addClass(c
+000007d0: 6c61 7373 5f66 6f72 5f74 6167 2874 6167  lass_for_tag(tag
+000007e0: 2929 0a20 2020 2020 2020 2020 2020 207d  )).            }
+000007f0: 290a 2020 2020 2020 2020 2020 290a 0a20  ).          ).. 
+00000800: 2020 2020 2020 2020 202f 2f20 7265 6163           // reac
+00000810: 7420 746f 2063 6861 6e67 6573 2069 6e20  t to changes in 
+00000820: 7461 6773 0a20 2020 2020 2020 2020 2063  tags.          c
+00000830: 656c 6c4d 6f64 656c 2e6d 6574 6164 6174  ellModel.metadat
+00000840: 6143 6861 6e67 6564 2e63 6f6e 6e65 6374  aChanged.connect
+00000850: 2828 7365 6e64 6572 3a20 4943 656c 6c4d  ((sender: ICellM
+00000860: 6f64 656c 2c20 6368 616e 6765 2920 3d3e  odel, change) =>
+00000870: 207b 0a20 2020 2020 2020 2020 2020 2063   {.            c
+00000880: 6f6e 736f 6c65 2e64 6562 7567 2827 6d65  onsole.debug('me
+00000890: 7461 6461 7461 2063 6861 6e67 6564 272c  tadata changed',
+000008a0: 2073 656e 6465 722c 2063 6861 6e67 6529   sender, change)
+000008b0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+000008c0: 2863 6861 6e67 652e 6b65 7920 213d 3d20  (change.key !== 
+000008d0: 2774 6167 7327 2920 7b0a 2020 2020 2020  'tags') {.      
+000008e0: 2020 2020 2020 2020 2f2f 2063 6f6e 736f          // conso
+000008f0: 6c65 2e64 6562 7567 2822 6967 6e6f 7269  le.debug("ignori
+00000900: 6e67 206e 6f6e 2d74 6167 7320 6d65 7461  ng non-tags meta
+00000910: 6461 7461 2063 6861 6e67 6522 290a 2020  data change").  
+00000920: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00000930: 726e 0a20 2020 2020 2020 2020 2020 207d  rn.            }
+00000940: 0a20 2020 2020 2020 2020 2020 202f 2f20  .            // 
+00000950: 646f 6573 206e 6f74 2073 6565 6d20 7573  does not seem us
+00000960: 6566 756c 2074 6f20 7265 636f 6d70 7574  eful to recomput
+00000970: 6520 7468 6973 0a20 2020 2020 2020 2020  e this.         
+00000980: 2020 202f 2f20 636f 6e73 7420 6365 6c6c     // const cell
+00000990: 5769 6467 6574 7320 3d20 6e6f 7465 626f  Widgets = notebo
+000009a0: 6f6b 5472 6163 6b65 722e 6375 7272 656e  okTracker.curren
+000009b0: 7457 6964 6765 743f 2e63 6f6e 7465 6e74  tWidget?.content
+000009c0: 2e77 6964 6765 7473 2e66 696c 7465 7228  .widgets.filter(
+000009d0: 0a20 2020 2020 2020 2020 2020 202f 2f20  .            // 
+000009e0: 2020 2863 656c 6c3a 2043 656c 6c2c 2069    (cell: Cell, i
+000009f0: 6e64 6578 3a20 6e75 6d62 6572 2920 3d3e  ndex: number) =>
+00000a00: 2028 6365 6c6c 2e6d 6f64 656c 2e69 6420   (cell.model.id 
+00000a10: 3d3d 3d20 6365 6c6c 4d6f 6465 6c2e 6964  === cellModel.id
+00000a20: 290a 2020 2020 2020 2020 2020 2020 2f2f  ).            //
+00000a30: 2029 0a20 2020 2020 2020 2020 2020 2069   ).            i
+00000a40: 6620 2863 6861 6e67 652e 7479 7065 203d  f (change.type =
+00000a50: 3d3d 2027 6368 616e 6765 2729 207b 0a20  == 'change') {. 
+00000a60: 2020 2020 2020 2020 2020 2020 2063 6f6e               con
+00000a70: 736f 6c65 2e64 6562 7567 2827 6368 616e  sole.debug('chan
+00000a80: 6765 272c 2063 6861 6e67 652c 2063 6861  ge', change, cha
+00000a90: 6e67 652e 6e65 7756 616c 7565 290a 2020  nge.newValue).  
+00000aa0: 2020 2020 2020 2020 2020 2020 2f2f 2063              // c
+00000ab0: 6f6d 7075 7465 2064 6966 6665 7265 6e63  ompute differenc
+00000ac0: 6520 6265 7477 6565 6e20 6f6c 6420 616e  e between old an
+00000ad0: 6420 6e65 7720 7461 6773 0a20 2020 2020  d new tags.     
+00000ae0: 2020 2020 2020 2020 2063 6f6e 7374 206f           const o
+00000af0: 6c64 5461 6773 203d 2063 6861 6e67 652e  ldTags = change.
+00000b00: 6f6c 6456 616c 7565 2061 7320 7374 7269  oldValue as stri
+00000b10: 6e67 5b5d 0a20 2020 2020 2020 2020 2020  ng[].           
+00000b20: 2020 2063 6f6e 7374 206e 6577 5461 6773     const newTags
+00000b30: 203d 2063 6861 6e67 652e 6e65 7756 616c   = change.newVal
+00000b40: 7565 2061 7320 7374 7269 6e67 5b5d 0a20  ue as string[]. 
+00000b50: 2020 2020 2020 2020 2020 2020 2063 6f6e               con
+00000b60: 7374 2061 6464 6564 5461 6773 203d 206e  st addedTags = n
+00000b70: 6577 5461 6773 2e66 696c 7465 7228 7461  ewTags.filter(ta
+00000b80: 6720 3d3e 2021 6f6c 6454 6167 732e 696e  g => !oldTags.in
+00000b90: 636c 7564 6573 2874 6167 2929 0a20 2020  cludes(tag)).   
+00000ba0: 2020 2020 2020 2020 2020 2063 6f6e 7374             const
+00000bb0: 2072 656d 6f76 6564 5461 6773 203d 206f   removedTags = o
+00000bc0: 6c64 5461 6773 2e66 696c 7465 7228 7461  ldTags.filter(ta
+00000bd0: 6720 3d3e 2021 6e65 7754 6167 732e 696e  g => !newTags.in
+00000be0: 636c 7564 6573 2874 6167 2929 0a20 2020  cludes(tag)).   
+00000bf0: 2020 2020 2020 2020 2020 202f 2f20 636f             // co
+00000c00: 6e73 6f6c 652e 6465 6275 6728 2761 6464  nsole.debug('add
+00000c10: 6564 5461 6773 272c 2061 6464 6564 5461  edTags', addedTa
+00000c20: 6773 290a 2020 2020 2020 2020 2020 2020  gs).            
+00000c30: 2020 2f2f 2063 6f6e 736f 6c65 2e64 6562    // console.deb
+00000c40: 7567 2827 7265 6d6f 7665 6454 6167 7327  ug('removedTags'
+00000c50: 2c20 7265 6d6f 7665 6454 6167 7329 0a20  , removedTags). 
+00000c60: 2020 2020 2020 2020 2020 2020 2063 656c               cel
+00000c70: 6c57 6964 6765 7473 2e66 6f72 4561 6368  lWidgets.forEach
+00000c80: 2863 656c 6c57 6964 6765 7420 3d3e 207b  (cellWidget => {
+00000c90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000ca0: 2061 6464 6564 5461 6773 2e66 6f72 4561   addedTags.forEa
+00000cb0: 6368 2874 6167 203d 3e20 7b0a 2020 2020  ch(tag => {.    
+00000cc0: 2020 2020 2020 2020 2020 2020 2020 636f                co
+00000cd0: 6e73 6f6c 652e 6465 6275 6728 6061 6464  nsole.debug(`add
+00000ce0: 696e 6720 636c 6173 7320 666f 7220 7461  ing class for ta
+00000cf0: 6720 247b 636c 6173 735f 666f 725f 7461  g ${class_for_ta
+00000d00: 6728 7461 6729 7d60 290a 2020 2020 2020  g(tag)}`).      
+00000d10: 2020 2020 2020 2020 2020 2020 6365 6c6c              cell
+00000d20: 5769 6467 6574 2e61 6464 436c 6173 7328  Widget.addClass(
+00000d30: 636c 6173 735f 666f 725f 7461 6728 7461  class_for_tag(ta
+00000d40: 6729 290a 2020 2020 2020 2020 2020 2020  g)).            
+00000d50: 2020 2020 7d29 0a20 2020 2020 2020 2020      }).         
+00000d60: 2020 2020 2020 2072 656d 6f76 6564 5461         removedTa
+00000d70: 6773 2e66 6f72 4561 6368 2874 6167 203d  gs.forEach(tag =
+00000d80: 3e20 7b0a 2020 2020 2020 2020 2020 2020  > {.            
+00000d90: 2020 2020 2020 636f 6e73 6f6c 652e 6465        console.de
+00000da0: 6275 6728 6072 656d 6f76 696e 6720 636c  bug(`removing cl
+00000db0: 6173 7320 666f 7220 7461 6720 247b 636c  ass for tag ${cl
+00000dc0: 6173 735f 666f 725f 7461 6728 7461 6729  ass_for_tag(tag)
+00000dd0: 7d60 290a 2020 2020 2020 2020 2020 2020  }`).            
+00000de0: 2020 2020 2020 6365 6c6c 5769 6467 6574        cellWidget
+00000df0: 2e72 656d 6f76 6543 6c61 7373 2863 6c61  .removeClass(cla
+00000e00: 7373 5f66 6f72 5f74 6167 2874 6167 2929  ss_for_tag(tag))
+00000e10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000e20: 207d 290a 2020 2020 2020 2020 2020 2020   }).            
+00000e30: 2020 7d29 0a20 2020 2020 2020 2020 2020    }).           
+00000e40: 207d 2065 6c73 6520 6966 2028 6368 616e   } else if (chan
+00000e50: 6765 2e74 7970 6520 3d3d 3d20 2761 6464  ge.type === 'add
+00000e60: 2729 207b 0a20 2020 2020 2020 2020 2020  ') {.           
+00000e70: 2020 2063 6f6e 736f 6c65 2e6c 6f67 2827     console.log('
+00000e80: 6164 6427 2c20 6368 616e 6765 2c20 6368  add', change, ch
+00000e90: 616e 6765 2e6e 6577 5661 6c75 6529 0a20  ange.newValue). 
+00000ea0: 2020 2020 2020 2020 2020 2020 2063 656c               cel
+00000eb0: 6c57 6964 6765 7473 2e66 6f72 4561 6368  lWidgets.forEach
+00000ec0: 2863 656c 6c57 6964 6765 7420 3d3e 207b  (cellWidget => {
+00000ed0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000ee0: 2066 6f72 2028 636f 6e73 7420 7461 6720   for (const tag 
+00000ef0: 6f66 2063 6861 6e67 652e 6e65 7756 616c  of change.newVal
+00000f00: 7565 2920 7b0a 2020 2020 2020 2020 2020  ue) {.          
+00000f10: 2020 2020 2020 2020 636f 6e73 6f6c 652e          console.
+00000f20: 6465 6275 6728 6061 6464 696e 6720 636c  debug(`adding cl
+00000f30: 6173 7320 666f 7220 7461 6720 247b 636c  ass for tag ${cl
+00000f40: 6173 735f 666f 725f 7461 6728 7461 6729  ass_for_tag(tag)
+00000f50: 7d60 290a 2020 2020 2020 2020 2020 2020  }`).            
+00000f60: 2020 2020 2020 6365 6c6c 5769 6467 6574        cellWidget
+00000f70: 2e61 6464 436c 6173 7328 636c 6173 735f  .addClass(class_
+00000f80: 666f 725f 7461 6728 7461 6729 290a 2020  for_tag(tag)).  
+00000f90: 2020 2020 2020 2020 2020 2020 2020 7d0a                }.
+00000fa0: 2020 2020 2020 2020 2020 2020 2020 7d29                })
+00000fb0: 0a20 2020 2020 2020 2020 2020 207d 2065  .            } e
+00000fc0: 6c73 6520 6966 2028 6368 616e 6765 2e74  lse if (change.t
+00000fd0: 7970 6520 3d3d 3d20 2772 656d 6f76 6527  ype === 'remove'
+00000fe0: 2920 7b0a 2020 2020 2020 2020 2020 2020  ) {.            
+00000ff0: 2020 636f 6e73 6f6c 652e 6c6f 6728 2772    console.log('r
+00001000: 656d 6f76 6527 2c20 6368 616e 6765 2c20  emove', change, 
+00001010: 6368 616e 6765 2e6e 6577 5661 6c75 6529  change.newValue)
+00001020: 0a20 2020 2020 2020 2020 2020 2020 2063  .              c
+00001030: 656c 6c57 6964 6765 7473 2e66 6f72 4561  ellWidgets.forEa
+00001040: 6368 2863 656c 6c57 6964 6765 7420 3d3e  ch(cellWidget =>
+00001050: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
+00001060: 2020 2066 6f72 2028 636f 6e73 7420 7461     for (const ta
+00001070: 6720 6f66 2063 6861 6e67 652e 6e65 7756  g of change.newV
+00001080: 616c 7565 2920 7b0a 2020 2020 2020 2020  alue) {.        
+00001090: 2020 2020 2020 2020 2020 636f 6e73 6f6c            consol
+000010a0: 652e 6465 6275 6728 6072 656d 6f76 696e  e.debug(`removin
+000010b0: 6720 636c 6173 7320 666f 7220 7461 6720  g class for tag 
+000010c0: 247b 636c 6173 735f 666f 725f 7461 6728  ${class_for_tag(
+000010d0: 7461 6729 7d60 290a 2020 2020 2020 2020  tag)}`).        
+000010e0: 2020 2020 2020 2020 2020 6365 6c6c 5769            cellWi
+000010f0: 6467 6574 2e72 656d 6f76 6543 6c61 7373  dget.removeClass
+00001100: 2863 6c61 7373 5f66 6f72 5f74 6167 2874  (class_for_tag(t
+00001110: 6167 2929 0a20 2020 2020 2020 2020 2020  ag)).           
+00001120: 2020 2020 207d 0a20 2020 2020 2020 2020       }.         
+00001130: 2020 2020 207d 290a 2020 2020 2020 2020       }).        
+00001140: 2020 2020 7d0a 2020 2020 2020 2020 2020      }.          
+00001150: 7d29 0a20 2020 2020 2020 207d 290a 2020  }).        }).  
+00001160: 2020 2020 7d29 0a20 2020 207d 290a 2020      }).    }).  
+00001170: 7d0a 7d0a 0a65 7870 6f72 7420 6465 6661  }.}..export defa
+00001180: 756c 7420 706c 7567 696e 0a0a 2f2f 2072  ult plugin..// r
+00001190: 652d 6578 706f 7274 206d 6574 6164 6174  e-export metadat
+000011a0: 6120 6865 6c70 6572 2066 756e 6374 696f  a helper functio
+000011b0: 6e73 0a65 7870 6f72 7420 7b20 6d64 5f67  ns.export { md_g
+000011c0: 6574 2c20 6d64 5f73 6574 2c20 6d64 5f75  et, md_set, md_u
+000011d0: 6e73 6574 2c20 6d64 5f68 6173 2c20 6d64  nset, md_has, md
+000011e0: 5f69 6e73 6572 742c 206d 645f 7265 6d6f  _insert, md_remo
+000011f0: 7665 2c20 6d64 5f74 6f67 676c 652c 206d  ve, md_toggle, m
+00001200: 645f 636c 6561 6e20 7d20 6672 6f6d 2027  d_clean } from '
+00001210: 2e2f 6d65 7461 6461 7461 270a            ./metadata'.
```

### Comparing `jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/remoteEntry.09eb75b8b35017dd61cc.js` & `jupyterlab_celltagsclasses-0.2.0/jupyterlab_celltagsclasses/labextension/static/remoteEntry.e8bcb578ed91b775bd99.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -182,16 +182,16 @@
     (() => {
         /******/ // This function allow to reference async chunks
         /******/
         __webpack_require__.u = (chunkId) => {
             /******/ // return url for filenames based on template
             /******/
             return "" + chunkId + "." + {
-                "lib_index_js": "69027069f0720bba2d30",
-                "style_index_js": "dcf32fced0a182594cc6"
+                "lib_index_js": "cddacca2ba0e6c761c6d",
+                "style_index_js": "4784725fff15b54ffe3d"
             } [chunkId] + ".js";
             /******/
         };
         /******/
     })();
     /******/
     /******/
@@ -426,15 +426,15 @@
             /******/
             var promises = [];
             /******/
             switch (name) {
                 /******/
                 case "default": {
                     /******/
-                    register("jupyterlab-celltagsclasses", "0.1.0", () => (__webpack_require__.e("lib_index_js").then(() => (() => (__webpack_require__( /*! ./lib/index.js */ "./lib/index.js"))))));
+                    register("jupyterlab-celltagsclasses", "0.2.0", () => (__webpack_require__.e("lib_index_js").then(() => (() => (__webpack_require__( /*! ./lib/index.js */ "./lib/index.js"))))));
                     /******/
                 }
                 /******/
                 break;
                 /******/
             }
             /******/
@@ -827,24 +827,28 @@
             /******/
         });
         /******/
         var installedModules = {};
         /******/
         var moduleToHandlerMapping = {
             /******/
-            "webpack/sharing/consume/default/@jupyterlab/notebook": () => (loadSingletonVersionCheck("default", "@jupyterlab/notebook", [1, 4, 0, 0, , "rc", 0]))
+            "webpack/sharing/consume/default/@jupyterlab/notebook": () => (loadSingletonVersionCheck("default", "@jupyterlab/notebook", [1, 4, 0, 0, , "beta", 2])),
+            /******/
+            "webpack/sharing/consume/default/@jupyterlab/cells": () => (loadVersionCheck("default", "@jupyterlab/cells", [1, 4, 0, 0, , "beta", 2]))
             /******/
         };
         /******/ // no consumes in initial chunks
         /******/
         var chunkMapping = {
             /******/
             "lib_index_js": [
                 /******/
-                "webpack/sharing/consume/default/@jupyterlab/notebook"
+                "webpack/sharing/consume/default/@jupyterlab/notebook",
+                /******/
+                "webpack/sharing/consume/default/@jupyterlab/cells"
                 /******/
             ]
             /******/
         };
         /******/
         __webpack_require__.f.consumes = (chunkId, promises) => {
             /******/
@@ -1071,8 +1075,8 @@
     /******/
     var __webpack_exports__ = __webpack_require__("webpack/container/entry/jupyterlab-celltagsclasses");
     /******/
     (_JUPYTERLAB = typeof _JUPYTERLAB === "undefined" ? {} : _JUPYTERLAB)["jupyterlab-celltagsclasses"] = __webpack_exports__;
     /******/
     /******/
 })();
-//# sourceMappingURL=remoteEntry.09eb75b8b35017dd61cc.js.map
+//# sourceMappingURL=remoteEntry.e8bcb578ed91b775bd99.js.map
```

### Comparing `jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/remoteEntry.09eb75b8b35017dd61cc.js.map` & `jupyterlab_celltagsclasses-0.2.0/jupyterlab_celltagsclasses/labextension/static/remoteEntry.cc30540db9a44cea877f.js.map`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9081632653061226%*

 * *Differences: {"'file'": "'remoteEntry.cc30540db9a44cea877f.js'",*

 * * "'sourcesContent'": "{insert: [(5, '// This function allow to reference async "*

 * *                     'chunks\\n__webpack_require__.u = (chunkId) => {\\n\\t// return url for '*

 * *                     'filenames based on template\\n\\treturn "" + chunkId + "." + '*

 * *                     '{"lib_index_js":"e0bf585461963e3d1e28","style_index_js":"4784725fff15b54ffe3d"}[chunkId] '*

 * *                     '+ ".js";\\n};\'), (10, \'__webpack_require__.S = {};\\nvar initP […]*

```diff
@@ -1,9 +1,9 @@
 {
-    "file": "remoteEntry.09eb75b8b35017dd61cc.js",
+    "file": "remoteEntry.cc30540db9a44cea877f.js",
     "mappings": ";;;;;;;;;;;AAAA;AACA;AACA;AACA,EAAE;AACF;AACA;AACA,EAAE;AACF;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,IAAI;AACJ;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;AAEA;AACA;AACA;AACA;AACA,CAAC;;;;;;UCpCD;UACA;;UAEA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;;;;;WC5BA;WACA;WACA;WACA;WACA;WACA,iCAAiC,WAAW;WAC5C;WACA;;;;;WCPA;WACA;WACA;WACA;WACA,yCAAyC,wCAAwC;WACjF;WACA;WACA;;;;;WCPA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;;;;;WCRA;WACA;WACA;WACA,8BAA8B,8EAA8E;WAC5G;;;;;WCJA;WACA;WACA;WACA;WACA,GAAG;WACH;WACA;WACA,CAAC;;;;;WCPD;;;;;WCAA;WACA;WACA;WACA;WACA,uBAAuB,4BAA4B;WACnD;WACA;WACA;WACA,iBAAiB,oBAAoB;WACrC;WACA,mGAAmG,YAAY;WAC/G;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,mEAAmE,iCAAiC;WACpG;WACA;WACA;WACA;;;;;WCxCA;WACA;WACA;WACA,uDAAuD,iBAAiB;WACxE;WACA,gDAAgD,aAAa;WAC7D;;;;;WCNA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,oJAAoJ;WACpJ;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,IAAI,aAAa;WACjB;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;;;;WC7CA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;;;;WClBA;WACA;WACA,WAAW,6BAA6B,iBAAiB,GAAG,qEAAqE;WACjI;WACA;WACA;WACA,qCAAqC,aAAa,EAAE,wDAAwD,2BAA2B,4BAA4B,2BAA2B,+CAA+C,mCAAmC;WAChR;WACA;WACA;WACA,qBAAqB,8BAA8B,SAAS,sDAAsD,gBAAgB,eAAe,KAAK,6DAA6D,SAAS,SAAS,QAAQ,eAAe,KAAK,eAAe,qGAAqG,WAAW,aAAa;WAC7Y;WACA;WACA;WACA,gBAAgB,8BAA8B,qBAAqB,YAAY,sBAAsB,SAAS,iDAAiD,6FAA6F,WAAW,uBAAuB,2BAA2B,wBAAwB,KAAK,oCAAoC,oBAAoB,wBAAwB,oBAAoB,SAAS,KAAK,yBAAyB,KAAK,gCAAgC,yBAAyB,QAAQ,eAAe,KAAK,eAAe,4DAA4D;WACtoB;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,CAAC;;WAED;WACA;WACA;WACA,CAAC;WACD;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM;WACN,KAAK,WAAW;WAChB,GAAG;WACH;WACA;;;;;WC1KA;;WAEA;WACA;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA,iCAAiC;;WAEjC;WACA;WACA;WACA,KAAK;WACL,eAAe;WACf;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM;WACN;WACA;WACA;;WAEA;;WAEA;;WAEA;;WAEA;;WAEA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM,qBAAqB;WAC3B;WACA;WACA;WACA;WACA;WACA;;WAEA;;WAEA;WACA;WACA;;;;;WCrFA;;;;;UEAA;UACA;UACA;UACA",
     "names": [],
     "sourceRoot": "",
     "sources": [
         "webpack://jupyterlab-celltagsclasses/webpack/container-entry",
         "webpack://jupyterlab-celltagsclasses/webpack/bootstrap",
         "webpack://jupyterlab-celltagsclasses/webpack/runtime/compat get default export",
@@ -25,22 +25,22 @@
     ],
     "sourcesContent": [
         "var moduleMap = {\n\t\"./index\": () => {\n\t\treturn __webpack_require__.e(\"lib_index_js\").then(() => (() => ((__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\")))));\n\t},\n\t\"./extension\": () => {\n\t\treturn __webpack_require__.e(\"lib_index_js\").then(() => (() => ((__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\")))));\n\t},\n\t\"./style\": () => {\n\t\treturn __webpack_require__.e(\"style_index_js\").then(() => (() => ((__webpack_require__(/*! ./style/index.js */ \"./style/index.js\")))));\n\t}\n};\nvar get = (module, getScope) => {\n\t__webpack_require__.R = getScope;\n\tgetScope = (\n\t\t__webpack_require__.o(moduleMap, module)\n\t\t\t? moduleMap[module]()\n\t\t\t: Promise.resolve().then(() => {\n\t\t\t\tthrow new Error('Module \"' + module + '\" does not exist in container.');\n\t\t\t})\n\t);\n\t__webpack_require__.R = undefined;\n\treturn getScope;\n};\nvar init = (shareScope, initScope) => {\n\tif (!__webpack_require__.S) return;\n\tvar name = \"default\"\n\tvar oldScope = __webpack_require__.S[name];\n\tif(oldScope && oldScope !== shareScope) throw new Error(\"Container initialization failed as it has already been initialized with a different share scope\");\n\t__webpack_require__.S[name] = shareScope;\n\treturn __webpack_require__.I(name, initScope);\n};\n\n// This exports getters to disallow modifications\n__webpack_require__.d(exports, {\n\tget: () => (get),\n\tinit: () => (init)\n});",
         "// The module cache\nvar __webpack_module_cache__ = {};\n\n// The require function\nfunction __webpack_require__(moduleId) {\n\t// Check if module is in cache\n\tvar cachedModule = __webpack_module_cache__[moduleId];\n\tif (cachedModule !== undefined) {\n\t\treturn cachedModule.exports;\n\t}\n\t// Create a new module (and put it into the cache)\n\tvar module = __webpack_module_cache__[moduleId] = {\n\t\tid: moduleId,\n\t\t// no module.loaded needed\n\t\texports: {}\n\t};\n\n\t// Execute the module function\n\t__webpack_modules__[moduleId](module, module.exports, __webpack_require__);\n\n\t// Return the exports of the module\n\treturn module.exports;\n}\n\n// expose the modules object (__webpack_modules__)\n__webpack_require__.m = __webpack_modules__;\n\n// expose the module cache\n__webpack_require__.c = __webpack_module_cache__;\n\n",
         "// getDefaultExport function for compatibility with non-harmony modules\n__webpack_require__.n = (module) => {\n\tvar getter = module && module.__esModule ?\n\t\t() => (module['default']) :\n\t\t() => (module);\n\t__webpack_require__.d(getter, { a: getter });\n\treturn getter;\n};",
         "// define getter functions for harmony exports\n__webpack_require__.d = (exports, definition) => {\n\tfor(var key in definition) {\n\t\tif(__webpack_require__.o(definition, key) && !__webpack_require__.o(exports, key)) {\n\t\t\tObject.defineProperty(exports, key, { enumerable: true, get: definition[key] });\n\t\t}\n\t}\n};",
         "__webpack_require__.f = {};\n// This file contains only the entry chunk.\n// The chunk loading function for additional chunks\n__webpack_require__.e = (chunkId) => {\n\treturn Promise.all(Object.keys(__webpack_require__.f).reduce((promises, key) => {\n\t\t__webpack_require__.f[key](chunkId, promises);\n\t\treturn promises;\n\t}, []));\n};",
-        "// This function allow to reference async chunks\n__webpack_require__.u = (chunkId) => {\n\t// return url for filenames based on template\n\treturn \"\" + chunkId + \".\" + {\"lib_index_js\":\"69027069f0720bba2d30\",\"style_index_js\":\"dcf32fced0a182594cc6\"}[chunkId] + \".js\";\n};",
+        "// This function allow to reference async chunks\n__webpack_require__.u = (chunkId) => {\n\t// return url for filenames based on template\n\treturn \"\" + chunkId + \".\" + {\"lib_index_js\":\"e0bf585461963e3d1e28\",\"style_index_js\":\"4784725fff15b54ffe3d\"}[chunkId] + \".js\";\n};",
         "__webpack_require__.g = (function() {\n\tif (typeof globalThis === 'object') return globalThis;\n\ttry {\n\t\treturn this || new Function('return this')();\n\t} catch (e) {\n\t\tif (typeof window === 'object') return window;\n\t}\n})();",
         "__webpack_require__.o = (obj, prop) => (Object.prototype.hasOwnProperty.call(obj, prop))",
         "var inProgress = {};\nvar dataWebpackPrefix = \"jupyterlab-celltagsclasses:\";\n// loadScript function to load a script via script tag\n__webpack_require__.l = (url, done, key, chunkId) => {\n\tif(inProgress[url]) { inProgress[url].push(done); return; }\n\tvar script, needAttach;\n\tif(key !== undefined) {\n\t\tvar scripts = document.getElementsByTagName(\"script\");\n\t\tfor(var i = 0; i < scripts.length; i++) {\n\t\t\tvar s = scripts[i];\n\t\t\tif(s.getAttribute(\"src\") == url || s.getAttribute(\"data-webpack\") == dataWebpackPrefix + key) { script = s; break; }\n\t\t}\n\t}\n\tif(!script) {\n\t\tneedAttach = true;\n\t\tscript = document.createElement('script');\n\n\t\tscript.charset = 'utf-8';\n\t\tscript.timeout = 120;\n\t\tif (__webpack_require__.nc) {\n\t\t\tscript.setAttribute(\"nonce\", __webpack_require__.nc);\n\t\t}\n\t\tscript.setAttribute(\"data-webpack\", dataWebpackPrefix + key);\n\t\tscript.src = url;\n\t}\n\tinProgress[url] = [done];\n\tvar onScriptComplete = (prev, event) => {\n\t\t// avoid mem leaks in IE.\n\t\tscript.onerror = script.onload = null;\n\t\tclearTimeout(timeout);\n\t\tvar doneFns = inProgress[url];\n\t\tdelete inProgress[url];\n\t\tscript.parentNode && script.parentNode.removeChild(script);\n\t\tdoneFns && doneFns.forEach((fn) => (fn(event)));\n\t\tif(prev) return prev(event);\n\t}\n\tvar timeout = setTimeout(onScriptComplete.bind(null, undefined, { type: 'timeout', target: script }), 120000);\n\tscript.onerror = onScriptComplete.bind(null, script.onerror);\n\tscript.onload = onScriptComplete.bind(null, script.onload);\n\tneedAttach && document.head.appendChild(script);\n};",
         "// define __esModule on exports\n__webpack_require__.r = (exports) => {\n\tif(typeof Symbol !== 'undefined' && Symbol.toStringTag) {\n\t\tObject.defineProperty(exports, Symbol.toStringTag, { value: 'Module' });\n\t}\n\tObject.defineProperty(exports, '__esModule', { value: true });\n};",
-        "__webpack_require__.S = {};\nvar initPromises = {};\nvar initTokens = {};\n__webpack_require__.I = (name, initScope) => {\n\tif(!initScope) initScope = [];\n\t// handling circular init calls\n\tvar initToken = initTokens[name];\n\tif(!initToken) initToken = initTokens[name] = {};\n\tif(initScope.indexOf(initToken) >= 0) return;\n\tinitScope.push(initToken);\n\t// only runs once\n\tif(initPromises[name]) return initPromises[name];\n\t// creates a new share scope if needed\n\tif(!__webpack_require__.o(__webpack_require__.S, name)) __webpack_require__.S[name] = {};\n\t// runs all init snippets from all modules reachable\n\tvar scope = __webpack_require__.S[name];\n\tvar warn = (msg) => {\n\t\tif (typeof console !== \"undefined\" && console.warn) console.warn(msg);\n\t};\n\tvar uniqueName = \"jupyterlab-celltagsclasses\";\n\tvar register = (name, version, factory, eager) => {\n\t\tvar versions = scope[name] = scope[name] || {};\n\t\tvar activeVersion = versions[version];\n\t\tif(!activeVersion || (!activeVersion.loaded && (!eager != !activeVersion.eager ? eager : uniqueName > activeVersion.from))) versions[version] = { get: factory, from: uniqueName, eager: !!eager };\n\t};\n\tvar initExternal = (id) => {\n\t\tvar handleError = (err) => (warn(\"Initialization of sharing external failed: \" + err));\n\t\ttry {\n\t\t\tvar module = __webpack_require__(id);\n\t\t\tif(!module) return;\n\t\t\tvar initFn = (module) => (module && module.init && module.init(__webpack_require__.S[name], initScope))\n\t\t\tif(module.then) return promises.push(module.then(initFn, handleError));\n\t\t\tvar initResult = initFn(module);\n\t\t\tif(initResult && initResult.then) return promises.push(initResult['catch'](handleError));\n\t\t} catch(err) { handleError(err); }\n\t}\n\tvar promises = [];\n\tswitch(name) {\n\t\tcase \"default\": {\n\t\t\tregister(\"jupyterlab-celltagsclasses\", \"0.1.0\", () => (__webpack_require__.e(\"lib_index_js\").then(() => (() => (__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\"))))));\n\t\t}\n\t\tbreak;\n\t}\n\tif(!promises.length) return initPromises[name] = 1;\n\treturn initPromises[name] = Promise.all(promises).then(() => (initPromises[name] = 1));\n};",
+        "__webpack_require__.S = {};\nvar initPromises = {};\nvar initTokens = {};\n__webpack_require__.I = (name, initScope) => {\n\tif(!initScope) initScope = [];\n\t// handling circular init calls\n\tvar initToken = initTokens[name];\n\tif(!initToken) initToken = initTokens[name] = {};\n\tif(initScope.indexOf(initToken) >= 0) return;\n\tinitScope.push(initToken);\n\t// only runs once\n\tif(initPromises[name]) return initPromises[name];\n\t// creates a new share scope if needed\n\tif(!__webpack_require__.o(__webpack_require__.S, name)) __webpack_require__.S[name] = {};\n\t// runs all init snippets from all modules reachable\n\tvar scope = __webpack_require__.S[name];\n\tvar warn = (msg) => {\n\t\tif (typeof console !== \"undefined\" && console.warn) console.warn(msg);\n\t};\n\tvar uniqueName = \"jupyterlab-celltagsclasses\";\n\tvar register = (name, version, factory, eager) => {\n\t\tvar versions = scope[name] = scope[name] || {};\n\t\tvar activeVersion = versions[version];\n\t\tif(!activeVersion || (!activeVersion.loaded && (!eager != !activeVersion.eager ? eager : uniqueName > activeVersion.from))) versions[version] = { get: factory, from: uniqueName, eager: !!eager };\n\t};\n\tvar initExternal = (id) => {\n\t\tvar handleError = (err) => (warn(\"Initialization of sharing external failed: \" + err));\n\t\ttry {\n\t\t\tvar module = __webpack_require__(id);\n\t\t\tif(!module) return;\n\t\t\tvar initFn = (module) => (module && module.init && module.init(__webpack_require__.S[name], initScope))\n\t\t\tif(module.then) return promises.push(module.then(initFn, handleError));\n\t\t\tvar initResult = initFn(module);\n\t\t\tif(initResult && initResult.then) return promises.push(initResult['catch'](handleError));\n\t\t} catch(err) { handleError(err); }\n\t}\n\tvar promises = [];\n\tswitch(name) {\n\t\tcase \"default\": {\n\t\t\tregister(\"jupyterlab-celltagsclasses\", \"0.2.0\", () => (__webpack_require__.e(\"lib_index_js\").then(() => (() => (__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\"))))));\n\t\t}\n\t\tbreak;\n\t}\n\tif(!promises.length) return initPromises[name] = 1;\n\treturn initPromises[name] = Promise.all(promises).then(() => (initPromises[name] = 1));\n};",
         "var scriptUrl;\nif (__webpack_require__.g.importScripts) scriptUrl = __webpack_require__.g.location + \"\";\nvar document = __webpack_require__.g.document;\nif (!scriptUrl && document) {\n\tif (document.currentScript)\n\t\tscriptUrl = document.currentScript.src;\n\tif (!scriptUrl) {\n\t\tvar scripts = document.getElementsByTagName(\"script\");\n\t\tif(scripts.length) {\n\t\t\tvar i = scripts.length - 1;\n\t\t\twhile (i > -1 && !scriptUrl) scriptUrl = scripts[i--].src;\n\t\t}\n\t}\n}\n// When supporting browsers where an automatic publicPath is not supported you must specify an output.publicPath manually via configuration\n// or pass an empty string (\"\") and set the __webpack_public_path__ variable from your code to use your own logic.\nif (!scriptUrl) throw new Error(\"Automatic publicPath is not supported in this browser\");\nscriptUrl = scriptUrl.replace(/#.*$/, \"\").replace(/\\?.*$/, \"\").replace(/\\/[^\\/]+$/, \"/\");\n__webpack_require__.p = scriptUrl;",
-        "var parseVersion = (str) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar p=p=>{return p.split(\".\").map((p=>{return+p==p?+p:p}))},n=/^([^-+]+)?(?:-([^+]+))?(?:\\+(.+))?$/.exec(str),r=n[1]?p(n[1]):[];return n[2]&&(r.length++,r.push.apply(r,p(n[2]))),n[3]&&(r.push([]),r.push.apply(r,p(n[3]))),r;\n}\nvar versionLt = (a, b) => {\n\t// see webpack/lib/util/semver.js for original code\n\ta=parseVersion(a),b=parseVersion(b);for(var r=0;;){if(r>=a.length)return r<b.length&&\"u\"!=(typeof b[r])[0];var e=a[r],n=(typeof e)[0];if(r>=b.length)return\"u\"==n;var t=b[r],f=(typeof t)[0];if(n!=f)return\"o\"==n&&\"n\"==f||(\"s\"==f||\"u\"==n);if(\"o\"!=n&&\"u\"!=n&&e!=t)return e<t;r++}\n}\nvar rangeToString = (range) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar r=range[0],n=\"\";if(1===range.length)return\"*\";if(r+.5){n+=0==r?\">=\":-1==r?\"<\":1==r?\"^\":2==r?\"~\":r>0?\"=\":\"!=\";for(var e=1,a=1;a<range.length;a++){e--,n+=\"u\"==(typeof(t=range[a]))[0]?\"-\":(e>0?\".\":\"\")+(e=2,t)}return n}var g=[];for(a=1;a<range.length;a++){var t=range[a];g.push(0===t?\"not(\"+o()+\")\":1===t?\"(\"+o()+\" || \"+o()+\")\":2===t?g.pop()+\" \"+g.pop():rangeToString(t))}return o();function o(){return g.pop().replace(/^\\((.+)\\)$/,\"$1\")}\n}\nvar satisfy = (range, version) => {\n\t// see webpack/lib/util/semver.js for original code\n\tif(0 in range){version=parseVersion(version);var e=range[0],r=e<0;r&&(e=-e-1);for(var n=0,i=1,a=!0;;i++,n++){var f,s,g=i<range.length?(typeof range[i])[0]:\"\";if(n>=version.length||\"o\"==(s=(typeof(f=version[n]))[0]))return!a||(\"u\"==g?i>e&&!r:\"\"==g!=r);if(\"u\"==s){if(!a||\"u\"!=g)return!1}else if(a)if(g==s)if(i<=e){if(f!=range[i])return!1}else{if(r?f>range[i]:f<range[i])return!1;f!=range[i]&&(a=!1)}else if(\"s\"!=g&&\"n\"!=g){if(r||i<=e)return!1;a=!1,i--}else{if(i<=e||s<g!=r)return!1;a=!1}else\"s\"!=g&&\"n\"!=g&&(a=!1,i--)}}var t=[],o=t.pop.bind(t);for(n=1;n<range.length;n++){var u=range[n];t.push(1==u?o()|o():2==u?o()&o():u?satisfy(u,version):!o())}return!!o();\n}\nvar ensureExistence = (scopeName, key) => {\n\tvar scope = __webpack_require__.S[scopeName];\n\tif(!scope || !__webpack_require__.o(scope, key)) throw new Error(\"Shared module \" + key + \" doesn't exist in shared scope \" + scopeName);\n\treturn scope;\n};\nvar findVersion = (scope, key) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar findSingletonVersionKey = (scope, key) => {\n\tvar versions = scope[key];\n\treturn Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || (!versions[a].loaded && versionLt(a, b)) ? b : a;\n\t}, 0);\n};\nvar getInvalidSingletonVersionMessage = (scope, key, version, requiredVersion) => {\n\treturn \"Unsatisfied version \" + version + \" from \" + (version && scope[key][version].from) + \" of shared singleton module \" + key + \" (required \" + rangeToString(requiredVersion) + \")\"\n};\nvar getSingleton = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\treturn get(scope[key][version]);\n};\nvar getSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) warn(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar getStrictSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) throw new Error(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar findValidVersion = (scope, key, requiredVersion) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\tif (!satisfy(requiredVersion, b)) return a;\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar getInvalidVersionMessage = (scope, scopeName, key, requiredVersion) => {\n\tvar versions = scope[key];\n\treturn \"No satisfying version (\" + rangeToString(requiredVersion) + \") of shared module \" + key + \" found in shared scope \" + scopeName + \".\\n\" +\n\t\t\"Available versions: \" + Object.keys(versions).map((key) => {\n\t\treturn key + \" from \" + versions[key].from;\n\t}).join(\", \");\n};\nvar getValidVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar entry = findValidVersion(scope, key, requiredVersion);\n\tif(entry) return get(entry);\n\tthrow new Error(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar warn = (msg) => {\n\tif (typeof console !== \"undefined\" && console.warn) console.warn(msg);\n};\nvar warnInvalidVersion = (scope, scopeName, key, requiredVersion) => {\n\twarn(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar get = (entry) => {\n\tentry.loaded = 1;\n\treturn entry.get()\n};\nvar init = (fn) => (function(scopeName, a, b, c) {\n\tvar promise = __webpack_require__.I(scopeName);\n\tif (promise && promise.then) return promise.then(fn.bind(fn, scopeName, __webpack_require__.S[scopeName], a, b, c));\n\treturn fn(scopeName, __webpack_require__.S[scopeName], a, b, c);\n});\n\nvar load = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn get(findVersion(scope, key));\n});\nvar loadFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\treturn scope && __webpack_require__.o(scope, key) ? get(findVersion(scope, key)) : fallback();\n});\nvar loadVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingleton = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getValidVersion(scope, scopeName, key, version);\n});\nvar loadStrictSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar loadVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingletonFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tvar entry = scope && __webpack_require__.o(scope, key) && findValidVersion(scope, key, version);\n\treturn entry ? get(entry) : fallback();\n});\nvar loadStrictSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar installedModules = {};\nvar moduleToHandlerMapping = {\n\t\"webpack/sharing/consume/default/@jupyterlab/notebook\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/notebook\", [1,4,0,0,,\"rc\",0]))\n};\n// no consumes in initial chunks\nvar chunkMapping = {\n\t\"lib_index_js\": [\n\t\t\"webpack/sharing/consume/default/@jupyterlab/notebook\"\n\t]\n};\n__webpack_require__.f.consumes = (chunkId, promises) => {\n\tif(__webpack_require__.o(chunkMapping, chunkId)) {\n\t\tchunkMapping[chunkId].forEach((id) => {\n\t\t\tif(__webpack_require__.o(installedModules, id)) return promises.push(installedModules[id]);\n\t\t\tvar onFactory = (factory) => {\n\t\t\t\tinstalledModules[id] = 0;\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tmodule.exports = factory();\n\t\t\t\t}\n\t\t\t};\n\t\t\tvar onError = (error) => {\n\t\t\t\tdelete installedModules[id];\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tthrow error;\n\t\t\t\t}\n\t\t\t};\n\t\t\ttry {\n\t\t\t\tvar promise = moduleToHandlerMapping[id]();\n\t\t\t\tif(promise.then) {\n\t\t\t\t\tpromises.push(installedModules[id] = promise.then(onFactory)['catch'](onError));\n\t\t\t\t} else onFactory(promise);\n\t\t\t} catch(e) { onError(e); }\n\t\t});\n\t}\n}",
+        "var parseVersion = (str) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar p=p=>{return p.split(\".\").map((p=>{return+p==p?+p:p}))},n=/^([^-+]+)?(?:-([^+]+))?(?:\\+(.+))?$/.exec(str),r=n[1]?p(n[1]):[];return n[2]&&(r.length++,r.push.apply(r,p(n[2]))),n[3]&&(r.push([]),r.push.apply(r,p(n[3]))),r;\n}\nvar versionLt = (a, b) => {\n\t// see webpack/lib/util/semver.js for original code\n\ta=parseVersion(a),b=parseVersion(b);for(var r=0;;){if(r>=a.length)return r<b.length&&\"u\"!=(typeof b[r])[0];var e=a[r],n=(typeof e)[0];if(r>=b.length)return\"u\"==n;var t=b[r],f=(typeof t)[0];if(n!=f)return\"o\"==n&&\"n\"==f||(\"s\"==f||\"u\"==n);if(\"o\"!=n&&\"u\"!=n&&e!=t)return e<t;r++}\n}\nvar rangeToString = (range) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar r=range[0],n=\"\";if(1===range.length)return\"*\";if(r+.5){n+=0==r?\">=\":-1==r?\"<\":1==r?\"^\":2==r?\"~\":r>0?\"=\":\"!=\";for(var e=1,a=1;a<range.length;a++){e--,n+=\"u\"==(typeof(t=range[a]))[0]?\"-\":(e>0?\".\":\"\")+(e=2,t)}return n}var g=[];for(a=1;a<range.length;a++){var t=range[a];g.push(0===t?\"not(\"+o()+\")\":1===t?\"(\"+o()+\" || \"+o()+\")\":2===t?g.pop()+\" \"+g.pop():rangeToString(t))}return o();function o(){return g.pop().replace(/^\\((.+)\\)$/,\"$1\")}\n}\nvar satisfy = (range, version) => {\n\t// see webpack/lib/util/semver.js for original code\n\tif(0 in range){version=parseVersion(version);var e=range[0],r=e<0;r&&(e=-e-1);for(var n=0,i=1,a=!0;;i++,n++){var f,s,g=i<range.length?(typeof range[i])[0]:\"\";if(n>=version.length||\"o\"==(s=(typeof(f=version[n]))[0]))return!a||(\"u\"==g?i>e&&!r:\"\"==g!=r);if(\"u\"==s){if(!a||\"u\"!=g)return!1}else if(a)if(g==s)if(i<=e){if(f!=range[i])return!1}else{if(r?f>range[i]:f<range[i])return!1;f!=range[i]&&(a=!1)}else if(\"s\"!=g&&\"n\"!=g){if(r||i<=e)return!1;a=!1,i--}else{if(i<=e||s<g!=r)return!1;a=!1}else\"s\"!=g&&\"n\"!=g&&(a=!1,i--)}}var t=[],o=t.pop.bind(t);for(n=1;n<range.length;n++){var u=range[n];t.push(1==u?o()|o():2==u?o()&o():u?satisfy(u,version):!o())}return!!o();\n}\nvar ensureExistence = (scopeName, key) => {\n\tvar scope = __webpack_require__.S[scopeName];\n\tif(!scope || !__webpack_require__.o(scope, key)) throw new Error(\"Shared module \" + key + \" doesn't exist in shared scope \" + scopeName);\n\treturn scope;\n};\nvar findVersion = (scope, key) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar findSingletonVersionKey = (scope, key) => {\n\tvar versions = scope[key];\n\treturn Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || (!versions[a].loaded && versionLt(a, b)) ? b : a;\n\t}, 0);\n};\nvar getInvalidSingletonVersionMessage = (scope, key, version, requiredVersion) => {\n\treturn \"Unsatisfied version \" + version + \" from \" + (version && scope[key][version].from) + \" of shared singleton module \" + key + \" (required \" + rangeToString(requiredVersion) + \")\"\n};\nvar getSingleton = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\treturn get(scope[key][version]);\n};\nvar getSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) warn(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar getStrictSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) throw new Error(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar findValidVersion = (scope, key, requiredVersion) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\tif (!satisfy(requiredVersion, b)) return a;\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar getInvalidVersionMessage = (scope, scopeName, key, requiredVersion) => {\n\tvar versions = scope[key];\n\treturn \"No satisfying version (\" + rangeToString(requiredVersion) + \") of shared module \" + key + \" found in shared scope \" + scopeName + \".\\n\" +\n\t\t\"Available versions: \" + Object.keys(versions).map((key) => {\n\t\treturn key + \" from \" + versions[key].from;\n\t}).join(\", \");\n};\nvar getValidVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar entry = findValidVersion(scope, key, requiredVersion);\n\tif(entry) return get(entry);\n\tthrow new Error(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar warn = (msg) => {\n\tif (typeof console !== \"undefined\" && console.warn) console.warn(msg);\n};\nvar warnInvalidVersion = (scope, scopeName, key, requiredVersion) => {\n\twarn(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar get = (entry) => {\n\tentry.loaded = 1;\n\treturn entry.get()\n};\nvar init = (fn) => (function(scopeName, a, b, c) {\n\tvar promise = __webpack_require__.I(scopeName);\n\tif (promise && promise.then) return promise.then(fn.bind(fn, scopeName, __webpack_require__.S[scopeName], a, b, c));\n\treturn fn(scopeName, __webpack_require__.S[scopeName], a, b, c);\n});\n\nvar load = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn get(findVersion(scope, key));\n});\nvar loadFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\treturn scope && __webpack_require__.o(scope, key) ? get(findVersion(scope, key)) : fallback();\n});\nvar loadVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingleton = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getValidVersion(scope, scopeName, key, version);\n});\nvar loadStrictSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar loadVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingletonFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tvar entry = scope && __webpack_require__.o(scope, key) && findValidVersion(scope, key, version);\n\treturn entry ? get(entry) : fallback();\n});\nvar loadStrictSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar installedModules = {};\nvar moduleToHandlerMapping = {\n\t\"webpack/sharing/consume/default/@jupyterlab/notebook\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/notebook\", [1,4,0,0,,\"beta\",2]))\n};\n// no consumes in initial chunks\nvar chunkMapping = {\n\t\"lib_index_js\": [\n\t\t\"webpack/sharing/consume/default/@jupyterlab/notebook\"\n\t]\n};\n__webpack_require__.f.consumes = (chunkId, promises) => {\n\tif(__webpack_require__.o(chunkMapping, chunkId)) {\n\t\tchunkMapping[chunkId].forEach((id) => {\n\t\t\tif(__webpack_require__.o(installedModules, id)) return promises.push(installedModules[id]);\n\t\t\tvar onFactory = (factory) => {\n\t\t\t\tinstalledModules[id] = 0;\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tmodule.exports = factory();\n\t\t\t\t}\n\t\t\t};\n\t\t\tvar onError = (error) => {\n\t\t\t\tdelete installedModules[id];\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tthrow error;\n\t\t\t\t}\n\t\t\t};\n\t\t\ttry {\n\t\t\t\tvar promise = moduleToHandlerMapping[id]();\n\t\t\t\tif(promise.then) {\n\t\t\t\t\tpromises.push(installedModules[id] = promise.then(onFactory)['catch'](onError));\n\t\t\t\t} else onFactory(promise);\n\t\t\t} catch(e) { onError(e); }\n\t\t});\n\t}\n}",
         "// no baseURI\n\n// object to store loaded and loading chunks\n// undefined = chunk not loaded, null = chunk preloaded/prefetched\n// [resolve, reject, Promise] = chunk loading, 0 = chunk loaded\nvar installedChunks = {\n\t\"jupyterlab-celltagsclasses\": 0\n};\n\n__webpack_require__.f.j = (chunkId, promises) => {\n\t\t// JSONP chunk loading for javascript\n\t\tvar installedChunkData = __webpack_require__.o(installedChunks, chunkId) ? installedChunks[chunkId] : undefined;\n\t\tif(installedChunkData !== 0) { // 0 means \"already installed\".\n\n\t\t\t// a Promise means \"currently loading\".\n\t\t\tif(installedChunkData) {\n\t\t\t\tpromises.push(installedChunkData[2]);\n\t\t\t} else {\n\t\t\t\tif(true) { // all chunks have JS\n\t\t\t\t\t// setup Promise in chunk cache\n\t\t\t\t\tvar promise = new Promise((resolve, reject) => (installedChunkData = installedChunks[chunkId] = [resolve, reject]));\n\t\t\t\t\tpromises.push(installedChunkData[2] = promise);\n\n\t\t\t\t\t// start chunk loading\n\t\t\t\t\tvar url = __webpack_require__.p + __webpack_require__.u(chunkId);\n\t\t\t\t\t// create error before stack unwound to get useful stacktrace later\n\t\t\t\t\tvar error = new Error();\n\t\t\t\t\tvar loadingEnded = (event) => {\n\t\t\t\t\t\tif(__webpack_require__.o(installedChunks, chunkId)) {\n\t\t\t\t\t\t\tinstalledChunkData = installedChunks[chunkId];\n\t\t\t\t\t\t\tif(installedChunkData !== 0) installedChunks[chunkId] = undefined;\n\t\t\t\t\t\t\tif(installedChunkData) {\n\t\t\t\t\t\t\t\tvar errorType = event && (event.type === 'load' ? 'missing' : event.type);\n\t\t\t\t\t\t\t\tvar realSrc = event && event.target && event.target.src;\n\t\t\t\t\t\t\t\terror.message = 'Loading chunk ' + chunkId + ' failed.\\n(' + errorType + ': ' + realSrc + ')';\n\t\t\t\t\t\t\t\terror.name = 'ChunkLoadError';\n\t\t\t\t\t\t\t\terror.type = errorType;\n\t\t\t\t\t\t\t\terror.request = realSrc;\n\t\t\t\t\t\t\t\tinstalledChunkData[1](error);\n\t\t\t\t\t\t\t}\n\t\t\t\t\t\t}\n\t\t\t\t\t};\n\t\t\t\t\t__webpack_require__.l(url, loadingEnded, \"chunk-\" + chunkId, chunkId);\n\t\t\t\t} else installedChunks[chunkId] = 0;\n\t\t\t}\n\t\t}\n};\n\n// no prefetching\n\n// no preloaded\n\n// no HMR\n\n// no HMR manifest\n\n// no on chunks loaded\n\n// install a JSONP callback for chunk loading\nvar webpackJsonpCallback = (parentChunkLoadingFunction, data) => {\n\tvar [chunkIds, moreModules, runtime] = data;\n\t// add \"moreModules\" to the modules object,\n\t// then flag all \"chunkIds\" as loaded and fire callback\n\tvar moduleId, chunkId, i = 0;\n\tif(chunkIds.some((id) => (installedChunks[id] !== 0))) {\n\t\tfor(moduleId in moreModules) {\n\t\t\tif(__webpack_require__.o(moreModules, moduleId)) {\n\t\t\t\t__webpack_require__.m[moduleId] = moreModules[moduleId];\n\t\t\t}\n\t\t}\n\t\tif(runtime) var result = runtime(__webpack_require__);\n\t}\n\tif(parentChunkLoadingFunction) parentChunkLoadingFunction(data);\n\tfor(;i < chunkIds.length; i++) {\n\t\tchunkId = chunkIds[i];\n\t\tif(__webpack_require__.o(installedChunks, chunkId) && installedChunks[chunkId]) {\n\t\t\tinstalledChunks[chunkId][0]();\n\t\t}\n\t\tinstalledChunks[chunkId] = 0;\n\t}\n\n}\n\nvar chunkLoadingGlobal = self[\"webpackChunkjupyterlab_celltagsclasses\"] = self[\"webpackChunkjupyterlab_celltagsclasses\"] || [];\nchunkLoadingGlobal.forEach(webpackJsonpCallback.bind(null, 0));\nchunkLoadingGlobal.push = webpackJsonpCallback.bind(null, chunkLoadingGlobal.push.bind(chunkLoadingGlobal));",
         "__webpack_require__.nc = undefined;",
         "",
         "// module cache are used so entry inlining is disabled\n// startup\n// Load entry module and return exports\nvar __webpack_exports__ = __webpack_require__(\"webpack/container/entry/jupyterlab-celltagsclasses\");\n",
         ""
     ],
     "version": 3
```

### Comparing `jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/remoteEntry.0a4c39b501971c60ffd2.js.map` & `jupyterlab_celltagsclasses-0.2.0/jupyterlab_celltagsclasses/labextension/static/remoteEntry.e8bcb578ed91b775bd99.js.map`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8367346938775511%*

 * *Differences: {"'file'": "'remoteEntry.e8bcb578ed91b775bd99.js'",*

 * * "'mappings'": "';;;;;;;;;;;AAAA;AACA;AACA;AACA,EAAE;AACF;AACA;AACA,EAAE;AACF;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,IAAI;AACJ;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;AAEA;AACA;AACA;AACA;AACA,CAAC;;;;;;UCpCD;UACA;;UAEA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;;;;;WC5BA;WACA;WACA;WACA;WACA;WACA,iCAAiC,WAAW;WAC5C;WACA;;;;;WCPA;WACA;WACA;WACA;WACA,yCAAyC,wCAAwC […]*

```diff
@@ -1,10 +1,10 @@
 {
-    "file": "remoteEntry.0a4c39b501971c60ffd2.js",
-    "mappings": ";;;;;;;;;;;AAAA;AACA;AACA;AACA,EAAE;AACF;AACA;AACA,EAAE;AACF;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,IAAI;AACJ;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;AAEA;AACA;AACA;AACA;AACA,CAAC;;;;;;UCpCD;UACA;;UAEA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;;;;;WC5BA;WACA;WACA;WACA;WACA;WACA,iCAAiC,WAAW;WAC5C;WACA;;;;;WCPA;WACA;WACA;WACA;WACA,yCAAyC,wCAAwC;WACjF;WACA;WACA;;;;;WCPA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;;;;;WCRA;WACA;WACA;WACA,8BAA8B,8EAA8E;WAC5G;;;;;WCJA;WACA;WACA;WACA;WACA,GAAG;WACH;WACA;WACA,CAAC;;;;;WCPD;;;;;WCAA;WACA;WACA;WACA;WACA,uBAAuB,4BAA4B;WACnD;WACA;WACA;WACA,iBAAiB,oBAAoB;WACrC;WACA,mGAAmG,YAAY;WAC/G;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,mEAAmE,iCAAiC;WACpG;WACA;WACA;WACA;;;;;WCxCA;WACA;WACA;WACA,uDAAuD,iBAAiB;WACxE;WACA,gDAAgD,aAAa;WAC7D;;;;;WCNA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,oJAAoJ;WACpJ;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,IAAI,aAAa;WACjB;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;;;;WC7CA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;;;;WClBA;WACA;WACA,WAAW,6BAA6B,iBAAiB,GAAG,qEAAqE;WACjI;WACA;WACA;WACA,qCAAqC,aAAa,EAAE,wDAAwD,2BAA2B,4BAA4B,2BAA2B,+CAA+C,mCAAmC;WAChR;WACA;WACA;WACA,qBAAqB,8BAA8B,SAAS,sDAAsD,gBAAgB,eAAe,KAAK,6DAA6D,SAAS,SAAS,QAAQ,eAAe,KAAK,eAAe,qGAAqG,WAAW,aAAa;WAC7Y;WACA;WACA;WACA,gBAAgB,8BAA8B,qBAAqB,YAAY,sBAAsB,SAAS,iDAAiD,6FAA6F,WAAW,uBAAuB,2BAA2B,wBAAwB,KAAK,oCAAoC,oBAAoB,wBAAwB,oBAAoB,SAAS,KAAK,yBAAyB,KAAK,gCAAgC,yBAAyB,QAAQ,eAAe,KAAK,eAAe,4DAA4D;WACtoB;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,CAAC;;WAED;WACA;WACA;WACA,CAAC;WACD;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM;WACN,KAAK,WAAW;WAChB,GAAG;WACH;WACA;;;;;WC1KA;;WAEA;WACA;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA,iCAAiC;;WAEjC;WACA;WACA;WACA,KAAK;WACL,eAAe;WACf;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM;WACN;WACA;WACA;;WAEA;;WAEA;;WAEA;;WAEA;;WAEA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM,qBAAqB;WAC3B;WACA;WACA;WACA;WACA;WACA;;WAEA;;WAEA;WACA;WACA;;;;;WCrFA;;;;;UEAA;UACA;UACA;UACA",
+    "file": "remoteEntry.e8bcb578ed91b775bd99.js",
+    "mappings": ";;;;;;;;;;;AAAA;AACA;AACA;AACA,EAAE;AACF;AACA;AACA,EAAE;AACF;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,IAAI;AACJ;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;AAEA;AACA;AACA;AACA;AACA,CAAC;;;;;;UCpCD;UACA;;UAEA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;;;;;WC5BA;WACA;WACA;WACA;WACA;WACA,iCAAiC,WAAW;WAC5C;WACA;;;;;WCPA;WACA;WACA;WACA;WACA,yCAAyC,wCAAwC;WACjF;WACA;WACA;;;;;WCPA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;;;;;WCRA;WACA;WACA;WACA,8BAA8B,8EAA8E;WAC5G;;;;;WCJA;WACA;WACA;WACA;WACA,GAAG;WACH;WACA;WACA,CAAC;;;;;WCPD;;;;;WCAA;WACA;WACA;WACA;WACA,uBAAuB,4BAA4B;WACnD;WACA;WACA;WACA,iBAAiB,oBAAoB;WACrC;WACA,mGAAmG,YAAY;WAC/G;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,mEAAmE,iCAAiC;WACpG;WACA;WACA;WACA;;;;;WCxCA;WACA;WACA;WACA,uDAAuD,iBAAiB;WACxE;WACA,gDAAgD,aAAa;WAC7D;;;;;WCNA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,oJAAoJ;WACpJ;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,IAAI,aAAa;WACjB;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;;;;WC7CA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;;;;WClBA;WACA;WACA,WAAW,6BAA6B,iBAAiB,GAAG,qEAAqE;WACjI;WACA;WACA;WACA,qCAAqC,aAAa,EAAE,wDAAwD,2BAA2B,4BAA4B,2BAA2B,+CAA+C,mCAAmC;WAChR;WACA;WACA;WACA,qBAAqB,8BAA8B,SAAS,sDAAsD,gBAAgB,eAAe,KAAK,6DAA6D,SAAS,SAAS,QAAQ,eAAe,KAAK,eAAe,qGAAqG,WAAW,aAAa;WAC7Y;WACA;WACA;WACA,gBAAgB,8BAA8B,qBAAqB,YAAY,sBAAsB,SAAS,iDAAiD,6FAA6F,WAAW,uBAAuB,2BAA2B,wBAAwB,KAAK,oCAAoC,oBAAoB,wBAAwB,oBAAoB,SAAS,KAAK,yBAAyB,KAAK,gCAAgC,yBAAyB,QAAQ,eAAe,KAAK,eAAe,4DAA4D;WACtoB;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,CAAC;;WAED;WACA;WACA;WACA,CAAC;WACD;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM;WACN,KAAK,WAAW;WAChB,GAAG;WACH;WACA;;;;;WC5KA;;WAEA;WACA;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA,iCAAiC;;WAEjC;WACA;WACA;WACA,KAAK;WACL,eAAe;WACf;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM;WACN;WACA;WACA;;WAEA;;WAEA;;WAEA;;WAEA;;WAEA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM,qBAAqB;WAC3B;WACA;WACA;WACA;WACA;WACA;;WAEA;;WAEA;WACA;WACA;;;;;WCrFA;;;;;UEAA;UACA;UACA;UACA",
     "names": [],
     "sourceRoot": "",
     "sources": [
         "webpack://jupyterlab-celltagsclasses/webpack/container-entry",
         "webpack://jupyterlab-celltagsclasses/webpack/bootstrap",
         "webpack://jupyterlab-celltagsclasses/webpack/runtime/compat get default export",
         "webpack://jupyterlab-celltagsclasses/webpack/runtime/define property getters",
@@ -25,22 +25,22 @@
     ],
     "sourcesContent": [
         "var moduleMap = {\n\t\"./index\": () => {\n\t\treturn __webpack_require__.e(\"lib_index_js\").then(() => (() => ((__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\")))));\n\t},\n\t\"./extension\": () => {\n\t\treturn __webpack_require__.e(\"lib_index_js\").then(() => (() => ((__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\")))));\n\t},\n\t\"./style\": () => {\n\t\treturn __webpack_require__.e(\"style_index_js\").then(() => (() => ((__webpack_require__(/*! ./style/index.js */ \"./style/index.js\")))));\n\t}\n};\nvar get = (module, getScope) => {\n\t__webpack_require__.R = getScope;\n\tgetScope = (\n\t\t__webpack_require__.o(moduleMap, module)\n\t\t\t? moduleMap[module]()\n\t\t\t: Promise.resolve().then(() => {\n\t\t\t\tthrow new Error('Module \"' + module + '\" does not exist in container.');\n\t\t\t})\n\t);\n\t__webpack_require__.R = undefined;\n\treturn getScope;\n};\nvar init = (shareScope, initScope) => {\n\tif (!__webpack_require__.S) return;\n\tvar name = \"default\"\n\tvar oldScope = __webpack_require__.S[name];\n\tif(oldScope && oldScope !== shareScope) throw new Error(\"Container initialization failed as it has already been initialized with a different share scope\");\n\t__webpack_require__.S[name] = shareScope;\n\treturn __webpack_require__.I(name, initScope);\n};\n\n// This exports getters to disallow modifications\n__webpack_require__.d(exports, {\n\tget: () => (get),\n\tinit: () => (init)\n});",
         "// The module cache\nvar __webpack_module_cache__ = {};\n\n// The require function\nfunction __webpack_require__(moduleId) {\n\t// Check if module is in cache\n\tvar cachedModule = __webpack_module_cache__[moduleId];\n\tif (cachedModule !== undefined) {\n\t\treturn cachedModule.exports;\n\t}\n\t// Create a new module (and put it into the cache)\n\tvar module = __webpack_module_cache__[moduleId] = {\n\t\tid: moduleId,\n\t\t// no module.loaded needed\n\t\texports: {}\n\t};\n\n\t// Execute the module function\n\t__webpack_modules__[moduleId](module, module.exports, __webpack_require__);\n\n\t// Return the exports of the module\n\treturn module.exports;\n}\n\n// expose the modules object (__webpack_modules__)\n__webpack_require__.m = __webpack_modules__;\n\n// expose the module cache\n__webpack_require__.c = __webpack_module_cache__;\n\n",
         "// getDefaultExport function for compatibility with non-harmony modules\n__webpack_require__.n = (module) => {\n\tvar getter = module && module.__esModule ?\n\t\t() => (module['default']) :\n\t\t() => (module);\n\t__webpack_require__.d(getter, { a: getter });\n\treturn getter;\n};",
         "// define getter functions for harmony exports\n__webpack_require__.d = (exports, definition) => {\n\tfor(var key in definition) {\n\t\tif(__webpack_require__.o(definition, key) && !__webpack_require__.o(exports, key)) {\n\t\t\tObject.defineProperty(exports, key, { enumerable: true, get: definition[key] });\n\t\t}\n\t}\n};",
         "__webpack_require__.f = {};\n// This file contains only the entry chunk.\n// The chunk loading function for additional chunks\n__webpack_require__.e = (chunkId) => {\n\treturn Promise.all(Object.keys(__webpack_require__.f).reduce((promises, key) => {\n\t\t__webpack_require__.f[key](chunkId, promises);\n\t\treturn promises;\n\t}, []));\n};",
-        "// This function allow to reference async chunks\n__webpack_require__.u = (chunkId) => {\n\t// return url for filenames based on template\n\treturn \"\" + chunkId + \".\" + {\"lib_index_js\":\"e0bf585461963e3d1e28\",\"style_index_js\":\"df6561a0531b63f9a29b\"}[chunkId] + \".js\";\n};",
+        "// This function allow to reference async chunks\n__webpack_require__.u = (chunkId) => {\n\t// return url for filenames based on template\n\treturn \"\" + chunkId + \".\" + {\"lib_index_js\":\"cddacca2ba0e6c761c6d\",\"style_index_js\":\"4784725fff15b54ffe3d\"}[chunkId] + \".js\";\n};",
         "__webpack_require__.g = (function() {\n\tif (typeof globalThis === 'object') return globalThis;\n\ttry {\n\t\treturn this || new Function('return this')();\n\t} catch (e) {\n\t\tif (typeof window === 'object') return window;\n\t}\n})();",
         "__webpack_require__.o = (obj, prop) => (Object.prototype.hasOwnProperty.call(obj, prop))",
         "var inProgress = {};\nvar dataWebpackPrefix = \"jupyterlab-celltagsclasses:\";\n// loadScript function to load a script via script tag\n__webpack_require__.l = (url, done, key, chunkId) => {\n\tif(inProgress[url]) { inProgress[url].push(done); return; }\n\tvar script, needAttach;\n\tif(key !== undefined) {\n\t\tvar scripts = document.getElementsByTagName(\"script\");\n\t\tfor(var i = 0; i < scripts.length; i++) {\n\t\t\tvar s = scripts[i];\n\t\t\tif(s.getAttribute(\"src\") == url || s.getAttribute(\"data-webpack\") == dataWebpackPrefix + key) { script = s; break; }\n\t\t}\n\t}\n\tif(!script) {\n\t\tneedAttach = true;\n\t\tscript = document.createElement('script');\n\n\t\tscript.charset = 'utf-8';\n\t\tscript.timeout = 120;\n\t\tif (__webpack_require__.nc) {\n\t\t\tscript.setAttribute(\"nonce\", __webpack_require__.nc);\n\t\t}\n\t\tscript.setAttribute(\"data-webpack\", dataWebpackPrefix + key);\n\t\tscript.src = url;\n\t}\n\tinProgress[url] = [done];\n\tvar onScriptComplete = (prev, event) => {\n\t\t// avoid mem leaks in IE.\n\t\tscript.onerror = script.onload = null;\n\t\tclearTimeout(timeout);\n\t\tvar doneFns = inProgress[url];\n\t\tdelete inProgress[url];\n\t\tscript.parentNode && script.parentNode.removeChild(script);\n\t\tdoneFns && doneFns.forEach((fn) => (fn(event)));\n\t\tif(prev) return prev(event);\n\t}\n\tvar timeout = setTimeout(onScriptComplete.bind(null, undefined, { type: 'timeout', target: script }), 120000);\n\tscript.onerror = onScriptComplete.bind(null, script.onerror);\n\tscript.onload = onScriptComplete.bind(null, script.onload);\n\tneedAttach && document.head.appendChild(script);\n};",
         "// define __esModule on exports\n__webpack_require__.r = (exports) => {\n\tif(typeof Symbol !== 'undefined' && Symbol.toStringTag) {\n\t\tObject.defineProperty(exports, Symbol.toStringTag, { value: 'Module' });\n\t}\n\tObject.defineProperty(exports, '__esModule', { value: true });\n};",
-        "__webpack_require__.S = {};\nvar initPromises = {};\nvar initTokens = {};\n__webpack_require__.I = (name, initScope) => {\n\tif(!initScope) initScope = [];\n\t// handling circular init calls\n\tvar initToken = initTokens[name];\n\tif(!initToken) initToken = initTokens[name] = {};\n\tif(initScope.indexOf(initToken) >= 0) return;\n\tinitScope.push(initToken);\n\t// only runs once\n\tif(initPromises[name]) return initPromises[name];\n\t// creates a new share scope if needed\n\tif(!__webpack_require__.o(__webpack_require__.S, name)) __webpack_require__.S[name] = {};\n\t// runs all init snippets from all modules reachable\n\tvar scope = __webpack_require__.S[name];\n\tvar warn = (msg) => {\n\t\tif (typeof console !== \"undefined\" && console.warn) console.warn(msg);\n\t};\n\tvar uniqueName = \"jupyterlab-celltagsclasses\";\n\tvar register = (name, version, factory, eager) => {\n\t\tvar versions = scope[name] = scope[name] || {};\n\t\tvar activeVersion = versions[version];\n\t\tif(!activeVersion || (!activeVersion.loaded && (!eager != !activeVersion.eager ? eager : uniqueName > activeVersion.from))) versions[version] = { get: factory, from: uniqueName, eager: !!eager };\n\t};\n\tvar initExternal = (id) => {\n\t\tvar handleError = (err) => (warn(\"Initialization of sharing external failed: \" + err));\n\t\ttry {\n\t\t\tvar module = __webpack_require__(id);\n\t\t\tif(!module) return;\n\t\t\tvar initFn = (module) => (module && module.init && module.init(__webpack_require__.S[name], initScope))\n\t\t\tif(module.then) return promises.push(module.then(initFn, handleError));\n\t\t\tvar initResult = initFn(module);\n\t\t\tif(initResult && initResult.then) return promises.push(initResult['catch'](handleError));\n\t\t} catch(err) { handleError(err); }\n\t}\n\tvar promises = [];\n\tswitch(name) {\n\t\tcase \"default\": {\n\t\t\tregister(\"jupyterlab-celltagsclasses\", \"0.1.0\", () => (__webpack_require__.e(\"lib_index_js\").then(() => (() => (__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\"))))));\n\t\t}\n\t\tbreak;\n\t}\n\tif(!promises.length) return initPromises[name] = 1;\n\treturn initPromises[name] = Promise.all(promises).then(() => (initPromises[name] = 1));\n};",
+        "__webpack_require__.S = {};\nvar initPromises = {};\nvar initTokens = {};\n__webpack_require__.I = (name, initScope) => {\n\tif(!initScope) initScope = [];\n\t// handling circular init calls\n\tvar initToken = initTokens[name];\n\tif(!initToken) initToken = initTokens[name] = {};\n\tif(initScope.indexOf(initToken) >= 0) return;\n\tinitScope.push(initToken);\n\t// only runs once\n\tif(initPromises[name]) return initPromises[name];\n\t// creates a new share scope if needed\n\tif(!__webpack_require__.o(__webpack_require__.S, name)) __webpack_require__.S[name] = {};\n\t// runs all init snippets from all modules reachable\n\tvar scope = __webpack_require__.S[name];\n\tvar warn = (msg) => {\n\t\tif (typeof console !== \"undefined\" && console.warn) console.warn(msg);\n\t};\n\tvar uniqueName = \"jupyterlab-celltagsclasses\";\n\tvar register = (name, version, factory, eager) => {\n\t\tvar versions = scope[name] = scope[name] || {};\n\t\tvar activeVersion = versions[version];\n\t\tif(!activeVersion || (!activeVersion.loaded && (!eager != !activeVersion.eager ? eager : uniqueName > activeVersion.from))) versions[version] = { get: factory, from: uniqueName, eager: !!eager };\n\t};\n\tvar initExternal = (id) => {\n\t\tvar handleError = (err) => (warn(\"Initialization of sharing external failed: \" + err));\n\t\ttry {\n\t\t\tvar module = __webpack_require__(id);\n\t\t\tif(!module) return;\n\t\t\tvar initFn = (module) => (module && module.init && module.init(__webpack_require__.S[name], initScope))\n\t\t\tif(module.then) return promises.push(module.then(initFn, handleError));\n\t\t\tvar initResult = initFn(module);\n\t\t\tif(initResult && initResult.then) return promises.push(initResult['catch'](handleError));\n\t\t} catch(err) { handleError(err); }\n\t}\n\tvar promises = [];\n\tswitch(name) {\n\t\tcase \"default\": {\n\t\t\tregister(\"jupyterlab-celltagsclasses\", \"0.2.0\", () => (__webpack_require__.e(\"lib_index_js\").then(() => (() => (__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\"))))));\n\t\t}\n\t\tbreak;\n\t}\n\tif(!promises.length) return initPromises[name] = 1;\n\treturn initPromises[name] = Promise.all(promises).then(() => (initPromises[name] = 1));\n};",
         "var scriptUrl;\nif (__webpack_require__.g.importScripts) scriptUrl = __webpack_require__.g.location + \"\";\nvar document = __webpack_require__.g.document;\nif (!scriptUrl && document) {\n\tif (document.currentScript)\n\t\tscriptUrl = document.currentScript.src;\n\tif (!scriptUrl) {\n\t\tvar scripts = document.getElementsByTagName(\"script\");\n\t\tif(scripts.length) {\n\t\t\tvar i = scripts.length - 1;\n\t\t\twhile (i > -1 && !scriptUrl) scriptUrl = scripts[i--].src;\n\t\t}\n\t}\n}\n// When supporting browsers where an automatic publicPath is not supported you must specify an output.publicPath manually via configuration\n// or pass an empty string (\"\") and set the __webpack_public_path__ variable from your code to use your own logic.\nif (!scriptUrl) throw new Error(\"Automatic publicPath is not supported in this browser\");\nscriptUrl = scriptUrl.replace(/#.*$/, \"\").replace(/\\?.*$/, \"\").replace(/\\/[^\\/]+$/, \"/\");\n__webpack_require__.p = scriptUrl;",
-        "var parseVersion = (str) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar p=p=>{return p.split(\".\").map((p=>{return+p==p?+p:p}))},n=/^([^-+]+)?(?:-([^+]+))?(?:\\+(.+))?$/.exec(str),r=n[1]?p(n[1]):[];return n[2]&&(r.length++,r.push.apply(r,p(n[2]))),n[3]&&(r.push([]),r.push.apply(r,p(n[3]))),r;\n}\nvar versionLt = (a, b) => {\n\t// see webpack/lib/util/semver.js for original code\n\ta=parseVersion(a),b=parseVersion(b);for(var r=0;;){if(r>=a.length)return r<b.length&&\"u\"!=(typeof b[r])[0];var e=a[r],n=(typeof e)[0];if(r>=b.length)return\"u\"==n;var t=b[r],f=(typeof t)[0];if(n!=f)return\"o\"==n&&\"n\"==f||(\"s\"==f||\"u\"==n);if(\"o\"!=n&&\"u\"!=n&&e!=t)return e<t;r++}\n}\nvar rangeToString = (range) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar r=range[0],n=\"\";if(1===range.length)return\"*\";if(r+.5){n+=0==r?\">=\":-1==r?\"<\":1==r?\"^\":2==r?\"~\":r>0?\"=\":\"!=\";for(var e=1,a=1;a<range.length;a++){e--,n+=\"u\"==(typeof(t=range[a]))[0]?\"-\":(e>0?\".\":\"\")+(e=2,t)}return n}var g=[];for(a=1;a<range.length;a++){var t=range[a];g.push(0===t?\"not(\"+o()+\")\":1===t?\"(\"+o()+\" || \"+o()+\")\":2===t?g.pop()+\" \"+g.pop():rangeToString(t))}return o();function o(){return g.pop().replace(/^\\((.+)\\)$/,\"$1\")}\n}\nvar satisfy = (range, version) => {\n\t// see webpack/lib/util/semver.js for original code\n\tif(0 in range){version=parseVersion(version);var e=range[0],r=e<0;r&&(e=-e-1);for(var n=0,i=1,a=!0;;i++,n++){var f,s,g=i<range.length?(typeof range[i])[0]:\"\";if(n>=version.length||\"o\"==(s=(typeof(f=version[n]))[0]))return!a||(\"u\"==g?i>e&&!r:\"\"==g!=r);if(\"u\"==s){if(!a||\"u\"!=g)return!1}else if(a)if(g==s)if(i<=e){if(f!=range[i])return!1}else{if(r?f>range[i]:f<range[i])return!1;f!=range[i]&&(a=!1)}else if(\"s\"!=g&&\"n\"!=g){if(r||i<=e)return!1;a=!1,i--}else{if(i<=e||s<g!=r)return!1;a=!1}else\"s\"!=g&&\"n\"!=g&&(a=!1,i--)}}var t=[],o=t.pop.bind(t);for(n=1;n<range.length;n++){var u=range[n];t.push(1==u?o()|o():2==u?o()&o():u?satisfy(u,version):!o())}return!!o();\n}\nvar ensureExistence = (scopeName, key) => {\n\tvar scope = __webpack_require__.S[scopeName];\n\tif(!scope || !__webpack_require__.o(scope, key)) throw new Error(\"Shared module \" + key + \" doesn't exist in shared scope \" + scopeName);\n\treturn scope;\n};\nvar findVersion = (scope, key) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar findSingletonVersionKey = (scope, key) => {\n\tvar versions = scope[key];\n\treturn Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || (!versions[a].loaded && versionLt(a, b)) ? b : a;\n\t}, 0);\n};\nvar getInvalidSingletonVersionMessage = (scope, key, version, requiredVersion) => {\n\treturn \"Unsatisfied version \" + version + \" from \" + (version && scope[key][version].from) + \" of shared singleton module \" + key + \" (required \" + rangeToString(requiredVersion) + \")\"\n};\nvar getSingleton = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\treturn get(scope[key][version]);\n};\nvar getSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) warn(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar getStrictSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) throw new Error(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar findValidVersion = (scope, key, requiredVersion) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\tif (!satisfy(requiredVersion, b)) return a;\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar getInvalidVersionMessage = (scope, scopeName, key, requiredVersion) => {\n\tvar versions = scope[key];\n\treturn \"No satisfying version (\" + rangeToString(requiredVersion) + \") of shared module \" + key + \" found in shared scope \" + scopeName + \".\\n\" +\n\t\t\"Available versions: \" + Object.keys(versions).map((key) => {\n\t\treturn key + \" from \" + versions[key].from;\n\t}).join(\", \");\n};\nvar getValidVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar entry = findValidVersion(scope, key, requiredVersion);\n\tif(entry) return get(entry);\n\tthrow new Error(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar warn = (msg) => {\n\tif (typeof console !== \"undefined\" && console.warn) console.warn(msg);\n};\nvar warnInvalidVersion = (scope, scopeName, key, requiredVersion) => {\n\twarn(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar get = (entry) => {\n\tentry.loaded = 1;\n\treturn entry.get()\n};\nvar init = (fn) => (function(scopeName, a, b, c) {\n\tvar promise = __webpack_require__.I(scopeName);\n\tif (promise && promise.then) return promise.then(fn.bind(fn, scopeName, __webpack_require__.S[scopeName], a, b, c));\n\treturn fn(scopeName, __webpack_require__.S[scopeName], a, b, c);\n});\n\nvar load = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn get(findVersion(scope, key));\n});\nvar loadFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\treturn scope && __webpack_require__.o(scope, key) ? get(findVersion(scope, key)) : fallback();\n});\nvar loadVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingleton = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getValidVersion(scope, scopeName, key, version);\n});\nvar loadStrictSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar loadVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingletonFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tvar entry = scope && __webpack_require__.o(scope, key) && findValidVersion(scope, key, version);\n\treturn entry ? get(entry) : fallback();\n});\nvar loadStrictSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar installedModules = {};\nvar moduleToHandlerMapping = {\n\t\"webpack/sharing/consume/default/@jupyterlab/notebook\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/notebook\", [1,4,0,0,,\"rc\",0]))\n};\n// no consumes in initial chunks\nvar chunkMapping = {\n\t\"lib_index_js\": [\n\t\t\"webpack/sharing/consume/default/@jupyterlab/notebook\"\n\t]\n};\n__webpack_require__.f.consumes = (chunkId, promises) => {\n\tif(__webpack_require__.o(chunkMapping, chunkId)) {\n\t\tchunkMapping[chunkId].forEach((id) => {\n\t\t\tif(__webpack_require__.o(installedModules, id)) return promises.push(installedModules[id]);\n\t\t\tvar onFactory = (factory) => {\n\t\t\t\tinstalledModules[id] = 0;\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tmodule.exports = factory();\n\t\t\t\t}\n\t\t\t};\n\t\t\tvar onError = (error) => {\n\t\t\t\tdelete installedModules[id];\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tthrow error;\n\t\t\t\t}\n\t\t\t};\n\t\t\ttry {\n\t\t\t\tvar promise = moduleToHandlerMapping[id]();\n\t\t\t\tif(promise.then) {\n\t\t\t\t\tpromises.push(installedModules[id] = promise.then(onFactory)['catch'](onError));\n\t\t\t\t} else onFactory(promise);\n\t\t\t} catch(e) { onError(e); }\n\t\t});\n\t}\n}",
+        "var parseVersion = (str) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar p=p=>{return p.split(\".\").map((p=>{return+p==p?+p:p}))},n=/^([^-+]+)?(?:-([^+]+))?(?:\\+(.+))?$/.exec(str),r=n[1]?p(n[1]):[];return n[2]&&(r.length++,r.push.apply(r,p(n[2]))),n[3]&&(r.push([]),r.push.apply(r,p(n[3]))),r;\n}\nvar versionLt = (a, b) => {\n\t// see webpack/lib/util/semver.js for original code\n\ta=parseVersion(a),b=parseVersion(b);for(var r=0;;){if(r>=a.length)return r<b.length&&\"u\"!=(typeof b[r])[0];var e=a[r],n=(typeof e)[0];if(r>=b.length)return\"u\"==n;var t=b[r],f=(typeof t)[0];if(n!=f)return\"o\"==n&&\"n\"==f||(\"s\"==f||\"u\"==n);if(\"o\"!=n&&\"u\"!=n&&e!=t)return e<t;r++}\n}\nvar rangeToString = (range) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar r=range[0],n=\"\";if(1===range.length)return\"*\";if(r+.5){n+=0==r?\">=\":-1==r?\"<\":1==r?\"^\":2==r?\"~\":r>0?\"=\":\"!=\";for(var e=1,a=1;a<range.length;a++){e--,n+=\"u\"==(typeof(t=range[a]))[0]?\"-\":(e>0?\".\":\"\")+(e=2,t)}return n}var g=[];for(a=1;a<range.length;a++){var t=range[a];g.push(0===t?\"not(\"+o()+\")\":1===t?\"(\"+o()+\" || \"+o()+\")\":2===t?g.pop()+\" \"+g.pop():rangeToString(t))}return o();function o(){return g.pop().replace(/^\\((.+)\\)$/,\"$1\")}\n}\nvar satisfy = (range, version) => {\n\t// see webpack/lib/util/semver.js for original code\n\tif(0 in range){version=parseVersion(version);var e=range[0],r=e<0;r&&(e=-e-1);for(var n=0,i=1,a=!0;;i++,n++){var f,s,g=i<range.length?(typeof range[i])[0]:\"\";if(n>=version.length||\"o\"==(s=(typeof(f=version[n]))[0]))return!a||(\"u\"==g?i>e&&!r:\"\"==g!=r);if(\"u\"==s){if(!a||\"u\"!=g)return!1}else if(a)if(g==s)if(i<=e){if(f!=range[i])return!1}else{if(r?f>range[i]:f<range[i])return!1;f!=range[i]&&(a=!1)}else if(\"s\"!=g&&\"n\"!=g){if(r||i<=e)return!1;a=!1,i--}else{if(i<=e||s<g!=r)return!1;a=!1}else\"s\"!=g&&\"n\"!=g&&(a=!1,i--)}}var t=[],o=t.pop.bind(t);for(n=1;n<range.length;n++){var u=range[n];t.push(1==u?o()|o():2==u?o()&o():u?satisfy(u,version):!o())}return!!o();\n}\nvar ensureExistence = (scopeName, key) => {\n\tvar scope = __webpack_require__.S[scopeName];\n\tif(!scope || !__webpack_require__.o(scope, key)) throw new Error(\"Shared module \" + key + \" doesn't exist in shared scope \" + scopeName);\n\treturn scope;\n};\nvar findVersion = (scope, key) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar findSingletonVersionKey = (scope, key) => {\n\tvar versions = scope[key];\n\treturn Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || (!versions[a].loaded && versionLt(a, b)) ? b : a;\n\t}, 0);\n};\nvar getInvalidSingletonVersionMessage = (scope, key, version, requiredVersion) => {\n\treturn \"Unsatisfied version \" + version + \" from \" + (version && scope[key][version].from) + \" of shared singleton module \" + key + \" (required \" + rangeToString(requiredVersion) + \")\"\n};\nvar getSingleton = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\treturn get(scope[key][version]);\n};\nvar getSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) warn(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar getStrictSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) throw new Error(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar findValidVersion = (scope, key, requiredVersion) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\tif (!satisfy(requiredVersion, b)) return a;\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar getInvalidVersionMessage = (scope, scopeName, key, requiredVersion) => {\n\tvar versions = scope[key];\n\treturn \"No satisfying version (\" + rangeToString(requiredVersion) + \") of shared module \" + key + \" found in shared scope \" + scopeName + \".\\n\" +\n\t\t\"Available versions: \" + Object.keys(versions).map((key) => {\n\t\treturn key + \" from \" + versions[key].from;\n\t}).join(\", \");\n};\nvar getValidVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar entry = findValidVersion(scope, key, requiredVersion);\n\tif(entry) return get(entry);\n\tthrow new Error(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar warn = (msg) => {\n\tif (typeof console !== \"undefined\" && console.warn) console.warn(msg);\n};\nvar warnInvalidVersion = (scope, scopeName, key, requiredVersion) => {\n\twarn(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar get = (entry) => {\n\tentry.loaded = 1;\n\treturn entry.get()\n};\nvar init = (fn) => (function(scopeName, a, b, c) {\n\tvar promise = __webpack_require__.I(scopeName);\n\tif (promise && promise.then) return promise.then(fn.bind(fn, scopeName, __webpack_require__.S[scopeName], a, b, c));\n\treturn fn(scopeName, __webpack_require__.S[scopeName], a, b, c);\n});\n\nvar load = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn get(findVersion(scope, key));\n});\nvar loadFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\treturn scope && __webpack_require__.o(scope, key) ? get(findVersion(scope, key)) : fallback();\n});\nvar loadVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingleton = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getValidVersion(scope, scopeName, key, version);\n});\nvar loadStrictSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar loadVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingletonFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tvar entry = scope && __webpack_require__.o(scope, key) && findValidVersion(scope, key, version);\n\treturn entry ? get(entry) : fallback();\n});\nvar loadStrictSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar installedModules = {};\nvar moduleToHandlerMapping = {\n\t\"webpack/sharing/consume/default/@jupyterlab/notebook\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/notebook\", [1,4,0,0,,\"beta\",2])),\n\t\"webpack/sharing/consume/default/@jupyterlab/cells\": () => (loadVersionCheck(\"default\", \"@jupyterlab/cells\", [1,4,0,0,,\"beta\",2]))\n};\n// no consumes in initial chunks\nvar chunkMapping = {\n\t\"lib_index_js\": [\n\t\t\"webpack/sharing/consume/default/@jupyterlab/notebook\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/cells\"\n\t]\n};\n__webpack_require__.f.consumes = (chunkId, promises) => {\n\tif(__webpack_require__.o(chunkMapping, chunkId)) {\n\t\tchunkMapping[chunkId].forEach((id) => {\n\t\t\tif(__webpack_require__.o(installedModules, id)) return promises.push(installedModules[id]);\n\t\t\tvar onFactory = (factory) => {\n\t\t\t\tinstalledModules[id] = 0;\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tmodule.exports = factory();\n\t\t\t\t}\n\t\t\t};\n\t\t\tvar onError = (error) => {\n\t\t\t\tdelete installedModules[id];\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tthrow error;\n\t\t\t\t}\n\t\t\t};\n\t\t\ttry {\n\t\t\t\tvar promise = moduleToHandlerMapping[id]();\n\t\t\t\tif(promise.then) {\n\t\t\t\t\tpromises.push(installedModules[id] = promise.then(onFactory)['catch'](onError));\n\t\t\t\t} else onFactory(promise);\n\t\t\t} catch(e) { onError(e); }\n\t\t});\n\t}\n}",
         "// no baseURI\n\n// object to store loaded and loading chunks\n// undefined = chunk not loaded, null = chunk preloaded/prefetched\n// [resolve, reject, Promise] = chunk loading, 0 = chunk loaded\nvar installedChunks = {\n\t\"jupyterlab-celltagsclasses\": 0\n};\n\n__webpack_require__.f.j = (chunkId, promises) => {\n\t\t// JSONP chunk loading for javascript\n\t\tvar installedChunkData = __webpack_require__.o(installedChunks, chunkId) ? installedChunks[chunkId] : undefined;\n\t\tif(installedChunkData !== 0) { // 0 means \"already installed\".\n\n\t\t\t// a Promise means \"currently loading\".\n\t\t\tif(installedChunkData) {\n\t\t\t\tpromises.push(installedChunkData[2]);\n\t\t\t} else {\n\t\t\t\tif(true) { // all chunks have JS\n\t\t\t\t\t// setup Promise in chunk cache\n\t\t\t\t\tvar promise = new Promise((resolve, reject) => (installedChunkData = installedChunks[chunkId] = [resolve, reject]));\n\t\t\t\t\tpromises.push(installedChunkData[2] = promise);\n\n\t\t\t\t\t// start chunk loading\n\t\t\t\t\tvar url = __webpack_require__.p + __webpack_require__.u(chunkId);\n\t\t\t\t\t// create error before stack unwound to get useful stacktrace later\n\t\t\t\t\tvar error = new Error();\n\t\t\t\t\tvar loadingEnded = (event) => {\n\t\t\t\t\t\tif(__webpack_require__.o(installedChunks, chunkId)) {\n\t\t\t\t\t\t\tinstalledChunkData = installedChunks[chunkId];\n\t\t\t\t\t\t\tif(installedChunkData !== 0) installedChunks[chunkId] = undefined;\n\t\t\t\t\t\t\tif(installedChunkData) {\n\t\t\t\t\t\t\t\tvar errorType = event && (event.type === 'load' ? 'missing' : event.type);\n\t\t\t\t\t\t\t\tvar realSrc = event && event.target && event.target.src;\n\t\t\t\t\t\t\t\terror.message = 'Loading chunk ' + chunkId + ' failed.\\n(' + errorType + ': ' + realSrc + ')';\n\t\t\t\t\t\t\t\terror.name = 'ChunkLoadError';\n\t\t\t\t\t\t\t\terror.type = errorType;\n\t\t\t\t\t\t\t\terror.request = realSrc;\n\t\t\t\t\t\t\t\tinstalledChunkData[1](error);\n\t\t\t\t\t\t\t}\n\t\t\t\t\t\t}\n\t\t\t\t\t};\n\t\t\t\t\t__webpack_require__.l(url, loadingEnded, \"chunk-\" + chunkId, chunkId);\n\t\t\t\t} else installedChunks[chunkId] = 0;\n\t\t\t}\n\t\t}\n};\n\n// no prefetching\n\n// no preloaded\n\n// no HMR\n\n// no HMR manifest\n\n// no on chunks loaded\n\n// install a JSONP callback for chunk loading\nvar webpackJsonpCallback = (parentChunkLoadingFunction, data) => {\n\tvar [chunkIds, moreModules, runtime] = data;\n\t// add \"moreModules\" to the modules object,\n\t// then flag all \"chunkIds\" as loaded and fire callback\n\tvar moduleId, chunkId, i = 0;\n\tif(chunkIds.some((id) => (installedChunks[id] !== 0))) {\n\t\tfor(moduleId in moreModules) {\n\t\t\tif(__webpack_require__.o(moreModules, moduleId)) {\n\t\t\t\t__webpack_require__.m[moduleId] = moreModules[moduleId];\n\t\t\t}\n\t\t}\n\t\tif(runtime) var result = runtime(__webpack_require__);\n\t}\n\tif(parentChunkLoadingFunction) parentChunkLoadingFunction(data);\n\tfor(;i < chunkIds.length; i++) {\n\t\tchunkId = chunkIds[i];\n\t\tif(__webpack_require__.o(installedChunks, chunkId) && installedChunks[chunkId]) {\n\t\t\tinstalledChunks[chunkId][0]();\n\t\t}\n\t\tinstalledChunks[chunkId] = 0;\n\t}\n\n}\n\nvar chunkLoadingGlobal = self[\"webpackChunkjupyterlab_celltagsclasses\"] = self[\"webpackChunkjupyterlab_celltagsclasses\"] || [];\nchunkLoadingGlobal.forEach(webpackJsonpCallback.bind(null, 0));\nchunkLoadingGlobal.push = webpackJsonpCallback.bind(null, chunkLoadingGlobal.push.bind(chunkLoadingGlobal));",
         "__webpack_require__.nc = undefined;",
         "",
         "// module cache are used so entry inlining is disabled\n// startup\n// Load entry module and return exports\nvar __webpack_exports__ = __webpack_require__(\"webpack/container/entry/jupyterlab-celltagsclasses\");\n",
         ""
     ],
     "version": 3
```

### Comparing `jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/style_index_js.012e4d3162293b291168.js` & `jupyterlab_celltagsclasses-0.2.0/jupyterlab_celltagsclasses/labextension/static/style_index_js.4784725fff15b54ffe3d.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -26,20 +26,20 @@
                 /* harmony import */
                 var _node_modules_css_loader_dist_runtime_api_js__WEBPACK_IMPORTED_MODULE_1___default = /*#__PURE__*/ __webpack_require__.n(_node_modules_css_loader_dist_runtime_api_js__WEBPACK_IMPORTED_MODULE_1__);
                 // Imports
 
 
                 var ___CSS_LOADER_EXPORT___ = _node_modules_css_loader_dist_runtime_api_js__WEBPACK_IMPORTED_MODULE_1___default()((_node_modules_css_loader_dist_runtime_sourceMaps_js__WEBPACK_IMPORTED_MODULE_0___default()));
                 // Module
-                ___CSS_LOADER_EXPORT___.push([module.id, "/*\n    See the JupyterLab Developer Guide for useful CSS Patterns:\n\n    https://jupyterlab.readthedocs.io/en/stable/developer/css.html\n*/\n\n/* hide only the input of cells with the tag 'hide-input' */\n.cell-tag-celltagsclasses-test1 {\n  padding: 10px;\n  border: 2.5px black solid;\n  border-radius: 10px;\n  background-color: yellow !important;  /* could be overridden if cell is active */\n}\n\n.cell-tag-celltagsclasses-test2 {\n  background-color: red;\n  /* see how it goes if cell is active */\n}\n\n/* hide the 6-buttons toolbar */\n.cell-tag-celltagsclasses-test2 .jp-cell-toolbar {\n  display: none;\n}", "", {
+                ___CSS_LOADER_EXPORT___.push([module.id, "/*\n    See the JupyterLab Developer Guide for useful CSS Patterns:\n\n    https://jupyterlab.readthedocs.io/en/stable/developer/css.html\n*/\n\n/* hide only the input of cells with the tag 'hide-input' */\n.cell-tag-celltagsclasses-test1 {\n  padding: 10px;\n  border: 2.5px black solid;\n  border-radius: 10px;\n\n  /* could be overridden if cell is active */\n  background-color: yellow !important;\n}\n\n.cell-tag-celltagsclasses-test2 {\n  /* see how it goes if cell is active */\n  background-color: red;\n}\n\n/* hide the 6-buttons toolbar */\n.cell-tag-celltagsclasses-test2 .jp-cell-toolbar {\n  display: none;\n}\n", "", {
                     "version": 3,
                     "sources": ["webpack://./style/base.css"],
                     "names": [],
-                    "mappings": "AAAA;;;;CAIC;;AAED,2DAA2D;AAC3D;EACE,aAAa;EACb,yBAAyB;EACzB,mBAAmB;EACnB,mCAAmC,GAAG,0CAA0C;AAClF;;AAEA;EACE,qBAAqB;EACrB,sCAAsC;AACxC;;AAEA,+BAA+B;AAC/B;EACE,aAAa;AACf",
-                    "sourcesContent": ["/*\n    See the JupyterLab Developer Guide for useful CSS Patterns:\n\n    https://jupyterlab.readthedocs.io/en/stable/developer/css.html\n*/\n\n/* hide only the input of cells with the tag 'hide-input' */\n.cell-tag-celltagsclasses-test1 {\n  padding: 10px;\n  border: 2.5px black solid;\n  border-radius: 10px;\n  background-color: yellow !important;  /* could be overridden if cell is active */\n}\n\n.cell-tag-celltagsclasses-test2 {\n  background-color: red;\n  /* see how it goes if cell is active */\n}\n\n/* hide the 6-buttons toolbar */\n.cell-tag-celltagsclasses-test2 .jp-cell-toolbar {\n  display: none;\n}"],
+                    "mappings": "AAAA;;;;CAIC;;AAED,2DAA2D;AAC3D;EACE,aAAa;EACb,yBAAyB;EACzB,mBAAmB;;EAEnB,0CAA0C;EAC1C,mCAAmC;AACrC;;AAEA;EACE,sCAAsC;EACtC,qBAAqB;AACvB;;AAEA,+BAA+B;AAC/B;EACE,aAAa;AACf",
+                    "sourcesContent": ["/*\n    See the JupyterLab Developer Guide for useful CSS Patterns:\n\n    https://jupyterlab.readthedocs.io/en/stable/developer/css.html\n*/\n\n/* hide only the input of cells with the tag 'hide-input' */\n.cell-tag-celltagsclasses-test1 {\n  padding: 10px;\n  border: 2.5px black solid;\n  border-radius: 10px;\n\n  /* could be overridden if cell is active */\n  background-color: yellow !important;\n}\n\n.cell-tag-celltagsclasses-test2 {\n  /* see how it goes if cell is active */\n  background-color: red;\n}\n\n/* hide the 6-buttons toolbar */\n.cell-tag-celltagsclasses-test2 .jp-cell-toolbar {\n  display: none;\n}\n"],
                     "sourceRoot": ""
                 }]);
                 // Exports
                 /* harmony default export */
                 const __WEBPACK_DEFAULT_EXPORT__ = (___CSS_LOADER_EXPORT___);
 
 
@@ -551,8 +551,8 @@
 
 
                 /***/
             })
 
     }
 ]);
-//# sourceMappingURL=style_index_js.012e4d3162293b291168.js.map
+//# sourceMappingURL=style_index_js.4784725fff15b54ffe3d.js.map
```

### Comparing `jupyterlab_celltagsclasses-0.1.2/jupyterlab_celltagsclasses/labextension/static/style_index_js.012e4d3162293b291168.js.map` & `jupyterlab_celltagsclasses-0.2.0/jupyterlab_celltagsclasses/labextension/static/style_index_js.4784725fff15b54ffe3d.js.map`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8351648351648352%*

 * *Differences: {"'file'": "'style_index_js.4784725fff15b54ffe3d.js'",*

 * * "'mappings'": "';;;;;;;;;;;;;;;;;AAAA;AAC0G;AACjB;AACzF,8BAA8B,mFAA2B,CAAC,4FAAqC;AAC/F;AACA,0RAA0R,kBAAkB,8BAA8B,wBAAwB,yFAAyF,GAAG,qCAAqC,qEAAqE,GAAG,wFAAwF,kBAAkB,GAAG,SAAS,oFAAoF,MAAM,YAAY,MAAM,UAAU,YAAY,cAAc,aAAa,aAAa,OAAO,KAAK,YAAY,aAAa,OAAO,YAAY,MAAM,UAAU,yQAAyQ,kBAAkB,8BAA8B,wBAAwB,yFAAyF,GAAG,qCAAqC,qEAAqE,GAAG,wFAAwF,kBAAkB,GAAG,qBAAqB;AAC/iD;AACA,iEAAe,uBAAuB,EAAC;;;;;;;;;;;ACP1B;;AAEb;AACA;AACA;AACA;AACA;AACA;;AAEA;AACA;AACA;AACA;AACA;AACA; […]*

```diff
@@ -1,10 +1,10 @@
 {
-    "file": "style_index_js.012e4d3162293b291168.js",
-    "mappings": ";;;;;;;;;;;;;;;;;AAAA;AAC0G;AACjB;AACzF,8BAA8B,mFAA2B,CAAC,4FAAqC;AAC/F;AACA,0RAA0R,kBAAkB,8BAA8B,wBAAwB,0CAA0C,8CAA8C,qCAAqC,0BAA0B,8CAA8C,wFAAwF,kBAAkB,GAAG,OAAO,oFAAoF,MAAM,YAAY,MAAM,UAAU,YAAY,aAAa,yBAAyB,OAAO,KAAK,YAAY,aAAa,OAAO,YAAY,MAAM,UAAU,yQAAyQ,kBAAkB,8BAA8B,wBAAwB,0CAA0C,8CAA8C,qCAAqC,0BAA0B,8CAA8C,wFAAwF,kBAAkB,GAAG,mBAAmB;AACjiD;AACA,iEAAe,uBAAuB,EAAC;;;;;;;;;;;ACP1B;;AAEb;AACA;AACA;AACA;AACA;AACA;;AAEA;AACA;AACA;AACA;AACA;AACA;AACA,qDAAqD;AACrD;AACA;AACA,gDAAgD;AAChD;AACA;AACA,qFAAqF;AACrF;AACA;AACA;AACA,qBAAqB;AACrB;AACA;AACA,qBAAqB;AACrB;AACA;AACA,qBAAqB;AACrB;AACA;AACA,KAAK;AACL;;AAEA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,sBAAsB,iBAAiB;AACvC;AACA;AACA;AACA;AACA;AACA;AACA,qBAAqB,qBAAqB;AAC1C;AACA;AACA;AACA;AACA;AACA;AACA;AACA,UAAU;AACV,sFAAsF,qBAAqB;AAC3G;AACA;AACA;AACA;AACA;AACA;AACA,UAAU;AACV,iDAAiD,qBAAqB;AACtE;AACA;AACA;AACA;AACA;AACA;AACA,UAAU;AACV,sDAAsD,qBAAqB;AAC3E;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;;;;;;;;;ACpFa;;AAEb;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,uDAAuD,cAAc;AACrE;AACA;AACA;AACA;AACA;;;;;;;;;;ACfa;;AAEb;AACA;AACA;AACA,kBAAkB,wBAAwB;AAC1C;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,kBAAkB,iBAAiB;AACnC;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,MAAM;AACN;AACA;AACA;AACA;AACA;AACA;AACA,OAAO;AACP;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,MAAM;AACN;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,oBAAoB,4BAA4B;AAChD;AACA;AACA;AACA;AACA;AACA,qBAAqB,6BAA6B;AAClD;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;;;;;;;;;ACnFa;;AAEb;;AAEA;AACA;AACA;AACA;;AAEA;AACA;AACA;AACA;AACA;AACA;AACA,QAAQ;AACR;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;AAEA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;;;;;;;;;ACjCa;;AAEb;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;;;;;;;;;ACTa;;AAEb;AACA;AACA,cAAc,KAAwC,GAAG,sBAAiB,GAAG,CAAI;AACjF;AACA;AACA;AACA;AACA;;;;;;;;;;ACTa;;AAEb;AACA;AACA;AACA;AACA,kDAAkD;AAClD;AACA;AACA,0CAA0C;AAC1C;AACA;AACA;AACA,iFAAiF;AACjF;AACA;AACA;AACA,aAAa;AACb;AACA;AACA,aAAa;AACb;AACA;AACA,aAAa;AACb;AACA;AACA;AACA,yDAAyD;AACzD;;AAEA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;AAEA;AACA;AACA;AACA;AACA,kCAAkC;AAClC;AACA;AACA;AACA;AACA;AACA;AACA;AACA,KAAK;AACL;AACA;AACA;AACA;AACA;AACA;;;;;;;;;;AC5Da;;AAEb;AACA;AACA;AACA;AACA,IAAI;AACJ;AACA;AACA;AACA;AACA;AACA;AACA;;;;;;;;;;;;ACboB;;;;;;;;;;;;;;;;;;;;;;;;;;;;;ACCpB,MAA+F;AAC/F,MAAqF;AACrF,MAA4F;AAC5F,MAA+G;AAC/G,MAAwG;AACxG,MAAwG;AACxG,MAAkG;AAClG;AACA;;AAEA;;AAEA,4BAA4B,qGAAmB;AAC/C,wBAAwB,kHAAa;;AAErC,uBAAuB,uGAAa;AACpC;AACA,iBAAiB,+FAAM;AACvB,6BAA6B,sGAAkB;;AAE/C,aAAa,0GAAG,CAAC,qFAAO;;;;AAI4C;AACpE,OAAO,iEAAe,qFAAO,IAAI,4FAAc,GAAG,4FAAc,YAAY,EAAC",
+    "file": "style_index_js.4784725fff15b54ffe3d.js",
+    "mappings": ";;;;;;;;;;;;;;;;;AAAA;AAC0G;AACjB;AACzF,8BAA8B,mFAA2B,CAAC,4FAAqC;AAC/F;AACA,0RAA0R,kBAAkB,8BAA8B,wBAAwB,yFAAyF,GAAG,qCAAqC,qEAAqE,GAAG,wFAAwF,kBAAkB,GAAG,SAAS,oFAAoF,MAAM,YAAY,MAAM,UAAU,YAAY,cAAc,aAAa,aAAa,OAAO,KAAK,YAAY,aAAa,OAAO,YAAY,MAAM,UAAU,yQAAyQ,kBAAkB,8BAA8B,wBAAwB,yFAAyF,GAAG,qCAAqC,qEAAqE,GAAG,wFAAwF,kBAAkB,GAAG,qBAAqB;AAC/iD;AACA,iEAAe,uBAAuB,EAAC;;;;;;;;;;;ACP1B;;AAEb;AACA;AACA;AACA;AACA;AACA;;AAEA;AACA;AACA;AACA;AACA;AACA;AACA,qDAAqD;AACrD;AACA;AACA,gDAAgD;AAChD;AACA;AACA,qFAAqF;AACrF;AACA;AACA;AACA,qBAAqB;AACrB;AACA;AACA,qBAAqB;AACrB;AACA;AACA,qBAAqB;AACrB;AACA;AACA,KAAK;AACL;;AAEA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,sBAAsB,iBAAiB;AACvC;AACA;AACA;AACA;AACA;AACA;AACA,qBAAqB,qBAAqB;AAC1C;AACA;AACA;AACA;AACA;AACA;AACA;AACA,UAAU;AACV,sFAAsF,qBAAqB;AAC3G;AACA;AACA;AACA;AACA;AACA;AACA,UAAU;AACV,iDAAiD,qBAAqB;AACtE;AACA;AACA;AACA;AACA;AACA;AACA,UAAU;AACV,sDAAsD,qBAAqB;AAC3E;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;;;;;;;;;ACpFa;;AAEb;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,uDAAuD,cAAc;AACrE;AACA;AACA;AACA;AACA;;;;;;;;;;ACfa;;AAEb;AACA;AACA;AACA,kBAAkB,wBAAwB;AAC1C;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,kBAAkB,iBAAiB;AACnC;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,MAAM;AACN;AACA;AACA;AACA;AACA;AACA;AACA,OAAO;AACP;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,MAAM;AACN;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,oBAAoB,4BAA4B;AAChD;AACA;AACA;AACA;AACA;AACA,qBAAqB,6BAA6B;AAClD;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;;;;;;;;;ACnFa;;AAEb;;AAEA;AACA;AACA;AACA;;AAEA;AACA;AACA;AACA;AACA;AACA;AACA,QAAQ;AACR;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;AAEA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;;;;;;;;;ACjCa;;AAEb;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;;;;;;;;;ACTa;;AAEb;AACA;AACA,cAAc,KAAwC,GAAG,sBAAiB,GAAG,CAAI;AACjF;AACA;AACA;AACA;AACA;;;;;;;;;;ACTa;;AAEb;AACA;AACA;AACA;AACA,kDAAkD;AAClD;AACA;AACA,0CAA0C;AAC1C;AACA;AACA;AACA,iFAAiF;AACjF;AACA;AACA;AACA,aAAa;AACb;AACA;AACA,aAAa;AACb;AACA;AACA,aAAa;AACb;AACA;AACA;AACA,yDAAyD;AACzD;;AAEA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;AAEA;AACA;AACA;AACA;AACA,kCAAkC;AAClC;AACA;AACA;AACA;AACA;AACA;AACA;AACA,KAAK;AACL;AACA;AACA;AACA;AACA;AACA;;;;;;;;;;AC5Da;;AAEb;AACA;AACA;AACA;AACA,IAAI;AACJ;AACA;AACA;AACA;AACA;AACA;AACA;;;;;;;;;;;;ACbmB;;;;;;;;;;;;;;;;;;;;;;;;;;;;;ACCnB,MAA+F;AAC/F,MAAqF;AACrF,MAA4F;AAC5F,MAA+G;AAC/G,MAAwG;AACxG,MAAwG;AACxG,MAAkG;AAClG;AACA;;AAEA;;AAEA,4BAA4B,qGAAmB;AAC/C,wBAAwB,kHAAa;;AAErC,uBAAuB,uGAAa;AACpC;AACA,iBAAiB,+FAAM;AACvB,6BAA6B,sGAAkB;;AAE/C,aAAa,0GAAG,CAAC,qFAAO;;;;AAI4C;AACpE,OAAO,iEAAe,qFAAO,IAAI,4FAAc,GAAG,4FAAc,YAAY,EAAC",
     "names": [],
     "sourceRoot": "",
     "sources": [
         "webpack://jupyterlab-celltagsclasses/./style/base.css",
         "webpack://jupyterlab-celltagsclasses/./node_modules/css-loader/dist/runtime/api.js",
         "webpack://jupyterlab-celltagsclasses/./node_modules/css-loader/dist/runtime/sourceMaps.js",
         "webpack://jupyterlab-celltagsclasses/./node_modules/style-loader/dist/runtime/injectStylesIntoStyleTag.js",
@@ -13,21 +13,21 @@
         "webpack://jupyterlab-celltagsclasses/./node_modules/style-loader/dist/runtime/setAttributesWithoutAttributes.js",
         "webpack://jupyterlab-celltagsclasses/./node_modules/style-loader/dist/runtime/styleDomAPI.js",
         "webpack://jupyterlab-celltagsclasses/./node_modules/style-loader/dist/runtime/styleTagTransform.js",
         "webpack://jupyterlab-celltagsclasses/./style/index.js",
         "webpack://jupyterlab-celltagsclasses/./style/base.css?1944"
     ],
     "sourcesContent": [
-        "// Imports\nimport ___CSS_LOADER_API_SOURCEMAP_IMPORT___ from \"../node_modules/css-loader/dist/runtime/sourceMaps.js\";\nimport ___CSS_LOADER_API_IMPORT___ from \"../node_modules/css-loader/dist/runtime/api.js\";\nvar ___CSS_LOADER_EXPORT___ = ___CSS_LOADER_API_IMPORT___(___CSS_LOADER_API_SOURCEMAP_IMPORT___);\n// Module\n___CSS_LOADER_EXPORT___.push([module.id, \"/*\\n    See the JupyterLab Developer Guide for useful CSS Patterns:\\n\\n    https://jupyterlab.readthedocs.io/en/stable/developer/css.html\\n*/\\n\\n/* hide only the input of cells with the tag 'hide-input' */\\n.cell-tag-celltagsclasses-test1 {\\n  padding: 10px;\\n  border: 2.5px black solid;\\n  border-radius: 10px;\\n  background-color: yellow !important;  /* could be overridden if cell is active */\\n}\\n\\n.cell-tag-celltagsclasses-test2 {\\n  background-color: red;\\n  /* see how it goes if cell is active */\\n}\\n\\n/* hide the 6-buttons toolbar */\\n.cell-tag-celltagsclasses-test2 .jp-cell-toolbar {\\n  display: none;\\n}\", \"\",{\"version\":3,\"sources\":[\"webpack://./style/base.css\"],\"names\":[],\"mappings\":\"AAAA;;;;CAIC;;AAED,2DAA2D;AAC3D;EACE,aAAa;EACb,yBAAyB;EACzB,mBAAmB;EACnB,mCAAmC,GAAG,0CAA0C;AAClF;;AAEA;EACE,qBAAqB;EACrB,sCAAsC;AACxC;;AAEA,+BAA+B;AAC/B;EACE,aAAa;AACf\",\"sourcesContent\":[\"/*\\n    See the JupyterLab Developer Guide for useful CSS Patterns:\\n\\n    https://jupyterlab.readthedocs.io/en/stable/developer/css.html\\n*/\\n\\n/* hide only the input of cells with the tag 'hide-input' */\\n.cell-tag-celltagsclasses-test1 {\\n  padding: 10px;\\n  border: 2.5px black solid;\\n  border-radius: 10px;\\n  background-color: yellow !important;  /* could be overridden if cell is active */\\n}\\n\\n.cell-tag-celltagsclasses-test2 {\\n  background-color: red;\\n  /* see how it goes if cell is active */\\n}\\n\\n/* hide the 6-buttons toolbar */\\n.cell-tag-celltagsclasses-test2 .jp-cell-toolbar {\\n  display: none;\\n}\"],\"sourceRoot\":\"\"}]);\n// Exports\nexport default ___CSS_LOADER_EXPORT___;\n",
+        "// Imports\nimport ___CSS_LOADER_API_SOURCEMAP_IMPORT___ from \"../node_modules/css-loader/dist/runtime/sourceMaps.js\";\nimport ___CSS_LOADER_API_IMPORT___ from \"../node_modules/css-loader/dist/runtime/api.js\";\nvar ___CSS_LOADER_EXPORT___ = ___CSS_LOADER_API_IMPORT___(___CSS_LOADER_API_SOURCEMAP_IMPORT___);\n// Module\n___CSS_LOADER_EXPORT___.push([module.id, \"/*\\n    See the JupyterLab Developer Guide for useful CSS Patterns:\\n\\n    https://jupyterlab.readthedocs.io/en/stable/developer/css.html\\n*/\\n\\n/* hide only the input of cells with the tag 'hide-input' */\\n.cell-tag-celltagsclasses-test1 {\\n  padding: 10px;\\n  border: 2.5px black solid;\\n  border-radius: 10px;\\n\\n  /* could be overridden if cell is active */\\n  background-color: yellow !important;\\n}\\n\\n.cell-tag-celltagsclasses-test2 {\\n  /* see how it goes if cell is active */\\n  background-color: red;\\n}\\n\\n/* hide the 6-buttons toolbar */\\n.cell-tag-celltagsclasses-test2 .jp-cell-toolbar {\\n  display: none;\\n}\\n\", \"\",{\"version\":3,\"sources\":[\"webpack://./style/base.css\"],\"names\":[],\"mappings\":\"AAAA;;;;CAIC;;AAED,2DAA2D;AAC3D;EACE,aAAa;EACb,yBAAyB;EACzB,mBAAmB;;EAEnB,0CAA0C;EAC1C,mCAAmC;AACrC;;AAEA;EACE,sCAAsC;EACtC,qBAAqB;AACvB;;AAEA,+BAA+B;AAC/B;EACE,aAAa;AACf\",\"sourcesContent\":[\"/*\\n    See the JupyterLab Developer Guide for useful CSS Patterns:\\n\\n    https://jupyterlab.readthedocs.io/en/stable/developer/css.html\\n*/\\n\\n/* hide only the input of cells with the tag 'hide-input' */\\n.cell-tag-celltagsclasses-test1 {\\n  padding: 10px;\\n  border: 2.5px black solid;\\n  border-radius: 10px;\\n\\n  /* could be overridden if cell is active */\\n  background-color: yellow !important;\\n}\\n\\n.cell-tag-celltagsclasses-test2 {\\n  /* see how it goes if cell is active */\\n  background-color: red;\\n}\\n\\n/* hide the 6-buttons toolbar */\\n.cell-tag-celltagsclasses-test2 .jp-cell-toolbar {\\n  display: none;\\n}\\n\"],\"sourceRoot\":\"\"}]);\n// Exports\nexport default ___CSS_LOADER_EXPORT___;\n",
         "\"use strict\";\n\n/*\n  MIT License http://www.opensource.org/licenses/mit-license.php\n  Author Tobias Koppers @sokra\n*/\nmodule.exports = function (cssWithMappingToString) {\n  var list = [];\n\n  // return the list of modules as css string\n  list.toString = function toString() {\n    return this.map(function (item) {\n      var content = \"\";\n      var needLayer = typeof item[5] !== \"undefined\";\n      if (item[4]) {\n        content += \"@supports (\".concat(item[4], \") {\");\n      }\n      if (item[2]) {\n        content += \"@media \".concat(item[2], \" {\");\n      }\n      if (needLayer) {\n        content += \"@layer\".concat(item[5].length > 0 ? \" \".concat(item[5]) : \"\", \" {\");\n      }\n      content += cssWithMappingToString(item);\n      if (needLayer) {\n        content += \"}\";\n      }\n      if (item[2]) {\n        content += \"}\";\n      }\n      if (item[4]) {\n        content += \"}\";\n      }\n      return content;\n    }).join(\"\");\n  };\n\n  // import a list of modules into the list\n  list.i = function i(modules, media, dedupe, supports, layer) {\n    if (typeof modules === \"string\") {\n      modules = [[null, modules, undefined]];\n    }\n    var alreadyImportedModules = {};\n    if (dedupe) {\n      for (var k = 0; k < this.length; k++) {\n        var id = this[k][0];\n        if (id != null) {\n          alreadyImportedModules[id] = true;\n        }\n      }\n    }\n    for (var _k = 0; _k < modules.length; _k++) {\n      var item = [].concat(modules[_k]);\n      if (dedupe && alreadyImportedModules[item[0]]) {\n        continue;\n      }\n      if (typeof layer !== \"undefined\") {\n        if (typeof item[5] === \"undefined\") {\n          item[5] = layer;\n        } else {\n          item[1] = \"@layer\".concat(item[5].length > 0 ? \" \".concat(item[5]) : \"\", \" {\").concat(item[1], \"}\");\n          item[5] = layer;\n        }\n      }\n      if (media) {\n        if (!item[2]) {\n          item[2] = media;\n        } else {\n          item[1] = \"@media \".concat(item[2], \" {\").concat(item[1], \"}\");\n          item[2] = media;\n        }\n      }\n      if (supports) {\n        if (!item[4]) {\n          item[4] = \"\".concat(supports);\n        } else {\n          item[1] = \"@supports (\".concat(item[4], \") {\").concat(item[1], \"}\");\n          item[4] = supports;\n        }\n      }\n      list.push(item);\n    }\n  };\n  return list;\n};",
         "\"use strict\";\n\nmodule.exports = function (item) {\n  var content = item[1];\n  var cssMapping = item[3];\n  if (!cssMapping) {\n    return content;\n  }\n  if (typeof btoa === \"function\") {\n    var base64 = btoa(unescape(encodeURIComponent(JSON.stringify(cssMapping))));\n    var data = \"sourceMappingURL=data:application/json;charset=utf-8;base64,\".concat(base64);\n    var sourceMapping = \"/*# \".concat(data, \" */\");\n    return [content].concat([sourceMapping]).join(\"\\n\");\n  }\n  return [content].join(\"\\n\");\n};",
         "\"use strict\";\n\nvar stylesInDOM = [];\nfunction getIndexByIdentifier(identifier) {\n  var result = -1;\n  for (var i = 0; i < stylesInDOM.length; i++) {\n    if (stylesInDOM[i].identifier === identifier) {\n      result = i;\n      break;\n    }\n  }\n  return result;\n}\nfunction modulesToDom(list, options) {\n  var idCountMap = {};\n  var identifiers = [];\n  for (var i = 0; i < list.length; i++) {\n    var item = list[i];\n    var id = options.base ? item[0] + options.base : item[0];\n    var count = idCountMap[id] || 0;\n    var identifier = \"\".concat(id, \" \").concat(count);\n    idCountMap[id] = count + 1;\n    var indexByIdentifier = getIndexByIdentifier(identifier);\n    var obj = {\n      css: item[1],\n      media: item[2],\n      sourceMap: item[3],\n      supports: item[4],\n      layer: item[5]\n    };\n    if (indexByIdentifier !== -1) {\n      stylesInDOM[indexByIdentifier].references++;\n      stylesInDOM[indexByIdentifier].updater(obj);\n    } else {\n      var updater = addElementStyle(obj, options);\n      options.byIndex = i;\n      stylesInDOM.splice(i, 0, {\n        identifier: identifier,\n        updater: updater,\n        references: 1\n      });\n    }\n    identifiers.push(identifier);\n  }\n  return identifiers;\n}\nfunction addElementStyle(obj, options) {\n  var api = options.domAPI(options);\n  api.update(obj);\n  var updater = function updater(newObj) {\n    if (newObj) {\n      if (newObj.css === obj.css && newObj.media === obj.media && newObj.sourceMap === obj.sourceMap && newObj.supports === obj.supports && newObj.layer === obj.layer) {\n        return;\n      }\n      api.update(obj = newObj);\n    } else {\n      api.remove();\n    }\n  };\n  return updater;\n}\nmodule.exports = function (list, options) {\n  options = options || {};\n  list = list || [];\n  var lastIdentifiers = modulesToDom(list, options);\n  return function update(newList) {\n    newList = newList || [];\n    for (var i = 0; i < lastIdentifiers.length; i++) {\n      var identifier = lastIdentifiers[i];\n      var index = getIndexByIdentifier(identifier);\n      stylesInDOM[index].references--;\n    }\n    var newLastIdentifiers = modulesToDom(newList, options);\n    for (var _i = 0; _i < lastIdentifiers.length; _i++) {\n      var _identifier = lastIdentifiers[_i];\n      var _index = getIndexByIdentifier(_identifier);\n      if (stylesInDOM[_index].references === 0) {\n        stylesInDOM[_index].updater();\n        stylesInDOM.splice(_index, 1);\n      }\n    }\n    lastIdentifiers = newLastIdentifiers;\n  };\n};",
         "\"use strict\";\n\nvar memo = {};\n\n/* istanbul ignore next  */\nfunction getTarget(target) {\n  if (typeof memo[target] === \"undefined\") {\n    var styleTarget = document.querySelector(target);\n\n    // Special case to return head of iframe instead of iframe itself\n    if (window.HTMLIFrameElement && styleTarget instanceof window.HTMLIFrameElement) {\n      try {\n        // This will throw an exception if access to iframe is blocked\n        // due to cross-origin restrictions\n        styleTarget = styleTarget.contentDocument.head;\n      } catch (e) {\n        // istanbul ignore next\n        styleTarget = null;\n      }\n    }\n    memo[target] = styleTarget;\n  }\n  return memo[target];\n}\n\n/* istanbul ignore next  */\nfunction insertBySelector(insert, style) {\n  var target = getTarget(insert);\n  if (!target) {\n    throw new Error(\"Couldn't find a style target. This probably means that the value for the 'insert' parameter is invalid.\");\n  }\n  target.appendChild(style);\n}\nmodule.exports = insertBySelector;",
         "\"use strict\";\n\n/* istanbul ignore next  */\nfunction insertStyleElement(options) {\n  var element = document.createElement(\"style\");\n  options.setAttributes(element, options.attributes);\n  options.insert(element, options.options);\n  return element;\n}\nmodule.exports = insertStyleElement;",
         "\"use strict\";\n\n/* istanbul ignore next  */\nfunction setAttributesWithoutAttributes(styleElement) {\n  var nonce = typeof __webpack_nonce__ !== \"undefined\" ? __webpack_nonce__ : null;\n  if (nonce) {\n    styleElement.setAttribute(\"nonce\", nonce);\n  }\n}\nmodule.exports = setAttributesWithoutAttributes;",
         "\"use strict\";\n\n/* istanbul ignore next  */\nfunction apply(styleElement, options, obj) {\n  var css = \"\";\n  if (obj.supports) {\n    css += \"@supports (\".concat(obj.supports, \") {\");\n  }\n  if (obj.media) {\n    css += \"@media \".concat(obj.media, \" {\");\n  }\n  var needLayer = typeof obj.layer !== \"undefined\";\n  if (needLayer) {\n    css += \"@layer\".concat(obj.layer.length > 0 ? \" \".concat(obj.layer) : \"\", \" {\");\n  }\n  css += obj.css;\n  if (needLayer) {\n    css += \"}\";\n  }\n  if (obj.media) {\n    css += \"}\";\n  }\n  if (obj.supports) {\n    css += \"}\";\n  }\n  var sourceMap = obj.sourceMap;\n  if (sourceMap && typeof btoa !== \"undefined\") {\n    css += \"\\n/*# sourceMappingURL=data:application/json;base64,\".concat(btoa(unescape(encodeURIComponent(JSON.stringify(sourceMap)))), \" */\");\n  }\n\n  // For old IE\n  /* istanbul ignore if  */\n  options.styleTagTransform(css, styleElement, options.options);\n}\nfunction removeStyleElement(styleElement) {\n  // istanbul ignore if\n  if (styleElement.parentNode === null) {\n    return false;\n  }\n  styleElement.parentNode.removeChild(styleElement);\n}\n\n/* istanbul ignore next  */\nfunction domAPI(options) {\n  if (typeof document === \"undefined\") {\n    return {\n      update: function update() {},\n      remove: function remove() {}\n    };\n  }\n  var styleElement = options.insertStyleElement(options);\n  return {\n    update: function update(obj) {\n      apply(styleElement, options, obj);\n    },\n    remove: function remove() {\n      removeStyleElement(styleElement);\n    }\n  };\n}\nmodule.exports = domAPI;",
         "\"use strict\";\n\n/* istanbul ignore next  */\nfunction styleTagTransform(css, styleElement) {\n  if (styleElement.styleSheet) {\n    styleElement.styleSheet.cssText = css;\n  } else {\n    while (styleElement.firstChild) {\n      styleElement.removeChild(styleElement.firstChild);\n    }\n    styleElement.appendChild(document.createTextNode(css));\n  }\n}\nmodule.exports = styleTagTransform;",
-        "import './base.css';\n",
+        "import './base.css'\n",
         "\n      import API from \"!../node_modules/style-loader/dist/runtime/injectStylesIntoStyleTag.js\";\n      import domAPI from \"!../node_modules/style-loader/dist/runtime/styleDomAPI.js\";\n      import insertFn from \"!../node_modules/style-loader/dist/runtime/insertBySelector.js\";\n      import setAttributes from \"!../node_modules/style-loader/dist/runtime/setAttributesWithoutAttributes.js\";\n      import insertStyleElement from \"!../node_modules/style-loader/dist/runtime/insertStyleElement.js\";\n      import styleTagTransformFn from \"!../node_modules/style-loader/dist/runtime/styleTagTransform.js\";\n      import content, * as namedExport from \"!!../node_modules/css-loader/dist/cjs.js!./base.css\";\n      \n      \n\nvar options = {};\n\noptions.styleTagTransform = styleTagTransformFn;\noptions.setAttributes = setAttributes;\n\n      options.insert = insertFn.bind(null, \"head\");\n    \noptions.domAPI = domAPI;\noptions.insertStyleElement = insertStyleElement;\n\nvar update = API(content, options);\n\n\n\nexport * from \"!!../node_modules/css-loader/dist/cjs.js!./base.css\";\n       export default content && content.locals ? content.locals : undefined;\n"
     ],
     "version": 3
 }
```

### Comparing `jupyterlab_celltagsclasses-0.1.2/media/screenshot.png` & `jupyterlab_celltagsclasses-0.2.0/media/screenshot.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_celltagsclasses-0.1.2/style/base.css` & `jupyterlab_celltagsclasses-0.2.0/style/base.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_celltagsclasses-0.1.2/.gitignore` & `jupyterlab_celltagsclasses-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyterlab_celltagsclasses-0.1.2/LICENSE` & `jupyterlab_celltagsclasses-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_celltagsclasses-0.1.2/pyproject.toml` & `jupyterlab_celltagsclasses-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyterlab_celltagsclasses-0.1.2/PKG-INFO` & `jupyterlab_celltagsclasses-0.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyterlab_celltagsclasses
-Version: 0.1.2
+Version: 0.2.0
 Summary: JLAB extension to add classes to cells based on their tags
 Project-URL: Homepage, https://github.com/parmentelat/jupyterlab-celltagsclasses
 Project-URL: Bug Tracker, https://github.com/parmentelat/jupyterlab-celltagsclasses/issues
 Project-URL: Repository, https://github.com/parmentelat/jupyterlab-celltagsclasses.git
 Author-email: Thierry Parmentelat <thierry.parmentelat@inria.fr>
 License: BSD 3-Clause License
         
@@ -75,21 +75,32 @@
 
 ```bash
 pip uninstall jupyterlab_celltagsclasses
 ```
 
 ## What it does
 
+### CSS classes
+
 each cell has its widget (the DOM element) classes kept in sync in terms of the cell's tags;  
 for example, adding tag `foobar` will result in the current cell having class `cell-tag-foobar` added
 
 specifically the DOM elements that are decorated have the `.jpCell` class set by jlab, like so, where we have set tag `celltagsclasses-test1`
 
 ![](media/screenshot.png)
 
+### metadata management helper functions
+
+it also exports utilities to manage a cell's metadata, specifically for
+* getting, setting or unsetting a key/value pair
+* adding, removing items in a list inside the metadata (e.g. tags)
+* cleaning the metadata for empty/useless items
+
+to that effect, see the `md_get` and similar functions
+
 ## Development
 
 See the documentation on Jlab extensions for more details; the gist of it is
 
 ### Development install
 
 ```bash
@@ -121,7 +132,24 @@
 In development mode, you will also need to remove the symlink created by `jupyter labextension develop`
 command. To find its location, you can run `jupyter labextension list` to figure out where the `labextensions`
 folder is located. Then you can remove the symlink named `jupyterlab-celltagsclasses` within that folder.
 
 ### Packaging the extension
 
 See [RELEASE](RELEASE.md)
+
+## testing
+
+### the metadata module
+
+probably suboptimal but that's my first..
+
+```terminal
+npm install -g typescript '@types/node'
+```
+
+```terminal
+rm src/*js
+tsc src/xpath*ts && node src/xpath-test.js
+```
+
+I have tried to use `ts-node` but to no avail so far
```

