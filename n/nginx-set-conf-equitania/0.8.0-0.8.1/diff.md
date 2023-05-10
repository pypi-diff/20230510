# Comparing `tmp/nginx-set-conf-equitania-0.8.0.tar.gz` & `tmp/nginx-set-conf-equitania-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nginx-set-conf-equitania-0.8.0.tar", last modified: Tue May  2 13:29:44 2023, max compression
+gzip compressed data, was "nginx-set-conf-equitania-0.8.1.tar", last modified: Wed May 10 12:47:39 2023, max compression
```

## Comparing `nginx-set-conf-equitania-0.8.0.tar` & `nginx-set-conf-equitania-0.8.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 picard     (501) staff       (20)        0 2023-05-02 13:29:44.861925 nginx-set-conf-equitania-0.8.0/
--rw-r--r--   0 picard     (501) staff       (20)    33892 2021-05-25 14:23:55.000000 nginx-set-conf-equitania-0.8.0/LICENSE.txt
--rw-r--r--   0 picard     (501) staff       (20)     3320 2023-05-02 13:29:44.861710 nginx-set-conf-equitania-0.8.0/PKG-INFO
--rw-r--r--   0 picard     (501) staff       (20)     2818 2023-01-21 08:58:48.000000 nginx-set-conf-equitania-0.8.0/README.md
-drwxr-xr-x   0 picard     (501) staff       (20)        0 2023-05-02 13:29:44.856279 nginx-set-conf-equitania-0.8.0/nginx_set_conf/
--rw-r--r--   0 picard     (501) staff       (20)       50 2021-05-27 17:15:29.000000 nginx-set-conf-equitania-0.8.0/nginx_set_conf/__init__.py
--rw-r--r--   0 picard     (501) staff       (20)    21170 2023-05-02 13:26:18.000000 nginx-set-conf-equitania-0.8.0/nginx_set_conf/config_templates.py
--rw-r--r--   0 picard     (501) staff       (20)     4006 2023-05-02 13:29:17.000000 nginx-set-conf-equitania-0.8.0/nginx_set_conf/nginx_set_conf.py
--rw-r--r--   0 picard     (501) staff       (20)     7078 2023-05-02 13:16:56.000000 nginx-set-conf-equitania-0.8.0/nginx_set_conf/utils.py
-drwxr-xr-x   0 picard     (501) staff       (20)        0 2023-05-02 13:29:44.861276 nginx-set-conf-equitania-0.8.0/nginx_set_conf_equitania.egg-info/
--rw-r--r--   0 picard     (501) staff       (20)     3320 2023-05-02 13:29:44.000000 nginx-set-conf-equitania-0.8.0/nginx_set_conf_equitania.egg-info/PKG-INFO
--rw-r--r--   0 picard     (501) staff       (20)      439 2023-05-02 13:29:44.000000 nginx-set-conf-equitania-0.8.0/nginx_set_conf_equitania.egg-info/SOURCES.txt
--rw-r--r--   0 picard     (501) staff       (20)        1 2023-05-02 13:29:44.000000 nginx-set-conf-equitania-0.8.0/nginx_set_conf_equitania.egg-info/dependency_links.txt
--rw-r--r--   0 picard     (501) staff       (20)       86 2023-05-02 13:29:44.000000 nginx-set-conf-equitania-0.8.0/nginx_set_conf_equitania.egg-info/entry_points.txt
--rw-r--r--   0 picard     (501) staff       (20)       27 2023-05-02 13:29:44.000000 nginx-set-conf-equitania-0.8.0/nginx_set_conf_equitania.egg-info/requires.txt
--rw-r--r--   0 picard     (501) staff       (20)       15 2023-05-02 13:29:44.000000 nginx-set-conf-equitania-0.8.0/nginx_set_conf_equitania.egg-info/top_level.txt
--rw-r--r--   0 picard     (501) staff       (20)       38 2023-05-02 13:29:44.861975 nginx-set-conf-equitania-0.8.0/setup.cfg
--rw-r--r--   0 picard     (501) staff       (20)      903 2023-05-02 13:28:10.000000 nginx-set-conf-equitania-0.8.0/setup.py
+drwxr-xr-x   0 picard     (501) staff       (20)        0 2023-05-10 12:47:39.837492 nginx-set-conf-equitania-0.8.1/
+-rw-r--r--   0 picard     (501) staff       (20)    33892 2021-05-25 14:23:55.000000 nginx-set-conf-equitania-0.8.1/LICENSE.txt
+-rw-r--r--   0 picard     (501) staff       (20)     3320 2023-05-10 12:47:39.837239 nginx-set-conf-equitania-0.8.1/PKG-INFO
+-rw-r--r--   0 picard     (501) staff       (20)     2818 2023-01-21 08:58:48.000000 nginx-set-conf-equitania-0.8.1/README.md
+drwxr-xr-x   0 picard     (501) staff       (20)        0 2023-05-10 12:47:39.833801 nginx-set-conf-equitania-0.8.1/nginx_set_conf/
+-rw-r--r--   0 picard     (501) staff       (20)       50 2021-05-27 17:15:29.000000 nginx-set-conf-equitania-0.8.1/nginx_set_conf/__init__.py
+-rw-r--r--   0 picard     (501) staff       (20)    21510 2023-05-10 12:46:09.000000 nginx-set-conf-equitania-0.8.1/nginx_set_conf/config_templates.py
+-rw-r--r--   0 picard     (501) staff       (20)     4006 2023-05-02 13:29:17.000000 nginx-set-conf-equitania-0.8.1/nginx_set_conf/nginx_set_conf.py
+-rw-r--r--   0 picard     (501) staff       (20)     7078 2023-05-02 13:16:56.000000 nginx-set-conf-equitania-0.8.1/nginx_set_conf/utils.py
+drwxr-xr-x   0 picard     (501) staff       (20)        0 2023-05-10 12:47:39.836617 nginx-set-conf-equitania-0.8.1/nginx_set_conf_equitania.egg-info/
+-rw-r--r--   0 picard     (501) staff       (20)     3320 2023-05-10 12:47:39.000000 nginx-set-conf-equitania-0.8.1/nginx_set_conf_equitania.egg-info/PKG-INFO
+-rw-r--r--   0 picard     (501) staff       (20)      439 2023-05-10 12:47:39.000000 nginx-set-conf-equitania-0.8.1/nginx_set_conf_equitania.egg-info/SOURCES.txt
+-rw-r--r--   0 picard     (501) staff       (20)        1 2023-05-10 12:47:39.000000 nginx-set-conf-equitania-0.8.1/nginx_set_conf_equitania.egg-info/dependency_links.txt
+-rw-r--r--   0 picard     (501) staff       (20)       86 2023-05-10 12:47:39.000000 nginx-set-conf-equitania-0.8.1/nginx_set_conf_equitania.egg-info/entry_points.txt
+-rw-r--r--   0 picard     (501) staff       (20)       27 2023-05-10 12:47:39.000000 nginx-set-conf-equitania-0.8.1/nginx_set_conf_equitania.egg-info/requires.txt
+-rw-r--r--   0 picard     (501) staff       (20)       15 2023-05-10 12:47:39.000000 nginx-set-conf-equitania-0.8.1/nginx_set_conf_equitania.egg-info/top_level.txt
+-rw-r--r--   0 picard     (501) staff       (20)       38 2023-05-10 12:47:39.837563 nginx-set-conf-equitania-0.8.1/setup.cfg
+-rw-r--r--   0 picard     (501) staff       (20)      903 2023-05-10 12:46:45.000000 nginx-set-conf-equitania-0.8.1/setup.py
```

### Comparing `nginx-set-conf-equitania-0.8.0/LICENSE.txt` & `nginx-set-conf-equitania-0.8.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nginx-set-conf-equitania-0.8.0/PKG-INFO` & `nginx-set-conf-equitania-0.8.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nginx-set-conf-equitania
-Version: 0.8.0
+Version: 0.8.1
 Summary: A package to create configurations for nginx with/without pagespeed for different web applications
 Author: Equitania Software GmbH
 Author-email: info@equitania.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `nginx-set-conf-equitania-0.8.0/README.md` & `nginx-set-conf-equitania-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `nginx-set-conf-equitania-0.8.0/nginx_set_conf/config_templates.py` & `nginx-set-conf-equitania-0.8.1/nginx_set_conf/config_templates.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 config_template_dict = {
 "ngx_code_server": """# Template for code-server configuration nginx incl. SSL/http2
-# Version 3.7 from 02.05.2023
+# Version 3.8 from 10.05.2023
 # upstream server.domain.de {
 #     server ip.ip.ip.ip weight=1 fail_timeout=0;
 # }
 
 server {
-    listen 80;
+    listen server.domain.de:80;
     server_name server.domain.de;
     rewrite ^/.*$ https://$host$request_uri? permanent;
 }
 
 server {
-    listen 443 ssl http2;
+    listen server.domain.de:443 ssl http2;
     server_name server.domain.de;
 
     add_header Strict-Transport-Security "max-age=15552000; includeSubDomains" always;
 
     access_log /var/log/nginx/server.domain.de-access.log;
     error_log /var/log/nginx/server.domain.de-error.log;
 
@@ -65,27 +65,27 @@
     }
     # Pagespeed
     pagespeed off;
 }
 """,
 
 "ngx_fast_report": """# Template for FastReport configuration nginx incl. SSL/http2
-# Version 3.7 from 02.05.2023
+# Version 3.8 from 10.05.2023
 # upstream server.domain.de {
 #     server ip.ip.ip.ip weight=1 fail_timeout=0;
 # }
 
 server {
-    listen 80;
+    listen server.domain.de:80;
     server_name server.domain.de;
     rewrite ^/.*$ https://$host$request_uri? permanent;
 }
 
 server {
-    listen 443 ssl http2;
+    listen server.domain.de:443 ssl http2;
     server_name server.domain.de;
 
     add_header Strict-Transport-Security "max-age=15552000; includeSubDomains" always;
 
     access_log /var/log/nginx/server.domain.de-access.log;
     error_log /var/log/nginx/server.domain.de-error.log;
 
@@ -134,27 +134,27 @@
     }
     # Pagespeed
     pagespeed off;
 }
 """,
 
 "ngx_nextcloud": """# Template for NextCloud configuration nginx incl. SSL/http2
-# Version 3.7 from 02.05.2023
+# Version 3.8 from 10.05.2023
 # upstream server.domain.de {
 #     server ip.ip.ip.ip weight=1 fail_timeout=0;
 # }
 
 server {
-    listen 80;
+    listen server.domain.de:80;
     server_name server.domain.de;
     rewrite ^/.*$ https://$host$request_uri? permanent;
 }
 
 server {
-    listen 443 ssl http2;
+    listen server.domain.de:443 ssl http2;
     server_name server.domain.de;
 
     add_header Strict-Transport-Security "max-age=15552000; includeSubDomains" always;
     add_header Referrer-Policy no-referrer always;
 
     access_log /var/log/nginx/server.domain.de-access.log;
     error_log /var/log/nginx/server.domain.de-error.log;
@@ -214,27 +214,27 @@
     }
     # Pagespeed
     pagespeed off;
 }""",
 
 
 "ngx_portainer": """# Template for Portainer configuration nginx incl. SSL/http2
-# Version 3.7 from 02.05.2023
+# Version 3.8 from 10.05.2023
 # upstream server.domain.de {
 #     server ip.ip.ip.ip weight=1 fail_timeout=0;
 # }
 
 server {
-    listen 80;
+    listen server.domain.de:80;
     server_name server.domain.de;
     rewrite ^/.*$ https://$host$request_uri? permanent;
 }
 
 server {
-    listen 443 ssl http2;
+    listen server.domain.de:443 ssl http2;
     server_name server.domain.de;
 
     add_header Strict-Transport-Security "max-age=15552000; includeSubDomains" always;
     add_header Referrer-Policy no-referrer always;
 
     access_log /var/log/nginx/server.domain.de-access.log;
     error_log /var/log/nginx/server.domain.de-error.log;
@@ -270,21 +270,21 @@
         proxy_pass http://127.0.0.1:oldport;
     }
     # Pagespeed
     pagespeed off;
 }""",
 
 "ngx_odoo_http": """# Template for Odoo configuration nginx
-# Version 3.7 from 02.05.2023
+# Version 3.8 from 10.05.2023
 # upstream server.domain.de {
 #     server ip.ip.ip.ip weight=1 fail_timeout=0;
 # }
 
 server {
-    listen 80;
+    listen server.domain.de:80;
     server_name server.domain.de;
     client_max_body_size 8192m;
     access_log /var/log/nginx/server.domain.de-access.log;
     error_log /var/log/nginx/server.domain.de-error.log;
 
     # increase proxy buffer to handle some Odoo web requests
     proxy_buffers 16 64k;
@@ -337,27 +337,27 @@
         proxy_pass http://127.0.0.1:oldport;
     }
     # Pagespeed
     pagespeed off;
 }""",
 
 "ngx_odoo_ssl": """# Template for Odoo configuration nginx incl. SSL
-# Version 3.7 from 02.05.2023
+# Version 3.8 from 10.05.2023
 # upstream server.domain.de {
 #     server ip.ip.ip.ip weight=1 fail_timeout=0;
 # }
 
 server {
-    listen 80;
+    listen server.domain.de:80;
     server_name server.domain.de;
     rewrite ^/.*$ https://$host$request_uri? permanent;
 }
 
 server {
-    listen 443 ssl http2;
+    listen server.domain.de:443 ssl http2;
     server_name server.domain.de;
     client_max_body_size 8192m;
     access_log /var/log/nginx/server.domain.de-access.log;
     error_log /var/log/nginx/server.domain.de-error.log;
 
     # ssl certificate files
     ssl_certificate /etc/letsencrypt/live/zertifikat.crt/fullchain.pem;
@@ -427,27 +427,27 @@
     pagespeed off;
 }
 
 """,
 
 "ngx_odoo_ssl_pagespeed": """# Template for Odoo configuration nginx incl. SSL/http2 and Google PageSpeed
 # source: https://github.com/apache/incubator-pagespeed-ngx/blob/master/scripts/build_ngx_pagespeed.sh
-# Version 3.7 from 02.05.2023
+# Version 3.8 from 10.05.2023
 # upstream server.domain.de {
 #     server ip.ip.ip.ip weight=1 fail_timeout=0;
 # }
 
 server {
-    listen 80;
+    listen server.domain.de:80;
     server_name server.domain.de;
     rewrite ^/.*$ https://$host$request_uri? permanent;
 }
 
 server {
-    listen 443 ssl http2;
+    listen server.domain.de:443 ssl http2;
     server_name server.domain.de;
     client_max_body_size 8192m;
     access_log /var/log/nginx/server.domain.de-access.log;
     error_log /var/log/nginx/server.domain.de-error.log;
 
     # ssl certificate files
     ssl_certificate /etc/letsencrypt/live/zertifikat.crt/fullchain.pem;
@@ -517,27 +517,27 @@
 
     include "pagespeed_main.conf";
     # Pagespeed
     pagespeed on;
 }""",
 
 "ngx_pgadmin": """# Template for pgAdmin configuration nginx incl. SSL/http2
-# Version 3.7 from 02.05.2023
+# Version 3.8 from 10.05.2023
 # upstream server.domain.de {
 #     server ip.ip.ip.ip weight=1 fail_timeout=0;
 # }
 
 server {
-    listen 80;
+    listen server.domain.de:80;
     server_name server.domain.de;
     rewrite ^/.*$ https://$host$request_uri? permanent;
 }
 
 server {
-    listen 443 ssl http2;
+    listen server.domain.de:443 ssl http2;
     server_name server.domain.de;
 
     add_header Strict-Transport-Security "max-age=15552000; includeSubDomains" always;
 
     access_log /var/log/nginx/server.domain.de-access.log;
     error_log /var/log/nginx/server.domain.de-error.log;
 
@@ -578,27 +578,27 @@
     }
     # Pagespeed
     pagespeed off;
 }
 """,
 
 "ngx_pwa": """# Template for Progressive Web App .NET Core configuration nginx incl. SSL/http2
-# Version 3.7 from 02.05.2023
+# Version 3.8 from 10.05.2023
 # upstream server.domain.de {
 #     server ip.ip.ip.ip weight=1 fail_timeout=0;
 # }
 
 server {
-    listen 80;
+    listen server.domain.de:80;
     server_name server.domain.de;
     rewrite ^/.*$ https://$host$request_uri? permanent;
 }
 
 server {
-    listen 443 ssl http2;
+    listen server.domain.de:443 ssl http2;
     server_name server.domain.de;
 
     add_header Strict-Transport-Security "max-age=15552000; includeSubDomains" always;
 
     access_log /var/log/nginx/server.domain.de-access.log;
     error_log /var/log/nginx/server.domain.de-error.log;
 
@@ -642,45 +642,45 @@
         proxy_pass http://127.0.0.1:oldport;
     }
     # Pagespeed
     pagespeed off;
 }""",
 
 "ngx_redirect": """# Template for Redirect Domain configuration nginx
-# Version 3.5 from 25.04.2022
+# Version 3.6 from 10.05.2023
 upstream server.domain.de {
     server ip.ip.ip.ip weight=1 fail_timeout=0;
 }
 
 server {
-    listen 80;
+    listen server.domain.de:80;
     server_name server.domain.de;
     rewrite ^/.*$ http://target.domain.de$request_uri? permanent;
     access_log /var/log/nginx/target.domain.de-access.log;
     error_log /var/log/nginx/target.domain.de-error.log;
     # Pagespeed
     pagespeed off;
 }""",
 
 "ngx_redirect_ssl": """# Template for Redirect domain configuration nginx ssl/http2
-# Version 3.7 from 02.05.2023
+# Version 3.8 from 10.05.2023
 # upstream server.domain.de {
 #     server ip.ip.ip.ip weight=1 fail_timeout=0;
 # }
 
 server {
-    listen 80;
+    listen server.domain.de:80;
     server_name server.domain.de;
     rewrite ^/.*$ http://target.domain.de$request_uri? permanent;
     access_log /var/log/nginx/target.domain.de-access.log;
     error_log /var/log/nginx/target.domain.de-error.log;
 }
 
 server {
-    listen 443 ssl http2;
+    listen server.domain.de:443 ssl http2;
     server_name server.domain.de;
     rewrite ^/.*$ https://target.domain.de$request_uri? permanent;
     access_log /var/log/nginx/target.domain.de-access.log;
     error_log /var/log/nginx/target.domain.de-error.log;
 
     # ssl certificate files
     ssl_certificate /etc/letsencrypt/live/zertifikat.crt/fullchain.pem;
```

### Comparing `nginx-set-conf-equitania-0.8.0/nginx_set_conf/nginx_set_conf.py` & `nginx-set-conf-equitania-0.8.1/nginx_set_conf/nginx_set_conf.py`

 * *Files identical despite different names*

### Comparing `nginx-set-conf-equitania-0.8.0/nginx_set_conf/utils.py` & `nginx-set-conf-equitania-0.8.1/nginx_set_conf/utils.py`

 * *Files identical despite different names*

### Comparing `nginx-set-conf-equitania-0.8.0/nginx_set_conf_equitania.egg-info/PKG-INFO` & `nginx-set-conf-equitania-0.8.1/nginx_set_conf_equitania.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nginx-set-conf-equitania
-Version: 0.8.0
+Version: 0.8.1
 Summary: A package to create configurations for nginx with/without pagespeed for different web applications
 Author: Equitania Software GmbH
 Author-email: info@equitania.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `nginx-set-conf-equitania-0.8.0/setup.py` & `nginx-set-conf-equitania-0.8.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="nginx-set-conf-equitania",
-    version="0.8.0",
+    version="0.8.1",
     author="Equitania Software GmbH",
     author_email="info@equitania.de",
     description="A package to create configurations for nginx with/without pagespeed for different web applications",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=['nginx_set_conf'],
     classifiers=[
```

