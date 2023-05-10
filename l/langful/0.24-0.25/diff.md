# Comparing `tmp/langful-0.24-py2.py3-none-any.whl.zip` & `tmp/langful-0.25-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 7703 bytes, number of entries: 9
--rw-rw-rw-  2.0 fat     1507 b- defN 23-Apr-15 03:44 langful/__init__.py
--rw-rw-rw-  2.0 fat      478 b- defN 23-Apr-16 03:28 langful/define.py
--rw-rw-rw-  2.0 fat     1590 b- defN 23-Apr-15 03:46 langful/function.py
--rw-rw-rw-  2.0 fat    13440 b- defN 23-Apr-16 05:05 langful/lang.py
--rw-rw-rw-  2.0 fat     1064 b- defN 23-Apr-16 05:06 langful-0.24.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     2603 b- defN 23-Apr-16 05:06 langful-0.24.dist-info/METADATA
--rw-rw-rw-  2.0 fat      110 b- defN 23-Apr-16 05:06 langful-0.24.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 23-Apr-16 05:06 langful-0.24.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      679 b- defN 23-Apr-16 05:06 langful-0.24.dist-info/RECORD
-9 files, 21479 bytes uncompressed, 6549 bytes compressed:  69.5%
+Zip file size: 7937 bytes, number of entries: 9
+-rw-rw-rw-  2.0 fat     1549 b- defN 23-May-10 08:22 langful/__init__.py
+-rw-rw-rw-  2.0 fat      611 b- defN 23-Apr-26 14:01 langful/define.py
+-rw-rw-rw-  2.0 fat     2453 b- defN 23-May-10 08:11 langful/function.py
+-rw-rw-rw-  2.0 fat    13089 b- defN 23-May-10 08:07 langful/lang.py
+-rw-rw-rw-  2.0 fat     1064 b- defN 23-May-10 08:29 langful-0.25.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     2641 b- defN 23-May-10 08:29 langful-0.25.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      110 b- defN 23-May-10 08:29 langful-0.25.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 23-May-10 08:29 langful-0.25.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      679 b- defN 23-May-10 08:29 langful-0.25.dist-info/RECORD
+9 files, 22204 bytes uncompressed, 6783 bytes compressed:  69.5%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: langful/function.py
 Comment: 
 
 Filename: langful/lang.py
 Comment: 
 
-Filename: langful-0.24.dist-info/LICENSE
+Filename: langful-0.25.dist-info/LICENSE
 Comment: 
 
-Filename: langful-0.24.dist-info/METADATA
+Filename: langful-0.25.dist-info/METADATA
 Comment: 
 
-Filename: langful-0.24.dist-info/WHEEL
+Filename: langful-0.25.dist-info/WHEEL
 Comment: 
 
-Filename: langful-0.24.dist-info/top_level.txt
+Filename: langful-0.25.dist-info/top_level.txt
 Comment: 
 
-Filename: langful-0.24.dist-info/RECORD
+Filename: langful-0.25.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## langful/__init__.py

```diff
@@ -33,34 +33,34 @@
 ```python
 import langful
 
 Text = langful.lang()
 
 print( Text.language_dict )
 
-print( Text.replace( "%hi%" , lang_str = "zh_cn" ) )
+print( Text.str_replace( "%hi%" , lang_str = "zh_cn" ) )
 
-print( Text.replace( "!hi!" , lang_str = "zh_cn" , change = "!" ) )
+print( Text.str_replace( "!hi!" , lang_str = "zh_cn" , change = "!" ) )
 
-print( Text.replace( "%welcome%" , lang_str = "zh_cn" ) )
+print( Text.str_replace( "%welcome%" , lang_str = "zh_cn" ) )
 
-print( Text.replace( "!welcome!" , lang_str = "zh_cn" , change = "!" ) )
+print( Text.str_replace( "!welcome!" , lang_str = "zh_cn" , change = "!" ) )
 
-print( Text.replace( "%hi%" , lang_str = "en_us" ) )
+print( Text.str_replace( "%hi%" , lang_str = "en_us" ) )
 
-print( Text.replace( "!hi!" , lang_str = "en_us" , change = "!" ) )
+print( Text.str_replace( "!hi!" , lang_str = "en_us" , change = "!" ) )
 
-print( Text.replace( "%welcome%" , lang_str = "en_us" ) )
+print( Text.str_replace( "%welcome%" , lang_str = "en_us" ) )
 
