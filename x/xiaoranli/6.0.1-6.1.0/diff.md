# Comparing `tmp/xiaoranli-6.0.1-py3-none-any.whl.zip` & `tmp/xiaoranli-6.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,19 @@
-Zip file size: 8622 bytes, number of entries: 17
--rw-r--r--  2.0 unx     2251 b- defN 23-Feb-08 01:56 xiaoranli/__init__.py
+Zip file size: 8713 bytes, number of entries: 17
+-rw-r--r--  2.0 unx     2158 b- defN 23-May-10 09:42 xiaoranli/__init__.py
 -rw-r--r--  2.0 unx     1920 b- defN 23-Feb-08 01:56 xiaoranli/data/rc_files/alias
 -rw-r--r--  2.0 unx       75 b- defN 22-Dec-06 01:51 xiaoranli/data/rc_files/dockerignore
 -rw-r--r--  2.0 unx      393 b- defN 22-Dec-06 01:51 xiaoranli/data/rc_files/gdbinit
 -rw-r--r--  2.0 unx      124 b- defN 23-Feb-08 01:56 xiaoranli/data/rc_files/gitconfig
 -rw-r--r--  2.0 unx      534 b- defN 22-Dec-06 01:51 xiaoranli/data/rc_files/inputrc
 -rw-r--r--  2.0 unx      903 b- defN 23-Feb-08 01:56 xiaoranli/data/rc_files/tmux.config
 -rw-r--r--  2.0 unx      356 b- defN 22-Dec-06 02:21 xiaoranli/data/rc_files/vimrc
 -rw-r--r--  2.0 unx      188 b- defN 23-Feb-08 01:56 xiaoranli/scripts/install_golang.sh
--rw-r--r--  2.0 unx     1562 b- defN 23-Feb-08 01:56 xiaoranli/scripts/install_useful_tools.sh
--rw-r--r--  2.0 unx      156 b- defN 23-Feb-08 01:56 xiaoranli/scripts/install_zsh.sh
--rw-r--r--  2.0 unx     1081 b- defN 23-Feb-08 01:58 xiaoranli-6.0.1.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      923 b- defN 23-Feb-08 01:58 xiaoranli-6.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Feb-08 01:58 xiaoranli-6.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       45 b- defN 23-Feb-08 01:58 xiaoranli-6.0.1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       10 b- defN 23-Feb-08 01:58 xiaoranli-6.0.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1467 b- defN 23-Feb-08 01:58 xiaoranli-6.0.1.dist-info/RECORD
-17 files, 12080 bytes uncompressed, 6172 bytes compressed:  48.9%
+-rw-r--r--  2.0 unx     1562 b- defN 23-Apr-20 01:26 xiaoranli/scripts/install_useful_tools.sh
+-rw-r--r--  2.0 unx      412 b- defN 23-May-10 09:38 xiaoranli/scripts/install_zsh.sh
+-rw-r--r--  2.0 unx     1081 b- defN 23-May-10 09:43 xiaoranli-6.1.0.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      923 b- defN 23-May-10 09:43 xiaoranli-6.1.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-10 09:43 xiaoranli-6.1.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       45 b- defN 23-May-10 09:43 xiaoranli-6.1.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       10 b- defN 23-May-10 09:43 xiaoranli-6.1.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1467 b- defN 23-May-10 09:43 xiaoranli-6.1.0.dist-info/RECORD
+17 files, 12243 bytes uncompressed, 6263 bytes compressed:  48.8%
```

## zipnote {}

```diff
@@ -27,26 +27,26 @@
 
 Filename: xiaoranli/scripts/install_useful_tools.sh
 Comment: 
 
 Filename: xiaoranli/scripts/install_zsh.sh
 Comment: 
 
-Filename: xiaoranli-6.0.1.dist-info/LICENSE.txt
+Filename: xiaoranli-6.1.0.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xiaoranli-6.0.1.dist-info/METADATA
+Filename: xiaoranli-6.1.0.dist-info/METADATA
 Comment: 
 
-Filename: xiaoranli-6.0.1.dist-info/WHEEL
+Filename: xiaoranli-6.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: xiaoranli-6.0.1.dist-info/entry_points.txt
+Filename: xiaoranli-6.1.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: xiaoranli-6.0.1.dist-info/top_level.txt
+Filename: xiaoranli-6.1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: xiaoranli-6.0.1.dist-info/RECORD
+Filename: xiaoranli-6.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xiaoranli/__init__.py

```diff
@@ -31,19 +31,14 @@
 
 
 def install_zsh():
     zsh_path = os.path.join(pkg_installed_path, "scripts/install_zsh.sh")
     os.system(f"bash {zsh_path}")
 
 
-def install_golang():
-    zsh_path = os.path.join(pkg_installed_path, "scripts/install_zsh.sh")
-    os.system(f"bash {zsh_path}")
-
-
 def install_packages():
     scripts_path = os.path.join(pkg_installed_path, "scripts/install_useful_tools.sh")
     os.system(f"bash -i {scripts_path}")
 
 
 def info():
     """print help info"""
@@ -63,14 +58,15 @@
 
 def main():
     fire.Fire(
         {
             "rc": setup_rc_files,
             "info": info,
             "zsh": install_zsh,
+            "setup_zshrc":setup_zshrc,
             "tools": install_packages,
         }
     )
 
 
 if __name__ == "__main__":
     main()
```

