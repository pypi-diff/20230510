# Comparing `tmp/hindilemmatizer-0.5.2-py3-none-any.whl.zip` & `tmp/hindilemmatizer-0.5.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 6835899 bytes, number of entries: 10
+Zip file size: 6835979 bytes, number of entries: 10
 -rw-r--r--  2.0 unx      156 b- defN 23-May-06 13:08 hindilemmatizer/__init__.py
--rw-r--r--  2.0 unx     3462 b- defN 23-May-10 00:41 hindilemmatizer/lemmatizer.py
+-rw-r--r--  2.0 unx     3677 b- defN 23-May-10 01:19 hindilemmatizer/lemmatizer.py
 -rw-r--r--  2.0 unx   555099 b- defN 23-May-08 16:44 hindilemmatizer/data/data.csv
 -rw-r--r--  2.0 unx   192237 b- defN 23-May-08 18:07 hindilemmatizer/data/direct.csv
 -rw-r--r--  2.0 unx 23623710 b- defN 23-May-08 16:44 hindilemmatizer/data/totalWords.txt
--rw-r--r--  2.0 unx     1071 b- defN 23-May-10 00:41 hindilemmatizer-0.5.2.dist-info/LICENSE
--rw-r--r--  2.0 unx      186 b- defN 23-May-10 00:41 hindilemmatizer-0.5.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-10 00:41 hindilemmatizer-0.5.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       16 b- defN 23-May-10 00:41 hindilemmatizer-0.5.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      868 b- defN 23-May-10 00:41 hindilemmatizer-0.5.2.dist-info/RECORD
-10 files, 24376897 bytes uncompressed, 6834417 bytes compressed:  72.0%
+-rw-r--r--  2.0 unx     1071 b- defN 23-May-10 01:20 hindilemmatizer-0.5.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx      186 b- defN 23-May-10 01:20 hindilemmatizer-0.5.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-10 01:20 hindilemmatizer-0.5.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       16 b- defN 23-May-10 01:19 hindilemmatizer-0.5.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      868 b- defN 23-May-10 01:20 hindilemmatizer-0.5.3.dist-info/RECORD
+10 files, 24377112 bytes uncompressed, 6834497 bytes compressed:  72.0%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: hindilemmatizer/data/direct.csv
 Comment: 
 
 Filename: hindilemmatizer/data/totalWords.txt
 Comment: 
 
-Filename: hindilemmatizer-0.5.2.dist-info/LICENSE
+Filename: hindilemmatizer-0.5.3.dist-info/LICENSE
 Comment: 
 
-Filename: hindilemmatizer-0.5.2.dist-info/METADATA
+Filename: hindilemmatizer-0.5.3.dist-info/METADATA
 Comment: 
 
-Filename: hindilemmatizer-0.5.2.dist-info/WHEEL
+Filename: hindilemmatizer-0.5.3.dist-info/WHEEL
 Comment: 
 
-Filename: hindilemmatizer-0.5.2.dist-info/top_level.txt
+Filename: hindilemmatizer-0.5.3.dist-info/top_level.txt
 Comment: 
 
-Filename: hindilemmatizer-0.5.2.dist-info/RECORD
+Filename: hindilemmatizer-0.5.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## hindilemmatizer/lemmatizer.py

```diff
@@ -100,26 +100,36 @@
 
     if possibleRootWords and len(possibleRootWords[0])>2:
       return possibleRootWords[0]
 
     return self.word
 
 def sanitizeLine(line):
-  return re.sub(r'\s+', ' ', re.sub(r'[{}[\]:;?@!#$%^&*()-_\'\"<>\u0964\u0965,]', ' ', line.encode("utf-8").decode("utf-8"))).split()
+  return re.sub(r'\s+', ' ', re.sub(r'[{}[\]:;_<>?@!#$%^&*()\u0964\u0965,\']', ' ', line.encode("utf-8").decode("utf-8"))).split()
 
 def processWord(word):
 
   if word in directRoots:
     alreadyLemmatizedWords[word] = directRoots[word]
 
   if word in alreadyLemmatizedWords:
     return alreadyLemmatizedWords[word]
 
   lemma= WordLemmatizer(word).lemmatize()
   alreadyLemmatizedWords[word]=lemma
   return lemma
 
+def is_hindi_word(word):
+  hindi_pattern = re.compile(r'^[\u0900-\u097F]+$')
+  return bool(hindi_pattern.match(word))
+
 def lemmatize(line):
   # this is the function that will be called by the user to lemmatize hindi text, it can accept both word and a line
   words = sanitizeLine(line)
+  result = []
+  for word in words:
+    if is_hindi_word(word):
+      result.append(processWord(word))
+    else:
+      result.append(word)
 
-  return " ".join([processWord(word) for word in words if word])
+  return " ".join(result)
```

## Comparing `hindilemmatizer-0.5.2.dist-info/LICENSE` & `hindilemmatizer-0.5.3.dist-info/LICENSE`

 * *Files identical despite different names*

