# Comparing `tmp/prev_gen-1.5.0-py3-none-any.whl.zip` & `tmp/prev_gen-2.0.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 35949 bytes, number of entries: 8
--rw-rw-rw-  2.0 fat       90 b- defN 23-Apr-05 16:57 prev_gen/__init__.py
+Zip file size: 70969 bytes, number of entries: 8
+-rw-rw-rw-  2.0 fat      102 b- defN 23-May-10 10:44 prev_gen/__init__.py
 -rw-rw-rw-  2.0 fat     1340 b- defN 23-Feb-11 16:01 prev_gen/example.txt
--rw-rw-rw-  2.0 fat    42233 b- defN 23-Apr-05 18:16 prev_gen/main.py
--rw-rw-rw-  2.0 fat    47132 b- defN 23-Jan-21 12:22 prev_gen/renogare.ttf
--rw-rw-rw-  2.0 fat     2439 b- defN 23-Apr-05 18:16 prev_gen-1.5.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-05 18:16 prev_gen-1.5.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 23-Apr-05 18:16 prev_gen-1.5.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      606 b- defN 23-Apr-05 18:16 prev_gen-1.5.0.dist-info/RECORD
-8 files, 93941 bytes uncompressed, 34901 bytes compressed:  62.8%
+-rw-rw-rw-  2.0 fat    46673 b- defN 23-May-10 13:17 prev_gen/main.py
+-rw-rw-rw-  2.0 fat   125452 b- defN 22-Sep-22 05:27 prev_gen/nunito.ttf
+-rw-rw-rw-  2.0 fat     2471 b- defN 23-May-10 13:19 prev_gen-2.0.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-10 13:19 prev_gen-2.0.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 23-May-10 13:19 prev_gen-2.0.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      606 b- defN 23-May-10 13:19 prev_gen-2.0.0.dist-info/RECORD
+8 files, 176745 bytes uncompressed, 69925 bytes compressed:  60.4%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: prev_gen/example.txt
 Comment: 
 
 Filename: prev_gen/main.py
 Comment: 
 
-Filename: prev_gen/renogare.ttf
+Filename: prev_gen/nunito.ttf
 Comment: 
 
-Filename: prev_gen-1.5.0.dist-info/METADATA
+Filename: prev_gen-2.0.0.dist-info/METADATA
 Comment: 
 
-Filename: prev_gen-1.5.0.dist-info/WHEEL
+Filename: prev_gen-2.0.0.dist-info/WHEEL
 Comment: 
 
-Filename: prev_gen-1.5.0.dist-info/top_level.txt
+Filename: prev_gen-2.0.0.dist-info/top_level.txt
 Comment: 
 
-Filename: prev_gen-1.5.0.dist-info/RECORD
+Filename: prev_gen-2.0.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## prev_gen/__init__.py

```diff
@@ -1 +1 @@
-from prev_gen.main import GUI, Reverse, Preview, Table, Field, Distance, Settings, Color
+from prev_gen.main import GUI, Reverse, PreviewSVG, Preview, Table, Field, Distance, Settings, Color
```

## prev_gen/main.py