-print( Text.replace( "!welcome!" , lang_str = "en_us" , change = "!" ) )
+print( Text.str_replace( "!welcome!" , lang_str = "en_us" , change = "!" ) )
 
 print( )
 
-print( Text.replace( "%%" ) )
-print( Text.replace( "!!" , change = "!" ) )
+print( Text.str_replace( "%%" ) )
+print( Text.str_replace( "!!" , change = "!" ) )
 ```
 
 ## Output
 
 ```python
 {'en_us': {'welcome': 'Welcome', 'hi': 'Hi'}, 'zh_cn': {'welcome': '欢迎', 'hi': '你好'}}
 你好
@@ -86,8 +86,8 @@
 """
 
 # 'lang' object
 from langful.lang import *
 # Some function for 'langful'
 from langful.function import *
 # define
-from langful.define import *
+from langful.define import *
```

## langful/define.py

```diff
@@ -8,19 +8,29 @@
 
 FILE = "file"
 DICT = "dict"
 # encode/decode
 UTF8 = "utf-8"
 
 def join( args : list ) -> str :
+    """
+    # "".join( )
+    """
     return "".join( args )
 
 def range_len( obj ) -> list :
+    """
+    # range( len( ) )
+    """
     return list( range( len( obj ) ) )
 
 def get_type( obj ) -> str :
+    """
+    # get type
+    # 获取类型
+    """
     if isinstance( obj , str ) :
         return FILE
     elif isinstance( obj , dict ) :
         return DICT
     else :
-        raise TypeError(f"can't use type { type( obj ) }")
+        raise TypeError(f"can't use type { type( obj ) }")
```

### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

## langful/function.py

```diff
@@ -1,35 +1,42 @@
 """
 # function
 """
-from langful.__init__ import *
 
 def if_then( text : str = "" , replace = "" , change : str = "%" , else_replace : str = "" ) -> str :
     """
     # 'if_then' function
     ---
     If the Boolean value of a particular item is true or false
 
     then replace it for the str or list
 
     ---
     text: the text
+
     replace: give str or list for replace the text
+
     change: Specifies what character to use for substitution , default is '%'
+
     else_replace: if it was not , then use it to replace
+
     ---
     如果某个特定项的布尔值为真或假
     
     那么替换为对应的字符串或列表
 
     ---
     text: 文本
+
     replace: 给一个字符串或列表 来替换文本
+
     change: 选择用什么符号做替换 默认为'%'
+
     else_replace: 如果为否 那么用这个来做替换
+
     ---
     """
     i , p = 0 , 0
     Ret = ""
     text = "".join( text ).split( change )
     for I in text :
         if i % 2 :
@@ -46,7 +53,46 @@
             else :
                 Ret += else_replace # 否则就使用 else_replace 变量中的字符串做替换
         else :
             Ret += I
         i += 1
     return Ret
 
+def to_json( lang : str ) :
+    """
+    # 'to_json' function
+    from .lang file to .json file
+
+    ---
+
+    把lang文件转换为json文件
+    """
+    ret={}
+    lang = lang.split("\n")
+    for i in lang :
+        I=i.split("#")[0]#移除注释
+        I=I.split("=")
+        if len(I) == 2 :
+            key , value = I
+            if value[0] == " " :
+                value = value[1:]
+            if key[-1] == " " :
+                key = key[:-1]
+            ret[key]=value
+    return ret
+
+def to_lang( dict : dict ) :
+    """
+    # 'to_lang' function
+    from .json file to .lang file
+
+    ---
+
+    把json文件转换为lang文件
+    """
+    ret = ""
+    for key , value in dict.items() :
+        if isinstance( value , str ) :
+            ret += f"{key} = {value}\n"
+        else :
+            raise TypeError( "" )
+    return ret
```

## langful/lang.py

```diff
@@ -2,16 +2,16 @@
 # lang
 """
 import traceback
 import locale
 import json
 import os
 
-from langful.__init__ import *
 from langful.define import *
