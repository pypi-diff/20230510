# Comparing `tmp/raspisump-1.4.1.tar.gz` & `tmp/raspisump-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/raspisump-1.4.1.tar", last modified: Sat Feb 19 01:04:10 2022, max compression
+gzip compressed data, was "raspisump-1.5.tar", last modified: Wed May 10 18:32:53 2023, max compression
```

## Comparing `raspisump-1.4.1.tar` & `raspisump-1.5.tar`

### file list

```diff
@@ -1,52 +1,54 @@
-drwxrwxr-x   0 al        (1000) al        (1000)        0 2022-02-19 01:04:10.000000 raspisump-1.4.1/
--rw-rw-r--   0 al        (1000) al        (1000)     3519 2022-02-19 00:39:27.000000 raspisump-1.4.1/README.md
--rwxrwxr-x   0 al        (1000) al        (1000)     2255 2022-02-19 00:48:53.000000 raspisump-1.4.1/setup.py
--rw-rw-r--   0 al        (1000) al        (1000)     5143 2022-02-19 01:04:10.000000 raspisump-1.4.1/PKG-INFO
--rw-rw-r--   0 al        (1000) al        (1000)      263 2022-02-15 13:14:18.000000 raspisump-1.4.1/MANIFEST.in
-drwxrwxr-x   0 al        (1000) al        (1000)        0 2022-02-19 01:04:10.000000 raspisump-1.4.1/docs/
--rw-rw-r--   0 al        (1000) al        (1000)      275 2022-02-11 16:41:18.000000 raspisump-1.4.1/docs/README.md
--rw-rw-r--   0 al        (1000) al        (1000)    10667 2022-02-19 00:39:27.000000 raspisump-1.4.1/docs/install.md
--rw-rw-r--   0 al        (1000) al        (1000)   127896 2022-02-19 00:39:27.000000 raspisump-1.4.1/docs/install.pdf
-drwxrwxr-x   0 al        (1000) al        (1000)        0 2022-02-19 01:04:10.000000 raspisump-1.4.1/raspisump/
--rw-rw-r--   0 al        (1000) al        (1000)     2541 2022-02-11 16:41:18.000000 raspisump-1.4.1/raspisump/todaychart.py
--rwxrwxr-x   0 al        (1000) al        (1000)        0 2020-06-19 12:02:07.000000 raspisump-1.4.1/raspisump/__init__.py
--rw-rw-r--   0 al        (1000) al        (1000)     1791 2020-06-19 12:02:07.000000 raspisump-1.4.1/raspisump/log.py
--rw-rw-r--   0 al        (1000) al        (1000)     2618 2020-06-19 12:02:07.000000 raspisump-1.4.1/raspisump/reading.py
--rw-rw-r--   0 al        (1000) al        (1000)     2053 2022-02-14 18:06:41.000000 raspisump-1.4.1/raspisump/emailtest.py
--rw-rw-r--   0 al        (1000) al        (1000)     4886 2020-06-19 12:02:07.000000 raspisump-1.4.1/raspisump/alerts.py
--rw-rw-r--   0 al        (1000) al        (1000)     1963 2020-06-19 12:02:07.000000 raspisump-1.4.1/raspisump/checkpid.py
--rw-rw-r--   0 al        (1000) al        (1000)     3670 2020-06-19 12:02:07.000000 raspisump-1.4.1/raspisump/heartbeat.py
--rw-rw-r--   0 al        (1000) al        (1000)     1488 2022-02-11 16:41:18.000000 raspisump-1.4.1/raspisump/webchart.py
--rw-rw-r--   0 al        (1000) al        (1000)       38 2022-02-19 01:04:10.000000 raspisump-1.4.1/setup.cfg
-drwxrwxr-x   0 al        (1000) al        (1000)        0 2022-02-19 01:04:10.000000 raspisump-1.4.1/conf/
--rw-rw-r--   0 al        (1000) al        (1000)     1114 2020-06-19 12:02:07.000000 raspisump-1.4.1/conf/lighttpd.conf
-drwxrwxr-x   0 al        (1000) al        (1000)        0 2022-02-19 01:04:10.000000 raspisump-1.4.1/conf/csv/
--rw-rw-r--   0 al        (1000) al        (1000)       80 2020-06-19 12:02:07.000000 raspisump-1.4.1/conf/csv/README.md
-drwxrwxr-x   0 al        (1000) al        (1000)        0 2022-02-19 01:04:10.000000 raspisump-1.4.1/conf/logs/
--rw-rw-r--   0 al        (1000) al        (1000)      217 2020-06-19 12:02:07.000000 raspisump-1.4.1/conf/logs/README.md
-drwxrwxr-x   0 al        (1000) al        (1000)        0 2022-02-19 01:04:10.000000 raspisump-1.4.1/conf/web/
-drwxrwxr-x   0 al        (1000) al        (1000)        0 2022-02-19 01:04:10.000000 raspisump-1.4.1/conf/web/css/
--rw-rw-r--   0 al        (1000) al        (1000)      614 2020-06-19 12:02:07.000000 raspisump-1.4.1/conf/web/css/raspi.css
--rw-rw-r--   0 al        (1000) al        (1000)        0 2020-06-19 12:02:07.000000 raspisump-1.4.1/conf/web/css/index.html
--rw-rw-r--   0 al        (1000) al        (1000)      690 2020-06-19 12:02:07.000000 raspisump-1.4.1/conf/web/css/raspi.css~
--rwxrwxr-x   0 al        (1000) al        (1000)      906 2020-06-19 12:02:07.000000 raspisump-1.4.1/conf/web/index.html
-drwxrwxr-x   0 al        (1000) al        (1000)        0 2022-02-19 01:04:10.000000 raspisump-1.4.1/conf/web/images/
--rw-rw-r--   0 al        (1000) al        (1000)    51981 2020-06-19 12:02:07.000000 raspisump-1.4.1/conf/web/images/logo.png
-drwxrwxr-x   0 al        (1000) al        (1000)        0 2022-02-19 01:04:10.000000 raspisump-1.4.1/conf/charts/
--rw-rw-r--   0 al        (1000) al        (1000)       80 2020-06-19 12:02:07.000000 raspisump-1.4.1/conf/charts/README.md
--rw-rw-r--   0 al        (1000) al        (1000)     5687 2022-02-13 16:49:05.000000 raspisump-1.4.1/conf/raspisump.conf
-drwxrwxr-x   0 al        (1000) al        (1000)        0 2022-02-19 01:04:10.000000 raspisump-1.4.1/cron/
--rw-rw-r--   0 al        (1000) al        (1000)      140 2020-06-19 12:02:07.000000 raspisump-1.4.1/cron/README.md
--rw-rw-r--   0 al        (1000) al        (1000)      258 2021-12-29 14:51:14.000000 raspisump-1.4.1/cron/picrontab
-drwxrwxr-x   0 al        (1000) al        (1000)        0 2022-02-19 01:04:10.000000 raspisump-1.4.1/bin/
--rwxrwxr-x   0 al        (1000) al        (1000)      696 2020-06-19 12:02:07.000000 raspisump-1.4.1/bin/rsump.py
--rwxrwxr-x   0 al        (1000) al        (1000)      617 2022-02-11 16:41:18.000000 raspisump-1.4.1/bin/rsumpchart.py
--rwxrwxr-x   0 al        (1000) al        (1000)      660 2020-06-19 12:02:07.000000 raspisump-1.4.1/bin/rsumpwebchart.py
--rw-rw-r--   0 al        (1000) al        (1000)      359 2022-02-14 18:06:41.000000 raspisump-1.4.1/bin/emailtest
--rwxrwxr-x   0 al        (1000) al        (1000)      520 2020-06-19 12:02:07.000000 raspisump-1.4.1/bin/rsumpmonitor.py
-drwxrwxr-x   0 al        (1000) al        (1000)        0 2022-02-19 01:04:10.000000 raspisump-1.4.1/raspisump.egg-info/
--rw-rw-r--   0 al        (1000) al        (1000)        1 2022-02-19 01:04:10.000000 raspisump-1.4.1/raspisump.egg-info/dependency_links.txt
--rw-rw-r--   0 al        (1000) al        (1000)       13 2022-02-19 01:04:10.000000 raspisump-1.4.1/raspisump.egg-info/requires.txt
--rw-rw-r--   0 al        (1000) al        (1000)     5143 2022-02-19 01:04:10.000000 raspisump-1.4.1/raspisump.egg-info/PKG-INFO
--rw-rw-r--   0 al        (1000) al        (1000)       10 2022-02-19 01:04:10.000000 raspisump-1.4.1/raspisump.egg-info/top_level.txt
--rw-rw-r--   0 al        (1000) al        (1000)      768 2022-02-19 01:04:10.000000 raspisump-1.4.1/raspisump.egg-info/SOURCES.txt
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-05-10 18:32:53.408204 raspisump-1.5/
+-rw-r--r--   0 al        (1000) users      (984)     1073 2023-02-19 16:52:26.000000 raspisump-1.5/LICENSE
+-rw-r--r--   0 al        (1000) users      (984)      278 2023-05-10 18:31:52.000000 raspisump-1.5/MANIFEST.in
+-rw-r--r--   0 al        (1000) users      (984)     3953 2023-05-10 18:32:53.408204 raspisump-1.5/PKG-INFO
+-rw-r--r--   0 al        (1000) users      (984)     3182 2023-05-10 18:31:52.000000 raspisump-1.5/README.md
+-rw-r--r--   0 al        (1000) users      (984)       22 2023-05-10 18:31:52.000000 raspisump-1.5/VERSION
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-05-10 18:32:53.401537 raspisump-1.5/bin/
+-rw-r--r--   0 al        (1000) users      (984)      359 2022-04-12 11:43:48.000000 raspisump-1.5/bin/emailtest
+-rwxr-xr-x   0 al        (1000) users      (984)      696 2022-04-12 11:43:48.000000 raspisump-1.5/bin/rsump.py
+-rwxr-xr-x   0 al        (1000) users      (984)      617 2022-04-12 11:43:48.000000 raspisump-1.5/bin/rsumpchart.py
+-rwxr-xr-x   0 al        (1000) users      (984)      535 2023-05-10 18:31:52.000000 raspisump-1.5/bin/rsumpmonitor.py
+-rwxr-xr-x   0 al        (1000) users      (984)      660 2022-04-12 11:43:48.000000 raspisump-1.5/bin/rsumpwebchart.py
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-05-10 18:32:53.401537 raspisump-1.5/conf/
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-05-10 18:32:53.401537 raspisump-1.5/conf/charts/
+-rw-r--r--   0 al        (1000) users      (984)       80 2022-04-12 11:43:48.000000 raspisump-1.5/conf/charts/README.md
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-05-10 18:32:53.401537 raspisump-1.5/conf/csv/
+-rw-r--r--   0 al        (1000) users      (984)       80 2022-04-12 11:43:48.000000 raspisump-1.5/conf/csv/README.md
+-rw-r--r--   0 al        (1000) users      (984)     1112 2023-05-10 18:31:52.000000 raspisump-1.5/conf/lighttpd.conf
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-05-10 18:32:53.401537 raspisump-1.5/conf/logs/
+-rw-r--r--   0 al        (1000) users      (984)      217 2022-04-12 11:43:48.000000 raspisump-1.5/conf/logs/README.md
+-rw-r--r--   0 al        (1000) users      (984)     5687 2022-04-12 11:43:48.000000 raspisump-1.5/conf/raspisump.conf
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-05-10 18:32:53.404870 raspisump-1.5/conf/web/
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-05-10 18:32:53.404870 raspisump-1.5/conf/web/css/
+-rw-r--r--   0 al        (1000) users      (984)        0 2022-04-12 11:43:48.000000 raspisump-1.5/conf/web/css/index.html
+-rw-r--r--   0 al        (1000) users      (984)      614 2022-04-12 11:43:48.000000 raspisump-1.5/conf/web/css/raspi.css
+-rw-r--r--   0 al        (1000) users      (984)      690 2022-04-12 11:43:48.000000 raspisump-1.5/conf/web/css/raspi.css~
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-05-10 18:32:53.404870 raspisump-1.5/conf/web/images/
+-rw-r--r--   0 al        (1000) users      (984)    51981 2022-04-12 11:43:48.000000 raspisump-1.5/conf/web/images/logo.png
+-rwxr-xr-x   0 al        (1000) users      (984)      906 2022-04-12 11:43:48.000000 raspisump-1.5/conf/web/index.html
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-05-10 18:32:53.404870 raspisump-1.5/cron/
+-rw-r--r--   0 al        (1000) users      (984)      140 2022-04-12 11:43:48.000000 raspisump-1.5/cron/README.md
+-rw-r--r--   0 al        (1000) users      (984)      258 2022-04-12 11:43:48.000000 raspisump-1.5/cron/picrontab
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-05-10 18:32:53.404870 raspisump-1.5/docs/
+-rw-r--r--   0 al        (1000) users      (984)      275 2022-04-12 11:43:48.000000 raspisump-1.5/docs/README.md
+-rw-r--r--   0 al        (1000) users      (984)    10942 2023-05-10 18:31:52.000000 raspisump-1.5/docs/install.md
+-rw-r--r--   0 al        (1000) users      (984)   133692 2023-05-10 18:31:52.000000 raspisump-1.5/docs/install.pdf
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-05-10 18:32:53.408204 raspisump-1.5/raspisump/
+-rwxr-xr-x   0 al        (1000) users      (984)        0 2022-04-12 11:43:48.000000 raspisump-1.5/raspisump/__init__.py
+-rw-r--r--   0 al        (1000) users      (984)     4886 2022-04-12 11:43:48.000000 raspisump-1.5/raspisump/alerts.py
+-rw-r--r--   0 al        (1000) users      (984)     1963 2022-04-12 11:43:48.000000 raspisump-1.5/raspisump/checkpid.py
+-rw-r--r--   0 al        (1000) users      (984)     2053 2022-04-12 11:43:48.000000 raspisump-1.5/raspisump/emailtest.py
+-rw-r--r--   0 al        (1000) users      (984)     3670 2022-04-12 11:43:48.000000 raspisump-1.5/raspisump/heartbeat.py
+-rw-r--r--   0 al        (1000) users      (984)     1791 2022-04-12 11:43:48.000000 raspisump-1.5/raspisump/log.py
+-rw-r--r--   0 al        (1000) users      (984)     2618 2022-04-12 11:43:48.000000 raspisump-1.5/raspisump/reading.py
+-rw-r--r--   0 al        (1000) users      (984)     2541 2022-04-12 11:43:48.000000 raspisump-1.5/raspisump/todaychart.py
+-rw-r--r--   0 al        (1000) users      (984)     1488 2022-04-12 11:43:48.000000 raspisump-1.5/raspisump/webchart.py
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-05-10 18:32:53.408204 raspisump-1.5/raspisump.egg-info/
+-rw-r--r--   0 al        (1000) users      (984)     3953 2023-05-10 18:32:53.000000 raspisump-1.5/raspisump.egg-info/PKG-INFO
+-rw-r--r--   0 al        (1000) users      (984)      784 2023-05-10 18:32:53.000000 raspisump-1.5/raspisump.egg-info/SOURCES.txt
+-rw-r--r--   0 al        (1000) users      (984)        1 2023-05-10 18:32:53.000000 raspisump-1.5/raspisump.egg-info/dependency_links.txt
+-rw-r--r--   0 al        (1000) users      (984)       13 2023-05-10 18:32:53.000000 raspisump-1.5/raspisump.egg-info/requires.txt
+-rw-r--r--   0 al        (1000) users      (984)       10 2023-05-10 18:32:53.000000 raspisump-1.5/raspisump.egg-info/top_level.txt
+-rw-r--r--   0 al        (1000) users      (984)       38 2023-05-10 18:32:53.408204 raspisump-1.5/setup.cfg
+-rwxr-xr-x   0 al        (1000) users      (984)     2229 2023-05-10 18:31:52.000000 raspisump-1.5/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `raspisump-1.4.1/README.md` & `raspisump-1.5/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -10,16 +10,14 @@
 
 See the [changelog](https://github.com/alaudet/raspi-sump/blob/master/changelog) for the latest information on Raspi-Sump features.
 
 # Supported Versions of Raspbian / Raspberry Pi OS
 
 Raspi-Sump is currently supported on Raspberry Pi OS (Bullseye) and Raspian (Buster and Stretch).
 
-Raspian 9 (Stretch) support will be discontinued in June 2022.  Please upgrade to Raspberry Pi OS 11 Bullseye if you are currently using Stretch.
-
 # Discord Group
 
 Discuss and get support from other users. Email (alaudet@linuxnorth.org) for an invite link.
 
 
 # Install Dependencies
 
@@ -45,23 +43,14 @@
 Read the configuration docs copied during setup on your pi at the following location;
 
     /home/pi/raspi-sump/docs
 
 They are also available on github https://github.com/alaudet/raspi-sump/blob/master/docs/install.md
 
 
-# Upgrading from Python2 to Python3
-
-    sudo pip uninstall raspisump
-    sudo pip3 install --no-binary :all: raspisump
-
-
-Your configuration file will be preserved in /home/pi/raspi-sump/
-
-
 # Python2 (End of Life was January 1, 2020)
 
 Python2 installs of Raspi-Sump are no longer be supported.
 
 
 # More Info
```