```diff
@@ -1,12 +1,14 @@
 from __future__ import annotations
-import colorsys
 import os.path
-from math import pow, sqrt, floor
+import colorsys
+import urllib.error
+import drawsvg as svg
 from dataclasses import dataclass
+from math import pow, sqrt, floor
 from PIL import Image, ImageDraw, ImageFont
 from typing import Optional, NamedTuple, Literal, Callable
 
 # some type aliases depend on the presence of classes
 # they are declared below their dependencies, spread throughout the file
 
 # used for normalized color representations
@@ -714,16 +716,19 @@
 
 @dataclass(kw_only=True, slots=True)
 class Settings:
     """
     Image generation settings
 
     Attributes:
-        file_name:         File name to save into (no extension - png)
-        font:              Font used (no extension - true type) if none, will use bundled
+        file_name:         File name to save into (no extension, png)
+        font_name:
+            for png = local file name (no extension, true type),
+            for svg = Google Font name
+        font_opts:         Google Fonts API options (for svg)
         grid_height:       Height of each individual color tile
         grid_width:        Width of each individual color tile
         bar_height:        Height of the darkened bar at the bottom of each tile
         name_offset:       Vertical offset of the color name printed within the tile
         hex_offset:        Vertical offset of the hex value printed below color name
         hex_offset_noname: Vertical offset of the hex value printed if no name given
         desc_offset_x:     Horizontal offset of the corner descriptions
@@ -732,15 +737,16 @@
         hex_size:          Text size of the hex value printed under the color name
         hex_size_noname:   Text size of the hex value printed if no name given
         desc_size:         Text size of the corner descriptions
         bar_col_fn:        Function to determine bar color from background color
         text_col_fn:       Function to determine text color from background color
     """
     file_name: str = 'result'
-    font: Optional[str] = None
+    font_name: Optional[str] = None
+    font_opts: Optional[dict] = None
     grid_height: int = 168
     grid_width: int = 224
     bar_height: int = 10
     name_offset: int = -10
     hex_offset: int = 35
     hex_offset_noname: int = 0
     desc_offset_x: int = 15
@@ -905,15 +911,15 @@
         )
 
 
 class Preview:
     """A wrapper for the main function to allow simpler usage"""
     def __new__(_,
                 palette: u1 | u2,
-                show: bool = False,
+                show: bool = True,
                 save: bool = False
                 ) -> Image:
         """
         Parameters:
             palette: The palette of colors to generate an image for
             show:    Whether to display the generated image
             save:    Whether to save the generated palette
@@ -921,31 +927,30 @@
         Returns:
             (PIL.Image) the created image
         """
         t = Table(palette)
         s = t.settings
         img = Image.new('RGBA', t.size)
         draw = ImageDraw.Draw(img)
-        if s.font is None:
+        if s.font_name is None:
             from inspect import currentframe, getabsfile
-            font = os.path.dirname(getabsfile(currentframe())) + '/renogare.ttf'
+            font = os.path.dirname(getabsfile(currentframe())) + '/nunito.ttf'
         else:
-            font = s.font + '.ttf'
-        png = s.file_name + '.png'
+            font = s.font_name + '.ttf'
         for i in t:
             l, t = i.pos
             w, h = i.size
             col = i.col
             bg_col = col.rgb_d
             bar_col = s.bar_col_fn(col).rgb_d
             text_col = s.text_col_fn(col).rgb_d
             draw.rectangle(
                 (
                     (l, t),
-                    (l + w, t + h)
+                    (l + w, t + h - s.bar_height - 1)
                 ),
                 fill=bg_col
             )
             draw.rectangle(
                 (
                     (l, t + h - s.bar_height),
                     (l + w, t + h)
@@ -988,37 +993,148 @@
                     (l + w - 1 - s.desc_offset_x, t + s.desc_offset_y),
                     col.desc_right,
                     font=ImageFont.truetype(font, size=s.desc_size),
                     fill=text_col,
                     anchor='rt'
                 )
         if save:
-            img.save(png)
+            img.save(s.file_name+'.png')
         if show:
             if not save:
                 img.show()
             else:
                 # a hacky system-agnostic way to try to open the image
                 # unlike what the name suggests, it will try to use native apps as well
                 from webbrowser import open
-                open(png)
+                open(s.file_name+'.png')
         return img
 
 
+class PreviewSVG:
+    """A wrapper for the main function to allow simpler usage"""
+    def __new__(_,
+                palette: u1 | u2,
+                show: bool = True,
+                save: bool = False
+                ) -> Image:
+        """
+        Parameters:
+            palette: The palette of colors to generate an image for
+            show:    Whether to display the generated image
+            save:    Whether to save the generated palette
+
+        Returns:
+            (drawsvg.Drawing) the created image
+        """
+        t = Table(palette)
+        s = t.settings
+        draw = svg.Drawing(*t.size, origin=(0, 0), id_prefix='prevgen')
+        font_name = s.font_name or 'Nunito'
+        font_opts = s.font_opts or {'wght': 700}
+        if 'wght' in font_opts:
+            draw.append_css('text{font-weight:'+str(font_opts['wght'])+';}')
+        # embed google font in svg for correct previews
+        try:
+            draw.embed_google_font(font_name, **font_opts)
+        except urllib.error.HTTPError:
+            print(f'\033[31;1mError: \'{font_name}\' with opts \'{font_opts}\' is not available in Google Fonts')
+            exit(1)
+        for i in t:
+            l, t = i.pos
+            w, h = i.size
+            col = i.col
+            bg_col = col.hex
+            bar_col = s.bar_col_fn(col).hex
+            text_col = s.text_col_fn(col).hex
+            draw.append(svg.Rectangle(
+                l, t,
+                w + 1, h - s.bar_height + 1,
+                fill=bg_col
+            ))
+            draw.append(svg.Rectangle(
+                l, t + h - s.bar_height + 1,
+                w + 1, s.bar_height,
+                fill=bar_col
+            ))
+            if col.name is not None:
+                draw.append(svg.Text(
+                    col.name,
+                    x=l + w / 2,
+                    y=t + h / 2 + s.name_offset,
+                    fill=text_col,
+                    center=True,
+                    font_size=s.name_size,
+                    font_family=font_name
+                ))
+                draw.append(svg.Text(
+                    col.hex,
+                    x=l + w / 2,
+                    y=t + h / 2 + s.hex_offset,
+                    fill=text_col,
+                    center=True,
+                    font_size=s.hex_size,
+                    font_family=font_name
+                ))
+            else:
+                draw.append(svg.Text(
+                    col.hex,
+                    x=l + w / 2,
+                    y=t + h / 2 + s.hex_offset_noname,
+                    fill=text_col,
+                    center=True,
+                    font_size=s.hex_size_noname,
+                    font_family=font_name
+                ))
+            if col.desc_left is not None:
+                draw.append(svg.Text(
+                    col.desc_left,
+                    x=l + s.desc_offset_x,
+                    y=t + s.desc_size/2 + s.desc_offset_y,
+                    center=True,
+                    text_anchor='start',
+                    fill=text_col,
+                    font_size=s.desc_size,
+                    font_family=font_name
+                ))
+            if col.desc_right is not None:
+                draw.append(svg.Text(
+                    col.desc_right,
+                    x=l + w - 1 - s.desc_offset_x,
+                    y=t + s.desc_size/2 + s.desc_offset_y,
+                    center=True,
+                    text_anchor='end',
+                    fill=text_col,
+                    font_size=s.desc_size,
+                    font_family=font_name
+                ))
+        draw.save_svg(s.file_name + '.svg')
+        if show:
+            # a hacky system-agnostic way to try to open the image
+            # unlike what the name suggests, it will try to use native apps as well
+            from webbrowser import open
+            from time import sleep
+            open(s.file_name + '.svg')
+            sleep(1)
+        # had to save temporarily to display in browser, remove if user did not intend to keep the file
+        if not save:
+            os.remove(s.file_name + '.svg')
+        return draw
+
+
 class Reverse:
     def __new__(_,
                 image: Image | str,
                 changes: tuple[int, int] = (0, 1)
                 ) -> u2:
         """
         Takes an image and returns the palette used to generate it
         Supports one bit of transparency
 
         Parameters:
-            image: The image generated with this tool (or compatible)
+            image: The image generated with this tool (png) (or compatible)
             changes: The amount of color changes in the x/y axis to ignore per tile (for the darker bar)
 
         Returns:
             the palette as a Python list
         """
         if isinstance(image, str):
             image = Image.open(image).convert('RGBA')
```

