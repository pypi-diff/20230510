# Comparing `tmp/AISAPLibrary-1.0.2.tar.gz` & `tmp/AISAPLibrary-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\Annas\SAP Modified\Build Wheel\dist\.tmp-wblm96e5\AISAPLibrary-1.0.2.tar", last modified: Fri Mar 10 07:30:33 2023, max compression
+gzip compressed data, was "D:\Annas\SAP Modified\Build Wheel\AISAPLibrary\dist\.tmp-w_o5yutk\AISAPLibrary-1.0.3.tar", last modified: Wed Mar 29 03:18:19 2023, max compression
```

## Comparing `AISAPLibrary-1.0.2.tar` & `AISAPLibrary-1.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-03-10 07:30:33.000000 AISAPLibrary-1.0.2/
--rw-rw-rw-   0        0        0      315 2023-03-10 07:30:33.000000 AISAPLibrary-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      524 2023-03-10 07:29:50.000000 AISAPLibrary-1.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-03-10 07:30:33.000000 AISAPLibrary-1.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-03-10 07:30:33.000000 AISAPLibrary-1.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-03-10 07:30:33.000000 AISAPLibrary-1.0.2/src/AISAPLibrary/
--rw-rw-rw-   0        0        0    40670 2023-03-10 07:28:49.000000 AISAPLibrary-1.0.2/src/AISAPLibrary/AISAPLibrary.py
--rw-rw-rw-   0        0        0       38 2023-03-10 02:17:15.000000 AISAPLibrary-1.0.2/src/AISAPLibrary/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-10 07:30:33.000000 AISAPLibrary-1.0.2/src/AISAPLibrary.egg-info/
--rw-rw-rw-   0        0        0      315 2023-03-10 07:30:33.000000 AISAPLibrary-1.0.2/src/AISAPLibrary.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      275 2023-03-10 07:30:33.000000 AISAPLibrary-1.0.2/src/AISAPLibrary.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-10 07:30:33.000000 AISAPLibrary-1.0.2/src/AISAPLibrary.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-03-10 07:30:33.000000 AISAPLibrary-1.0.2/src/AISAPLibrary.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-03-10 07:30:33.000000 AISAPLibrary-1.0.2/src/AISAPLibrary.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-03-29 03:18:19.000000 AISAPLibrary-1.0.3/
+-rw-rw-rw-   0        0        0      315 2023-03-29 03:18:19.000000 AISAPLibrary-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      448 2023-03-13 07:56:31.000000 AISAPLibrary-1.0.3/README.md
+-rw-rw-rw-   0        0        0      487 2023-03-29 03:17:45.000000 AISAPLibrary-1.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-03-29 03:18:19.000000 AISAPLibrary-1.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-03-29 03:18:19.000000 AISAPLibrary-1.0.3/src/
+drwxrwxrwx   0        0        0        0 2023-03-29 03:18:19.000000 AISAPLibrary-1.0.3/src/AISAPLibrary/
+-rw-rw-rw-   0        0        0    42620 2023-03-29 03:17:02.000000 AISAPLibrary-1.0.3/src/AISAPLibrary/AISAPLibrary.py
+-rw-rw-rw-   0        0        0       38 2023-03-10 07:38:40.000000 AISAPLibrary-1.0.3/src/AISAPLibrary/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-29 03:18:19.000000 AISAPLibrary-1.0.3/src/AISAPLibrary.egg-info/
+-rw-rw-rw-   0        0        0      315 2023-03-29 03:18:19.000000 AISAPLibrary-1.0.3/src/AISAPLibrary.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      246 2023-03-29 03:18:19.000000 AISAPLibrary-1.0.3/src/AISAPLibrary.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-03-29 03:18:19.000000 AISAPLibrary-1.0.3/src/AISAPLibrary.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-03-29 03:18:19.000000 AISAPLibrary-1.0.3/src/AISAPLibrary.egg-info/top_level.txt
```

### Comparing `AISAPLibrary-1.0.2/src/AISAPLibrary/AISAPLibrary.py` & `AISAPLibrary-1.0.3/src/AISAPLibrary/AISAPLibrary.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import pythoncom
 import win32com.client
 import time
 from pythoncom import com_error
 import robot.libraries.Screenshot as screenshot
 import os
 from robot.api import logger