### Comparing `raspisump-1.4.1/setup.py` & `raspisump-1.5/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 import os
 
-version = "1.4.1"
+version = "1.5"
 
 homedir = "/home/pi/raspi-sump/"
 
 if os.path.isfile(homedir + "raspisump.conf"):
     cmd = "cp -u " + homedir + "raspisump.conf " + homedir + "raspisump.conf.save"
     os.system(cmd)
 
@@ -27,29 +27,29 @@
     (homedir + "docs", ["docs/install.md"]),
     (homedir + "cron", ["cron/README.md"]),
     (homedir + "cron", ["cron/picrontab"]),
     (homedir + "web", ["conf/web/index.html"]),
     (homedir + "web/images", ["conf/web/images/logo.png"]),
     (homedir + "web/css", ["conf/web/css/index.html"]),
     (homedir + "web/css", ["conf/web/css/raspi.css"]),
+    (homedir, ["VERSION"])
 ]
 
 setup(
     name="raspisump",
     version=version,
     description="A sump pit monitoring system for Raspberry Pi",
     long_description_content_type="text/markdown",
     long_description=open("./README.md", "r").read(),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Console",
         "Intended Audience :: End Users/Desktop",
         "Natural Language :: English",
         "Operating System :: POSIX :: Linux",
-        "Programming Language :: Python :: 3.5",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.9",
         "Topic :: Home Automation",
         "License :: OSI Approved :: MIT License",
     ],
     author="Al Audet",
     author_email="alaudet@linuxnorth.org",