+from langful.function import to_json , to_lang
 
 class lang :
 
     def __init__( self , lang_dir = "lang" , default_lang : str = "en_us" , file_type : str = JSON , change : str = "%" ) -> None :
         """
         # lang object
 
@@ -61,29 +61,23 @@
                 lang_file = default_lang + file_suffix
 
             for filename in os.listdir( lang_dir ): # 尝试加载所有能加载的模块
                 if len( filename ) > file_suffix_len and filename[ -file_suffix_len: ] == file_suffix :
                     try :
                         with open( os.path.join( lang_dir , filename ) , encoding = UTF8 ) as file :
                             if file_type == JSON :
-                                l = json.load( file ) # 直接加载JSON文件
+                                loaded_lang_file = json.load( file ) # 直接加载JSON文件
                             elif file_type == LANG :
-                                l = {}
-                                for i in file.read().split( "\n" ) : # 去换行
-                                    if i :
-                                        k , v = i.split( "=" ) # 键 = 值
-                                        if v and v[0] == " " : # 去空格
-                                            v = v[ 1: ]
-                                        l[ join( k.split() ) ] = v
+                                loaded_lang_file = to_json( file.read() )
                             else :
                                 raise TypeError( f"can't use type '{file_type}'" )
-                        language_dict[ filename[ :-file_suffix_len ] ] = l # 加载文件
+                        language_dict[ filename[ :-file_suffix_len ] ] = loaded_lang_file # 加载文件
                         lang_file_list.append( filename )
-                    except Exception as e :
-                        print( f"{e}\n" )
+                    except Exception as error :
+                        print( f"{error}\n" )
                         traceback.print_exc()
 
         elif self.type == DICT :
             use_locale = default_lang
             if default_lang not in lang_dir :
                 raise KeyError( f"'{default_lang}' not find" )
             if default_locale in lang_dir :
@@ -154,30 +148,28 @@
         to save all lang file
 
         ---
 
         保存所有lang文件
         """
         if self.type == FILE :
-            for k , v in self.language_dict.items() :
+            for key , value in self.language_dict.items() :
                 try :
-                    with open( os.path.join( self.lang_dir , k + self.file_suffix ) , "w+" , encoding = UTF8 ) as file :
+                    with open( os.path.join( self.lang_dir , key + self.file_suffix ) , "w+" , encoding = UTF8 ) as file :
                         if self.file_type == JSON :
-                            file.write( json.dumps( v , indent = 4 , separators = ( " ," , ": " ) , ensure_ascii = False ) )
+                            file.write( json.dumps( value , indent = 4 , separators = ( " ," , ": " ) , ensure_ascii = False ) )
                         elif self.file_type == LANG :
-                            for i_k , i_v in v.items() :
-                                s = f"{i_k} = {i_v}\n"
-                                file.write( s )
-                except Exception as e :
-                    print( f"{e}\n" )
+                            file.write( to_lang( value ) )
+                except Exception as error :
+                    print( f"{error}\n" )
                     traceback.print_exc()
         else :
             raise TypeError( f"{self.type} can't to save" )
 
-    def get( self , key:str , lang_str:str = None ) -> str : # 输入键 获取对应的值
+    def get( self , key : str , lang_str : str = None ) -> str : # 输入键 获取对应的值
         """
 
         # get
 
         Get one value in some one dictionary
 
         在某个字典中获取一个值
@@ -199,15 +191,14 @@
             lang_str = self.use_locale
 
         if lang_str in self.lang_str_list :
             if key in self.language_dict[ lang_str ] :
                 return self.language_dict[ lang_str ] [ key ]
             else :
                 raise KeyError( f"key '{key}' has not in dictionary!" )
-            
         else :
             raise KeyError( f"lang '{lang_str}' has not find!" )
 
     def set( self , key : str , value : str , lang_str : str = None ) -> None : # 设置某个键值
         """
 
         Set one value with one key in some one dictionary
@@ -393,20 +384,20 @@
             change = self.change
 
         i = 0
         ret = ""
         text = join( args ).split( change )
         language = self._lang_str_to_language( lang_str )
 
-        for I in text :
+        for split_text in text :
             if i % 2 :
-                if I in language :
-                    ret += language[I]
-                elif not I :
+                if split_text in language :
+                    ret += language[split_text]
+                elif not split_text :
                     ret += change
                 else :
-                    raise KeyError( f"key '{I}' has not find!" )
+                    raise KeyError( f"key '{split_text}' has not find!" )
             else :
-                ret += I
+                ret += split_text
             i += 1
 
-        return ret
+        return ret
```

## Comparing `langful-0.24.dist-info/LICENSE` & `langful-0.25.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `langful-0.24.dist-info/METADATA` & `langful-0.25.dist-info/METADATA`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langful
-Version: 0.24
+Version: 0.25
 Home-page: https://github.com/cueavyqwp/langful
 Author: cueavyqwp
 Author-email: cueavyqwp@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: > 3.6