## xiaoranli/scripts/install_zsh.sh

```diff
@@ -1,4 +1,6 @@
 alias sudo='sudo env "PATH=$PATH" '
 
 sudo apt install -y zsh
-sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
+sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
+git clone https://github.com/zsh-users/zsh-syntax-highlighting.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-syntax-highlighting
+git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions
```

## Comparing `xiaoranli-6.0.1.dist-info/LICENSE.txt` & `xiaoranli-6.1.0.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `xiaoranli-6.0.1.dist-info/METADATA` & `xiaoranli-6.1.0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xiaoranli
-Version: 6.0.1
+Version: 6.1.0
 Summary: setup linux env, such as bashrc etc.
 Home-page: https://github.com/xiaoranliMS/env-setup.git
 Author: Li Xiaoran
 Author-email: 1240897116@qq.com
 Project-URL: Funding,  https://github.com/xiaoranliMS
 Project-URL: Source, https://github.com/xiaoranliMS/env-setup.git
 Keywords: env setup,development,xiaoranli
```

## Comparing `xiaoranli-6.0.1.dist-info/RECORD` & `xiaoranli-6.1.0.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-xiaoranli/__init__.py,sha256=9R0d0bDFvoYGOeFZbsfXSTehrx5C9w-wsqWCDQhwOD0,2251
+xiaoranli/__init__.py,sha256=jL0DKhEaN-jjywFbLafEpvsN5oxNbkEEbsO6UR8DVxw,2158
 xiaoranli/data/rc_files/alias,sha256=kxHI2nOHQLggc-GLAS3mgKBZXe_D54IlrYSvQOB8j3E,1920
 xiaoranli/data/rc_files/dockerignore,sha256=fNTcMXrdUU9h9Y0tkLpfQKbLhwRwaVNd-MyP-ycI3sE,75
 xiaoranli/data/rc_files/gdbinit,sha256=Om1pIhhf-_lIfLgx8Gt730W2R4vvZLr05hbgnhNy0Hs,393
 xiaoranli/data/rc_files/gitconfig,sha256=sSooqGwfXpEHUvL047wvYQOMl1zQUgN8GVWWMhRLYII,124
 xiaoranli/data/rc_files/inputrc,sha256=LBnvTQA6YANbPWZPboj8cPjf6dWwOETn-Uu24vNrqPY,534
 xiaoranli/data/rc_files/tmux.config,sha256=kk88x2Skt6csucriayhCNORaufCV8FsLMycVzEkrwHA,903
 xiaoranli/data/rc_files/vimrc,sha256=f4aZHW70bg168Rm9oY4ku9t4V1ri3DZcqzRdc2MzAyo,356
 xiaoranli/scripts/install_golang.sh,sha256=sR2H-HL-Bj6dj9bTD0apJsRLlEQaLoD0Ay5S3qUycxc,188
 xiaoranli/scripts/install_useful_tools.sh,sha256=dvomQdYawpqPtaK8iEqPbLQKAv0lEL6c0Dr7_3XAWDc,1562
-xiaoranli/scripts/install_zsh.sh,sha256=TuRcGNmCyXCQu9PGdKfXtRZcMghpGcCbmpKZYF-0JA0,156
-xiaoranli-6.0.1.dist-info/LICENSE.txt,sha256=ceC9ZJOV9H6CtQDcYmHOS46NA3dHJ_WD4J9blH513pc,1081
-xiaoranli-6.0.1.dist-info/METADATA,sha256=e3PA2Mz9RjUWGIuF50qsNVeo-uUE8SADFKHrK_esYZA,923
-xiaoranli-6.0.1.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-xiaoranli-6.0.1.dist-info/entry_points.txt,sha256=T3ZBwdXMY38i4JvMaIXq1WIMdrDEDrVkaWIgKfVsrTc,45
-xiaoranli-6.0.1.dist-info/top_level.txt,sha256=DjwPuFyAkwL8uNM0Z41wNraAt9-71lDJ8SRwYTqRRcs,10
-xiaoranli-6.0.1.dist-info/RECORD,,
+xiaoranli/scripts/install_zsh.sh,sha256=BGxPv7GsKOcOH7x6uLLVkBcKaywBY30CGmLxcK6dV0U,412
+xiaoranli-6.1.0.dist-info/LICENSE.txt,sha256=ceC9ZJOV9H6CtQDcYmHOS46NA3dHJ_WD4J9blH513pc,1081
+xiaoranli-6.1.0.dist-info/METADATA,sha256=brdq6iCQvk1ELVxZbT-A3u0ignFV49L7M1C9cnAABK4,923
+xiaoranli-6.1.0.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+xiaoranli-6.1.0.dist-info/entry_points.txt,sha256=T3ZBwdXMY38i4JvMaIXq1WIMdrDEDrVkaWIgKfVsrTc,45
+xiaoranli-6.1.0.dist-info/top_level.txt,sha256=DjwPuFyAkwL8uNM0Z41wNraAt9-71lDJ8SRwYTqRRcs,10
+xiaoranli-6.1.0.dist-info/RECORD,,
```