-from subprocess import check_output,call
+from subprocess import check_output,Popen
 
 class AISAPLibrary:
     """The SapGuiLibrary is a library that enables users to create tests for the Sap Gui application
 
     The library uses the Sap Scripting Engine, therefore Scripting must be enabled in Sap in order for this library to work.
 
     = Opening a connection / Before running tests =
@@ -795,45 +795,86 @@
         except:
             pass
         
         try:
             self.click_element('wnd[1]/usr/btnSPOP-OPTION1')
         except:
             pass
-    
+        
+    def shell_content_dynamic_selection(self,shell_element=None,interactions='expand',node_num='1'):
+        ''' Script untuk interaksi dengan sheell element pada SAP GUI pada dynamic selection
+        ada beberapa interaksi yang dapat dilakukan yaitu select, top, expand dan double klik     
+        '''
+        try:
+            if interactions=='top':
+                self.session.findById(shell_element).topNode = "         "+node_num
+            if interactions=='select':
+                self.session.findById(shell_element).selectNode("         "+node_num)
+            if interactions=='expand':
+                self.session.findById(shell_element).expandNode("         "+node_num)                
+            if interactions=='doubleclick':
+                self.session.findById(shell_element).doubleClickNode("         "+node_num)
+        except Exception as e:
+            raise RuntimeError(e)
+
+    def shell_content_element(self,shell_element=None,interactions='get',row_num=1,col_name=None):
+        ''' Script untuk interaksi dengan sheell element pada SAP GUI, terutama untuk pada tabel data,
+        ada dua interaksi yang bisa dilakukan yaitu get (mengambil data, text value) dan click (melakukan double klik pada sel terpilih)    
+        '''
+        try:
+            if interactions=='get':
+                return self.session.findById(shell_element).GetCellValue(row_num,col_name)
+            if interactions=='click':
+                click = self.session.findById(shell_element)
+                click.SetCurrentCell(row_num,col_name)
+                click.DoubleClickCurrentCell()
+                return "Cell Clicked"
+        except Exception as e:
+            raise RuntimeError(e)
+        
     def login_sap(self, config):
         """ Script untuk Login SAP
             mengembalikan variabel status (boolean) dan message (string)
             
             True = Login berhasil, False = Login gagal
             
             pola configurasi dictionary : {"connection":"koneksi_anda","username":"username_anda","password":"password_anda","client":"client_anda"}
             
             contoh penggunaan :
             
-                ${status}    ${msg}=    Login Sap    ${config}
+                ${msg}=    Login Sap    ${config}
             
             """
             
-        call([r'C:/Program Files (x86)/SAP/FrontEnd/SAPgui/saplogon.exe'])
+        Popen([r'C:/Program Files (x86)/SAP/FrontEnd/SAPgui/saplogon.exe'])
+        
+        # for i in range(10):
+        #     s = check_output('tasklist', shell=True)
+        #     if "saplogon.exe" in str(s):
+        #         break
+        #     else :
+        #         time.sleep(2)
         
         for i in range(10):
-            s = check_output('tasklist', shell=True)
-            if "saplogon.exe" in str(s):
+            try:
+                self.connect_to_session()
                 break
-            else :
+            except :
                 time.sleep(2)
         
-        self.connect_to_session()
-                
+        if self.sapapp == -1:
+            raise RuntimeError('Cannot connect to session')
+
         self.open_connection(config['connection'])
         self.input_text("wnd[0]/usr/txtRSYST-BNAME",config["username"])
         self.input_password("wnd[0]/usr/pwdRSYST-BCODE",config["password"])
         self.input_text("wnd[0]/usr/txtRSYST-MANDT",config['client'])
         self.send_vkey(0)
+
+        time.sleep(5)
         
         
         msg = "Success Login"
         
         try:
             self.session.findById("wnd[1]/usr/pwdRSYST-NCODE")
             msg = self.notifikasi_login['Popup Change Password']
```

