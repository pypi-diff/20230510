# Comparing `tmp/hindilemmatizer-0.5.0-py3-none-any.whl.zip` & `tmp/hindilemmatizer-0.5.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 6835884 bytes, number of entries: 10
+Zip file size: 6835900 bytes, number of entries: 10
 -rw-r--r--  2.0 unx      156 b- defN 23-May-06 13:08 hindilemmatizer/__init__.py
--rw-r--r--  2.0 unx     3380 b- defN 23-May-08 17:01 hindilemmatizer/lemmatizer.py
+-rw-r--r--  2.0 unx     3465 b- defN 23-May-09 11:54 hindilemmatizer/lemmatizer.py
 -rw-r--r--  2.0 unx   555099 b- defN 23-May-08 16:44 hindilemmatizer/data/data.csv
 -rw-r--r--  2.0 unx   192237 b- defN 23-May-08 18:07 hindilemmatizer/data/direct.csv
 -rw-r--r--  2.0 unx 23623710 b- defN 23-May-08 16:44 hindilemmatizer/data/totalWords.txt
--rw-r--r--  2.0 unx     1071 b- defN 23-May-08 18:07 hindilemmatizer-0.5.0.dist-info/LICENSE
--rw-r--r--  2.0 unx      186 b- defN 23-May-08 18:07 hindilemmatizer-0.5.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-08 18:07 hindilemmatizer-0.5.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       16 b- defN 23-May-08 18:07 hindilemmatizer-0.5.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      868 b- defN 23-May-08 18:07 hindilemmatizer-0.5.0.dist-info/RECORD
-10 files, 24376815 bytes uncompressed, 6834402 bytes compressed:  72.0%
+-rw-r--r--  2.0 unx     1071 b- defN 23-May-10 00:22 hindilemmatizer-0.5.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx      186 b- defN 23-May-10 00:22 hindilemmatizer-0.5.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-10 00:22 hindilemmatizer-0.5.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       16 b- defN 23-May-10 00:22 hindilemmatizer-0.5.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      868 b- defN 23-May-10 00:22 hindilemmatizer-0.5.1.dist-info/RECORD
+10 files, 24376900 bytes uncompressed, 6834418 bytes compressed:  72.0%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: hindilemmatizer/data/direct.csv
 Comment: 
 
 Filename: hindilemmatizer/data/totalWords.txt
 Comment: 
 
-Filename: hindilemmatizer-0.5.0.dist-info/LICENSE
+Filename: hindilemmatizer-0.5.1.dist-info/LICENSE
 Comment: 
 
-Filename: hindilemmatizer-0.5.0.dist-info/METADATA
+Filename: hindilemmatizer-0.5.1.dist-info/METADATA
 Comment: 
 
-Filename: hindilemmatizer-0.5.0.dist-info/WHEEL
+Filename: hindilemmatizer-0.5.1.dist-info/WHEEL
 Comment: 
 
-Filename: hindilemmatizer-0.5.0.dist-info/top_level.txt
+Filename: hindilemmatizer-0.5.1.dist-info/top_level.txt
 Comment: 
 
-Filename: hindilemmatizer-0.5.0.dist-info/RECORD
+Filename: hindilemmatizer-0.5.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## hindilemmatizer/lemmatizer.py

```diff
@@ -71,26 +71,26 @@
     if(len(self.possibleRootWords)):
       return self.finalReturn()
     
     return self.step2()
   
   def step2(self):
     for l in range(2,len(self.word)):
-      if self.word[l:] in globalSuffixWordsSet and len(self.word[l:])>1 and self.word[:l] in totalWords:
+      if self.word[l:] in globalSuffixWordsSet and len(self.word[l:])>1 and (self.word[:l] in totalWords or self.word[:l] in globalRootWordsSet):
         self.possibleRootWords.add(WordLemmatizer(self.word[:l]).lemmatize())
 
     if(len(self.possibleRootWords)):
       return self.finalReturn()
 
-    return self.word
+    return self.step3()
 
   def step3(self):
 
     for r in range(1,len(self.inflectedWord)-1):
-      if self.word[:r] in globalPrefixWordsSet and self.word[r:] in totalWords:
+      if self.word[:r] in globalPrefixWordsSet and (self.word[r:] in totalWords or self.word[r:] in globalRootWordsSet):
         self.possibleRootWords.add(WordLemmatizer(self.word[r:]).lemmatize())
     if(len(self.possibleRootWords)):
       return self.finalReturn()
 
     return self.word
 
   def finalReturn(self):
```

## Comparing `hindilemmatizer-0.5.0.dist-info/LICENSE` & `hindilemmatizer-0.5.1.dist-info/LICENSE`

 * *Files identical despite different names*