## Comparing `prev_gen-1.5.0.dist-info/METADATA` & `prev_gen-2.0.0.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prev-gen
-Version: 1.5.0
+Version: 2.0.0
 Summary: Create a palette preview image by using a simple config file
 Home-page: https://github.com/Aonodensetsu/prev_gen
 Author: Remigiusz Dończyk
 Author-email: aonodensetsu@aonodensetsu.me
 License: GPL-3.0
 Keywords: palette,preview,generator,image
 Classifier: Development Status :: 5 - Production/Stable
@@ -14,19 +14,20 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Artistic Software
 Classifier: Topic :: Multimedia :: Graphics :: Presentation
 Classifier: Typing :: Typed
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: pillow
+Requires-Dist: drawsvg (~=2.0)
 
 ## Create a palette preview image by using a simple config file
 
 ![size](https://img.shields.io/github/repo-size/aonodensetsu/prev_gen?label=size) ![files](https://img.shields.io/github/directory-file-count/aonodensetsu/prev_gen) ![lines](https://img.shields.io/tokei/lines/github/aonodensetsu/prev_gen)   
-![py dep](https://img.shields.io/pypi/pyversions/prev-gen) [![version](https://img.shields.io/pypi/v/prev-gen)](https://pypi.org/project/prev-gen/1.5.0/)  
+![py dep](https://img.shields.io/pypi/pyversions/prev-gen) [![version](https://img.shields.io/pypi/v/prev-gen)](https://pypi.org/project/prev-gen/2.0.0/)  
 ![license](https://img.shields.io/pypi/l/prev-gen) [![downloads](https://img.shields.io/badge/releases-here-green?logo=pypi)](https://pypi.org/project/prev-gen/#history)  
 [![downloads](https://img.shields.io/badge/wiki-here-pink)](https://github.com/Aonodensetsu/prev_gen/blob/main/WIKI.md) [![downloads](https://img.shields.io/badge/changelog-here-pink)](https://github.com/Aonodensetsu/prev_gen/blob/main/CHANGELOG.md)  
 
 # Usage:
 1. `pip install prev_gen`
 2. Open up [the wiki](https://github.com/Aonodensetsu/prev_gen/blob/main/WIKI.md) to see how everything works
 3. Create a file based on instructions (or just edit [the example](https://github.com/Aonodensetsu/prev_gen/blob/main/example.py))
```