@@ -62,9 +62,8 @@
     install_requires=["hcsr04sensor"],
 )
 
 if os.path.isdir(homedir):
     cmd = "chown -R pi " + homedir
     os.system(cmd)
     cmd = "chmod 600 " + homedir + "raspisump.conf"
-    os.system(cmd)
-
+    os.system(cmd)
```

### Comparing `raspisump-1.4.1/PKG-INFO` & `raspisump-1.5/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,121 +1,109 @@
 Metadata-Version: 2.1
 Name: raspisump
-Version: 1.4.1
+Version: 1.5
 Summary: A sump pit monitoring system for Raspberry Pi
 Home-page: http://www.linuxnorth.org/raspi-sump/
+Download-URL: https://github.com/alaudet/raspi-sump/releases
 Author: Al Audet
 Author-email: alaudet@linuxnorth.org
 License: MIT License
-Download-URL: https://github.com/alaudet/raspi-sump/releases
-Description: Raspi-sump is a sump pit water level monitoring system using a Raspberry Pi and an Ultrasonic Sensor (HC-SR04).
-        
-        ![Chart](https://raspisump.linuxnorth.org/static/today.png)
-        
-        
-        Currently the system monitors the water level in your pit at defined intervals. It sends
-        email sms alerts if the water reaches a critical level, indicating a possible sump pump failure.
-        
-        # What's New
-        
-        See the [changelog](https://github.com/alaudet/raspi-sump/blob/master/changelog) for the latest information on Raspi-Sump features.
-        
-        # Supported Versions of Raspbian / Raspberry Pi OS
-        
-        Raspi-Sump is currently supported on Raspberry Pi OS (Bullseye) and Raspian (Buster and Stretch).
-        
-        Raspian 9 (Stretch) support will be discontinued in June 2022.  Please upgrade to Raspberry Pi OS 11 Bullseye if you are currently using Stretch.
-        
-        # Discord Group
-        
-        Discuss and get support from other users. Email (alaudet@linuxnorth.org) for an invite link.
-        
-        
-        # Install Dependencies
-        
-            sudo apt install python3-pip python3-rpi.gpio python3-matplotlib
-        
-        # Install Raspi-Sump
-        
-        Pip installs default to Wheels which omits some folder setup in setup.py.
-        Always use the '--no-binary :all:' option when installing or upgrading Raspi-Sump with pip.
-        
-            sudo pip3 install --no-binary :all: raspisump
-        
-        
-        # Upgrading Raspi-Sump 
-        
-        Upgrading an existing version
-        
-            sudo pip3 install -U --no-binary :all: raspisump
-        
-        This will also install the [HCSR04sensor](https://github.com/alaudet/hcsr04sensor) 
-        
-        
-        Read the configuration docs copied during setup on your pi at the following location;
-        
-            /home/pi/raspi-sump/docs
-        
-        They are also available on github https://github.com/alaudet/raspi-sump/blob/master/docs/install.md
-        
-        
-        # Upgrading from Python2 to Python3
-        
-            sudo pip uninstall raspisump
-            sudo pip3 install --no-binary :all: raspisump
-        
-        
-        Your configuration file will be preserved in /home/pi/raspi-sump/
-        
-        
-        # Python2 (End of Life was January 1, 2020)
-        
-        Python2 installs of Raspi-Sump are no longer be supported.
-        
-        
-        # More Info
-        
-        Further details provided at http://www.linuxnorth.org/raspi-sump/
-        
-        An example hourly updating graph is available for view.
-        http://www.linuxnorth.org/raspi-sump/raspi-sump-today.html
-        
-        # Disclaimer
-        
-        You are welcome to use Raspi-Sump but there is no guarantee it will work. Your house may still flood if your sump pump fails. This software comes with no warranty. See License details.
-        
-        This is not a replacement for a properly maintained water pumping system. It is one tool you can use to give yourself extra piece-of-mind.
-        
-        Best practices should include:
-        
-        * A backup pump that triggers at a slightly higher water level than your main pump.
-        * The secondary pump should be connected to a seperate dedicated electrical breaker. 
-        * You should also have a generator that can provide power should you have an extended outage during the spring or other unseasonally wet time of year.
-        * if you are building a new home, pay attention to the grade of your property, as you may be able to let gravity empty your pit for you.  That would be the best approach with a backup pump for added protection.
-        
-        Once you have done all of these things, then consider using a monitoring system like Raspi-Sump.
-        
-        # License
-        
-        MIT License.  I want you to do whatever you want with Raspi-Sump.  If you
-        improve it please let me know.
-        
-        # Contributing
-        
-        Please refer to the [Contributing Guidelines](https://github.com/alaudet/raspi-sump/blob/master/CONTRIBUTING.md) before issuing a pull request.
-        
-        # Donate
-        
-        [Your Donation is Appreciated](https://www.linuxnorth.org/donate/)
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Home Automation
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+Raspi-sump is a sump pit water level monitoring system using a Raspberry Pi and an Ultrasonic Sensor (HC-SR04).
+
+![Chart](https://raspisump.linuxnorth.org/static/today.png)
+
+
+Currently the system monitors the water level in your pit at defined intervals. It sends
+email sms alerts if the water reaches a critical level, indicating a possible sump pump failure.
+
+# What's New
+
+See the [changelog](https://github.com/alaudet/raspi-sump/blob/master/changelog) for the latest information on Raspi-Sump features.
+
+# Supported Versions of Raspbian / Raspberry Pi OS
+
+Raspi-Sump is currently supported on Raspberry Pi OS (Bullseye) and Raspian (Buster and Stretch).
+
+# Discord Group
+
+Discuss and get support from other users. Email (alaudet@linuxnorth.org) for an invite link.
+
+
+# Install Dependencies
+
+    sudo apt install python3-pip python3-rpi.gpio python3-matplotlib
+
+# Install Raspi-Sump
+
+Pip installs default to Wheels which omits some folder setup in setup.py.
+Always use the '--no-binary :all:' option when installing or upgrading Raspi-Sump with pip.
+
+    sudo pip3 install --no-binary :all: raspisump
+
+
+# Upgrading Raspi-Sump 
+
+Upgrading an existing version
+
+    sudo pip3 install -U --no-binary :all: raspisump
+
+This will also install the [HCSR04sensor](https://github.com/alaudet/hcsr04sensor) 
+
+
+Read the configuration docs copied during setup on your pi at the following location;
+
+    /home/pi/raspi-sump/docs
+
+They are also available on github https://github.com/alaudet/raspi-sump/blob/master/docs/install.md
+
+
+# Python2 (End of Life was January 1, 2020)
+
+Python2 installs of Raspi-Sump are no longer be supported.
+
+
+# More Info
+
+Further details provided at http://www.linuxnorth.org/raspi-sump/
+
+An example hourly updating graph is available for view.
+http://www.linuxnorth.org/raspi-sump/raspi-sump-today.html
+
+# Disclaimer
+
+You are welcome to use Raspi-Sump but there is no guarantee it will work. Your house may still flood if your sump pump fails. This software comes with no warranty. See License details.
+
+This is not a replacement for a properly maintained water pumping system. It is one tool you can use to give yourself extra piece-of-mind.
+
+Best practices should include:
+
+* A backup pump that triggers at a slightly higher water level than your main pump.
+* The secondary pump should be connected to a seperate dedicated electrical breaker. 
+* You should also have a generator that can provide power should you have an extended outage during the spring or other unseasonally wet time of year.
+* if you are building a new home, pay attention to the grade of your property, as you may be able to let gravity empty your pit for you.  That would be the best approach with a backup pump for added protection.
+
+Once you have done all of these things, then consider using a monitoring system like Raspi-Sump.
+
+# License
+
+MIT License.  I want you to do whatever you want with Raspi-Sump.  If you
+improve it please let me know.
+
+# Contributing
+
+Please refer to the [Contributing Guidelines](https://github.com/alaudet/raspi-sump/blob/master/CONTRIBUTING.md) before issuing a pull request.
+
+# Donate
+
+[Your Donation is Appreciated](https://www.linuxnorth.org/donate/)
```

### Comparing `raspisump-1.4.1/docs/install.md` & `raspisump-1.5/docs/install.md`

 * *Files 10% similar despite different names*

```diff
@@ -7,28 +7,55 @@
 
 Supported OS Versions
 =====================
 Raspberry Pi OS 11 (Bullseye)
 
 Raspbian OS 10 (Buster)
 
-Raspbian OS 9 (Stretch) - Support ends June 30, 2022
+Raspbian OS 9 (Stretch) - Support ended on June 30, 2022.  Upgrade to Bullseye
 
 
+Default 'pi' User Account
+=========================
+
+Raspberry Pi OS have changed the automatic creation of the 'pi' user account on Raspberry Pi OS 11 (Bullseye).  Raspi-Sump depends on that account existing.  When installing Raspberry Pi OS for the first time, you must create a user named pi for Raspi-Sump to work.
+
+For more information see the [Raspberry PI OS Announcement](https://www.raspberrypi.com/news/raspberry-pi-bullseye-update-april-2022/) on the default pi user account.
+
+
+Creating a pi user
+==================
+
+** Note (if user 'pi' already exists then skip this step)
+
+If you are installing Raspi-Sump on an existing Raspberry Pi OS that does not have a pi user, create it as follows. This command will also add the pi user to the sudo and gpio groups.  The gpio group is required for accessing the gpio pins as a regular user.
+
+    sudo useradd -m -g users -G sudo,gpio -s /bin/bash pi
+
+Give the pi user a password
+
+    sudo passwd pi
+
+You must log out and log back in for the new groups to take effect.
+
 Install Dependencies
 ====================
 
+Login as the pi user on Raspberry Pi OS.
+
 Install Pip, RPi.GPIO and Matplotlib
 
     sudo apt update && sudo apt -y upgrade
     sudo apt install python3-pip python3-rpi.gpio python3-matplotlib
 
 RPi.GPIO is the library that controls the sensor.  Matplotlib is used to generate charts.
 The Pip package manager is required to install Raspi-Sump in the next step.
 
+
+
 Install Raspi-Sump
 ==================
 
 The following will automatically install hcsr04sensor if it is not already
 installed on your Pi.
 
     sudo pip3 install --no-binary :all: raspisump
@@ -163,15 +190,15 @@
 root. 
 Add to pi user crontab as follows;
 
 1 - crontab -e
 
 2 - enter line in crontab as follows;
 
-    */5 * * * * sudo /usr/local/bin/rsumpmonitor.py
+    */5 * * * * /usr/local/bin/rsumpmonitor.py &> /dev/null
 
 3 - Save crontab
 
 This will check the rsump.py process every 5 minutes and restart it if it is stopped.
 
 
 Making Line Charts of Sump Activity
@@ -243,15 +270,15 @@
 ===========
 
 If you have not done so in a while run the following command to update your Pi.
 This command updates repository information and then upgrades packages that are
 installed on your Pi.  If you did this already earlier in the instructions then
 it is not necessary to do again.
 
-    sudo apt-get update && sudo apt-get -y upgrade
+    sudo apt update && sudo apt -y upgrade
 
 
 Getting Started
 ===============
 
 These instructions will do the following
 - install the Lighttpd webserver on your Pi
@@ -259,64 +286,39 @@
 - link charts to web folder to view charts
 - configure cron to run the script to create for graphs of sump pump activity
 
 
 To view your sump pit activity install the Lighttpd webserver on your
 Raspberry Pi as follows.
 
-    sudo apt-get install lighttpd
+    sudo apt install lighttpd
 
 Copy the provided lighttpd.conf as follows;
 
 
     sudo cp /home/pi/raspi-sump/sample_config/lighttpd.conf /etc/lighttpd
 
 
 Enable directory listing for historical charts
 
     sudo lighttpd-enable-mod dir-listing
 
-Restart the web server Raspian < 10
+Restart the web server
 
     sudo /etc/init.d/lighttpd force-reload
 
-The lighttpd web server software that ships on Raspbian Buster made a change to the naming of a file for mime.types.
-There are two ways you can address this issue, only select one of them;
-
-A. Create a softlink to the new file with the old naming convention;
-    
-	cd /usr/share/lighttpd
-	sudo ln -s create-mime.conf.pl create-mime.assign.pl
-	sudo /etc/init.d/lighttpd stop
-	sudo /etc/init.d/lighttpd stop
-
-B. Modify the lighttpd.conf file with the proper entry and restart the webserver.
-
-	sudo nano /etc/lighttpd/lighttpd.conf
-    
-	Replace the following line;
-	include_shell "/usr/share/lighttpd/create-mime.assign.pl"
-    
-	With this line;
-	include_shell "/usr/share/lighttpd/create-mime.conf.pl"
-
-Save the file and restart the webserver
-
-    sudo /etc/init.d/lighttpd stop
-    sudo /etc/init.d/lighttpd start
-
 
 Create a cron job to generate an hourly graph of your sump pit activity for
 viewing on your pi webserver
 
     1 - crontab -e
 
     2 - enter line in crontab as follows;
 
-    59 * * * * /usr/local/bin/rsumpwebchart.py
+    59 * * * * /usr/local/bin/rsumpwebchart.py &> /dev/null
 
     3 - Save crontab
 
     4 - run the script manually to create the first chart
         
         rsumpwebchart.py
```

### Comparing `raspisump-1.4.1/raspisump/todaychart.py` & `raspisump-1.5/raspisump/todaychart.py`

 * *Files identical despite different names*

### Comparing `raspisump-1.4.1/raspisump/log.py` & `raspisump-1.5/raspisump/log.py`

 * *Files identical despite different names*

### Comparing `raspisump-1.4.1/raspisump/reading.py` & `raspisump-1.5/raspisump/reading.py`

 * *Files identical despite different names*

### Comparing `raspisump-1.4.1/raspisump/emailtest.py` & `raspisump-1.5/raspisump/emailtest.py`

 * *Files identical despite different names*

### Comparing `raspisump-1.4.1/raspisump/alerts.py` & `raspisump-1.5/raspisump/alerts.py`

 * *Files identical despite different names*

### Comparing `raspisump-1.4.1/raspisump/checkpid.py` & `raspisump-1.5/raspisump/checkpid.py`

 * *Files identical despite different names*

### Comparing `raspisump-1.4.1/raspisump/heartbeat.py` & `raspisump-1.5/raspisump/heartbeat.py`

 * *Files identical despite different names*

### Comparing `raspisump-1.4.1/raspisump/webchart.py` & `raspisump-1.5/raspisump/webchart.py`

 * *Files identical despite different names*

### Comparing `raspisump-1.4.1/conf/lighttpd.conf` & `raspisump-1.5/conf/lighttpd.conf`

 * *Files 1% similar despite different names*

```diff
@@ -21,9 +21,9 @@
 static-file.exclude-extensions = ( ".php", ".pl", ".fcgi" )
 
 compress.cache-dir          = "/var/cache/lighttpd/compress/"
 compress.filetype           = ( "application/javascript", "text/css", "text/html", "text/plain" )
 
 # default listening port for IPv6 falls back to the IPv4 port
 include_shell "/usr/share/lighttpd/use-ipv6.pl " + server.port
-include_shell "/usr/share/lighttpd/create-mime.assign.pl"
+include_shell "/usr/share/lighttpd/create-mime.conf.pl"
 include_shell "/usr/share/lighttpd/include-conf-enabled.pl"
```

### Comparing `raspisump-1.4.1/conf/web/css/raspi.css` & `raspisump-1.5/conf/web/css/raspi.css`

 * *Files identical despite different names*

### Comparing `raspisump-1.4.1/conf/web/css/raspi.css~` & `raspisump-1.5/conf/web/css/raspi.css~`

 * *Files identical despite different names*

### Comparing `raspisump-1.4.1/conf/web/index.html` & `raspisump-1.5/conf/web/index.html`

 * *Files identical despite different names*

### Comparing `raspisump-1.4.1/conf/web/images/logo.png` & `raspisump-1.5/conf/web/images/logo.png`

 * *Files identical despite different names*

### Comparing `raspisump-1.4.1/conf/raspisump.conf` & `raspisump-1.5/conf/raspisump.conf`

 * *Files identical despite different names*

### Comparing `raspisump-1.4.1/bin/rsump.py` & `raspisump-1.5/bin/rsump.py`

 * *Files identical despite different names*

### Comparing `raspisump-1.4.1/bin/rsumpchart.py` & `raspisump-1.5/bin/rsumpchart.py`

 * *Files identical despite different names*

### Comparing `raspisump-1.4.1/bin/rsumpwebchart.py` & `raspisump-1.5/bin/rsumpwebchart.py`

 * *Files identical despite different names*

### Comparing `raspisump-1.4.1/bin/rsumpmonitor.py` & `raspisump-1.5/bin/rsumpmonitor.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,12 +9,12 @@
 
 from raspisump import checkpid
 
 
 def main():
     '''run checkpid.py module to restart Raspi-Sump if the rsump.py process is
     stopped or has spawned multiple processes.'''
-    process = 'rsump.py'
+    process = '/usr/local/bin/rsump.py'
     checkpid.check_pid(process)
 
 if __name__ == "__main__":
     main()
```

### Comparing `raspisump-1.4.1/raspisump.egg-info/PKG-INFO` & `raspisump-1.5/raspisump.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,121 +1,109 @@
 Metadata-Version: 2.1
 Name: raspisump
-Version: 1.4.1
+Version: 1.5
 Summary: A sump pit monitoring system for Raspberry Pi
 Home-page: http://www.linuxnorth.org/raspi-sump/
+Download-URL: https://github.com/alaudet/raspi-sump/releases
 Author: Al Audet
 Author-email: alaudet@linuxnorth.org
 License: MIT License
-Download-URL: https://github.com/alaudet/raspi-sump/releases
-Description: Raspi-sump is a sump pit water level monitoring system using a Raspberry Pi and an Ultrasonic Sensor (HC-SR04).
-        
-        ![Chart](https://raspisump.linuxnorth.org/static/today.png)
-        
-        
-        Currently the system monitors the water level in your pit at defined intervals. It sends
-        email sms alerts if the water reaches a critical level, indicating a possible sump pump failure.
-        
-        # What's New
-        
-        See the [changelog](https://github.com/alaudet/raspi-sump/blob/master/changelog) for the latest information on Raspi-Sump features.
-        
-        # Supported Versions of Raspbian / Raspberry Pi OS
-        
-        Raspi-Sump is currently supported on Raspberry Pi OS (Bullseye) and Raspian (Buster and Stretch).
-        
-        Raspian 9 (Stretch) support will be discontinued in June 2022.  Please upgrade to Raspberry Pi OS 11 Bullseye if you are currently using Stretch.
-        
-        # Discord Group
-        
-        Discuss and get support from other users. Email (alaudet@linuxnorth.org) for an invite link.
-        
-        
-        # Install Dependencies
-        
-            sudo apt install python3-pip python3-rpi.gpio python3-matplotlib
-        
-        # Install Raspi-Sump
-        
-        Pip installs default to Wheels which omits some folder setup in setup.py.
-        Always use the '--no-binary :all:' option when installing or upgrading Raspi-Sump with pip.
-        
-            sudo pip3 install --no-binary :all: raspisump
-        
-        
-        # Upgrading Raspi-Sump 
-        
-        Upgrading an existing version
-        
-            sudo pip3 install -U --no-binary :all: raspisump
-        
-        This will also install the [HCSR04sensor](https://github.com/alaudet/hcsr04sensor) 
-        
-        
-        Read the configuration docs copied during setup on your pi at the following location;
-        
-            /home/pi/raspi-sump/docs
-        
-        They are also available on github https://github.com/alaudet/raspi-sump/blob/master/docs/install.md
-        
-        
-        # Upgrading from Python2 to Python3
-        
-            sudo pip uninstall raspisump
-            sudo pip3 install --no-binary :all: raspisump
-        
-        
-        Your configuration file will be preserved in /home/pi/raspi-sump/
-        
-        
-        # Python2 (End of Life was January 1, 2020)
-        
-        Python2 installs of Raspi-Sump are no longer be supported.
-        
-        
-        # More Info
-        
-        Further details provided at http://www.linuxnorth.org/raspi-sump/
-        
-        An example hourly updating graph is available for view.
-        http://www.linuxnorth.org/raspi-sump/raspi-sump-today.html
-        
-        # Disclaimer
-        
-        You are welcome to use Raspi-Sump but there is no guarantee it will work. Your house may still flood if your sump pump fails. This software comes with no warranty. See License details.
-        
-        This is not a replacement for a properly maintained water pumping system. It is one tool you can use to give yourself extra piece-of-mind.
-        
-        Best practices should include:
-        
-        * A backup pump that triggers at a slightly higher water level than your main pump.
-        * The secondary pump should be connected to a seperate dedicated electrical breaker. 
-        * You should also have a generator that can provide power should you have an extended outage during the spring or other unseasonally wet time of year.
-        * if you are building a new home, pay attention to the grade of your property, as you may be able to let gravity empty your pit for you.  That would be the best approach with a backup pump for added protection.
-        
-        Once you have done all of these things, then consider using a monitoring system like Raspi-Sump.
-        
-        # License
-        
-        MIT License.  I want you to do whatever you want with Raspi-Sump.  If you
-        improve it please let me know.
-        
-        # Contributing
-        
-        Please refer to the [Contributing Guidelines](https://github.com/alaudet/raspi-sump/blob/master/CONTRIBUTING.md) before issuing a pull request.
-        
-        # Donate
-        
-        [Your Donation is Appreciated](https://www.linuxnorth.org/donate/)
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Home Automation
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+Raspi-sump is a sump pit water level monitoring system using a Raspberry Pi and an Ultrasonic Sensor (HC-SR04).
+
+![Chart](https://raspisump.linuxnorth.org/static/today.png)
+
+
+Currently the system monitors the water level in your pit at defined intervals. It sends
+email sms alerts if the water reaches a critical level, indicating a possible sump pump failure.
+
+# What's New
+
+See the [changelog](https://github.com/alaudet/raspi-sump/blob/master/changelog) for the latest information on Raspi-Sump features.
+
+# Supported Versions of Raspbian / Raspberry Pi OS
+
+Raspi-Sump is currently supported on Raspberry Pi OS (Bullseye) and Raspian (Buster and Stretch).
+
+# Discord Group
+
+Discuss and get support from other users. Email (alaudet@linuxnorth.org) for an invite link.
+
+
+# Install Dependencies
+
+    sudo apt install python3-pip python3-rpi.gpio python3-matplotlib
+
+# Install Raspi-Sump
+
+Pip installs default to Wheels which omits some folder setup in setup.py.
+Always use the '--no-binary :all:' option when installing or upgrading Raspi-Sump with pip.
+
+    sudo pip3 install --no-binary :all: raspisump
+
+
+# Upgrading Raspi-Sump 
+
+Upgrading an existing version
+
+    sudo pip3 install -U --no-binary :all: raspisump
+
+This will also install the [HCSR04sensor](https://github.com/alaudet/hcsr04sensor) 
+
+
+Read the configuration docs copied during setup on your pi at the following location;
+
+    /home/pi/raspi-sump/docs
+
+They are also available on github https://github.com/alaudet/raspi-sump/blob/master/docs/install.md
+
+
+# Python2 (End of Life was January 1, 2020)
+
+Python2 installs of Raspi-Sump are no longer be supported.
+
+
+# More Info
+
+Further details provided at http://www.linuxnorth.org/raspi-sump/
+
+An example hourly updating graph is available for view.
+http://www.linuxnorth.org/raspi-sump/raspi-sump-today.html
+
+# Disclaimer
+
+You are welcome to use Raspi-Sump but there is no guarantee it will work. Your house may still flood if your sump pump fails. This software comes with no warranty. See License details.
+
+This is not a replacement for a properly maintained water pumping system. It is one tool you can use to give yourself extra piece-of-mind.
+
+Best practices should include:
+
+* A backup pump that triggers at a slightly higher water level than your main pump.
+* The secondary pump should be connected to a seperate dedicated electrical breaker. 
+* You should also have a generator that can provide power should you have an extended outage during the spring or other unseasonally wet time of year.
+* if you are building a new home, pay attention to the grade of your property, as you may be able to let gravity empty your pit for you.  That would be the best approach with a backup pump for added protection.
+
+Once you have done all of these things, then consider using a monitoring system like Raspi-Sump.
+
+# License
+
+MIT License.  I want you to do whatever you want with Raspi-Sump.  If you
+improve it please let me know.
+
+# Contributing
+
+Please refer to the [Contributing Guidelines](https://github.com/alaudet/raspi-sump/blob/master/CONTRIBUTING.md) before issuing a pull request.
+
+# Donate
+
+[Your Donation is Appreciated](https://www.linuxnorth.org/donate/)
```

### Comparing `raspisump-1.4.1/raspisump.egg-info/SOURCES.txt` & `raspisump-1.5/raspisump.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,11 @@
+LICENSE
 MANIFEST.in
 README.md
+VERSION
 setup.py
 bin/emailtest
 bin/rsump.py
 bin/rsumpchart.py
 bin/rsumpmonitor.py
 bin/rsumpwebchart.py
 conf/lighttpd.conf
```