@@ -25,15 +25,14 @@
     </a>
     <a href="https://github.com/cueavyqwp/langful">
         <img alt="Github stars" src="https://img.shields.io/github/stars/cueavyqwp/langful?color=blue">
     </a>
     <a href="https://github.com/cueavyqwp/langful">
         <img alt="Github issues" src="https://img.shields.io/github/issues/cueavyqwp/langful?color=blue">
     </a>
-
 </p>
 
 # install
 
 Use `pip` to install `pip install langful` or `pip3 install langful`
 
 # example
@@ -66,34 +65,34 @@
 ```python
 import langful
 
 Text = langful.lang()
 
 print( Text.language_dict )
 
-print( Text.replace( "%hi%" , lang_str = "zh_cn" ) )
+print( Text.str_replace( "%hi%" , lang_str = "zh_cn" ) )
 
-print( Text.replace( "!hi!" , lang_str = "zh_cn" , change = "!" ) )
+print( Text.str_replace( "!hi!" , lang_str = "zh_cn" , change = "!" ) )
 
-print( Text.replace( "%welcome%" , lang_str = "zh_cn" ) )
+print( Text.str_replace( "%welcome%" , lang_str = "zh_cn" ) )
 
-print( Text.replace( "!welcome!" , lang_str = "zh_cn" , change = "!" ) )
+print( Text.str_replace( "!welcome!" , lang_str = "zh_cn" , change = "!" ) )
 
-print( Text.replace( "%hi%" , lang_str = "en_us" ) )
+print( Text.str_replace( "%hi%" , lang_str = "en_us" ) )
 
-print( Text.replace( "!hi!" , lang_str = "en_us" , change = "!" ) )
+print( Text.str_replace( "!hi!" , lang_str = "en_us" , change = "!" ) )
 
-print( Text.replace( "%welcome%" , lang_str = "en_us" ) )
+print( Text.str_replace( "%welcome%" , lang_str = "en_us" ) )
 
-print( Text.replace( "!welcome!" , lang_str = "en_us" , change = "!" ) )
+print( Text.str_replace( "!welcome!" , lang_str = "en_us" , change = "!" ) )
 
 print( )
 
-print( Text.replace( "%%" ) )
-print( Text.replace( "!!" , change = "!" ) )
+print( Text.str_replace( "%%" ) )
+print( Text.str_replace( "!!" , change = "!" ) )
 ```
 
 ## Output
 
 ```python
 {'en_us': {'welcome': 'Welcome', 'hi': 'Hi'}, 'zh_cn': {'welcome': '欢迎', 'hi': '你好'}}
 你好
```

### html2text {}

```diff
@@ -1,24 +1,25 @@
-Metadata-Version: 2.1 Name: langful Version: 0.24 Home-page: https://
+Metadata-Version: 2.1 Name: langful Version: 0.25 Home-page: https://
 github.com/cueavyqwp/langful Author: cueavyqwp Author-email:
 cueavyqwp@outlook.com Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Requires-Python: > 3.6 Description-Content-Type: text/
 markdown License-File: LICENSE # langful
    [PyPI_version] [Python_version] [license] [Github_stars] [Github_issues]
 # install Use `pip` to install `pip install langful` or `pip3 install langful`
 # example - test.py - lang - zh_cn.json - en_us.json ## zh_cn.json ```json
 { "hi" : "ä½ å¥½" , "welcome" : "æ¬¢è¿" } ``` ## en_us.json ```json { "hi" :
 "Hi" , "welcome" : "Welcome" } ``` ## tset.py ```python import langful Text =
-langful.lang() print( Text.language_dict ) print( Text.replace( "%hi%" ,
-lang_str = "zh_cn" ) ) print( Text.replace( "!hi!" , lang_str = "zh_cn" ,
-change = "!" ) ) print( Text.replace( "%welcome%" , lang_str = "zh_cn" ) )
-print( Text.replace( "!welcome!" , lang_str = "zh_cn" , change = "!" ) ) print
-( Text.replace( "%hi%" , lang_str = "en_us" ) ) print( Text.replace( "!hi!" ,
-lang_str = "en_us" , change = "!" ) ) print( Text.replace( "%welcome%" ,
-lang_str = "en_us" ) ) print( Text.replace( "!welcome!" , lang_str = "en_us" ,
-change = "!" ) ) print( ) print( Text.replace( "%%" ) ) print( Text.replace
-( "!!" , change = "!" ) ) ``` ## Output ```python {'en_us': {'welcome':
-'Welcome', 'hi': 'Hi'}, 'zh_cn': {'welcome': 'æ¬¢è¿', 'hi': 'ä½ å¥½'}} ä½ å¥½
-ä½ å¥½ æ¬¢è¿ æ¬¢è¿ Hi Hi Welcome Welcome % ! ``` # About github: https://
-github.com/cueavyqwp/langful pypi: https://pypi.org/project/langful issues:
-https://github.com/cueavyqwp/langful/issues
+langful.lang() print( Text.language_dict ) print( Text.str_replace( "%hi%" ,
+lang_str = "zh_cn" ) ) print( Text.str_replace( "!hi!" , lang_str = "zh_cn" ,
+change = "!" ) ) print( Text.str_replace( "%welcome%" , lang_str = "zh_cn" ) )
+print( Text.str_replace( "!welcome!" , lang_str = "zh_cn" , change = "!" ) )
+print( Text.str_replace( "%hi%" , lang_str = "en_us" ) ) print
+( Text.str_replace( "!hi!" , lang_str = "en_us" , change = "!" ) ) print
+( Text.str_replace( "%welcome%" , lang_str = "en_us" ) ) print
+( Text.str_replace( "!welcome!" , lang_str = "en_us" , change = "!" ) ) print
+( ) print( Text.str_replace( "%%" ) ) print( Text.str_replace( "!!" , change =
+"!" ) ) ``` ## Output ```python {'en_us': {'welcome': 'Welcome', 'hi': 'Hi'},
+'zh_cn': {'welcome': 'æ¬¢è¿', 'hi': 'ä½ å¥½'}} ä½ å¥½ ä½ å¥½ æ¬¢è¿ æ¬¢è¿ Hi
+Hi Welcome Welcome % ! ``` # About github: https://github.com/cueavyqwp/langful
+pypi: https://pypi.org/project/langful issues: https://github.com/cueavyqwp/
+langful/issues
```

## Comparing `langful-0.24.dist-info/RECORD` & `langful-0.25.dist-info/RECORD`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-langful/__init__.py,sha256=acMlfNAB_D7hO1g0oOQ3DaR6HIHtAcOoreZtRZofFVg,1507
-langful/define.py,sha256=rpCzASHLkAcVdxBjamux4emXHWBquNbmxKT2vpOZseQ,478
-langful/function.py,sha256=PgMc6q1w9m1LogCGLMz8F2uUc7DVZ_jrUSUQ035X0Lg,1590
-langful/lang.py,sha256=bnGsvF_PQMhum28aLjfJoW71KMref17GxhB4ytdwQVo,13440
-langful-0.24.dist-info/LICENSE,sha256=wtOXhcoLntZcyZBfSBI51OyCoeuHjed_JMZTnGOL3IY,1064
-langful-0.24.dist-info/METADATA,sha256=J_JUJzks8v9ASDdfEoQ7QX80KE3Ky1e6dN2Snch46Uw,2603
-langful-0.24.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
-langful-0.24.dist-info/top_level.txt,sha256=EkKV_WnIZfE3A6EhWwDIt2uwZhMVHWXTUueKJL6K15w,8
-langful-0.24.dist-info/RECORD,,
+langful/__init__.py,sha256=gWLqEkz8uaZ6JRGvEN97xOeBQOOoSZqIZyMLhgyp0sY,1549
+langful/define.py,sha256=yP9jBssIuO6Z6cYogFKHiRgx3bw7tJajEB8GBYucwC8,611
+langful/function.py,sha256=a_xEfPyycooj2HKjlbLVIG_ZCcJ_uCk9QLHP9odXQvI,2453
+langful/lang.py,sha256=A7HO3Mqo29tGetEVieaotuRvQEhHCeIWGVq-P24WwYI,13089
+langful-0.25.dist-info/LICENSE,sha256=wtOXhcoLntZcyZBfSBI51OyCoeuHjed_JMZTnGOL3IY,1064
+langful-0.25.dist-info/METADATA,sha256=Y19vCBSx2AE1sD3rFmYFl8n6OkM6j9CI9D-0Dg85Wkw,2641
+langful-0.25.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
+langful-0.25.dist-info/top_level.txt,sha256=EkKV_WnIZfE3A6EhWwDIt2uwZhMVHWXTUueKJL6K15w,8
+langful-0.25.dist-info/RECORD,,
```

