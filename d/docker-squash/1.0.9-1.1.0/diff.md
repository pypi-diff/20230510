# Comparing `tmp/docker-squash-1.0.9.tar.gz` & `tmp/docker-squash-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docker-squash-1.0.9.tar", last modified: Fri Nov 26 12:10:37 2021, max compression
+gzip compressed data, was "docker-squash-1.1.0.tar", last modified: Wed May 10 12:46:29 2023, max compression
```

## Comparing `docker-squash-1.0.9.tar` & `docker-squash-1.1.0.tar`

### file list

```diff
@@ -1,28 +1,27 @@
-drwxr-xr-x   0 goldmann  (1000) goldmann  (1000)        0 2021-11-26 12:10:37.943900 docker-squash-1.0.9/
--rw-r--r--   0 goldmann  (1000) goldmann  (1000)     1081 2019-05-09 07:50:25.000000 docker-squash-1.0.9/LICENSE
--rw-r--r--   0 goldmann  (1000) goldmann  (1000)       41 2019-05-09 07:50:25.000000 docker-squash-1.0.9/MANIFEST.in
--rw-r--r--   0 goldmann  (1000) goldmann  (1000)    15653 2021-11-26 12:10:37.943900 docker-squash-1.0.9/PKG-INFO
--rw-r--r--   0 goldmann  (1000) goldmann  (1000)    15294 2021-11-26 11:56:21.000000 docker-squash-1.0.9/README.rst
-drwxr-xr-x   0 goldmann  (1000) goldmann  (1000)        0 2021-11-26 12:10:37.942900 docker-squash-1.0.9/docker_squash/
--rw-r--r--   0 goldmann  (1000) goldmann  (1000)       64 2019-05-09 07:50:25.000000 docker-squash-1.0.9/docker_squash/__init__.py
--rw-r--r--   0 goldmann  (1000) goldmann  (1000)     4152 2021-11-24 15:45:33.000000 docker-squash-1.0.9/docker_squash/cli.py
--rw-r--r--   0 goldmann  (1000) goldmann  (1000)      132 2019-05-09 07:50:25.000000 docker-squash-1.0.9/docker_squash/errors.py
--rw-r--r--   0 goldmann  (1000) goldmann  (1000)    37574 2021-11-26 11:52:08.000000 docker-squash-1.0.9/docker_squash/image.py
-drwxr-xr-x   0 goldmann  (1000) goldmann  (1000)        0 2021-11-26 12:10:37.943900 docker-squash-1.0.9/docker_squash/lib/
--rw-r--r--   0 goldmann  (1000) goldmann  (1000)        0 2019-05-09 07:50:25.000000 docker-squash-1.0.9/docker_squash/lib/__init__.py
--rw-r--r--   0 goldmann  (1000) goldmann  (1000)     2206 2019-05-09 07:50:25.000000 docker-squash-1.0.9/docker_squash/lib/common.py
--rw-r--r--   0 goldmann  (1000) goldmann  (1000)     3925 2019-05-09 07:50:25.000000 docker-squash-1.0.9/docker_squash/lib/xtarfile.py
--rw-r--r--   0 goldmann  (1000) goldmann  (1000)     4200 2021-11-26 11:52:08.000000 docker-squash-1.0.9/docker_squash/squash.py
--rw-r--r--   0 goldmann  (1000) goldmann  (1000)     2746 2019-05-09 07:50:25.000000 docker-squash-1.0.9/docker_squash/v1_image.py
--rw-r--r--   0 goldmann  (1000) goldmann  (1000)    12213 2021-11-24 15:45:33.000000 docker-squash-1.0.9/docker_squash/v2_image.py
--rw-r--r--   0 goldmann  (1000) goldmann  (1000)       18 2021-11-26 11:57:40.000000 docker-squash-1.0.9/docker_squash/version.py
-drwxr-xr-x   0 goldmann  (1000) goldmann  (1000)        0 2021-11-26 12:10:37.943900 docker-squash-1.0.9/docker_squash.egg-info/
--rw-r--r--   0 goldmann  (1000) goldmann  (1000)    15653 2021-11-26 12:10:37.000000 docker-squash-1.0.9/docker_squash.egg-info/PKG-INFO
--rw-r--r--   0 goldmann  (1000) goldmann  (1000)      563 2021-11-26 12:10:37.000000 docker-squash-1.0.9/docker_squash.egg-info/SOURCES.txt
--rw-r--r--   0 goldmann  (1000) goldmann  (1000)        1 2021-11-26 12:10:37.000000 docker-squash-1.0.9/docker_squash.egg-info/dependency_links.txt
--rw-r--r--   0 goldmann  (1000) goldmann  (1000)       57 2021-11-26 12:10:37.000000 docker-squash-1.0.9/docker_squash.egg-info/entry_points.txt
--rw-r--r--   0 goldmann  (1000) goldmann  (1000)       11 2021-11-26 12:10:37.000000 docker-squash-1.0.9/docker_squash.egg-info/requires.txt
--rw-r--r--   0 goldmann  (1000) goldmann  (1000)       14 2021-11-26 12:10:37.000000 docker-squash-1.0.9/docker_squash.egg-info/top_level.txt
--rw-r--r--   0 goldmann  (1000) goldmann  (1000)       11 2019-05-09 07:50:25.000000 docker-squash-1.0.9/requirements.txt
--rw-r--r--   0 goldmann  (1000) goldmann  (1000)       38 2021-11-26 12:10:37.943900 docker-squash-1.0.9/setup.cfg
--rw-r--r--   0 goldmann  (1000) goldmann  (1000)      860 2019-05-09 07:50:25.000000 docker-squash-1.0.9/setup.py
+drwxr-xr-x   0 goldmann  (1000) goldmann  (1000)        0 2023-05-10 12:46:29.946259 docker-squash-1.1.0/
+-rw-r--r--   0 goldmann  (1000) goldmann  (1000)     1081 2018-08-29 09:42:24.000000 docker-squash-1.1.0/LICENSE
+-rw-r--r--   0 goldmann  (1000) goldmann  (1000)       41 2018-08-29 09:42:12.000000 docker-squash-1.1.0/MANIFEST.in
+-rw-r--r--   0 goldmann  (1000) goldmann  (1000)    15557 2023-05-10 12:46:29.946259 docker-squash-1.1.0/PKG-INFO
+-rw-r--r--   0 goldmann  (1000) goldmann  (1000)    15218 2023-05-10 12:43:33.000000 docker-squash-1.1.0/README.rst
+drwxr-xr-x   0 goldmann  (1000) goldmann  (1000)        0 2023-05-10 12:46:29.946259 docker-squash-1.1.0/docker_squash/
+-rw-r--r--   0 goldmann  (1000) goldmann  (1000)       65 2023-05-10 12:43:33.000000 docker-squash-1.1.0/docker_squash/__init__.py
+-rw-r--r--   0 goldmann  (1000) goldmann  (1000)     5161 2023-05-10 12:43:33.000000 docker-squash-1.1.0/docker_squash/cli.py
+-rw-r--r--   0 goldmann  (1000) goldmann  (1000)      132 2023-05-10 12:43:33.000000 docker-squash-1.1.0/docker_squash/errors.py
+-rw-r--r--   0 goldmann  (1000) goldmann  (1000)    38931 2023-05-10 12:43:33.000000 docker-squash-1.1.0/docker_squash/image.py
+drwxr-xr-x   0 goldmann  (1000) goldmann  (1000)        0 2023-05-10 12:46:29.946259 docker-squash-1.1.0/docker_squash/lib/
+-rw-r--r--   0 goldmann  (1000) goldmann  (1000)        0 2018-08-29 09:42:29.000000 docker-squash-1.1.0/docker_squash/lib/__init__.py
+-rw-r--r--   0 goldmann  (1000) goldmann  (1000)     2268 2023-05-10 12:43:33.000000 docker-squash-1.1.0/docker_squash/lib/common.py
+-rw-r--r--   0 goldmann  (1000) goldmann  (1000)     4611 2023-05-10 12:43:33.000000 docker-squash-1.1.0/docker_squash/squash.py
+-rw-r--r--   0 goldmann  (1000) goldmann  (1000)     2699 2023-05-10 12:43:33.000000 docker-squash-1.1.0/docker_squash/v1_image.py
+-rw-r--r--   0 goldmann  (1000) goldmann  (1000)    12371 2023-05-10 12:43:33.000000 docker-squash-1.1.0/docker_squash/v2_image.py
+-rw-r--r--   0 goldmann  (1000) goldmann  (1000)       18 2023-05-10 12:45:35.000000 docker-squash-1.1.0/docker_squash/version.py
+drwxr-xr-x   0 goldmann  (1000) goldmann  (1000)        0 2023-05-10 12:46:29.946259 docker-squash-1.1.0/docker_squash.egg-info/
+-rw-r--r--   0 goldmann  (1000) goldmann  (1000)    15557 2023-05-10 12:46:29.000000 docker-squash-1.1.0/docker_squash.egg-info/PKG-INFO
+-rw-r--r--   0 goldmann  (1000) goldmann  (1000)      543 2023-05-10 12:46:29.000000 docker-squash-1.1.0/docker_squash.egg-info/SOURCES.txt
+-rw-r--r--   0 goldmann  (1000) goldmann  (1000)        1 2023-05-10 12:46:29.000000 docker-squash-1.1.0/docker_squash.egg-info/dependency_links.txt
+-rw-r--r--   0 goldmann  (1000) goldmann  (1000)       56 2023-05-10 12:46:29.000000 docker-squash-1.1.0/docker_squash.egg-info/entry_points.txt
+-rw-r--r--   0 goldmann  (1000) goldmann  (1000)        7 2023-05-10 12:46:29.000000 docker-squash-1.1.0/docker_squash.egg-info/requires.txt
+-rw-r--r--   0 goldmann  (1000) goldmann  (1000)       14 2023-05-10 12:46:29.000000 docker-squash-1.1.0/docker_squash.egg-info/top_level.txt
+-rw-r--r--   0 goldmann  (1000) goldmann  (1000)        7 2023-05-10 12:43:33.000000 docker-squash-1.1.0/requirements.txt
+-rw-r--r--   0 goldmann  (1000) goldmann  (1000)      281 2023-05-10 12:46:29.947259 docker-squash-1.1.0/setup.cfg
+-rw-r--r--   0 goldmann  (1000) goldmann  (1000)      842 2023-05-10 12:43:33.000000 docker-squash-1.1.0/setup.py
```

### Comparing `docker-squash-1.0.9/LICENSE` & `docker-squash-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `docker-squash-1.0.9/PKG-INFO` & `docker-squash-1.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: docker-squash
-Version: 1.0.9
+Version: 1.1.0
 Summary: Docker layer squashing tool
 Home-page: https://github.com/goldmann/docker-squash
+Download-URL: https://github.com/goldmann/docker-squash/archive/1.1.0.tar.gz
 Author: Marek Goldmann
 Author-email: marek.goldmann@gmail.com
 License: MIT
-Download-URL: https://github.com/goldmann/docker-squash/archive/1.0.9.tar.gz
 Keywords: docker
-Platform: UNKNOWN
 License-File: LICENSE
 
 ``docker-squash``
 ==================
 
 .. image:: https://github.com/goldmann/docker-squash/actions/workflows/squash.yml/badge.svg
     :target: https://github.com/goldmann/docker-squash/actions/workflows/squash.yml
@@ -50,14 +49,16 @@
 
 From PyPi
 
 ::
 
     $ pip install docker-squash
 
+It is supported on Python 3.6 and above.
+
 Usage
 -----
 
 ::
 
     $ docker-squash -h
     usage: cli.py [-h] [-v] [--version] [-d] [-f FROM_LAYER] [-t TAG]
@@ -71,23 +72,29 @@
 
     optional arguments:
       -h, --help            show this help message and exit
       -v, --verbose         Verbose output
       --version             Show version and exit
       -d, --development     Does not clean up after failure for easier debugging
       -f FROM_LAYER, --from-layer FROM_LAYER
-                            ID of the layer or image ID or image name. If not
-                            specified will squash all layers in the image
-      -t TAG, --tag TAG     Specify the tag to be used for the new image. By
-                            default it'll be set to 'image' argument
+                            Number of layers to squash or ID of the layer (or image ID or image name) to squash from.
+                            In case the provided value is an integer, specified number of layers will be squashed.
+                            Every layer in the image will be squashed if the parameter is not provided.
+      -t TAG, --tag TAG     Specify the tag to be used for the new image. If not specified no tag will be applied
+      -m MESSAGE, --message MESSAGE
+                            Specify a commit message (comment) for the new image.
+      -c, --cleanup         Remove source image from Docker after squashing
       --tmp-dir TMP_DIR     Temporary directory to be created and used
       --output-path OUTPUT_PATH
-                            Path where the image should be stored after squashing.
-                            If not provided, image will be loaded into Docker
-                            daemon
+                            Path where the image may be stored after squashing.
+      --load-image [LOAD_IMAGE]
+                            Whether to load the image into Docker daemon after squashing
+                            Default: true
+
+Note that environment variables may be set as documented in `here <docs/environment_variables.adoc>`_.
 
 License
 -------
 
 MIT
 
 Examples
@@ -95,34 +102,34 @@
 
 We start with image like this:
 
 ::
 
     $ docker history jboss/wildfly:latest
     IMAGE               CREATED             CREATED BY                                      SIZE                COMMENT
-    25954e6d2300        3 weeks ago         /bin/sh -c #(nop) CMD ["/opt/jboss/wildfly/bi   0 B                 
-    5ae69cb454a5        3 weeks ago         /bin/sh -c #(nop) EXPOSE 8080/tcp               0 B                 
-    dc24712f35c4        3 weeks ago         /bin/sh -c #(nop) ENV LAUNCH_JBOSS_IN_BACKGRO   0 B                 
-    d929129d4c8e        3 weeks ago         /bin/sh -c cd $HOME     && curl -O https://do   160.8 MB            
-    b8fa3caf7d6d        3 weeks ago         /bin/sh -c #(nop) ENV JBOSS_HOME=/opt/jboss/w   0 B                 
-    38b8f85e74bf        3 weeks ago         /bin/sh -c #(nop) ENV WILDFLY_SHA1=c0dd7552c5   0 B                 
-    ae79b646b9a9        3 weeks ago         /bin/sh -c #(nop) ENV WILDFLY_VERSION=10.0.0.   0 B                 
-    2b4606dc9dc7        3 weeks ago         /bin/sh -c #(nop) ENV JAVA_HOME=/usr/lib/jvm/   0 B                 
-    118fa9e33576        3 weeks ago         /bin/sh -c #(nop) USER [jboss]                  0 B                 
-    5f7e8f36c3bb        3 weeks ago         /bin/sh -c yum -y install java-1.8.0-openjdk-   197.4 MB            
-    3d4d0228f161        3 weeks ago         /bin/sh -c #(nop) USER [root]                   0 B                 
-    f7ab4ea19708        3 weeks ago         /bin/sh -c #(nop) MAINTAINER Marek Goldmann <   0 B                 
-    4bb15f3b6977        3 weeks ago         /bin/sh -c #(nop) USER [jboss]                  0 B                 
-    5dc1e49f4361        3 weeks ago         /bin/sh -c #(nop) WORKDIR /opt/jboss            0 B                 
-    7f0f9eb31174        3 weeks ago         /bin/sh -c groupadd -r jboss -g 1000 && usera   4.349 kB            
-    bd515f044af7        3 weeks ago         /bin/sh -c yum update -y && yum -y install xm   25.18 MB            
-    b78336099045        3 weeks ago         /bin/sh -c #(nop) MAINTAINER Marek Goldmann <   0 B                 
-    4816a298548c        3 weeks ago         /bin/sh -c #(nop) CMD ["/bin/bash"]             0 B                 
-    6ee235cf4473        3 weeks ago         /bin/sh -c #(nop) LABEL name=CentOS Base Imag   0 B                 
-    474c2ee77fa3        3 weeks ago         /bin/sh -c #(nop) ADD file:72852fc7626d233343   196.6 MB            
+    25954e6d2300        3 weeks ago         /bin/sh -c #(nop) CMD ["/opt/jboss/wildfly/bi   0 B
+    5ae69cb454a5        3 weeks ago         /bin/sh -c #(nop) EXPOSE 8080/tcp               0 B
+    dc24712f35c4        3 weeks ago         /bin/sh -c #(nop) ENV LAUNCH_JBOSS_IN_BACKGRO   0 B
+    d929129d4c8e        3 weeks ago         /bin/sh -c cd $HOME     && curl -O https://do   160.8 MB
+    b8fa3caf7d6d        3 weeks ago         /bin/sh -c #(nop) ENV JBOSS_HOME=/opt/jboss/w   0 B
+    38b8f85e74bf        3 weeks ago         /bin/sh -c #(nop) ENV WILDFLY_SHA1=c0dd7552c5   0 B
+    ae79b646b9a9        3 weeks ago         /bin/sh -c #(nop) ENV WILDFLY_VERSION=10.0.0.   0 B
+    2b4606dc9dc7        3 weeks ago         /bin/sh -c #(nop) ENV JAVA_HOME=/usr/lib/jvm/   0 B
+    118fa9e33576        3 weeks ago         /bin/sh -c #(nop) USER [jboss]                  0 B
+    5f7e8f36c3bb        3 weeks ago         /bin/sh -c yum -y install java-1.8.0-openjdk-   197.4 MB
+    3d4d0228f161        3 weeks ago         /bin/sh -c #(nop) USER [root]                   0 B
+    f7ab4ea19708        3 weeks ago         /bin/sh -c #(nop) MAINTAINER Marek Goldmann <   0 B
+    4bb15f3b6977        3 weeks ago         /bin/sh -c #(nop) USER [jboss]                  0 B
+    5dc1e49f4361        3 weeks ago         /bin/sh -c #(nop) WORKDIR /opt/jboss            0 B
+    7f0f9eb31174        3 weeks ago         /bin/sh -c groupadd -r jboss -g 1000 && usera   4.349 kB
+    bd515f044af7        3 weeks ago         /bin/sh -c yum update -y && yum -y install xm   25.18 MB
+    b78336099045        3 weeks ago         /bin/sh -c #(nop) MAINTAINER Marek Goldmann <   0 B
+    4816a298548c        3 weeks ago         /bin/sh -c #(nop) CMD ["/bin/bash"]             0 B
+    6ee235cf4473        3 weeks ago         /bin/sh -c #(nop) LABEL name=CentOS Base Imag   0 B
+    474c2ee77fa3        3 weeks ago         /bin/sh -c #(nop) ADD file:72852fc7626d233343   196.6 MB
     1544084fad81        6 months ago        /bin/sh -c #(nop) MAINTAINER The CentOS Proje   0 B
 
 And we want to squash all the layers down to layer ``4bb15f3b6977``.
 
 ::
 
     $ docker-squash -f 4bb15f3b6977 -t jboss/wildfly:squashed jboss/wildfly:latest
@@ -156,23 +163,23 @@
 
 We can now confirm the layer structure:
 
 ::
 
     $ docker history jboss/wildfly:squashed
     IMAGE               CREATED             CREATED BY                                      SIZE                COMMENT
-    52255e75d3eb        40 seconds ago                                                      358.2 MB            
-    4bb15f3b6977        3 weeks ago         /bin/sh -c #(nop) USER [jboss]                  0 B                 
-    5dc1e49f4361        3 weeks ago         /bin/sh -c #(nop) WORKDIR /opt/jboss            0 B                 
-    7f0f9eb31174        3 weeks ago         /bin/sh -c groupadd -r jboss -g 1000 && usera   4.349 kB            
-    bd515f044af7        3 weeks ago         /bin/sh -c yum update -y && yum -y install xm   25.18 MB            
-    b78336099045        3 weeks ago         /bin/sh -c #(nop) MAINTAINER Marek Goldmann <   0 B                 
-    4816a298548c        3 weeks ago         /bin/sh -c #(nop) CMD ["/bin/bash"]             0 B                 
-    6ee235cf4473        3 weeks ago         /bin/sh -c #(nop) LABEL name=CentOS Base Imag   0 B                 
-    474c2ee77fa3        3 weeks ago         /bin/sh -c #(nop) ADD file:72852fc7626d233343   196.6 MB            
+    52255e75d3eb        40 seconds ago                                                      358.2 MB
+    4bb15f3b6977        3 weeks ago         /bin/sh -c #(nop) USER [jboss]                  0 B
+    5dc1e49f4361        3 weeks ago         /bin/sh -c #(nop) WORKDIR /opt/jboss            0 B
+    7f0f9eb31174        3 weeks ago         /bin/sh -c groupadd -r jboss -g 1000 && usera   4.349 kB
+    bd515f044af7        3 weeks ago         /bin/sh -c yum update -y && yum -y install xm   25.18 MB
+    b78336099045        3 weeks ago         /bin/sh -c #(nop) MAINTAINER Marek Goldmann <   0 B
+    4816a298548c        3 weeks ago         /bin/sh -c #(nop) CMD ["/bin/bash"]             0 B
+    6ee235cf4473        3 weeks ago         /bin/sh -c #(nop) LABEL name=CentOS Base Imag   0 B
+    474c2ee77fa3        3 weeks ago         /bin/sh -c #(nop) ADD file:72852fc7626d233343   196.6 MB
     1544084fad81        6 months ago        /bin/sh -c #(nop) MAINTAINER The CentOS Proje   0 B
 
 Other option is to specify how many layers (counting from the newest layer) we want to squash.\
 Let's squash last 10 layers from the ``jboss/wildfly:latest`` image:
 
 ::
 
@@ -205,22 +212,19 @@
 
 Let's confirm the image structure now:
 
 ::
 
     $ docker history jboss/wildfly:squashed
     IMAGE               CREATED             CREATED BY                                      SIZE                COMMENT
-    fde7edd2e568        32 seconds ago                                                      358.2 MB            
-    3d4d0228f161        3 weeks ago         /bin/sh -c #(nop) USER [root]                   0 B                 
-    f7ab4ea19708        3 weeks ago         /bin/sh -c #(nop) MAINTAINER Marek Goldmann <   0 B                 
-    4bb15f3b6977        3 weeks ago         /bin/sh -c #(nop) USER [jboss]                  0 B                 
-    5dc1e49f4361        3 weeks ago         /bin/sh -c #(nop) WORKDIR /opt/jboss            0 B                 
-    7f0f9eb31174        3 weeks ago         /bin/sh -c groupadd -r jboss -g 1000 && usera   4.349 kB            
-    bd515f044af7        3 weeks ago         /bin/sh -c yum update -y && yum -y install xm   25.18 MB            
-    b78336099045        3 weeks ago         /bin/sh -c #(nop) MAINTAINER Marek Goldmann <   0 B                 
-    4816a298548c        3 weeks ago         /bin/sh -c #(nop) CMD ["/bin/bash"]             0 B                 
-    6ee235cf4473        3 weeks ago         /bin/sh -c #(nop) LABEL name=CentOS Base Imag   0 B                 
-    474c2ee77fa3        3 weeks ago         /bin/sh -c #(nop) ADD file:72852fc7626d233343   196.6 MB            
+    fde7edd2e568        32 seconds ago                                                      358.2 MB
+    3d4d0228f161        3 weeks ago         /bin/sh -c #(nop) USER [root]                   0 B
+    f7ab4ea19708        3 weeks ago         /bin/sh -c #(nop) MAINTAINER Marek Goldmann <   0 B
+    4bb15f3b6977        3 weeks ago         /bin/sh -c #(nop) USER [jboss]                  0 B
+    5dc1e49f4361        3 weeks ago         /bin/sh -c #(nop) WORKDIR /opt/jboss            0 B
+    7f0f9eb31174        3 weeks ago         /bin/sh -c groupadd -r jboss -g 1000 && usera   4.349 kB
+    bd515f044af7        3 weeks ago         /bin/sh -c yum update -y && yum -y install xm   25.18 MB
+    b78336099045        3 weeks ago         /bin/sh -c #(nop) MAINTAINER Marek Goldmann <   0 B
+    4816a298548c        3 weeks ago         /bin/sh -c #(nop) CMD ["/bin/bash"]             0 B
+    6ee235cf4473        3 weeks ago         /bin/sh -c #(nop) LABEL name=CentOS Base Imag   0 B
+    474c2ee77fa3        3 weeks ago         /bin/sh -c #(nop) ADD file:72852fc7626d233343   196.6 MB
     1544084fad81        6 months ago        /bin/sh -c #(nop) MAINTAINER The CentOS Proje   0 B
-
-
-
```

### Comparing `docker-squash-1.0.9/README.rst` & `docker-squash-1.1.0/docker_squash.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,956 +1,973 @@
-00000000: 6060 646f 636b 6572 2d73 7175 6173 6860  ``docker-squash`
-00000010: 600a 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  `.==============
-00000020: 3d3d 3d3d 0a0a 2e2e 2069 6d61 6765 3a3a  ====.... image::
-00000030: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
-00000040: 636f 6d2f 676f 6c64 6d61 6e6e 2f64 6f63  com/goldmann/doc
-00000050: 6b65 722d 7371 7561 7368 2f61 6374 696f  ker-squash/actio
-00000060: 6e73 2f77 6f72 6b66 6c6f 7773 2f73 7175  ns/workflows/squ
-00000070: 6173 682e 796d 6c2f 6261 6467 652e 7376  ash.yml/badge.sv
-00000080: 670a 2020 2020 3a74 6172 6765 743a 2068  g.    :target: h
-00000090: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-000000a0: 6d2f 676f 6c64 6d61 6e6e 2f64 6f63 6b65  m/goldmann/docke
-000000b0: 722d 7371 7561 7368 2f61 6374 696f 6e73  r-squash/actions
-000000c0: 2f77 6f72 6b66 6c6f 7773 2f73 7175 6173  /workflows/squas
-000000d0: 682e 796d 6c0a 0a54 6865 2070 726f 626c  h.yml..The probl
-000000e0: 656d 0a2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a0a  em.-----------..
-000000f0: 446f 636b 6572 2063 7265 6174 6573 206d  Docker creates m
-00000100: 616e 7920 6c61 7965 7273 2077 6869 6c65  any layers while
-00000110: 2062 7569 6c64 696e 6720 7468 6520 696d   building the im
-00000120: 6167 652e 2053 6f6d 6574 696d 6573 2069  age. Sometimes i
-00000130: 7427 7320 6e6f 7420 6e65 6365 7373 6172  t's not necessar
-00000140: 7920 6f72 2064 6573 6972 6561 626c 650a  y or desireable.
-00000150: 746f 2068 6176 6520 7468 656d 2069 6e20  to have them in 
-00000160: 7468 6520 696d 6167 652e 2046 6f72 2065  the image. For e
-00000170: 7861 6d70 6c65 2061 2044 6f63 6b65 7266  xample a Dockerf
-00000180: 696c 6520 6041 4444 6020 696e 7374 7275  ile `ADD` instru
-00000190: 6374 696f 6e20 6372 6561 7465 7320 6120  ction creates a 
-000001a0: 7369 6e67 6c65 206c 6179 6572 0a77 6974  single layer.wit
-000001b0: 6820 6669 6c65 7320 796f 7520 7761 6e74  h files you want
-000001c0: 2074 6f20 6d61 6b65 2061 7661 696c 6162   to make availab
-000001d0: 6c65 2069 6e20 7468 6520 696d 6167 652e  le in the image.
-000001e0: 2054 6865 2070 726f 626c 656d 2061 7269   The problem ari
-000001f0: 7365 7320 7768 656e 2074 6865 7365 2066  ses when these f
-00000200: 696c 6573 2061 7265 0a6f 6e6c 7920 7465  iles are.only te
-00000210: 6d70 6f72 6172 7920 6669 6c65 7320 2866  mporary files (f
-00000220: 6f72 2065 7861 6d70 6c65 2070 726f 6475  or example produ
-00000230: 6374 2064 6973 7472 6962 7574 696f 6e20  ct distribution 
-00000240: 7468 6174 2079 6f75 2077 616e 7420 746f  that you want to
-00000250: 2075 6e70 6163 6b29 2e20 446f 636b 6572   unpack). Docker
-00000260: 2077 696c 6c0a 6361 7272 7920 7468 6973   will.carry this
-00000270: 2075 6e6e 6563 6573 7361 7279 206c 6179   unnecessary lay
-00000280: 6572 2061 6c77 6179 7320 7769 7468 2074  er always with t
-00000290: 6865 2069 6d61 6765 2c20 6576 656e 2069  he image, even i
-000002a0: 6620 796f 7520 6465 6c65 7465 2074 6865  f you delete the
-000002b0: 7365 2066 696c 6573 2069 6e20 6e65 7874  se files in next
-000002c0: 0a6c 6179 6572 2e20 5468 6973 2061 2077  .layer. This a w
-000002d0: 6173 7465 206f 6620 7469 6d65 2028 6d6f  aste of time (mo
-000002e0: 7265 2064 6174 6120 746f 2070 7573 682f  re data to push/
-000002f0: 6c6f 6164 2f73 6176 6529 2061 6e64 2072  load/save) and r
-00000300: 6573 6f75 7263 6573 2028 6269 6767 6572  esources (bigger
-00000310: 2069 6d61 6765 292e 0a0a 5371 7561 7368   image)...Squash
-00000320: 696e 6720 6865 6c70 7320 7769 7468 206f  ing helps with o
-00000330: 7267 616e 697a 696e 6720 696d 6167 6573  rganizing images
-00000340: 2069 6e20 6c6f 6769 6361 6c20 6c61 7965   in logical laye
-00000350: 7273 2e20 496e 7374 6561 6420 6f66 0a68  rs. Instead of.h
-00000360: 6176 696e 6720 616e 2069 6d61 6765 2077  aving an image w
-00000370: 6974 6820 6d75 6c74 6970 6c65 2028 696e  ith multiple (in
-00000380: 2061 6c6d 6f73 7420 616c 6c20 6361 7365   almost all case
-00000390: 7329 2075 6e6e 6563 6573 7361 7279 206c  s) unnecessary l
-000003a0: 6179 6572 7320 2d0a 7765 2063 616e 2063  ayers -.we can c
-000003b0: 6f6e 7472 6f6c 2074 6865 2073 7472 7563  ontrol the struc
-000003c0: 7475 7265 206f 6620 7468 6520 696d 6167  ture of the imag
-000003d0: 652e 0a0a 4665 6174 7572 6573 0a2d 2d2d  e...Features.---
-000003e0: 2d2d 2d2d 2d0a 0a2d 2043 616e 2073 7175  -----..- Can squ
-000003f0: 6173 6820 6c61 7374 206e 206c 6179 6572  ash last n layer
-00000400: 7320 6672 6f6d 2061 6e20 696d 6167 650a  s from an image.
-00000410: 2d20 4361 6e20 7371 7561 7368 2066 726f  - Can squash fro
-00000420: 6d20 6120 7365 6c65 6374 6564 206c 6179  m a selected lay
-00000430: 6572 2074 6f20 7468 6520 656e 6420 286e  er to the end (n
-00000440: 6f74 2061 6c77 6179 7320 706f 7373 6962  ot always possib
-00000450: 6c65 2c20 6465 7065 6e64 7320 6f6e 2074  le, depends on t
-00000460: 6865 2069 6d61 6765 290a 2d20 5375 7070  he image).- Supp
-00000470: 6f72 7420 666f 7220 446f 636b 6572 2031  ort for Docker 1
-00000480: 2e39 206f 7220 6e65 7765 7220 286f 6c64  .9 or newer (old
-00000490: 6572 2072 656c 6561 7365 7320 6d61 7920  er releases may 
-000004a0: 7275 6e20 7065 7266 6563 746c 7920 6669  run perfectly fi
-000004b0: 6e65 2074 6f6f 2c20 7472 7920 6974 2129  ne too, try it!)
-000004c0: 0a2d 2053 7175 6173 6865 6420 696d 6167  .- Squashed imag
-000004d0: 6520 6361 6e20 6265 206c 6f61 6465 6420  e can be loaded 
-000004e0: 6261 636b 2074 6f20 7468 6520 446f 636b  back to the Dock
-000004f0: 6572 2064 6165 6d6f 6e20 6f72 2073 746f  er daemon or sto
-00000500: 7265 6420 6173 2074 6172 2061 7263 6869  red as tar archi
-00000510: 7665 2073 6f6d 6577 6865 7265 0a0a 496e  ve somewhere..In
-00000520: 7374 616c 6c61 7469 6f6e 0a2d 2d2d 2d2d  stallation.-----
-00000530: 2d2d 2d2d 2d2d 2d0a 0a46 726f 6d20 736f  -------..From so
-00000540: 7572 6365 2063 6f64 650a 0a3a 3a0a 0a20  urce code..::.. 
-00000550: 2020 2024 2070 6970 2069 6e73 7461 6c6c     $ pip install
-00000560: 202d 2d75 7365 7220 6874 7470 733a 2f2f   --user https://
-00000570: 6769 7468 7562 2e63 6f6d 2f67 6f6c 646d  github.com/goldm
-00000580: 616e 6e2f 646f 636b 6572 2d73 7175 6173  ann/docker-squas
-00000590: 682f 6172 6368 6976 652f 6d61 7374 6572  h/archive/master
-000005a0: 2e7a 6970 0a0a 4672 6f6d 2050 7950 690a  .zip..From PyPi.
-000005b0: 0a3a 3a0a 0a20 2020 2024 2070 6970 2069  .::..    $ pip i
-000005c0: 6e73 7461 6c6c 2064 6f63 6b65 722d 7371  nstall docker-sq
-000005d0: 7561 7368 0a0a 5573 6167 650a 2d2d 2d2d  uash..Usage.----
-000005e0: 2d0a 0a3a 3a0a 0a20 2020 2024 2064 6f63  -..::..    $ doc
-000005f0: 6b65 722d 7371 7561 7368 202d 680a 2020  ker-squash -h.  
-00000600: 2020 7573 6167 653a 2063 6c69 2e70 7920    usage: cli.py 
-00000610: 5b2d 685d 205b 2d76 5d20 5b2d 2d76 6572  [-h] [-v] [--ver
-00000620: 7369 6f6e 5d20 5b2d 645d 205b 2d66 2046  sion] [-d] [-f F
-00000630: 524f 4d5f 4c41 5945 525d 205b 2d74 2054  ROM_LAYER] [-t T
-00000640: 4147 5d0a 2020 2020 2020 2020 2020 2020  AG].            
-00000650: 2020 2020 2020 5b2d 2d74 6d70 2d64 6972        [--tmp-dir
-00000660: 2054 4d50 5f44 4952 5d20 5b2d 2d6f 7574   TMP_DIR] [--out
-00000670: 7075 742d 7061 7468 204f 5554 5055 545f  put-path OUTPUT_
-00000680: 5041 5448 5d0a 2020 2020 2020 2020 2020  PATH].          
-00000690: 2020 2020 2020 2020 696d 6167 650a 0a20          image.. 
-000006a0: 2020 2044 6f63 6b65 7220 6c61 7965 7220     Docker layer 
-000006b0: 7371 7561 7368 696e 6720 746f 6f6c 0a0a  squashing tool..
-000006c0: 2020 2020 706f 7369 7469 6f6e 616c 2061      positional a
-000006d0: 7267 756d 656e 7473 3a0a 2020 2020 2020  rguments:.      
-000006e0: 696d 6167 6520 2020 2020 2020 2020 2020  image           
-000006f0: 2020 2020 2020 496d 6167 6520 746f 2062        Image to b
-00000700: 6520 7371 7561 7368 6564 0a0a 2020 2020  e squashed..    
-00000710: 6f70 7469 6f6e 616c 2061 7267 756d 656e  optional argumen
-00000720: 7473 3a0a 2020 2020 2020 2d68 2c20 2d2d  ts:.      -h, --
-00000730: 6865 6c70 2020 2020 2020 2020 2020 2020  help            
-00000740: 7368 6f77 2074 6869 7320 6865 6c70 206d  show this help m
-00000750: 6573 7361 6765 2061 6e64 2065 7869 740a  essage and exit.
-00000760: 2020 2020 2020 2d76 2c20 2d2d 7665 7262        -v, --verb
-00000770: 6f73 6520 2020 2020 2020 2020 5665 7262  ose         Verb
-00000780: 6f73 6520 6f75 7470 7574 0a20 2020 2020  ose output.     
-00000790: 202d 2d76 6572 7369 6f6e 2020 2020 2020   --version      
-000007a0: 2020 2020 2020 2053 686f 7720 7665 7273         Show vers
-000007b0: 696f 6e20 616e 6420 6578 6974 0a20 2020  ion and exit.   
-000007c0: 2020 202d 642c 202d 2d64 6576 656c 6f70     -d, --develop
-000007d0: 6d65 6e74 2020 2020 2044 6f65 7320 6e6f  ment     Does no
-000007e0: 7420 636c 6561 6e20 7570 2061 6674 6572  t clean up after
-000007f0: 2066 6169 6c75 7265 2066 6f72 2065 6173   failure for eas
-00000800: 6965 7220 6465 6275 6767 696e 670a 2020  ier debugging.  
-00000810: 2020 2020 2d66 2046 524f 4d5f 4c41 5945      -f FROM_LAYE
-00000820: 522c 202d 2d66 726f 6d2d 6c61 7965 7220  R, --from-layer 
-00000830: 4652 4f4d 5f4c 4159 4552 0a20 2020 2020  FROM_LAYER.     
-00000840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000850: 2020 2020 2020 2049 4420 6f66 2074 6865         ID of the
-00000860: 206c 6179 6572 206f 7220 696d 6167 6520   layer or image 
-00000870: 4944 206f 7220 696d 6167 6520 6e61 6d65  ID or image name
-00000880: 2e20 4966 206e 6f74 0a20 2020 2020 2020  . If not.       
-00000890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000008a0: 2020 2020 2073 7065 6369 6669 6564 2077       specified w
-000008b0: 696c 6c20 7371 7561 7368 2061 6c6c 206c  ill squash all l
-000008c0: 6179 6572 7320 696e 2074 6865 2069 6d61  ayers in the ima
-000008d0: 6765 0a20 2020 2020 202d 7420 5441 472c  ge.      -t TAG,
-000008e0: 202d 2d74 6167 2054 4147 2020 2020 2053   --tag TAG     S
-000008f0: 7065 6369 6679 2074 6865 2074 6167 2074  pecify the tag t
-00000900: 6f20 6265 2075 7365 6420 666f 7220 7468  o be used for th
-00000910: 6520 6e65 7720 696d 6167 652e 2042 790a  e new image. By.
-00000920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000930: 2020 2020 2020 2020 2020 2020 6465 6661              defa
-00000940: 756c 7420 6974 276c 6c20 6265 2073 6574  ult it'll be set
-00000950: 2074 6f20 2769 6d61 6765 2720 6172 6775   to 'image' argu
-00000960: 6d65 6e74 0a20 2020 2020 202d 2d74 6d70  ment.      --tmp
-00000970: 2d64 6972 2054 4d50 5f44 4952 2020 2020  -dir TMP_DIR    
-00000980: 2054 656d 706f 7261 7279 2064 6972 6563   Temporary direc
-00000990: 746f 7279 2074 6f20 6265 2063 7265 6174  tory to be creat
-000009a0: 6564 2061 6e64 2075 7365 640a 2020 2020  ed and used.    
-000009b0: 2020 2d2d 6f75 7470 7574 2d70 6174 6820    --output-path 
-000009c0: 4f55 5450 5554 5f50 4154 480a 2020 2020  OUTPUT_PATH.    
-000009d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000009e0: 2020 2020 2020 2020 5061 7468 2077 6865          Path whe
-000009f0: 7265 2074 6865 2069 6d61 6765 2073 686f  re the image sho
-00000a00: 756c 6420 6265 2073 746f 7265 6420 6166  uld be stored af
-00000a10: 7465 7220 7371 7561 7368 696e 672e 0a20  ter squashing.. 
-00000a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000a30: 2020 2020 2020 2020 2020 2049 6620 6e6f             If no
-00000a40: 7420 7072 6f76 6964 6564 2c20 696d 6167  t provided, imag
-00000a50: 6520 7769 6c6c 2062 6520 6c6f 6164 6564  e will be loaded
-00000a60: 2069 6e74 6f20 446f 636b 6572 0a20 2020   into Docker.   
-00000a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000a80: 2020 2020 2020 2020 2064 6165 6d6f 6e0a           daemon.
-00000a90: 0a4c 6963 656e 7365 0a2d 2d2d 2d2d 2d2d  .License.-------
-00000aa0: 0a0a 4d49 540a 0a45 7861 6d70 6c65 730a  ..MIT..Examples.
-00000ab0: 2d2d 2d2d 2d2d 2d2d 0a0a 5765 2073 7461  --------..We sta
-00000ac0: 7274 2077 6974 6820 696d 6167 6520 6c69  rt with image li
-00000ad0: 6b65 2074 6869 733a 0a0a 3a3a 0a0a 2020  ke this:..::..  
-00000ae0: 2020 2420 646f 636b 6572 2068 6973 746f    $ docker histo
-00000af0: 7279 206a 626f 7373 2f77 696c 6466 6c79  ry jboss/wildfly
-00000b00: 3a6c 6174 6573 740a 2020 2020 494d 4147  :latest.    IMAG
-00000b10: 4520 2020 2020 2020 2020 2020 2020 2020  E               
-00000b20: 4352 4541 5445 4420 2020 2020 2020 2020  CREATED         
-00000b30: 2020 2020 4352 4541 5445 4420 4259 2020      CREATED BY  
-00000b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000b60: 2020 2020 5349 5a45 2020 2020 2020 2020      SIZE        
-00000b70: 2020 2020 2020 2020 434f 4d4d 454e 540a          COMMENT.
-00000b80: 2020 2020 3235 3935 3465 3664 3233 3030      25954e6d2300
-00000b90: 2020 2020 2020 2020 3320 7765 656b 7320          3 weeks 
-00000ba0: 6167 6f20 2020 2020 2020 2020 2f62 696e  ago         /bin
-00000bb0: 2f73 6820 2d63 2023 286e 6f70 2920 434d  /sh -c #(nop) CM
-00000bc0: 4420 5b22 2f6f 7074 2f6a 626f 7373 2f77  D ["/opt/jboss/w
-00000bd0: 696c 6466 6c79 2f62 6920 2020 3020 4220  ildfly/bi   0 B 
-00000be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000bf0: 0a20 2020 2035 6165 3639 6362 3435 3461  .    5ae69cb454a
-00000c00: 3520 2020 2020 2020 2033 2077 6565 6b73  5        3 weeks
-00000c10: 2061 676f 2020 2020 2020 2020 202f 6269   ago         /bi
-00000c20: 6e2f 7368 202d 6320 2328 6e6f 7029 2045  n/sh -c #(nop) E
-00000c30: 5850 4f53 4520 3830 3830 2f74 6370 2020  XPOSE 8080/tcp  
-00000c40: 2020 2020 2020 2020 2020 2020 2030 2042               0 B
-00000c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000c60: 200a 2020 2020 6463 3234 3731 3266 3335   .    dc24712f35
-00000c70: 6334 2020 2020 2020 2020 3320 7765 656b  c4        3 week
-00000c80: 7320 6167 6f20 2020 2020 2020 2020 2f62  s ago         /b
-00000c90: 696e 2f73 6820 2d63 2023 286e 6f70 2920  in/sh -c #(nop) 
-00000ca0: 454e 5620 4c41 554e 4348 5f4a 424f 5353  ENV LAUNCH_JBOSS
-00000cb0: 5f49 4e5f 4241 434b 4752 4f20 2020 3020  _IN_BACKGRO   0 
-00000cc0: 4220 2020 2020 2020 2020 2020 2020 2020  B               
-00000cd0: 2020 0a20 2020 2064 3932 3931 3239 6434    .    d929129d4
-00000ce0: 6338 6520 2020 2020 2020 2033 2077 6565  c8e        3 wee
-00000cf0: 6b73 2061 676f 2020 2020 2020 2020 202f  ks ago         /
-00000d00: 6269 6e2f 7368 202d 6320 6364 2024 484f  bin/sh -c cd $HO
-00000d10: 4d45 2020 2020 2026 2620 6375 726c 202d  ME     && curl -
-00000d20: 4f20 6874 7470 733a 2f2f 646f 2020 2031  O https://do   1
-00000d30: 3630 2e38 204d 4220 2020 2020 2020 2020  60.8 MB         
-00000d40: 2020 200a 2020 2020 6238 6661 3363 6166     .    b8fa3caf
-00000d50: 3764 3664 2020 2020 2020 2020 3320 7765  7d6d        3 we
-00000d60: 656b 7320 6167 6f20 2020 2020 2020 2020  eks ago         
-00000d70: 2f62 696e 2f73 6820 2d63 2023 286e 6f70  /bin/sh -c #(nop
-00000d80: 2920 454e 5620 4a42 4f53 535f 484f 4d45  ) ENV JBOSS_HOME
-00000d90: 3d2f 6f70 742f 6a62 6f73 732f 7720 2020  =/opt/jboss/w   
-00000da0: 3020 4220 2020 2020 2020 2020 2020 2020  0 B             
-00000db0: 2020 2020 0a20 2020 2033 3862 3866 3835      .    38b8f85
-00000dc0: 6537 3462 6620 2020 2020 2020 2033 2077  e74bf        3 w
-00000dd0: 6565 6b73 2061 676f 2020 2020 2020 2020  eeks ago        
-00000de0: 202f 6269 6e2f 7368 202d 6320 2328 6e6f   /bin/sh -c #(no
-00000df0: 7029 2045 4e56 2057 494c 4446 4c59 5f53  p) ENV WILDFLY_S
-00000e00: 4841 313d 6330 6464 3735 3532 6335 2020  HA1=c0dd7552c5  
-00000e10: 2030 2042 2020 2020 2020 2020 2020 2020   0 B            
-00000e20: 2020 2020 200a 2020 2020 6165 3739 6236       .    ae79b6
-00000e30: 3436 6239 6139 2020 2020 2020 2020 3320  46b9a9        3 
-00000e40: 7765 656b 7320 6167 6f20 2020 2020 2020  weeks ago       
-00000e50: 2020 2f62 696e 2f73 6820 2d63 2023 286e    /bin/sh -c #(n
-00000e60: 6f70 2920 454e 5620 5749 4c44 464c 595f  op) ENV WILDFLY_
-00000e70: 5645 5253 494f 4e3d 3130 2e30 2e30 2e20  VERSION=10.0.0. 
-00000e80: 2020 3020 4220 2020 2020 2020 2020 2020    0 B           
-00000e90: 2020 2020 2020 0a20 2020 2032 6234 3630        .    2b460
-00000ea0: 3664 6339 6463 3720 2020 2020 2020 2033  6dc9dc7        3
-00000eb0: 2077 6565 6b73 2061 676f 2020 2020 2020   weeks ago      
-00000ec0: 2020 202f 6269 6e2f 7368 202d 6320 2328     /bin/sh -c #(
-00000ed0: 6e6f 7029 2045 4e56 204a 4156 415f 484f  nop) ENV JAVA_HO
-00000ee0: 4d45 3d2f 7573 722f 6c69 622f 6a76 6d2f  ME=/usr/lib/jvm/
-00000ef0: 2020 2030 2042 2020 2020 2020 2020 2020     0 B          
-00000f00: 2020 2020 2020 200a 2020 2020 3131 3866         .    118f
-00000f10: 6139 6533 3335 3736 2020 2020 2020 2020  a9e33576        
-00000f20: 3320 7765 656b 7320 6167 6f20 2020 2020  3 weeks ago     
-00000f30: 2020 2020 2f62 696e 2f73 6820 2d63 2023      /bin/sh -c #
-00000f40: 286e 6f70 2920 5553 4552 205b 6a62 6f73  (nop) USER [jbos
-00000f50: 735d 2020 2020 2020 2020 2020 2020 2020  s]              
-00000f60: 2020 2020 3020 4220 2020 2020 2020 2020      0 B         
-00000f70: 2020 2020 2020 2020 0a20 2020 2035 6637          .    5f7
-00000f80: 6538 6633 3663 3362 6220 2020 2020 2020  e8f36c3bb       
-00000f90: 2033 2077 6565 6b73 2061 676f 2020 2020   3 weeks ago    
-00000fa0: 2020 2020 202f 6269 6e2f 7368 202d 6320       /bin/sh -c 
-00000fb0: 7975 6d20 2d79 2069 6e73 7461 6c6c 206a  yum -y install j
-00000fc0: 6176 612d 312e 382e 302d 6f70 656e 6a64  ava-1.8.0-openjd
-00000fd0: 6b2d 2020 2031 3937 2e34 204d 4220 2020  k-   197.4 MB   
-00000fe0: 2020 2020 2020 2020 200a 2020 2020 3364           .    3d
-00000ff0: 3464 3032 3238 6631 3631 2020 2020 2020  4d0228f161      
-00001000: 2020 3320 7765 656b 7320 6167 6f20 2020    3 weeks ago   
-00001010: 2020 2020 2020 2f62 696e 2f73 6820 2d63        /bin/sh -c
-00001020: 2023 286e 6f70 2920 5553 4552 205b 726f   #(nop) USER [ro
-00001030: 6f74 5d20 2020 2020 2020 2020 2020 2020  ot]             
-00001040: 2020 2020 2020 3020 4220 2020 2020 2020        0 B       
-00001050: 2020 2020 2020 2020 2020 0a20 2020 2066            .    f
-00001060: 3761 6234 6561 3139 3730 3820 2020 2020  7ab4ea19708     
-00001070: 2020 2033 2077 6565 6b73 2061 676f 2020     3 weeks ago  
-00001080: 2020 2020 2020 202f 6269 6e2f 7368 202d         /bin/sh -
-00001090: 6320 2328 6e6f 7029 204d 4149 4e54 4149  c #(nop) MAINTAI
-000010a0: 4e45 5220 4d61 7265 6b20 476f 6c64 6d61  NER Marek Goldma
-000010b0: 6e6e 203c 2020 2030 2042 2020 2020 2020  nn <   0 B      
-000010c0: 2020 2020 2020 2020 2020 200a 2020 2020             .    
-000010d0: 3462 6231 3566 3362 3639 3737 2020 2020  4bb15f3b6977    
-000010e0: 2020 2020 3320 7765 656b 7320 6167 6f20      3 weeks ago 
-000010f0: 2020 2020 2020 2020 2f62 696e 2f73 6820          /bin/sh 
-00001100: 2d63 2023 286e 6f70 2920 5553 4552 205b  -c #(nop) USER [
-00001110: 6a62 6f73 735d 2020 2020 2020 2020 2020  jboss]          
-00001120: 2020 2020 2020 2020 3020 4220 2020 2020          0 B     
-00001130: 2020 2020 2020 2020 2020 2020 0a20 2020              .   
-00001140: 2035 6463 3165 3439 6634 3336 3120 2020   5dc1e49f4361   
-00001150: 2020 2020 2033 2077 6565 6b73 2061 676f       3 weeks ago
-00001160: 2020 2020 2020 2020 202f 6269 6e2f 7368           /bin/sh
-00001170: 202d 6320 2328 6e6f 7029 2057 4f52 4b44   -c #(nop) WORKD
-00001180: 4952 202f 6f70 742f 6a62 6f73 7320 2020  IR /opt/jboss   
-00001190: 2020 2020 2020 2020 2030 2042 2020 2020           0 B    
-000011a0: 2020 2020 2020 2020 2020 2020 200a 2020               .  
-000011b0: 2020 3766 3066 3965 6233 3131 3734 2020    7f0f9eb31174  
-000011c0: 2020 2020 2020 3320 7765 656b 7320 6167        3 weeks ag
-000011d0: 6f20 2020 2020 2020 2020 2f62 696e 2f73  o         /bin/s
-000011e0: 6820 2d63 2067 726f 7570 6164 6420 2d72  h -c groupadd -r
-000011f0: 206a 626f 7373 202d 6720 3130 3030 2026   jboss -g 1000 &
-00001200: 2620 7573 6572 6120 2020 342e 3334 3920  & usera   4.349 
-00001210: 6b42 2020 2020 2020 2020 2020 2020 0a20  kB            . 
-00001220: 2020 2062 6435 3135 6630 3434 6166 3720     bd515f044af7 
-00001230: 2020 2020 2020 2033 2077 6565 6b73 2061         3 weeks a
-00001240: 676f 2020 2020 2020 2020 202f 6269 6e2f  go         /bin/
-00001250: 7368 202d 6320 7975 6d20 7570 6461 7465  sh -c yum update
-00001260: 202d 7920 2626 2079 756d 202d 7920 696e   -y && yum -y in
-00001270: 7374 616c 6c20 786d 2020 2032 352e 3138  stall xm   25.18
-00001280: 204d 4220 2020 2020 2020 2020 2020 200a   MB            .
-00001290: 2020 2020 6237 3833 3336 3039 3930 3435      b78336099045
-000012a0: 2020 2020 2020 2020 3320 7765 656b 7320          3 weeks 
-000012b0: 6167 6f20 2020 2020 2020 2020 2f62 696e  ago         /bin
-000012c0: 2f73 6820 2d63 2023 286e 6f70 2920 4d41  /sh -c #(nop) MA
-000012d0: 494e 5441 494e 4552 204d 6172 656b 2047  INTAINER Marek G
-000012e0: 6f6c 646d 616e 6e20 3c20 2020 3020 4220  oldmann <   0 B 
-000012f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001300: 0a20 2020 2034 3831 3661 3239 3835 3438  .    4816a298548
-00001310: 6320 2020 2020 2020 2033 2077 6565 6b73  c        3 weeks
-00001320: 2061 676f 2020 2020 2020 2020 202f 6269   ago         /bi
-00001330: 6e2f 7368 202d 6320 2328 6e6f 7029 2043  n/sh -c #(nop) C
-00001340: 4d44 205b 222f 6269 6e2f 6261 7368 225d  MD ["/bin/bash"]
-00001350: 2020 2020 2020 2020 2020 2020 2030 2042               0 B
-00001360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001370: 200a 2020 2020 3665 6532 3335 6366 3434   .    6ee235cf44
-00001380: 3733 2020 2020 2020 2020 3320 7765 656b  73        3 week
-00001390: 7320 6167 6f20 2020 2020 2020 2020 2f62  s ago         /b
-000013a0: 696e 2f73 6820 2d63 2023 286e 6f70 2920  in/sh -c #(nop) 
-000013b0: 4c41 4245 4c20 6e61 6d65 3d43 656e 744f  LABEL name=CentO
-000013c0: 5320 4261 7365 2049 6d61 6720 2020 3020  S Base Imag   0 
-000013d0: 4220 2020 2020 2020 2020 2020 2020 2020  B               
-000013e0: 2020 0a20 2020 2034 3734 6332 6565 3737    .    474c2ee77
-000013f0: 6661 3320 2020 2020 2020 2033 2077 6565  fa3        3 wee
-00001400: 6b73 2061 676f 2020 2020 2020 2020 202f  ks ago         /
-00001410: 6269 6e2f 7368 202d 6320 2328 6e6f 7029  bin/sh -c #(nop)
-00001420: 2041 4444 2066 696c 653a 3732 3835 3266   ADD file:72852f
-00001430: 6337 3632 3664 3233 3333 3433 2020 2031  c7626d233343   1
-00001440: 3936 2e36 204d 4220 2020 2020 2020 2020  96.6 MB         
-00001450: 2020 200a 2020 2020 3135 3434 3038 3466     .    1544084f
-00001460: 6164 3831 2020 2020 2020 2020 3620 6d6f  ad81        6 mo
-00001470: 6e74 6873 2061 676f 2020 2020 2020 2020  nths ago        
-00001480: 2f62 696e 2f73 6820 2d63 2023 286e 6f70  /bin/sh -c #(nop
-00001490: 2920 4d41 494e 5441 494e 4552 2054 6865  ) MAINTAINER The
-000014a0: 2043 656e 744f 5320 5072 6f6a 6520 2020   CentOS Proje   
-000014b0: 3020 420a 0a41 6e64 2077 6520 7761 6e74  0 B..And we want
-000014c0: 2074 6f20 7371 7561 7368 2061 6c6c 2074   to squash all t
-000014d0: 6865 206c 6179 6572 7320 646f 776e 2074  he layers down t
-000014e0: 6f20 6c61 7965 7220 6060 3462 6231 3566  o layer ``4bb15f
-000014f0: 3362 3639 3737 6060 2e0a 0a3a 3a0a 0a20  3b6977``...::.. 
-00001500: 2020 2024 2064 6f63 6b65 722d 7371 7561     $ docker-squa
-00001510: 7368 202d 6620 3462 6231 3566 3362 3639  sh -f 4bb15f3b69
-00001520: 3737 202d 7420 6a62 6f73 732f 7769 6c64  77 -t jboss/wild
-00001530: 666c 793a 7371 7561 7368 6564 206a 626f  fly:squashed jbo
-00001540: 7373 2f77 696c 6466 6c79 3a6c 6174 6573  ss/wildfly:lates
-00001550: 740a 2020 2020 3230 3136 2d30 342d 3031  t.    2016-04-01
-00001560: 2031 333a 3131 3a30 322c 3335 3820 726f   13:11:02,358 ro
-00001570: 6f74 2020 2020 2020 2020 2049 4e46 4f20  ot         INFO 
-00001580: 2020 2020 646f 636b 6572 2d73 6372 6970      docker-scrip
-00001590: 7473 2076 6572 7369 6f6e 2031 2e30 2e30  ts version 1.0.0
-000015a0: 6465 762c 2044 6f63 6b65 7220 3732 3036  dev, Docker 7206
-000015b0: 3632 312c 2041 5049 2031 2e32 312e 2e2e  621, API 1.21...
-000015c0: 0a20 2020 2032 3031 362d 3034 2d30 3120  .    2016-04-01 
-000015d0: 3133 3a31 313a 3032 2c33 3538 2072 6f6f  13:11:02,358 roo
-000015e0: 7420 2020 2020 2020 2020 494e 464f 2020  t         INFO  
-000015f0: 2020 2055 7369 6e67 2076 3120 696d 6167     Using v1 imag
-00001600: 6520 666f 726d 6174 0a20 2020 2032 3031  e format.    201
-00001610: 362d 3034 2d30 3120 3133 3a31 313a 3032  6-04-01 13:11:02
-00001620: 2c33 3734 2072 6f6f 7420 2020 2020 2020  ,374 root       
-00001630: 2020 494e 464f 2020 2020 204f 6c64 2069    INFO     Old i
-00001640: 6d61 6765 2068 6173 2032 3120 6c61 7965  mage has 21 laye
-00001650: 7273 0a20 2020 2032 3031 362d 3034 2d30  rs.    2016-04-0
-00001660: 3120 3133 3a31 313a 3032 2c33 3738 2072  1 13:11:02,378 r
-00001670: 6f6f 7420 2020 2020 2020 2020 494e 464f  oot         INFO
-00001680: 2020 2020 2043 6865 636b 696e 6720 6966       Checking if
-00001690: 2073 7175 6173 6869 6e67 2069 7320 6e65   squashing is ne
-000016a0: 6365 7373 6172 792e 2e2e 0a20 2020 2032  cessary....    2
-000016b0: 3031 362d 3034 2d30 3120 3133 3a31 313a  016-04-01 13:11:
-000016c0: 3032 2c33 3738 2072 6f6f 7420 2020 2020  02,378 root     
-000016d0: 2020 2020 494e 464f 2020 2020 2041 7474      INFO     Att
-000016e0: 656d 7074 696e 6720 746f 2073 7175 6173  empting to squas
-000016f0: 6820 6c61 7374 2031 3220 6c61 7965 7273  h last 12 layers
-00001700: 2e2e 2e0a 2020 2020 3230 3136 2d30 342d  ....    2016-04-
-00001710: 3031 2031 333a 3131 3a30 322c 3337 3820  01 13:11:02,378 
-00001720: 726f 6f74 2020 2020 2020 2020 2049 4e46  root         INF
-00001730: 4f20 2020 2020 5361 7669 6e67 2069 6d61  O     Saving ima
-00001740: 6765 2032 3539 3534 6536 6432 3330 3030  ge 25954e6d23000
-00001750: 3632 3335 6565 6362 3766 3063 6335 3630  6235eecb7f0cc560
-00001760: 3236 3464 3733 3134 3639 3835 6332 6432  264d73146985c2d2
-00001770: 6536 3633 6261 6339 3533 6436 3630 6238  e663bac953d660b8
-00001780: 3733 3020 746f 202f 746d 702f 646f 636b  730 to /tmp/dock
-00001790: 6572 2d73 7175 6173 682d 6662 785a 7a34  er-squash-fbxZz4
-000017a0: 2f6f 6c64 2f69 6d61 6765 2e74 6172 2066  /old/image.tar f
-000017b0: 696c 652e 2e2e 0a20 2020 2032 3031 362d  ile....    2016-
-000017c0: 3034 2d30 3120 3133 3a31 313a 3038 2c30  04-01 13:11:08,0
-000017d0: 3033 2072 6f6f 7420 2020 2020 2020 2020  03 root         
-000017e0: 494e 464f 2020 2020 2049 6d61 6765 2073  INFO     Image s
-000017f0: 6176 6564 210a 2020 2020 3230 3136 2d30  aved!.    2016-0
-00001800: 342d 3031 2031 333a 3131 3a30 382c 3033  4-01 13:11:08,03
-00001810: 3120 726f 6f74 2020 2020 2020 2020 2049  1 root         I
-00001820: 4e46 4f20 2020 2020 556e 7061 636b 696e  NFO     Unpackin
-00001830: 6720 2f74 6d70 2f64 6f63 6b65 722d 7371  g /tmp/docker-sq
-00001840: 7561 7368 2d66 6278 5a7a 342f 6f6c 642f  uash-fbxZz4/old/
-00001850: 696d 6167 652e 7461 7220 7461 7220 6669  image.tar tar fi
-00001860: 6c65 2074 6f20 2f74 6d70 2f64 6f63 6b65  le to /tmp/docke
-00001870: 722d 7371 7561 7368 2d66 6278 5a7a 342f  r-squash-fbxZz4/
-00001880: 6f6c 6420 6469 7265 6374 6f72 790a 2020  old directory.  
-00001890: 2020 3230 3136 2d30 342d 3031 2031 333a    2016-04-01 13:
-000018a0: 3131 3a30 382c 3538 3820 726f 6f74 2020  11:08,588 root  
-000018b0: 2020 2020 2020 2049 4e46 4f20 2020 2020         INFO     
-000018c0: 4172 6368 6976 6520 756e 7061 636b 6564  Archive unpacked
-000018d0: 210a 2020 2020 3230 3136 2d30 342d 3031  !.    2016-04-01
-000018e0: 2031 333a 3131 3a30 382c 3633 3620 726f   13:11:08,636 ro
-000018f0: 6f74 2020 2020 2020 2020 2049 4e46 4f20  ot         INFO 
-00001900: 2020 2020 5371 7561 7368 696e 6720 696d      Squashing im
-00001910: 6167 6520 276a 626f 7373 2f77 696c 6466  age 'jboss/wildf
-00001920: 6c79 3a6c 6174 6573 7427 2e2e 2e0a 2020  ly:latest'....  
-00001930: 2020 3230 3136 2d30 342d 3031 2031 333a    2016-04-01 13:
-00001940: 3131 3a30 382c 3633 3720 726f 6f74 2020  11:08,637 root  
-00001950: 2020 2020 2020 2049 4e46 4f20 2020 2020         INFO     
-00001960: 5374 6172 7469 6e67 2073 7175 6173 6869  Starting squashi
-00001970: 6e67 2e2e 2e0a 2020 2020 3230 3136 2d30  ng....    2016-0
-00001980: 342d 3031 2031 333a 3131 3a30 382c 3633  4-01 13:11:08,63
-00001990: 3720 726f 6f74 2020 2020 2020 2020 2049  7 root         I
-000019a0: 4e46 4f20 2020 2020 5371 7561 7368 696e  NFO     Squashin
-000019b0: 6720 6669 6c65 2027 2f74 6d70 2f64 6f63  g file '/tmp/doc
-000019c0: 6b65 722d 7371 7561 7368 2d66 6278 5a7a  ker-squash-fbxZz
-000019d0: 342f 6f6c 642f 3235 3935 3465 3664 3233  4/old/25954e6d23
-000019e0: 3030 3036 3233 3565 6563 6237 6630 6363  0006235eecb7f0cc
-000019f0: 3536 3032 3634 6437 3331 3436 3938 3563  560264d73146985c
-00001a00: 3264 3265 3636 3362 6163 3935 3364 3636  2d2e663bac953d66
-00001a10: 3062 3837 3330 2f6c 6179 6572 2e74 6172  0b8730/layer.tar
-00001a20: 272e 2e2e 0a20 2020 2032 3031 362d 3034  '....    2016-04
-00001a30: 2d30 3120 3133 3a31 313a 3038 2c36 3337  -01 13:11:08,637
-00001a40: 2072 6f6f 7420 2020 2020 2020 2020 494e   root         IN
-00001a50: 464f 2020 2020 2053 7175 6173 6869 6e67  FO     Squashing
-00001a60: 2066 696c 6520 272f 746d 702f 646f 636b   file '/tmp/dock
-00001a70: 6572 2d73 7175 6173 682d 6662 785a 7a34  er-squash-fbxZz4
-00001a80: 2f6f 6c64 2f35 6165 3639 6362 3435 3461  /old/5ae69cb454a
-00001a90: 3561 3534 3266 3633 6531 3438 6365 3430  5a542f63e148ce40
-00001aa0: 6662 3965 3031 6465 3562 6230 3138 3035  fb9e01de5bb01805
-00001ab0: 6234 6465 6432 3338 3834 3162 6332 6365  b4ded238841bc2ce
-00001ac0: 3865 3839 352f 6c61 7965 722e 7461 7227  8e895/layer.tar'
-00001ad0: 2e2e 2e0a 2020 2020 3230 3136 2d30 342d  ....    2016-04-
-00001ae0: 3031 2031 333a 3131 3a30 382c 3633 3720  01 13:11:08,637 
-00001af0: 726f 6f74 2020 2020 2020 2020 2049 4e46  root         INF
-00001b00: 4f20 2020 2020 5371 7561 7368 696e 6720  O     Squashing 
-00001b10: 6669 6c65 2027 2f74 6d70 2f64 6f63 6b65  file '/tmp/docke
-00001b20: 722d 7371 7561 7368 2d66 6278 5a7a 342f  r-squash-fbxZz4/
-00001b30: 6f6c 642f 6463 3234 3731 3266 3335 6334  old/dc24712f35c4
-00001b40: 3065 3935 3862 6538 6163 6132 3733 3165  0e958be8aca2731e
-00001b50: 3762 6638 3335 3362 3962 3138 6261 6136  7bf8353b9b18baa6
-00001b60: 6139 3461 6438 3463 3639 3532 6362 6337  a94ad84c6952cbc7
-00001b70: 3730 3034 2f6c 6179 6572 2e74 6172 272e  7004/layer.tar'.
-00001b80: 2e2e 0a20 2020 2032 3031 362d 3034 2d30  ...    2016-04-0
-00001b90: 3120 3133 3a31 313a 3038 2c36 3338 2072  1 13:11:08,638 r
-00001ba0: 6f6f 7420 2020 2020 2020 2020 494e 464f  oot         INFO
-00001bb0: 2020 2020 2053 7175 6173 6869 6e67 2066       Squashing f
-00001bc0: 696c 6520 272f 746d 702f 646f 636b 6572  ile '/tmp/docker
-00001bd0: 2d73 7175 6173 682d 6662 785a 7a34 2f6f  -squash-fbxZz4/o
-00001be0: 6c64 2f64 3932 3931 3239 6434 6338 6536  ld/d929129d4c8e6
-00001bf0: 3165 6133 3636 3165 6234 3263 3330 6430  1ea3661eb42c30d0
-00001c00: 3166 3463 3135 3234 3138 3638 3931 3738  1f4c152418689178
-00001c10: 6166 6337 6463 3831 3835 6133 3738 3134  afc7dc8185a37814
-00001c20: 3532 382f 6c61 7965 722e 7461 7227 2e2e  528/layer.tar'..
-00001c30: 2e0a 2020 2020 3230 3136 2d30 342d 3031  ..    2016-04-01
-00001c40: 2031 333a 3131 3a30 392c 3131 3320 726f   13:11:09,113 ro
-00001c50: 6f74 2020 2020 2020 2020 2049 4e46 4f20  ot         INFO 
-00001c60: 2020 2020 5371 7561 7368 696e 6720 6669      Squashing fi
-00001c70: 6c65 2027 2f74 6d70 2f64 6f63 6b65 722d  le '/tmp/docker-
-00001c80: 7371 7561 7368 2d66 6278 5a7a 342f 6f6c  squash-fbxZz4/ol
-00001c90: 642f 6238 6661 3363 6166 3764 3664 6332  d/b8fa3caf7d6dc2
-00001ca0: 3238 6266 3234 3939 6133 6166 3836 6535  28bf2499a3af86e5
-00001cb0: 3037 3361 6430 6331 3733 3034 6333 3930  073ad0c17304c390
-00001cc0: 3066 6133 3431 6539 6432 6665 3465 3536  0fa341e9d2fe4e56
-00001cd0: 3535 2f6c 6179 6572 2e74 6172 272e 2e2e  55/layer.tar'...
-00001ce0: 0a20 2020 2032 3031 362d 3034 2d30 3120  .    2016-04-01 
-00001cf0: 3133 3a31 313a 3039 2c31 3135 2072 6f6f  13:11:09,115 roo
-00001d00: 7420 2020 2020 2020 2020 494e 464f 2020  t         INFO  
-00001d10: 2020 2053 7175 6173 6869 6e67 2066 696c     Squashing fil
-00001d20: 6520 272f 746d 702f 646f 636b 6572 2d73  e '/tmp/docker-s
-00001d30: 7175 6173 682d 6662 785a 7a34 2f6f 6c64  quash-fbxZz4/old
-00001d40: 2f33 3862 3866 3835 6537 3462 6661 3737  /38b8f85e74bfa77
-00001d50: 3361 3061 6436 3964 6132 3230 3564 6330  3a0ad69da2205dc0
-00001d60: 3134 3839 3435 6536 6635 6137 6365 6230  148945e6f5a7ceb0
-00001d70: 3466 6134 6538 3631 3965 3164 6534 3235  4fa4e8619e1de425
-00001d80: 622f 6c61 7965 722e 7461 7227 2e2e 2e0a  b/layer.tar'....
-00001d90: 2020 2020 3230 3136 2d30 342d 3031 2031      2016-04-01 1
-00001da0: 333a 3131 3a30 392c 3131 3520 726f 6f74  3:11:09,115 root
-00001db0: 2020 2020 2020 2020 2049 4e46 4f20 2020           INFO   
-00001dc0: 2020 5371 7561 7368 696e 6720 6669 6c65    Squashing file
-00001dd0: 2027 2f74 6d70 2f64 6f63 6b65 722d 7371   '/tmp/docker-sq
-00001de0: 7561 7368 2d66 6278 5a7a 342f 6f6c 642f  uash-fbxZz4/old/
-00001df0: 6165 3739 6236 3436 6239 6139 6132 3837  ae79b646b9a9a287
-00001e00: 6335 6636 6130 3138 3731 6363 3964 3965  c5f6a01871cc9d9e
-00001e10: 6535 3936 6461 6665 6532 6462 3934 3237  e596dafee2db9427
-00001e20: 3134 6361 3364 6561 3063 3036 6565 6633  14ca3dea0c06eef3
-00001e30: 2f6c 6179 6572 2e74 6172 272e 2e2e 0a20  /layer.tar'.... 
-00001e40: 2020 2032 3031 362d 3034 2d30 3120 3133     2016-04-01 13
-00001e50: 3a31 313a 3039 2c31 3135 2072 6f6f 7420  :11:09,115 root 
-00001e60: 2020 2020 2020 2020 494e 464f 2020 2020          INFO    
-00001e70: 2053 7175 6173 6869 6e67 2066 696c 6520   Squashing file 
-00001e80: 272f 746d 702f 646f 636b 6572 2d73 7175  '/tmp/docker-squ
-00001e90: 6173 682d 6662 785a 7a34 2f6f 6c64 2f32  ash-fbxZz4/old/2
-00001ea0: 6234 3630 3664 6339 6463 3737 3361 6132  b4606dc9dc773aa2
-00001eb0: 3230 6136 3533 3531 6665 3864 3534 6630  20a65351fe8d54f0
-00001ec0: 3335 3334 6335 3866 6561 3233 3039 3630  3534c58fea230960
-00001ed0: 6539 3539 3135 3232 3233 3636 3037 342f  e95915222366074/
-00001ee0: 6c61 7965 722e 7461 7227 2e2e 2e0a 2020  layer.tar'....  
-00001ef0: 2020 3230 3136 2d30 342d 3031 2031 333a    2016-04-01 13:
-00001f00: 3131 3a30 392c 3131 3520 726f 6f74 2020  11:09,115 root  
-00001f10: 2020 2020 2020 2049 4e46 4f20 2020 2020         INFO     
-00001f20: 5371 7561 7368 696e 6720 6669 6c65 2027  Squashing file '
-00001f30: 2f74 6d70 2f64 6f63 6b65 722d 7371 7561  /tmp/docker-squa
-00001f40: 7368 2d66 6278 5a7a 342f 6f6c 642f 3131  sh-fbxZz4/old/11
-00001f50: 3866 6139 6533 3335 3736 6563 6336 3235  8fa9e33576ecc625
-00001f60: 6562 6262 6664 6632 3830 3963 3135 3237  ebbbfdf2809c1527
-00001f70: 6537 3136 6362 3466 6435 6362 3430 3534  e716cb4fd5cb4054
-00001f80: 3865 6236 6433 3530 3361 3735 6139 2f6c  8eb6d3503a75a9/l
-00001f90: 6179 6572 2e74 6172 272e 2e2e 0a20 2020  ayer.tar'....   
-00001fa0: 2032 3031 362d 3034 2d30 3120 3133 3a31   2016-04-01 13:1
-00001fb0: 313a 3039 2c31 3135 2072 6f6f 7420 2020  1:09,115 root   
-00001fc0: 2020 2020 2020 494e 464f 2020 2020 2053        INFO     S
-00001fd0: 7175 6173 6869 6e67 2066 696c 6520 272f  quashing file '/
-00001fe0: 746d 702f 646f 636b 6572 2d73 7175 6173  tmp/docker-squas
-00001ff0: 682d 6662 785a 7a34 2f6f 6c64 2f35 6637  h-fbxZz4/old/5f7
-00002000: 6538 6633 3663 3362 6232 3063 3964 6237  e8f36c3bb20c9db7
-00002010: 3437 3061 3232 6638 3238 3731 3062 3464  470a22f828710b4d
-00002020: 3238 6165 6465 3634 3936 3663 3432 3561  28aede64966c425a
-00002030: 6464 3438 6131 6231 3466 6532 332f 6c61  dd48a1b14fe23/la
-00002040: 7965 722e 7461 7227 2e2e 2e0a 2020 2020  yer.tar'....    
-00002050: 3230 3136 2d30 342d 3031 2031 333a 3131  2016-04-01 13:11
-00002060: 3a31 302c 3132 3720 726f 6f74 2020 2020  :10,127 root    
-00002070: 2020 2020 2049 4e46 4f20 2020 2020 5371       INFO     Sq
-00002080: 7561 7368 696e 6720 6669 6c65 2027 2f74  uashing file '/t
-00002090: 6d70 2f64 6f63 6b65 722d 7371 7561 7368  mp/docker-squash
-000020a0: 2d66 6278 5a7a 342f 6f6c 642f 3364 3464  -fbxZz4/old/3d4d
-000020b0: 3032 3238 6631 3631 6236 3765 6234 3666  0228f161b67eb46f
-000020c0: 6462 3432 3561 6431 3438 6333 3164 3939  db425ad148c31d99
-000020d0: 3434 6463 6238 3232 6636 3765 6163 3365  44dcb822f67eac3e
-000020e0: 3261 6332 6566 6665 6663 3733 2f6c 6179  2ac2effefc73/lay
-000020f0: 6572 2e74 6172 272e 2e2e 0a20 2020 2032  er.tar'....    2
-00002100: 3031 362d 3034 2d30 3120 3133 3a31 313a  016-04-01 13:11:
-00002110: 3130 2c31 3239 2072 6f6f 7420 2020 2020  10,129 root     
-00002120: 2020 2020 494e 464f 2020 2020 2053 7175      INFO     Squ
-00002130: 6173 6869 6e67 2066 696c 6520 272f 746d  ashing file '/tm
-00002140: 702f 646f 636b 6572 2d73 7175 6173 682d  p/docker-squash-
-00002150: 6662 785a 7a34 2f6f 6c64 2f66 3761 6234  fbxZz4/old/f7ab4
-00002160: 6561 3139 3730 3834 6162 3734 3833 6132  ea197084ab7483a2
-00002170: 6361 3534 3039 6264 6366 3534 3733 3134  ca5409bdcf547314
-00002180: 3162 6662 3631 6238 3638 3762 3133 3239  1bfb61b8687b1329
-00002190: 3934 3333 3539 6363 3366 652f 6c61 7965  943359cc3fe/laye
-000021a0: 722e 7461 7227 2e2e 2e0a 2020 2020 3230  r.tar'....    20
-000021b0: 3136 2d30 342d 3031 2031 333a 3131 3a31  16-04-01 13:11:1
-000021c0: 302c 3733 3220 726f 6f74 2020 2020 2020  0,732 root      
-000021d0: 2020 2049 4e46 4f20 2020 2020 5371 7561     INFO     Squa
-000021e0: 7368 696e 6720 6669 6e69 7368 6564 210a  shing finished!.
-000021f0: 2020 2020 3230 3136 2d30 342d 3031 2031      2016-04-01 1
-00002200: 333a 3131 3a31 302c 3733 3720 726f 6f74  3:11:10,737 root
-00002210: 2020 2020 2020 2020 2049 4e46 4f20 2020           INFO   
-00002220: 2020 4e65 7720 7371 7561 7368 6564 2069    New squashed i
-00002230: 6d61 6765 2049 4420 6973 2035 3232 3535  mage ID is 52255
-00002240: 6537 3564 3365 6238 3331 3233 6530 3734  e75d3eb83123e074
-00002250: 6638 3937 6538 6339 3731 6465 6339 6431  f897e8c971dec9d1
-00002260: 3136 3861 3563 3832 6437 6331 3439 3661  168a5c82d7c1496a
-00002270: 3139 3064 6132 6534 3065 660a 2020 2020  190da2e40ef.    
-00002280: 3230 3136 2d30 342d 3031 2031 333a 3131  2016-04-01 13:11
-00002290: 3a31 342c 3536 3320 726f 6f74 2020 2020  :14,563 root    
-000022a0: 2020 2020 2049 4e46 4f20 2020 2020 496d       INFO     Im
-000022b0: 6167 6520 7265 6769 7374 6572 6564 2069  age registered i
-000022c0: 6e20 446f 636b 6572 2064 6165 6d6f 6e20  n Docker daemon 
-000022d0: 6173 206a 626f 7373 2f77 696c 6466 6c79  as jboss/wildfly
-000022e0: 3a73 7175 6173 6865 640a 2020 2020 3230  :squashed.    20
-000022f0: 3136 2d30 342d 3031 2031 333a 3131 3a31  16-04-01 13:11:1
-00002300: 342c 3635 3220 726f 6f74 2020 2020 2020  4,652 root      
-00002310: 2020 2049 4e46 4f20 2020 2020 446f 6e65     INFO     Done
-00002320: 0a0a 5765 2063 616e 206e 6f77 2063 6f6e  ..We can now con
-00002330: 6669 726d 2074 6865 206c 6179 6572 2073  firm the layer s
-00002340: 7472 7563 7475 7265 3a0a 0a3a 3a0a 0a20  tructure:..::.. 
-00002350: 2020 2024 2064 6f63 6b65 7220 6869 7374     $ docker hist
-00002360: 6f72 7920 6a62 6f73 732f 7769 6c64 666c  ory jboss/wildfl
-00002370: 793a 7371 7561 7368 6564 0a20 2020 2049  y:squashed.    I
-00002380: 4d41 4745 2020 2020 2020 2020 2020 2020  MAGE            
-00002390: 2020 2043 5245 4154 4544 2020 2020 2020     CREATED      
-000023a0: 2020 2020 2020 2043 5245 4154 4544 2042         CREATED B
-000023b0: 5920 2020 2020 2020 2020 2020 2020 2020  Y               
-000023c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000023d0: 2020 2020 2020 2053 495a 4520 2020 2020         SIZE     
-000023e0: 2020 2020 2020 2020 2020 2043 4f4d 4d45             COMME
-000023f0: 4e54 0a20 2020 2035 3232 3535 6537 3564  NT.    52255e75d
-00002400: 3365 6220 2020 2020 2020 2034 3020 7365  3eb        40 se
-00002410: 636f 6e64 7320 6167 6f20 2020 2020 2020  conds ago       
-00002420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002440: 2020 2020 2020 2020 2020 2020 2020 2033                 3
-00002450: 3538 2e32 204d 4220 2020 2020 2020 2020  58.2 MB         
-00002460: 2020 200a 2020 2020 3462 6231 3566 3362     .    4bb15f3b
-00002470: 3639 3737 2020 2020 2020 2020 3320 7765  6977        3 we
-00002480: 656b 7320 6167 6f20 2020 2020 2020 2020  eks ago         
-00002490: 2f62 696e 2f73 6820 2d63 2023 286e 6f70  /bin/sh -c #(nop
-000024a0: 2920 5553 4552 205b 6a62 6f73 735d 2020  ) USER [jboss]  
-000024b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000024c0: 3020 4220 2020 2020 2020 2020 2020 2020  0 B             
-000024d0: 2020 2020 0a20 2020 2035 6463 3165 3439      .    5dc1e49
-000024e0: 6634 3336 3120 2020 2020 2020 2033 2077  f4361        3 w
-000024f0: 6565 6b73 2061 676f 2020 2020 2020 2020  eeks ago        
-00002500: 202f 6269 6e2f 7368 202d 6320 2328 6e6f   /bin/sh -c #(no
-00002510: 7029 2057 4f52 4b44 4952 202f 6f70 742f  p) WORKDIR /opt/
-00002520: 6a62 6f73 7320 2020 2020 2020 2020 2020  jboss           
-00002530: 2030 2042 2020 2020 2020 2020 2020 2020   0 B            
-00002540: 2020 2020 200a 2020 2020 3766 3066 3965       .    7f0f9e
-00002550: 6233 3131 3734 2020 2020 2020 2020 3320  b31174        3 
-00002560: 7765 656b 7320 6167 6f20 2020 2020 2020  weeks ago       
-00002570: 2020 2f62 696e 2f73 6820 2d63 2067 726f    /bin/sh -c gro
-00002580: 7570 6164 6420 2d72 206a 626f 7373 202d  upadd -r jboss -
-00002590: 6720 3130 3030 2026 2620 7573 6572 6120  g 1000 && usera 
-000025a0: 2020 342e 3334 3920 6b42 2020 2020 2020    4.349 kB      
-000025b0: 2020 2020 2020 0a20 2020 2062 6435 3135        .    bd515
-000025c0: 6630 3434 6166 3720 2020 2020 2020 2033  f044af7        3
-000025d0: 2077 6565 6b73 2061 676f 2020 2020 2020   weeks ago      
-000025e0: 2020 202f 6269 6e2f 7368 202d 6320 7975     /bin/sh -c yu
-000025f0: 6d20 7570 6461 7465 202d 7920 2626 2079  m update -y && y
-00002600: 756d 202d 7920 696e 7374 616c 6c20 786d  um -y install xm
-00002610: 2020 2032 352e 3138 204d 4220 2020 2020     25.18 MB     
-00002620: 2020 2020 2020 200a 2020 2020 6237 3833         .    b783
-00002630: 3336 3039 3930 3435 2020 2020 2020 2020  36099045        
-00002640: 3320 7765 656b 7320 6167 6f20 2020 2020  3 weeks ago     
-00002650: 2020 2020 2f62 696e 2f73 6820 2d63 2023      /bin/sh -c #
-00002660: 286e 6f70 2920 4d41 494e 5441 494e 4552  (nop) MAINTAINER
-00002670: 204d 6172 656b 2047 6f6c 646d 616e 6e20   Marek Goldmann 
-00002680: 3c20 2020 3020 4220 2020 2020 2020 2020  <   0 B         
-00002690: 2020 2020 2020 2020 0a20 2020 2034 3831          .    481
-000026a0: 3661 3239 3835 3438 6320 2020 2020 2020  6a298548c       
-000026b0: 2033 2077 6565 6b73 2061 676f 2020 2020   3 weeks ago    
-000026c0: 2020 2020 202f 6269 6e2f 7368 202d 6320       /bin/sh -c 
-000026d0: 2328 6e6f 7029 2043 4d44 205b 222f 6269  #(nop) CMD ["/bi
-000026e0: 6e2f 6261 7368 225d 2020 2020 2020 2020  n/bash"]        
-000026f0: 2020 2020 2030 2042 2020 2020 2020 2020       0 B        
-00002700: 2020 2020 2020 2020 200a 2020 2020 3665           .    6e
-00002710: 6532 3335 6366 3434 3733 2020 2020 2020  e235cf4473      
-00002720: 2020 3320 7765 656b 7320 6167 6f20 2020    3 weeks ago   
-00002730: 2020 2020 2020 2f62 696e 2f73 6820 2d63        /bin/sh -c
-00002740: 2023 286e 6f70 2920 4c41 4245 4c20 6e61   #(nop) LABEL na
-00002750: 6d65 3d43 656e 744f 5320 4261 7365 2049  me=CentOS Base I
-00002760: 6d61 6720 2020 3020 4220 2020 2020 2020  mag   0 B       
-00002770: 2020 2020 2020 2020 2020 0a20 2020 2034            .    4
-00002780: 3734 6332 6565 3737 6661 3320 2020 2020  74c2ee77fa3     
-00002790: 2020 2033 2077 6565 6b73 2061 676f 2020     3 weeks ago  
-000027a0: 2020 2020 2020 202f 6269 6e2f 7368 202d         /bin/sh -
-000027b0: 6320 2328 6e6f 7029 2041 4444 2066 696c  c #(nop) ADD fil
-000027c0: 653a 3732 3835 3266 6337 3632 3664 3233  e:72852fc7626d23
-000027d0: 3333 3433 2020 2031 3936 2e36 204d 4220  3343   196.6 MB 
-000027e0: 2020 2020 2020 2020 2020 200a 2020 2020             .    
-000027f0: 3135 3434 3038 3466 6164 3831 2020 2020  1544084fad81    
-00002800: 2020 2020 3620 6d6f 6e74 6873 2061 676f      6 months ago
-00002810: 2020 2020 2020 2020 2f62 696e 2f73 6820          /bin/sh 
-00002820: 2d63 2023 286e 6f70 2920 4d41 494e 5441  -c #(nop) MAINTA
-00002830: 494e 4552 2054 6865 2043 656e 744f 5320  INER The CentOS 
-00002840: 5072 6f6a 6520 2020 3020 420a 0a4f 7468  Proje   0 B..Oth
-00002850: 6572 206f 7074 696f 6e20 6973 2074 6f20  er option is to 
-00002860: 7370 6563 6966 7920 686f 7720 6d61 6e79  specify how many
-00002870: 206c 6179 6572 7320 2863 6f75 6e74 696e   layers (countin
-00002880: 6720 6672 6f6d 2074 6865 206e 6577 6573  g from the newes
-00002890: 7420 6c61 7965 7229 2077 6520 7761 6e74  t layer) we want
-000028a0: 2074 6f20 7371 7561 7368 2e5c 0a4c 6574   to squash.\.Let
-000028b0: 2773 2073 7175 6173 6820 6c61 7374 2031  's squash last 1
-000028c0: 3020 6c61 7965 7273 2066 726f 6d20 7468  0 layers from th
-000028d0: 6520 6060 6a62 6f73 732f 7769 6c64 666c  e ``jboss/wildfl
-000028e0: 793a 6c61 7465 7374 6060 2069 6d61 6765  y:latest`` image
-000028f0: 3a0a 0a3a 3a0a 0a20 2020 2024 2064 6f63  :..::..    $ doc
-00002900: 6b65 722d 7371 7561 7368 202d 6620 3130  ker-squash -f 10
-00002910: 202d 7420 6a62 6f73 732f 7769 6c64 666c   -t jboss/wildfl
-00002920: 793a 7371 7561 7368 6564 206a 626f 7373  y:squashed jboss
-00002930: 2f77 696c 6466 6c79 3a6c 6174 6573 740a  /wildfly:latest.
-00002940: 2020 2020 3230 3136 2d30 342d 3031 2031      2016-04-01 1
-00002950: 333a 3135 3a30 362c 3438 3820 726f 6f74  3:15:06,488 root
-00002960: 2020 2020 2020 2020 2049 4e46 4f20 2020           INFO   
-00002970: 2020 646f 636b 6572 2d73 6372 6970 7473    docker-scripts
-00002980: 2076 6572 7369 6f6e 2031 2e30 2e30 6465   version 1.0.0de
-00002990: 762c 2044 6f63 6b65 7220 3732 3036 3632  v, Docker 720662
-000029a0: 312c 2041 5049 2031 2e32 312e 2e2e 0a20  1, API 1.21.... 
-000029b0: 2020 2032 3031 362d 3034 2d30 3120 3133     2016-04-01 13
-000029c0: 3a31 353a 3036 2c34 3838 2072 6f6f 7420  :15:06,488 root 
-000029d0: 2020 2020 2020 2020 494e 464f 2020 2020          INFO    
-000029e0: 2055 7369 6e67 2076 3120 696d 6167 6520   Using v1 image 
-000029f0: 666f 726d 6174 0a20 2020 2032 3031 362d  format.    2016-
-00002a00: 3034 2d30 3120 3133 3a31 353a 3036 2c35  04-01 13:15:06,5
-00002a10: 3034 2072 6f6f 7420 2020 2020 2020 2020  04 root         
-00002a20: 494e 464f 2020 2020 204f 6c64 2069 6d61  INFO     Old ima
-00002a30: 6765 2068 6173 2032 3120 6c61 7965 7273  ge has 21 layers
-00002a40: 0a20 2020 2032 3031 362d 3034 2d30 3120  .    2016-04-01 
-00002a50: 3133 3a31 353a 3036 2c35 3034 2072 6f6f  13:15:06,504 roo
-00002a60: 7420 2020 2020 2020 2020 494e 464f 2020  t         INFO  
-00002a70: 2020 2043 6865 636b 696e 6720 6966 2073     Checking if s
-00002a80: 7175 6173 6869 6e67 2069 7320 6e65 6365  quashing is nece
-00002a90: 7373 6172 792e 2e2e 0a20 2020 2032 3031  ssary....    201
-00002aa0: 362d 3034 2d30 3120 3133 3a31 353a 3036  6-04-01 13:15:06
-00002ab0: 2c35 3034 2072 6f6f 7420 2020 2020 2020  ,504 root       
-00002ac0: 2020 494e 464f 2020 2020 2041 7474 656d    INFO     Attem
-00002ad0: 7074 696e 6720 746f 2073 7175 6173 6820  pting to squash 
-00002ae0: 6c61 7374 2031 3020 6c61 7965 7273 2e2e  last 10 layers..
-00002af0: 2e0a 2020 2020 3230 3136 2d30 342d 3031  ..    2016-04-01
-00002b00: 2031 333a 3135 3a30 362c 3530 3520 726f   13:15:06,505 ro
-00002b10: 6f74 2020 2020 2020 2020 2049 4e46 4f20  ot         INFO 
-00002b20: 2020 2020 5361 7669 6e67 2069 6d61 6765      Saving image
-00002b30: 2032 3539 3534 6536 6432 3330 3030 3632   25954e6d2300062
-00002b40: 3335 6565 6362 3766 3063 6335 3630 3236  35eecb7f0cc56026
-00002b50: 3464 3733 3134 3639 3835 6332 6432 6536  4d73146985c2d2e6
-00002b60: 3633 6261 6339 3533 6436 3630 6238 3733  63bac953d660b873
-00002b70: 3020 746f 202f 746d 702f 646f 636b 6572  0 to /tmp/docker
-00002b80: 2d73 7175 6173 682d 6675 3830 4358 2f6f  -squash-fu80CX/o
-00002b90: 6c64 2f69 6d61 6765 2e74 6172 2066 696c  ld/image.tar fil
-00002ba0: 652e 2e2e 0a20 2020 2032 3031 362d 3034  e....    2016-04
-00002bb0: 2d30 3120 3133 3a31 353a 3132 2c31 3336  -01 13:15:12,136
-00002bc0: 2072 6f6f 7420 2020 2020 2020 2020 494e   root         IN
-00002bd0: 464f 2020 2020 2049 6d61 6765 2073 6176  FO     Image sav
-00002be0: 6564 210a 2020 2020 3230 3136 2d30 342d  ed!.    2016-04-
-00002bf0: 3031 2031 333a 3135 3a31 322c 3136 3720  01 13:15:12,167 
-00002c00: 726f 6f74 2020 2020 2020 2020 2049 4e46  root         INF
-00002c10: 4f20 2020 2020 556e 7061 636b 696e 6720  O     Unpacking 
-00002c20: 2f74 6d70 2f64 6f63 6b65 722d 7371 7561  /tmp/docker-squa
-00002c30: 7368 2d66 7538 3043 582f 6f6c 642f 696d  sh-fu80CX/old/im
-00002c40: 6167 652e 7461 7220 7461 7220 6669 6c65  age.tar tar file
-00002c50: 2074 6f20 2f74 6d70 2f64 6f63 6b65 722d   to /tmp/docker-
-00002c60: 7371 7561 7368 2d66 7538 3043 582f 6f6c  squash-fu80CX/ol
-00002c70: 6420 6469 7265 6374 6f72 790a 2020 2020  d directory.    
-00002c80: 3230 3136 2d30 342d 3031 2031 333a 3135  2016-04-01 13:15
-00002c90: 3a31 322c 3730 3620 726f 6f74 2020 2020  :12,706 root    
-00002ca0: 2020 2020 2049 4e46 4f20 2020 2020 4172       INFO     Ar
-00002cb0: 6368 6976 6520 756e 7061 636b 6564 210a  chive unpacked!.
-00002cc0: 2020 2020 3230 3136 2d30 342d 3031 2031      2016-04-01 1
-00002cd0: 333a 3135 3a31 322c 3735 3620 726f 6f74  3:15:12,756 root
-00002ce0: 2020 2020 2020 2020 2049 4e46 4f20 2020           INFO   
-00002cf0: 2020 5371 7561 7368 696e 6720 696d 6167    Squashing imag
-00002d00: 6520 276a 626f 7373 2f77 696c 6466 6c79  e 'jboss/wildfly
-00002d10: 3a6c 6174 6573 7427 2e2e 2e0a 2020 2020  :latest'....    
-00002d20: 3230 3136 2d30 342d 3031 2031 333a 3135  2016-04-01 13:15
-00002d30: 3a31 322c 3735 3620 726f 6f74 2020 2020  :12,756 root    
-00002d40: 2020 2020 2049 4e46 4f20 2020 2020 5374       INFO     St
-00002d50: 6172 7469 6e67 2073 7175 6173 6869 6e67  arting squashing
-00002d60: 2e2e 2e0a 2020 2020 3230 3136 2d30 342d  ....    2016-04-
-00002d70: 3031 2031 333a 3135 3a31 322c 3735 3620  01 13:15:12,756 
-00002d80: 726f 6f74 2020 2020 2020 2020 2049 4e46  root         INF
-00002d90: 4f20 2020 2020 5371 7561 7368 696e 6720  O     Squashing 
-00002da0: 6669 6c65 2027 2f74 6d70 2f64 6f63 6b65  file '/tmp/docke
-00002db0: 722d 7371 7561 7368 2d66 7538 3043 582f  r-squash-fu80CX/
-00002dc0: 6f6c 642f 3235 3935 3465 3664 3233 3030  old/25954e6d2300
-00002dd0: 3036 3233 3565 6563 6237 6630 6363 3536  06235eecb7f0cc56
-00002de0: 3032 3634 6437 3331 3436 3938 3563 3264  0264d73146985c2d
-00002df0: 3265 3636 3362 6163 3935 3364 3636 3062  2e663bac953d660b
-00002e00: 3837 3330 2f6c 6179 6572 2e74 6172 272e  8730/layer.tar'.
-00002e10: 2e2e 0a20 2020 2032 3031 362d 3034 2d30  ...    2016-04-0
-00002e20: 3120 3133 3a31 353a 3132 2c37 3537 2072  1 13:15:12,757 r
-00002e30: 6f6f 7420 2020 2020 2020 2020 494e 464f  oot         INFO
-00002e40: 2020 2020 2053 7175 6173 6869 6e67 2066       Squashing f
-00002e50: 696c 6520 272f 746d 702f 646f 636b 6572  ile '/tmp/docker
-00002e60: 2d73 7175 6173 682d 6675 3830 4358 2f6f  -squash-fu80CX/o
-00002e70: 6c64 2f35 6165 3639 6362 3435 3461 3561  ld/5ae69cb454a5a
-00002e80: 3534 3266 3633 6531 3438 6365 3430 6662  542f63e148ce40fb
-00002e90: 3965 3031 6465 3562 6230 3138 3035 6234  9e01de5bb01805b4
-00002ea0: 6465 6432 3338 3834 3162 6332 6365 3865  ded238841bc2ce8e
-00002eb0: 3839 352f 6c61 7965 722e 7461 7227 2e2e  895/layer.tar'..
-00002ec0: 2e0a 2020 2020 3230 3136 2d30 342d 3031  ..    2016-04-01
-00002ed0: 2031 333a 3135 3a31 322c 3735 3720 726f   13:15:12,757 ro
-00002ee0: 6f74 2020 2020 2020 2020 2049 4e46 4f20  ot         INFO 
-00002ef0: 2020 2020 5371 7561 7368 696e 6720 6669      Squashing fi
-00002f00: 6c65 2027 2f74 6d70 2f64 6f63 6b65 722d  le '/tmp/docker-
-00002f10: 7371 7561 7368 2d66 7538 3043 582f 6f6c  squash-fu80CX/ol
-00002f20: 642f 6463 3234 3731 3266 3335 6334 3065  d/dc24712f35c40e
-00002f30: 3935 3862 6538 6163 6132 3733 3165 3762  958be8aca2731e7b
-00002f40: 6638 3335 3362 3962 3138 6261 6136 6139  f8353b9b18baa6a9
-00002f50: 3461 6438 3463 3639 3532 6362 6337 3730  4ad84c6952cbc770
-00002f60: 3034 2f6c 6179 6572 2e74 6172 272e 2e2e  04/layer.tar'...
-00002f70: 0a20 2020 2032 3031 362d 3034 2d30 3120  .    2016-04-01 
-00002f80: 3133 3a31 353a 3132 2c37 3537 2072 6f6f  13:15:12,757 roo
-00002f90: 7420 2020 2020 2020 2020 494e 464f 2020  t         INFO  
-00002fa0: 2020 2053 7175 6173 6869 6e67 2066 696c     Squashing fil
-00002fb0: 6520 272f 746d 702f 646f 636b 6572 2d73  e '/tmp/docker-s
-00002fc0: 7175 6173 682d 6675 3830 4358 2f6f 6c64  quash-fu80CX/old
-00002fd0: 2f64 3932 3931 3239 6434 6338 6536 3165  /d929129d4c8e61e
-00002fe0: 6133 3636 3165 6234 3263 3330 6430 3166  a3661eb42c30d01f
-00002ff0: 3463 3135 3234 3138 3638 3931 3738 6166  4c152418689178af
-00003000: 6337 6463 3831 3835 6133 3738 3134 3532  c7dc8185a3781452
-00003010: 382f 6c61 7965 722e 7461 7227 2e2e 2e0a  8/layer.tar'....
-00003020: 2020 2020 3230 3136 2d30 342d 3031 2031      2016-04-01 1
-00003030: 333a 3135 3a31 332c 3233 3420 726f 6f74  3:15:13,234 root
-00003040: 2020 2020 2020 2020 2049 4e46 4f20 2020           INFO   
-00003050: 2020 5371 7561 7368 696e 6720 6669 6c65    Squashing file
-00003060: 2027 2f74 6d70 2f64 6f63 6b65 722d 7371   '/tmp/docker-sq
-00003070: 7561 7368 2d66 7538 3043 582f 6f6c 642f  uash-fu80CX/old/
-00003080: 6238 6661 3363 6166 3764 3664 6332 3238  b8fa3caf7d6dc228
-00003090: 6266 3234 3939 6133 6166 3836 6535 3037  bf2499a3af86e507
-000030a0: 3361 6430 6331 3733 3034 6333 3930 3066  3ad0c17304c3900f
-000030b0: 6133 3431 6539 6432 6665 3465 3536 3535  a341e9d2fe4e5655
-000030c0: 2f6c 6179 6572 2e74 6172 272e 2e2e 0a20  /layer.tar'.... 
-000030d0: 2020 2032 3031 362d 3034 2d30 3120 3133     2016-04-01 13
-000030e0: 3a31 353a 3133 2c32 3335 2072 6f6f 7420  :15:13,235 root 
-000030f0: 2020 2020 2020 2020 494e 464f 2020 2020          INFO    
-00003100: 2053 7175 6173 6869 6e67 2066 696c 6520   Squashing file 
-00003110: 272f 746d 702f 646f 636b 6572 2d73 7175  '/tmp/docker-squ
-00003120: 6173 682d 6675 3830 4358 2f6f 6c64 2f33  ash-fu80CX/old/3
-00003130: 3862 3866 3835 6537 3462 6661 3737 3361  8b8f85e74bfa773a
-00003140: 3061 6436 3964 6132 3230 3564 6330 3134  0ad69da2205dc014
-00003150: 3839 3435 6536 6635 6137 6365 6230 3466  8945e6f5a7ceb04f
-00003160: 6134 6538 3631 3965 3164 6534 3235 622f  a4e8619e1de425b/
-00003170: 6c61 7965 722e 7461 7227 2e2e 2e0a 2020  layer.tar'....  
-00003180: 2020 3230 3136 2d30 342d 3031 2031 333a    2016-04-01 13:
-00003190: 3135 3a31 332c 3233 3520 726f 6f74 2020  15:13,235 root  
-000031a0: 2020 2020 2020 2049 4e46 4f20 2020 2020         INFO     
-000031b0: 5371 7561 7368 696e 6720 6669 6c65 2027  Squashing file '
-000031c0: 2f74 6d70 2f64 6f63 6b65 722d 7371 7561  /tmp/docker-squa
-000031d0: 7368 2d66 7538 3043 582f 6f6c 642f 6165  sh-fu80CX/old/ae
-000031e0: 3739 6236 3436 6239 6139 6132 3837 6335  79b646b9a9a287c5
-000031f0: 6636 6130 3138 3731 6363 3964 3965 6535  f6a01871cc9d9ee5
-00003200: 3936 6461 6665 6532 6462 3934 3237 3134  96dafee2db942714
-00003210: 6361 3364 6561 3063 3036 6565 6633 2f6c  ca3dea0c06eef3/l
-00003220: 6179 6572 2e74 6172 272e 2e2e 0a20 2020  ayer.tar'....   
-00003230: 2032 3031 362d 3034 2d30 3120 3133 3a31   2016-04-01 13:1
-00003240: 353a 3133 2c32 3335 2072 6f6f 7420 2020  5:13,235 root   
-00003250: 2020 2020 2020 494e 464f 2020 2020 2053        INFO     S
-00003260: 7175 6173 6869 6e67 2066 696c 6520 272f  quashing file '/
-00003270: 746d 702f 646f 636b 6572 2d73 7175 6173  tmp/docker-squas
-00003280: 682d 6675 3830 4358 2f6f 6c64 2f32 6234  h-fu80CX/old/2b4
-00003290: 3630 3664 6339 6463 3737 3361 6132 3230  606dc9dc773aa220
-000032a0: 6136 3533 3531 6665 3864 3534 6630 3335  a65351fe8d54f035
-000032b0: 3334 6335 3866 6561 3233 3039 3630 6539  34c58fea230960e9
-000032c0: 3539 3135 3232 3233 3636 3037 342f 6c61  5915222366074/la
-000032d0: 7965 722e 7461 7227 2e2e 2e0a 2020 2020  yer.tar'....    
-000032e0: 3230 3136 2d30 342d 3031 2031 333a 3135  2016-04-01 13:15
-000032f0: 3a31 332c 3233 3620 726f 6f74 2020 2020  :13,236 root    
-00003300: 2020 2020 2049 4e46 4f20 2020 2020 5371       INFO     Sq
-00003310: 7561 7368 696e 6720 6669 6c65 2027 2f74  uashing file '/t
-00003320: 6d70 2f64 6f63 6b65 722d 7371 7561 7368  mp/docker-squash
-00003330: 2d66 7538 3043 582f 6f6c 642f 3131 3866  -fu80CX/old/118f
-00003340: 6139 6533 3335 3736 6563 6336 3235 6562  a9e33576ecc625eb
-00003350: 6262 6664 6632 3830 3963 3135 3237 6537  bbfdf2809c1527e7
-00003360: 3136 6362 3466 6435 6362 3430 3534 3865  16cb4fd5cb40548e
-00003370: 6236 6433 3530 3361 3735 6139 2f6c 6179  b6d3503a75a9/lay
-00003380: 6572 2e74 6172 272e 2e2e 0a20 2020 2032  er.tar'....    2
-00003390: 3031 362d 3034 2d30 3120 3133 3a31 353a  016-04-01 13:15:
-000033a0: 3133 2c32 3336 2072 6f6f 7420 2020 2020  13,236 root     
-000033b0: 2020 2020 494e 464f 2020 2020 2053 7175      INFO     Squ
-000033c0: 6173 6869 6e67 2066 696c 6520 272f 746d  ashing file '/tm
-000033d0: 702f 646f 636b 6572 2d73 7175 6173 682d  p/docker-squash-
-000033e0: 6675 3830 4358 2f6f 6c64 2f35 6637 6538  fu80CX/old/5f7e8
-000033f0: 6633 3663 3362 6232 3063 3964 6237 3437  f36c3bb20c9db747
-00003400: 3061 3232 6638 3238 3731 3062 3464 3238  0a22f828710b4d28
-00003410: 6165 6465 3634 3936 3663 3432 3561 6464  aede64966c425add
-00003420: 3438 6131 6231 3466 6532 332f 6c61 7965  48a1b14fe23/laye
-00003430: 722e 7461 7227 2e2e 2e0a 2020 2020 3230  r.tar'....    20
-00003440: 3136 2d30 342d 3031 2031 333a 3135 3a31  16-04-01 13:15:1
-00003450: 342c 3834 3820 726f 6f74 2020 2020 2020  4,848 root      
-00003460: 2020 2049 4e46 4f20 2020 2020 5371 7561     INFO     Squa
-00003470: 7368 696e 6720 6669 6e69 7368 6564 210a  shing finished!.
-00003480: 2020 2020 3230 3136 2d30 342d 3031 2031      2016-04-01 1
-00003490: 333a 3135 3a31 342c 3835 3320 726f 6f74  3:15:14,853 root
-000034a0: 2020 2020 2020 2020 2049 4e46 4f20 2020           INFO   
-000034b0: 2020 4e65 7720 7371 7561 7368 6564 2069    New squashed i
-000034c0: 6d61 6765 2049 4420 6973 2066 6465 3765  mage ID is fde7e
-000034d0: 6464 3265 3536 3833 6339 3762 6564 6639  dd2e5683c97bedf9
-000034e0: 6330 6266 3532 6164 3531 3530 6462 3536  c0bf52ad5150db56
-000034f0: 3530 6534 3231 6465 3364 3932 3933 6365  50e421de3d9293ce
-00003500: 3532 3233 6232 3536 3435 350a 2020 2020  5223b256455.    
-00003510: 3230 3136 2d30 342d 3031 2031 333a 3135  2016-04-01 13:15
-00003520: 3a31 382c 3936 3320 726f 6f74 2020 2020  :18,963 root    
-00003530: 2020 2020 2049 4e46 4f20 2020 2020 496d       INFO     Im
-00003540: 6167 6520 7265 6769 7374 6572 6564 2069  age registered i
-00003550: 6e20 446f 636b 6572 2064 6165 6d6f 6e20  n Docker daemon 
-00003560: 6173 206a 626f 7373 2f77 696c 6466 6c79  as jboss/wildfly
-00003570: 3a73 7175 6173 6865 640a 2020 2020 3230  :squashed.    20
-00003580: 3136 2d30 342d 3031 2031 333a 3135 3a31  16-04-01 13:15:1
-00003590: 392c 3035 3920 726f 6f74 2020 2020 2020  9,059 root      
-000035a0: 2020 2049 4e46 4f20 2020 2020 446f 6e65     INFO     Done
-000035b0: 0a0a 4c65 7427 7320 636f 6e66 6972 6d20  ..Let's confirm 
-000035c0: 7468 6520 696d 6167 6520 7374 7275 6374  the image struct
-000035d0: 7572 6520 6e6f 773a 0a0a 3a3a 0a0a 2020  ure now:..::..  
-000035e0: 2020 2420 646f 636b 6572 2068 6973 746f    $ docker histo
-000035f0: 7279 206a 626f 7373 2f77 696c 6466 6c79  ry jboss/wildfly
-00003600: 3a73 7175 6173 6865 640a 2020 2020 494d  :squashed.    IM
-00003610: 4147 4520 2020 2020 2020 2020 2020 2020  AGE             
-00003620: 2020 4352 4541 5445 4420 2020 2020 2020    CREATED       
-00003630: 2020 2020 2020 4352 4541 5445 4420 4259        CREATED BY
-00003640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003660: 2020 2020 2020 5349 5a45 2020 2020 2020        SIZE      
-00003670: 2020 2020 2020 2020 2020 434f 4d4d 454e            COMMEN
-00003680: 540a 2020 2020 6664 6537 6564 6432 6535  T.    fde7edd2e5
-00003690: 3638 2020 2020 2020 2020 3332 2073 6563  68        32 sec
-000036a0: 6f6e 6473 2061 676f 2020 2020 2020 2020  onds ago        
-000036b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000036c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000036d0: 2020 2020 2020 2020 2020 2020 2020 3335                35
-000036e0: 382e 3220 4d42 2020 2020 2020 2020 2020  8.2 MB          
-000036f0: 2020 0a20 2020 2033 6434 6430 3232 3866    .    3d4d0228f
-00003700: 3136 3120 2020 2020 2020 2033 2077 6565  161        3 wee
-00003710: 6b73 2061 676f 2020 2020 2020 2020 202f  ks ago         /
-00003720: 6269 6e2f 7368 202d 6320 2328 6e6f 7029  bin/sh -c #(nop)
-00003730: 2055 5345 5220 5b72 6f6f 745d 2020 2020   USER [root]    
-00003740: 2020 2020 2020 2020 2020 2020 2020 2030                 0
-00003750: 2042 2020 2020 2020 2020 2020 2020 2020   B              
-00003760: 2020 200a 2020 2020 6637 6162 3465 6131     .    f7ab4ea1
-00003770: 3937 3038 2020 2020 2020 2020 3320 7765  9708        3 we
-00003780: 656b 7320 6167 6f20 2020 2020 2020 2020  eks ago         
-00003790: 2f62 696e 2f73 6820 2d63 2023 286e 6f70  /bin/sh -c #(nop
-000037a0: 2920 4d41 494e 5441 494e 4552 204d 6172  ) MAINTAINER Mar
-000037b0: 656b 2047 6f6c 646d 616e 6e20 3c20 2020  ek Goldmann <   
-000037c0: 3020 4220 2020 2020 2020 2020 2020 2020  0 B             
-000037d0: 2020 2020 0a20 2020 2034 6262 3135 6633      .    4bb15f3
-000037e0: 6236 3937 3720 2020 2020 2020 2033 2077  b6977        3 w
-000037f0: 6565 6b73 2061 676f 2020 2020 2020 2020  eeks ago        
-00003800: 202f 6269 6e2f 7368 202d 6320 2328 6e6f   /bin/sh -c #(no
-00003810: 7029 2055 5345 5220 5b6a 626f 7373 5d20  p) USER [jboss] 
-00003820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003830: 2030 2042 2020 2020 2020 2020 2020 2020   0 B            
-00003840: 2020 2020 200a 2020 2020 3564 6331 6534       .    5dc1e4
-00003850: 3966 3433 3631 2020 2020 2020 2020 3320  9f4361        3 
-00003860: 7765 656b 7320 6167 6f20 2020 2020 2020  weeks ago       
-00003870: 2020 2f62 696e 2f73 6820 2d63 2023 286e    /bin/sh -c #(n
-00003880: 6f70 2920 574f 524b 4449 5220 2f6f 7074  op) WORKDIR /opt
-00003890: 2f6a 626f 7373 2020 2020 2020 2020 2020  /jboss          
-000038a0: 2020 3020 4220 2020 2020 2020 2020 2020    0 B           
-000038b0: 2020 2020 2020 0a20 2020 2037 6630 6639        .    7f0f9
-000038c0: 6562 3331 3137 3420 2020 2020 2020 2033  eb31174        3
-000038d0: 2077 6565 6b73 2061 676f 2020 2020 2020   weeks ago      
-000038e0: 2020 202f 6269 6e2f 7368 202d 6320 6772     /bin/sh -c gr
-000038f0: 6f75 7061 6464 202d 7220 6a62 6f73 7320  oupadd -r jboss 
-00003900: 2d67 2031 3030 3020 2626 2075 7365 7261  -g 1000 && usera
-00003910: 2020 2034 2e33 3439 206b 4220 2020 2020     4.349 kB     
-00003920: 2020 2020 2020 200a 2020 2020 6264 3531         .    bd51
-00003930: 3566 3034 3461 6637 2020 2020 2020 2020  5f044af7        
-00003940: 3320 7765 656b 7320 6167 6f20 2020 2020  3 weeks ago     
-00003950: 2020 2020 2f62 696e 2f73 6820 2d63 2079      /bin/sh -c y
-00003960: 756d 2075 7064 6174 6520 2d79 2026 2620  um update -y && 
-00003970: 7975 6d20 2d79 2069 6e73 7461 6c6c 2078  yum -y install x
-00003980: 6d20 2020 3235 2e31 3820 4d42 2020 2020  m   25.18 MB    
-00003990: 2020 2020 2020 2020 0a20 2020 2062 3738          .    b78
-000039a0: 3333 3630 3939 3034 3520 2020 2020 2020  336099045       
-000039b0: 2033 2077 6565 6b73 2061 676f 2020 2020   3 weeks ago    
-000039c0: 2020 2020 202f 6269 6e2f 7368 202d 6320       /bin/sh -c 
-000039d0: 2328 6e6f 7029 204d 4149 4e54 4149 4e45  #(nop) MAINTAINE
-000039e0: 5220 4d61 7265 6b20 476f 6c64 6d61 6e6e  R Marek Goldmann
-000039f0: 203c 2020 2030 2042 2020 2020 2020 2020   <   0 B        
-00003a00: 2020 2020 2020 2020 200a 2020 2020 3438           .    48
-00003a10: 3136 6132 3938 3534 3863 2020 2020 2020  16a298548c      
-00003a20: 2020 3320 7765 656b 7320 6167 6f20 2020    3 weeks ago   
-00003a30: 2020 2020 2020 2f62 696e 2f73 6820 2d63        /bin/sh -c
-00003a40: 2023 286e 6f70 2920 434d 4420 5b22 2f62   #(nop) CMD ["/b
-00003a50: 696e 2f62 6173 6822 5d20 2020 2020 2020  in/bash"]       
-00003a60: 2020 2020 2020 3020 4220 2020 2020 2020        0 B       
-00003a70: 2020 2020 2020 2020 2020 0a20 2020 2036            .    6
-00003a80: 6565 3233 3563 6634 3437 3320 2020 2020  ee235cf4473     
+00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
+00000010: 3a20 322e 310a 4e61 6d65 3a20 646f 636b  : 2.1.Name: dock
+00000020: 6572 2d73 7175 6173 680a 5665 7273 696f  er-squash.Versio
+00000030: 6e3a 2031 2e31 2e30 0a53 756d 6d61 7279  n: 1.1.0.Summary
+00000040: 3a20 446f 636b 6572 206c 6179 6572 2073  : Docker layer s
+00000050: 7175 6173 6869 6e67 2074 6f6f 6c0a 486f  quashing tool.Ho
+00000060: 6d65 2d70 6167 653a 2068 7474 7073 3a2f  me-page: https:/
+00000070: 2f67 6974 6875 622e 636f 6d2f 676f 6c64  /github.com/gold
+00000080: 6d61 6e6e 2f64 6f63 6b65 722d 7371 7561  mann/docker-squa
+00000090: 7368 0a44 6f77 6e6c 6f61 642d 5552 4c3a  sh.Download-URL:
+000000a0: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
+000000b0: 636f 6d2f 676f 6c64 6d61 6e6e 2f64 6f63  com/goldmann/doc
+000000c0: 6b65 722d 7371 7561 7368 2f61 7263 6869  ker-squash/archi
+000000d0: 7665 2f31 2e31 2e30 2e74 6172 2e67 7a0a  ve/1.1.0.tar.gz.
+000000e0: 4175 7468 6f72 3a20 4d61 7265 6b20 476f  Author: Marek Go
+000000f0: 6c64 6d61 6e6e 0a41 7574 686f 722d 656d  ldmann.Author-em
+00000100: 6169 6c3a 206d 6172 656b 2e67 6f6c 646d  ail: marek.goldm
+00000110: 616e 6e40 676d 6169 6c2e 636f 6d0a 4c69  ann@gmail.com.Li
+00000120: 6365 6e73 653a 204d 4954 0a4b 6579 776f  cense: MIT.Keywo
+00000130: 7264 733a 2064 6f63 6b65 720a 4c69 6365  rds: docker.Lice
+00000140: 6e73 652d 4669 6c65 3a20 4c49 4345 4e53  nse-File: LICENS
+00000150: 450a 0a60 6064 6f63 6b65 722d 7371 7561  E..``docker-squa
+00000160: 7368 6060 0a3d 3d3d 3d3d 3d3d 3d3d 3d3d  sh``.===========
+00000170: 3d3d 3d3d 3d3d 3d0a 0a2e 2e20 696d 6167  =======.... imag
+00000180: 653a 3a20 6874 7470 733a 2f2f 6769 7468  e:: https://gith
+00000190: 7562 2e63 6f6d 2f67 6f6c 646d 616e 6e2f  ub.com/goldmann/
+000001a0: 646f 636b 6572 2d73 7175 6173 682f 6163  docker-squash/ac
+000001b0: 7469 6f6e 732f 776f 726b 666c 6f77 732f  tions/workflows/
+000001c0: 7371 7561 7368 2e79 6d6c 2f62 6164 6765  squash.yml/badge
+000001d0: 2e73 7667 0a20 2020 203a 7461 7267 6574  .svg.    :target
+000001e0: 3a20 6874 7470 733a 2f2f 6769 7468 7562  : https://github
+000001f0: 2e63 6f6d 2f67 6f6c 646d 616e 6e2f 646f  .com/goldmann/do
+00000200: 636b 6572 2d73 7175 6173 682f 6163 7469  cker-squash/acti
+00000210: 6f6e 732f 776f 726b 666c 6f77 732f 7371  ons/workflows/sq
+00000220: 7561 7368 2e79 6d6c 0a0a 5468 6520 7072  uash.yml..The pr
+00000230: 6f62 6c65 6d0a 2d2d 2d2d 2d2d 2d2d 2d2d  oblem.----------
+00000240: 2d0a 0a44 6f63 6b65 7220 6372 6561 7465  -..Docker create
+00000250: 7320 6d61 6e79 206c 6179 6572 7320 7768  s many layers wh
+00000260: 696c 6520 6275 696c 6469 6e67 2074 6865  ile building the
+00000270: 2069 6d61 6765 2e20 536f 6d65 7469 6d65   image. Sometime
+00000280: 7320 6974 2773 206e 6f74 206e 6563 6573  s it's not neces
+00000290: 7361 7279 206f 7220 6465 7369 7265 6162  sary or desireab
+000002a0: 6c65 0a74 6f20 6861 7665 2074 6865 6d20  le.to have them 
+000002b0: 696e 2074 6865 2069 6d61 6765 2e20 466f  in the image. Fo
+000002c0: 7220 6578 616d 706c 6520 6120 446f 636b  r example a Dock
+000002d0: 6572 6669 6c65 2060 4144 4460 2069 6e73  erfile `ADD` ins
+000002e0: 7472 7563 7469 6f6e 2063 7265 6174 6573  truction creates
+000002f0: 2061 2073 696e 676c 6520 6c61 7965 720a   a single layer.
+00000300: 7769 7468 2066 696c 6573 2079 6f75 2077  with files you w
+00000310: 616e 7420 746f 206d 616b 6520 6176 6169  ant to make avai
+00000320: 6c61 626c 6520 696e 2074 6865 2069 6d61  lable in the ima
+00000330: 6765 2e20 5468 6520 7072 6f62 6c65 6d20  ge. The problem 
+00000340: 6172 6973 6573 2077 6865 6e20 7468 6573  arises when thes
+00000350: 6520 6669 6c65 7320 6172 650a 6f6e 6c79  e files are.only
+00000360: 2074 656d 706f 7261 7279 2066 696c 6573   temporary files
+00000370: 2028 666f 7220 6578 616d 706c 6520 7072   (for example pr
+00000380: 6f64 7563 7420 6469 7374 7269 6275 7469  oduct distributi
+00000390: 6f6e 2074 6861 7420 796f 7520 7761 6e74  on that you want
+000003a0: 2074 6f20 756e 7061 636b 292e 2044 6f63   to unpack). Doc
+000003b0: 6b65 7220 7769 6c6c 0a63 6172 7279 2074  ker will.carry t
+000003c0: 6869 7320 756e 6e65 6365 7373 6172 7920  his unnecessary 
+000003d0: 6c61 7965 7220 616c 7761 7973 2077 6974  layer always wit
+000003e0: 6820 7468 6520 696d 6167 652c 2065 7665  h the image, eve
+000003f0: 6e20 6966 2079 6f75 2064 656c 6574 6520  n if you delete 
+00000400: 7468 6573 6520 6669 6c65 7320 696e 206e  these files in n
+00000410: 6578 740a 6c61 7965 722e 2054 6869 7320  ext.layer. This 
+00000420: 6120 7761 7374 6520 6f66 2074 696d 6520  a waste of time 
+00000430: 286d 6f72 6520 6461 7461 2074 6f20 7075  (more data to pu
+00000440: 7368 2f6c 6f61 642f 7361 7665 2920 616e  sh/load/save) an
+00000450: 6420 7265 736f 7572 6365 7320 2862 6967  d resources (big
+00000460: 6765 7220 696d 6167 6529 2e0a 0a53 7175  ger image)...Squ
+00000470: 6173 6869 6e67 2068 656c 7073 2077 6974  ashing helps wit
+00000480: 6820 6f72 6761 6e69 7a69 6e67 2069 6d61  h organizing ima
+00000490: 6765 7320 696e 206c 6f67 6963 616c 206c  ges in logical l
+000004a0: 6179 6572 732e 2049 6e73 7465 6164 206f  ayers. Instead o
+000004b0: 660a 6861 7669 6e67 2061 6e20 696d 6167  f.having an imag
+000004c0: 6520 7769 7468 206d 756c 7469 706c 6520  e with multiple 
+000004d0: 2869 6e20 616c 6d6f 7374 2061 6c6c 2063  (in almost all c
+000004e0: 6173 6573 2920 756e 6e65 6365 7373 6172  ases) unnecessar
+000004f0: 7920 6c61 7965 7273 202d 0a77 6520 6361  y layers -.we ca
+00000500: 6e20 636f 6e74 726f 6c20 7468 6520 7374  n control the st
+00000510: 7275 6374 7572 6520 6f66 2074 6865 2069  ructure of the i
+00000520: 6d61 6765 2e0a 0a46 6561 7475 7265 730a  mage...Features.
+00000530: 2d2d 2d2d 2d2d 2d2d 0a0a 2d20 4361 6e20  --------..- Can 
+00000540: 7371 7561 7368 206c 6173 7420 6e20 6c61  squash last n la
+00000550: 7965 7273 2066 726f 6d20 616e 2069 6d61  yers from an ima
+00000560: 6765 0a2d 2043 616e 2073 7175 6173 6820  ge.- Can squash 
+00000570: 6672 6f6d 2061 2073 656c 6563 7465 6420  from a selected 
+00000580: 6c61 7965 7220 746f 2074 6865 2065 6e64  layer to the end
+00000590: 2028 6e6f 7420 616c 7761 7973 2070 6f73   (not always pos
+000005a0: 7369 626c 652c 2064 6570 656e 6473 206f  sible, depends o
+000005b0: 6e20 7468 6520 696d 6167 6529 0a2d 2053  n the image).- S
+000005c0: 7570 706f 7274 2066 6f72 2044 6f63 6b65  upport for Docke
+000005d0: 7220 312e 3920 6f72 206e 6577 6572 2028  r 1.9 or newer (
+000005e0: 6f6c 6465 7220 7265 6c65 6173 6573 206d  older releases m
+000005f0: 6179 2072 756e 2070 6572 6665 6374 6c79  ay run perfectly
+00000600: 2066 696e 6520 746f 6f2c 2074 7279 2069   fine too, try i
+00000610: 7421 290a 2d20 5371 7561 7368 6564 2069  t!).- Squashed i
+00000620: 6d61 6765 2063 616e 2062 6520 6c6f 6164  mage can be load
+00000630: 6564 2062 6163 6b20 746f 2074 6865 2044  ed back to the D
+00000640: 6f63 6b65 7220 6461 656d 6f6e 206f 7220  ocker daemon or 
+00000650: 7374 6f72 6564 2061 7320 7461 7220 6172  stored as tar ar
+00000660: 6368 6976 6520 736f 6d65 7768 6572 650a  chive somewhere.
+00000670: 0a49 6e73 7461 6c6c 6174 696f 6e0a 2d2d  .Installation.--
+00000680: 2d2d 2d2d 2d2d 2d2d 2d2d 0a0a 4672 6f6d  ----------..From
+00000690: 2073 6f75 7263 6520 636f 6465 0a0a 3a3a   source code..::
+000006a0: 0a0a 2020 2020 2420 7069 7020 696e 7374  ..    $ pip inst
+000006b0: 616c 6c20 2d2d 7573 6572 2068 7474 7073  all --user https
+000006c0: 3a2f 2f67 6974 6875 622e 636f 6d2f 676f  ://github.com/go
+000006d0: 6c64 6d61 6e6e 2f64 6f63 6b65 722d 7371  ldmann/docker-sq
+000006e0: 7561 7368 2f61 7263 6869 7665 2f6d 6173  uash/archive/mas
+000006f0: 7465 722e 7a69 700a 0a46 726f 6d20 5079  ter.zip..From Py
+00000700: 5069 0a0a 3a3a 0a0a 2020 2020 2420 7069  Pi..::..    $ pi
+00000710: 7020 696e 7374 616c 6c20 646f 636b 6572  p install docker
+00000720: 2d73 7175 6173 680a 0a49 7420 6973 2073  -squash..It is s
+00000730: 7570 706f 7274 6564 206f 6e20 5079 7468  upported on Pyth
+00000740: 6f6e 2033 2e36 2061 6e64 2061 626f 7665  on 3.6 and above
+00000750: 2e0a 0a55 7361 6765 0a2d 2d2d 2d2d 0a0a  ...Usage.-----..
+00000760: 3a3a 0a0a 2020 2020 2420 646f 636b 6572  ::..    $ docker
+00000770: 2d73 7175 6173 6820 2d68 0a20 2020 2075  -squash -h.    u
+00000780: 7361 6765 3a20 636c 692e 7079 205b 2d68  sage: cli.py [-h
+00000790: 5d20 5b2d 765d 205b 2d2d 7665 7273 696f  ] [-v] [--versio
+000007a0: 6e5d 205b 2d64 5d20 5b2d 6620 4652 4f4d  n] [-d] [-f FROM
+000007b0: 5f4c 4159 4552 5d20 5b2d 7420 5441 475d  _LAYER] [-t TAG]
+000007c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000007d0: 2020 205b 2d2d 746d 702d 6469 7220 544d     [--tmp-dir TM
+000007e0: 505f 4449 525d 205b 2d2d 6f75 7470 7574  P_DIR] [--output
+000007f0: 2d70 6174 6820 4f55 5450 5554 5f50 4154  -path OUTPUT_PAT
+00000800: 485d 0a20 2020 2020 2020 2020 2020 2020  H].             
+00000810: 2020 2020 2069 6d61 6765 0a0a 2020 2020       image..    
+00000820: 446f 636b 6572 206c 6179 6572 2073 7175  Docker layer squ
+00000830: 6173 6869 6e67 2074 6f6f 6c0a 0a20 2020  ashing tool..   
+00000840: 2070 6f73 6974 696f 6e61 6c20 6172 6775   positional argu
+00000850: 6d65 6e74 733a 0a20 2020 2020 2069 6d61  ments:.      ima
+00000860: 6765 2020 2020 2020 2020 2020 2020 2020  ge              
+00000870: 2020 2049 6d61 6765 2074 6f20 6265 2073     Image to be s
+00000880: 7175 6173 6865 640a 0a20 2020 206f 7074  quashed..    opt
+00000890: 696f 6e61 6c20 6172 6775 6d65 6e74 733a  ional arguments:
+000008a0: 0a20 2020 2020 202d 682c 202d 2d68 656c  .      -h, --hel
+000008b0: 7020 2020 2020 2020 2020 2020 2073 686f  p            sho
+000008c0: 7720 7468 6973 2068 656c 7020 6d65 7373  w this help mess
+000008d0: 6167 6520 616e 6420 6578 6974 0a20 2020  age and exit.   
+000008e0: 2020 202d 762c 202d 2d76 6572 626f 7365     -v, --verbose
+000008f0: 2020 2020 2020 2020 2056 6572 626f 7365           Verbose
+00000900: 206f 7574 7075 740a 2020 2020 2020 2d2d   output.      --
+00000910: 7665 7273 696f 6e20 2020 2020 2020 2020  version         
+00000920: 2020 2020 5368 6f77 2076 6572 7369 6f6e      Show version
+00000930: 2061 6e64 2065 7869 740a 2020 2020 2020   and exit.      
+00000940: 2d64 2c20 2d2d 6465 7665 6c6f 706d 656e  -d, --developmen
+00000950: 7420 2020 2020 446f 6573 206e 6f74 2063  t     Does not c
+00000960: 6c65 616e 2075 7020 6166 7465 7220 6661  lean up after fa
+00000970: 696c 7572 6520 666f 7220 6561 7369 6572  ilure for easier
+00000980: 2064 6562 7567 6769 6e67 0a20 2020 2020   debugging.     
+00000990: 202d 6620 4652 4f4d 5f4c 4159 4552 2c20   -f FROM_LAYER, 
+000009a0: 2d2d 6672 6f6d 2d6c 6179 6572 2046 524f  --from-layer FRO
+000009b0: 4d5f 4c41 5945 520a 2020 2020 2020 2020  M_LAYER.        
+000009c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000009d0: 2020 2020 4e75 6d62 6572 206f 6620 6c61      Number of la
+000009e0: 7965 7273 2074 6f20 7371 7561 7368 206f  yers to squash o
+000009f0: 7220 4944 206f 6620 7468 6520 6c61 7965  r ID of the laye
+00000a00: 7220 286f 7220 696d 6167 6520 4944 206f  r (or image ID o
+00000a10: 7220 696d 6167 6520 6e61 6d65 2920 746f  r image name) to
+00000a20: 2073 7175 6173 6820 6672 6f6d 2e0a 2020   squash from..  
+00000a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000a40: 2020 2020 2020 2020 2020 496e 2063 6173            In cas
+00000a50: 6520 7468 6520 7072 6f76 6964 6564 2076  e the provided v
+00000a60: 616c 7565 2069 7320 616e 2069 6e74 6567  alue is an integ
+00000a70: 6572 2c20 7370 6563 6966 6965 6420 6e75  er, specified nu
+00000a80: 6d62 6572 206f 6620 6c61 7965 7273 2077  mber of layers w
+00000a90: 696c 6c20 6265 2073 7175 6173 6865 642e  ill be squashed.
+00000aa0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000ab0: 2020 2020 2020 2020 2020 2020 2045 7665               Eve
+00000ac0: 7279 206c 6179 6572 2069 6e20 7468 6520  ry layer in the 
+00000ad0: 696d 6167 6520 7769 6c6c 2062 6520 7371  image will be sq
+00000ae0: 7561 7368 6564 2069 6620 7468 6520 7061  uashed if the pa
+00000af0: 7261 6d65 7465 7220 6973 206e 6f74 2070  rameter is not p
+00000b00: 726f 7669 6465 642e 0a20 2020 2020 202d  rovided..      -
+00000b10: 7420 5441 472c 202d 2d74 6167 2054 4147  t TAG, --tag TAG
+00000b20: 2020 2020 2053 7065 6369 6679 2074 6865       Specify the
+00000b30: 2074 6167 2074 6f20 6265 2075 7365 6420   tag to be used 
+00000b40: 666f 7220 7468 6520 6e65 7720 696d 6167  for the new imag
+00000b50: 652e 2049 6620 6e6f 7420 7370 6563 6966  e. If not specif
+00000b60: 6965 6420 6e6f 2074 6167 2077 696c 6c20  ied no tag will 
+00000b70: 6265 2061 7070 6c69 6564 0a20 2020 2020  be applied.     
+00000b80: 202d 6d20 4d45 5353 4147 452c 202d 2d6d   -m MESSAGE, --m
+00000b90: 6573 7361 6765 204d 4553 5341 4745 0a20  essage MESSAGE. 
+00000ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000bb0: 2020 2020 2020 2020 2020 2053 7065 6369             Speci
+00000bc0: 6679 2061 2063 6f6d 6d69 7420 6d65 7373  fy a commit mess
+00000bd0: 6167 6520 2863 6f6d 6d65 6e74 2920 666f  age (comment) fo
+00000be0: 7220 7468 6520 6e65 7720 696d 6167 652e  r the new image.
+00000bf0: 0a20 2020 2020 202d 632c 202d 2d63 6c65  .      -c, --cle
+00000c00: 616e 7570 2020 2020 2020 2020 2052 656d  anup         Rem
+00000c10: 6f76 6520 736f 7572 6365 2069 6d61 6765  ove source image
+00000c20: 2066 726f 6d20 446f 636b 6572 2061 6674   from Docker aft
+00000c30: 6572 2073 7175 6173 6869 6e67 0a20 2020  er squashing.   
+00000c40: 2020 202d 2d74 6d70 2d64 6972 2054 4d50     --tmp-dir TMP
+00000c50: 5f44 4952 2020 2020 2054 656d 706f 7261  _DIR     Tempora
+00000c60: 7279 2064 6972 6563 746f 7279 2074 6f20  ry directory to 
+00000c70: 6265 2063 7265 6174 6564 2061 6e64 2075  be created and u
+00000c80: 7365 640a 2020 2020 2020 2d2d 6f75 7470  sed.      --outp
+00000c90: 7574 2d70 6174 6820 4f55 5450 5554 5f50  ut-path OUTPUT_P
+00000ca0: 4154 480a 2020 2020 2020 2020 2020 2020  ATH.            
+00000cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000cc0: 5061 7468 2077 6865 7265 2074 6865 2069  Path where the i
+00000cd0: 6d61 6765 206d 6179 2062 6520 7374 6f72  mage may be stor
+00000ce0: 6564 2061 6674 6572 2073 7175 6173 6869  ed after squashi
+00000cf0: 6e67 2e0a 2020 2020 2020 2d2d 6c6f 6164  ng..      --load
+00000d00: 2d69 6d61 6765 205b 4c4f 4144 5f49 4d41  -image [LOAD_IMA
+00000d10: 4745 5d0a 2020 2020 2020 2020 2020 2020  GE].            
+00000d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000d30: 5768 6574 6865 7220 746f 206c 6f61 6420  Whether to load 
+00000d40: 7468 6520 696d 6167 6520 696e 746f 2044  the image into D
+00000d50: 6f63 6b65 7220 6461 656d 6f6e 2061 6674  ocker daemon aft
+00000d60: 6572 2073 7175 6173 6869 6e67 0a20 2020  er squashing.   
+00000d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000d80: 2020 2020 2020 2020 2044 6566 6175 6c74           Default
+00000d90: 3a20 7472 7565 0a0a 4e6f 7465 2074 6861  : true..Note tha
+00000da0: 7420 656e 7669 726f 6e6d 656e 7420 7661  t environment va
+00000db0: 7269 6162 6c65 7320 6d61 7920 6265 2073  riables may be s
+00000dc0: 6574 2061 7320 646f 6375 6d65 6e74 6564  et as documented
+00000dd0: 2069 6e20 6068 6572 6520 3c64 6f63 732f   in `here <docs/
+00000de0: 656e 7669 726f 6e6d 656e 745f 7661 7269  environment_vari
+00000df0: 6162 6c65 732e 6164 6f63 3e60 5f2e 0a0a  ables.adoc>`_...
+00000e00: 4c69 6365 6e73 650a 2d2d 2d2d 2d2d 2d0a  License.-------.
+00000e10: 0a4d 4954 0a0a 4578 616d 706c 6573 0a2d  .MIT..Examples.-
+00000e20: 2d2d 2d2d 2d2d 2d0a 0a57 6520 7374 6172  -------..We star
+00000e30: 7420 7769 7468 2069 6d61 6765 206c 696b  t with image lik
+00000e40: 6520 7468 6973 3a0a 0a3a 3a0a 0a20 2020  e this:..::..   
+00000e50: 2024 2064 6f63 6b65 7220 6869 7374 6f72   $ docker histor
+00000e60: 7920 6a62 6f73 732f 7769 6c64 666c 793a  y jboss/wildfly:
+00000e70: 6c61 7465 7374 0a20 2020 2049 4d41 4745  latest.    IMAGE
+00000e80: 2020 2020 2020 2020 2020 2020 2020 2043                 C
+00000e90: 5245 4154 4544 2020 2020 2020 2020 2020  REATED          
+00000ea0: 2020 2043 5245 4154 4544 2042 5920 2020     CREATED BY   
+00000eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000ed0: 2020 2053 495a 4520 2020 2020 2020 2020     SIZE         
+00000ee0: 2020 2020 2020 2043 4f4d 4d45 4e54 0a20         COMMENT. 
+00000ef0: 2020 2032 3539 3534 6536 6432 3330 3020     25954e6d2300 
+00000f00: 2020 2020 2020 2033 2077 6565 6b73 2061         3 weeks a
+00000f10: 676f 2020 2020 2020 2020 202f 6269 6e2f  go         /bin/
+00000f20: 7368 202d 6320 2328 6e6f 7029 2043 4d44  sh -c #(nop) CMD
+00000f30: 205b 222f 6f70 742f 6a62 6f73 732f 7769   ["/opt/jboss/wi
+00000f40: 6c64 666c 792f 6269 2020 2030 2042 0a20  ldfly/bi   0 B. 
+00000f50: 2020 2035 6165 3639 6362 3435 3461 3520     5ae69cb454a5 
+00000f60: 2020 2020 2020 2033 2077 6565 6b73 2061         3 weeks a
+00000f70: 676f 2020 2020 2020 2020 202f 6269 6e2f  go         /bin/
+00000f80: 7368 202d 6320 2328 6e6f 7029 2045 5850  sh -c #(nop) EXP
+00000f90: 4f53 4520 3830 3830 2f74 6370 2020 2020  OSE 8080/tcp    
+00000fa0: 2020 2020 2020 2020 2020 2030 2042 0a20             0 B. 
+00000fb0: 2020 2064 6332 3437 3132 6633 3563 3420     dc24712f35c4 
+00000fc0: 2020 2020 2020 2033 2077 6565 6b73 2061         3 weeks a
+00000fd0: 676f 2020 2020 2020 2020 202f 6269 6e2f  go         /bin/
+00000fe0: 7368 202d 6320 2328 6e6f 7029 2045 4e56  sh -c #(nop) ENV
+00000ff0: 204c 4155 4e43 485f 4a42 4f53 535f 494e   LAUNCH_JBOSS_IN
+00001000: 5f42 4143 4b47 524f 2020 2030 2042 0a20  _BACKGRO   0 B. 
+00001010: 2020 2064 3932 3931 3239 6434 6338 6520     d929129d4c8e 
+00001020: 2020 2020 2020 2033 2077 6565 6b73 2061         3 weeks a
+00001030: 676f 2020 2020 2020 2020 202f 6269 6e2f  go         /bin/
+00001040: 7368 202d 6320 6364 2024 484f 4d45 2020  sh -c cd $HOME  
+00001050: 2020 2026 2620 6375 726c 202d 4f20 6874     && curl -O ht
+00001060: 7470 733a 2f2f 646f 2020 2031 3630 2e38  tps://do   160.8
+00001070: 204d 420a 2020 2020 6238 6661 3363 6166   MB.    b8fa3caf
+00001080: 3764 3664 2020 2020 2020 2020 3320 7765  7d6d        3 we
+00001090: 656b 7320 6167 6f20 2020 2020 2020 2020  eks ago         
+000010a0: 2f62 696e 2f73 6820 2d63 2023 286e 6f70  /bin/sh -c #(nop
+000010b0: 2920 454e 5620 4a42 4f53 535f 484f 4d45  ) ENV JBOSS_HOME
+000010c0: 3d2f 6f70 742f 6a62 6f73 732f 7720 2020  =/opt/jboss/w   
+000010d0: 3020 420a 2020 2020 3338 6238 6638 3565  0 B.    38b8f85e
+000010e0: 3734 6266 2020 2020 2020 2020 3320 7765  74bf        3 we
+000010f0: 656b 7320 6167 6f20 2020 2020 2020 2020  eks ago         
+00001100: 2f62 696e 2f73 6820 2d63 2023 286e 6f70  /bin/sh -c #(nop
+00001110: 2920 454e 5620 5749 4c44 464c 595f 5348  ) ENV WILDFLY_SH
+00001120: 4131 3d63 3064 6437 3535 3263 3520 2020  A1=c0dd7552c5   
+00001130: 3020 420a 2020 2020 6165 3739 6236 3436  0 B.    ae79b646
+00001140: 6239 6139 2020 2020 2020 2020 3320 7765  b9a9        3 we
+00001150: 656b 7320 6167 6f20 2020 2020 2020 2020  eks ago         
+00001160: 2f62 696e 2f73 6820 2d63 2023 286e 6f70  /bin/sh -c #(nop
+00001170: 2920 454e 5620 5749 4c44 464c 595f 5645  ) ENV WILDFLY_VE
+00001180: 5253 494f 4e3d 3130 2e30 2e30 2e20 2020  RSION=10.0.0.   
+00001190: 3020 420a 2020 2020 3262 3436 3036 6463  0 B.    2b4606dc
+000011a0: 3964 6337 2020 2020 2020 2020 3320 7765  9dc7        3 we
+000011b0: 656b 7320 6167 6f20 2020 2020 2020 2020  eks ago         
+000011c0: 2f62 696e 2f73 6820 2d63 2023 286e 6f70  /bin/sh -c #(nop
+000011d0: 2920 454e 5620 4a41 5641 5f48 4f4d 453d  ) ENV JAVA_HOME=
+000011e0: 2f75 7372 2f6c 6962 2f6a 766d 2f20 2020  /usr/lib/jvm/   
+000011f0: 3020 420a 2020 2020 3131 3866 6139 6533  0 B.    118fa9e3
+00001200: 3335 3736 2020 2020 2020 2020 3320 7765  3576        3 we
+00001210: 656b 7320 6167 6f20 2020 2020 2020 2020  eks ago         
+00001220: 2f62 696e 2f73 6820 2d63 2023 286e 6f70  /bin/sh -c #(nop
+00001230: 2920 5553 4552 205b 6a62 6f73 735d 2020  ) USER [jboss]  
+00001240: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001250: 3020 420a 2020 2020 3566 3765 3866 3336  0 B.    5f7e8f36
+00001260: 6333 6262 2020 2020 2020 2020 3320 7765  c3bb        3 we
+00001270: 656b 7320 6167 6f20 2020 2020 2020 2020  eks ago         
+00001280: 2f62 696e 2f73 6820 2d63 2079 756d 202d  /bin/sh -c yum -
+00001290: 7920 696e 7374 616c 6c20 6a61 7661 2d31  y install java-1
+000012a0: 2e38 2e30 2d6f 7065 6e6a 646b 2d20 2020  .8.0-openjdk-   
+000012b0: 3139 372e 3420 4d42 0a20 2020 2033 6434  197.4 MB.    3d4
+000012c0: 6430 3232 3866 3136 3120 2020 2020 2020  d0228f161       
+000012d0: 2033 2077 6565 6b73 2061 676f 2020 2020   3 weeks ago    
+000012e0: 2020 2020 202f 6269 6e2f 7368 202d 6320       /bin/sh -c 
+000012f0: 2328 6e6f 7029 2055 5345 5220 5b72 6f6f  #(nop) USER [roo
+00001300: 745d 2020 2020 2020 2020 2020 2020 2020  t]              
+00001310: 2020 2020 2030 2042 0a20 2020 2066 3761       0 B.    f7a
+00001320: 6234 6561 3139 3730 3820 2020 2020 2020  b4ea19708       
+00001330: 2033 2077 6565 6b73 2061 676f 2020 2020   3 weeks ago    
+00001340: 2020 2020 202f 6269 6e2f 7368 202d 6320       /bin/sh -c 
+00001350: 2328 6e6f 7029 204d 4149 4e54 4149 4e45  #(nop) MAINTAINE
+00001360: 5220 4d61 7265 6b20 476f 6c64 6d61 6e6e  R Marek Goldmann
+00001370: 203c 2020 2030 2042 0a20 2020 2034 6262   <   0 B.    4bb
+00001380: 3135 6633 6236 3937 3720 2020 2020 2020  15f3b6977       
+00001390: 2033 2077 6565 6b73 2061 676f 2020 2020   3 weeks ago    
+000013a0: 2020 2020 202f 6269 6e2f 7368 202d 6320       /bin/sh -c 
+000013b0: 2328 6e6f 7029 2055 5345 5220 5b6a 626f  #(nop) USER [jbo
+000013c0: 7373 5d20 2020 2020 2020 2020 2020 2020  ss]             
+000013d0: 2020 2020 2030 2042 0a20 2020 2035 6463       0 B.    5dc
+000013e0: 3165 3439 6634 3336 3120 2020 2020 2020  1e49f4361       
+000013f0: 2033 2077 6565 6b73 2061 676f 2020 2020   3 weeks ago    
+00001400: 2020 2020 202f 6269 6e2f 7368 202d 6320       /bin/sh -c 
+00001410: 2328 6e6f 7029 2057 4f52 4b44 4952 202f  #(nop) WORKDIR /
+00001420: 6f70 742f 6a62 6f73 7320 2020 2020 2020  opt/jboss       
+00001430: 2020 2020 2030 2042 0a20 2020 2037 6630       0 B.    7f0
+00001440: 6639 6562 3331 3137 3420 2020 2020 2020  f9eb31174       
+00001450: 2033 2077 6565 6b73 2061 676f 2020 2020   3 weeks ago    
+00001460: 2020 2020 202f 6269 6e2f 7368 202d 6320       /bin/sh -c 
+00001470: 6772 6f75 7061 6464 202d 7220 6a62 6f73  groupadd -r jbos
+00001480: 7320 2d67 2031 3030 3020 2626 2075 7365  s -g 1000 && use
+00001490: 7261 2020 2034 2e33 3439 206b 420a 2020  ra   4.349 kB.  
+000014a0: 2020 6264 3531 3566 3034 3461 6637 2020    bd515f044af7  
+000014b0: 2020 2020 2020 3320 7765 656b 7320 6167        3 weeks ag
+000014c0: 6f20 2020 2020 2020 2020 2f62 696e 2f73  o         /bin/s
+000014d0: 6820 2d63 2079 756d 2075 7064 6174 6520  h -c yum update 
+000014e0: 2d79 2026 2620 7975 6d20 2d79 2069 6e73  -y && yum -y ins
+000014f0: 7461 6c6c 2078 6d20 2020 3235 2e31 3820  tall xm   25.18 
+00001500: 4d42 0a20 2020 2062 3738 3333 3630 3939  MB.    b78336099
+00001510: 3034 3520 2020 2020 2020 2033 2077 6565  045        3 wee
+00001520: 6b73 2061 676f 2020 2020 2020 2020 202f  ks ago         /
+00001530: 6269 6e2f 7368 202d 6320 2328 6e6f 7029  bin/sh -c #(nop)
+00001540: 204d 4149 4e54 4149 4e45 5220 4d61 7265   MAINTAINER Mare
+00001550: 6b20 476f 6c64 6d61 6e6e 203c 2020 2030  k Goldmann <   0
+00001560: 2042 0a20 2020 2034 3831 3661 3239 3835   B.    4816a2985
+00001570: 3438 6320 2020 2020 2020 2033 2077 6565  48c        3 wee
+00001580: 6b73 2061 676f 2020 2020 2020 2020 202f  ks ago         /
+00001590: 6269 6e2f 7368 202d 6320 2328 6e6f 7029  bin/sh -c #(nop)
+000015a0: 2043 4d44 205b 222f 6269 6e2f 6261 7368   CMD ["/bin/bash
+000015b0: 225d 2020 2020 2020 2020 2020 2020 2030  "]             0
+000015c0: 2042 0a20 2020 2036 6565 3233 3563 6634   B.    6ee235cf4
+000015d0: 3437 3320 2020 2020 2020 2033 2077 6565  473        3 wee
+000015e0: 6b73 2061 676f 2020 2020 2020 2020 202f  ks ago         /
+000015f0: 6269 6e2f 7368 202d 6320 2328 6e6f 7029  bin/sh -c #(nop)
+00001600: 204c 4142 454c 206e 616d 653d 4365 6e74   LABEL name=Cent
+00001610: 4f53 2042 6173 6520 496d 6167 2020 2030  OS Base Imag   0
+00001620: 2042 0a20 2020 2034 3734 6332 6565 3737   B.    474c2ee77
+00001630: 6661 3320 2020 2020 2020 2033 2077 6565  fa3        3 wee
+00001640: 6b73 2061 676f 2020 2020 2020 2020 202f  ks ago         /
+00001650: 6269 6e2f 7368 202d 6320 2328 6e6f 7029  bin/sh -c #(nop)
+00001660: 2041 4444 2066 696c 653a 3732 3835 3266   ADD file:72852f
+00001670: 6337 3632 3664 3233 3333 3433 2020 2031  c7626d233343   1
+00001680: 3936 2e36 204d 420a 2020 2020 3135 3434  96.6 MB.    1544
+00001690: 3038 3466 6164 3831 2020 2020 2020 2020  084fad81        
+000016a0: 3620 6d6f 6e74 6873 2061 676f 2020 2020  6 months ago    
+000016b0: 2020 2020 2f62 696e 2f73 6820 2d63 2023      /bin/sh -c #
+000016c0: 286e 6f70 2920 4d41 494e 5441 494e 4552  (nop) MAINTAINER
+000016d0: 2054 6865 2043 656e 744f 5320 5072 6f6a   The CentOS Proj
+000016e0: 6520 2020 3020 420a 0a41 6e64 2077 6520  e   0 B..And we 
+000016f0: 7761 6e74 2074 6f20 7371 7561 7368 2061  want to squash a
+00001700: 6c6c 2074 6865 206c 6179 6572 7320 646f  ll the layers do
+00001710: 776e 2074 6f20 6c61 7965 7220 6060 3462  wn to layer ``4b
+00001720: 6231 3566 3362 3639 3737 6060 2e0a 0a3a  b15f3b6977``...:
+00001730: 3a0a 0a20 2020 2024 2064 6f63 6b65 722d  :..    $ docker-
+00001740: 7371 7561 7368 202d 6620 3462 6231 3566  squash -f 4bb15f
+00001750: 3362 3639 3737 202d 7420 6a62 6f73 732f  3b6977 -t jboss/
+00001760: 7769 6c64 666c 793a 7371 7561 7368 6564  wildfly:squashed
+00001770: 206a 626f 7373 2f77 696c 6466 6c79 3a6c   jboss/wildfly:l
+00001780: 6174 6573 740a 2020 2020 3230 3136 2d30  atest.    2016-0
+00001790: 342d 3031 2031 333a 3131 3a30 322c 3335  4-01 13:11:02,35
+000017a0: 3820 726f 6f74 2020 2020 2020 2020 2049  8 root         I
+000017b0: 4e46 4f20 2020 2020 646f 636b 6572 2d73  NFO     docker-s
+000017c0: 6372 6970 7473 2076 6572 7369 6f6e 2031  cripts version 1
+000017d0: 2e30 2e30 6465 762c 2044 6f63 6b65 7220  .0.0dev, Docker 
+000017e0: 3732 3036 3632 312c 2041 5049 2031 2e32  7206621, API 1.2
+000017f0: 312e 2e2e 0a20 2020 2032 3031 362d 3034  1....    2016-04
+00001800: 2d30 3120 3133 3a31 313a 3032 2c33 3538  -01 13:11:02,358
+00001810: 2072 6f6f 7420 2020 2020 2020 2020 494e   root         IN
+00001820: 464f 2020 2020 2055 7369 6e67 2076 3120  FO     Using v1 
+00001830: 696d 6167 6520 666f 726d 6174 0a20 2020  image format.   
+00001840: 2032 3031 362d 3034 2d30 3120 3133 3a31   2016-04-01 13:1
+00001850: 313a 3032 2c33 3734 2072 6f6f 7420 2020  1:02,374 root   
+00001860: 2020 2020 2020 494e 464f 2020 2020 204f        INFO     O
+00001870: 6c64 2069 6d61 6765 2068 6173 2032 3120  ld image has 21 
+00001880: 6c61 7965 7273 0a20 2020 2032 3031 362d  layers.    2016-
+00001890: 3034 2d30 3120 3133 3a31 313a 3032 2c33  04-01 13:11:02,3
+000018a0: 3738 2072 6f6f 7420 2020 2020 2020 2020  78 root         
+000018b0: 494e 464f 2020 2020 2043 6865 636b 696e  INFO     Checkin
+000018c0: 6720 6966 2073 7175 6173 6869 6e67 2069  g if squashing i
+000018d0: 7320 6e65 6365 7373 6172 792e 2e2e 0a20  s necessary.... 
+000018e0: 2020 2032 3031 362d 3034 2d30 3120 3133     2016-04-01 13
+000018f0: 3a31 313a 3032 2c33 3738 2072 6f6f 7420  :11:02,378 root 
+00001900: 2020 2020 2020 2020 494e 464f 2020 2020          INFO    
+00001910: 2041 7474 656d 7074 696e 6720 746f 2073   Attempting to s
+00001920: 7175 6173 6820 6c61 7374 2031 3220 6c61  quash last 12 la
+00001930: 7965 7273 2e2e 2e0a 2020 2020 3230 3136  yers....    2016
+00001940: 2d30 342d 3031 2031 333a 3131 3a30 322c  -04-01 13:11:02,
+00001950: 3337 3820 726f 6f74 2020 2020 2020 2020  378 root        
+00001960: 2049 4e46 4f20 2020 2020 5361 7669 6e67   INFO     Saving
+00001970: 2069 6d61 6765 2032 3539 3534 6536 6432   image 25954e6d2
+00001980: 3330 3030 3632 3335 6565 6362 3766 3063  30006235eecb7f0c
+00001990: 6335 3630 3236 3464 3733 3134 3639 3835  c560264d73146985
+000019a0: 6332 6432 6536 3633 6261 6339 3533 6436  c2d2e663bac953d6
+000019b0: 3630 6238 3733 3020 746f 202f 746d 702f  60b8730 to /tmp/
+000019c0: 646f 636b 6572 2d73 7175 6173 682d 6662  docker-squash-fb
+000019d0: 785a 7a34 2f6f 6c64 2f69 6d61 6765 2e74  xZz4/old/image.t
+000019e0: 6172 2066 696c 652e 2e2e 0a20 2020 2032  ar file....    2
+000019f0: 3031 362d 3034 2d30 3120 3133 3a31 313a  016-04-01 13:11:
+00001a00: 3038 2c30 3033 2072 6f6f 7420 2020 2020  08,003 root     
+00001a10: 2020 2020 494e 464f 2020 2020 2049 6d61      INFO     Ima
+00001a20: 6765 2073 6176 6564 210a 2020 2020 3230  ge saved!.    20
+00001a30: 3136 2d30 342d 3031 2031 333a 3131 3a30  16-04-01 13:11:0
+00001a40: 382c 3033 3120 726f 6f74 2020 2020 2020  8,031 root      
+00001a50: 2020 2049 4e46 4f20 2020 2020 556e 7061     INFO     Unpa
+00001a60: 636b 696e 6720 2f74 6d70 2f64 6f63 6b65  cking /tmp/docke
+00001a70: 722d 7371 7561 7368 2d66 6278 5a7a 342f  r-squash-fbxZz4/
+00001a80: 6f6c 642f 696d 6167 652e 7461 7220 7461  old/image.tar ta
+00001a90: 7220 6669 6c65 2074 6f20 2f74 6d70 2f64  r file to /tmp/d
+00001aa0: 6f63 6b65 722d 7371 7561 7368 2d66 6278  ocker-squash-fbx
+00001ab0: 5a7a 342f 6f6c 6420 6469 7265 6374 6f72  Zz4/old director
+00001ac0: 790a 2020 2020 3230 3136 2d30 342d 3031  y.    2016-04-01
+00001ad0: 2031 333a 3131 3a30 382c 3538 3820 726f   13:11:08,588 ro
+00001ae0: 6f74 2020 2020 2020 2020 2049 4e46 4f20  ot         INFO 
+00001af0: 2020 2020 4172 6368 6976 6520 756e 7061      Archive unpa
+00001b00: 636b 6564 210a 2020 2020 3230 3136 2d30  cked!.    2016-0
+00001b10: 342d 3031 2031 333a 3131 3a30 382c 3633  4-01 13:11:08,63
+00001b20: 3620 726f 6f74 2020 2020 2020 2020 2049  6 root         I
+00001b30: 4e46 4f20 2020 2020 5371 7561 7368 696e  NFO     Squashin
+00001b40: 6720 696d 6167 6520 276a 626f 7373 2f77  g image 'jboss/w
+00001b50: 696c 6466 6c79 3a6c 6174 6573 7427 2e2e  ildfly:latest'..
+00001b60: 2e0a 2020 2020 3230 3136 2d30 342d 3031  ..    2016-04-01
+00001b70: 2031 333a 3131 3a30 382c 3633 3720 726f   13:11:08,637 ro
+00001b80: 6f74 2020 2020 2020 2020 2049 4e46 4f20  ot         INFO 
+00001b90: 2020 2020 5374 6172 7469 6e67 2073 7175      Starting squ
+00001ba0: 6173 6869 6e67 2e2e 2e0a 2020 2020 3230  ashing....    20
+00001bb0: 3136 2d30 342d 3031 2031 333a 3131 3a30  16-04-01 13:11:0
+00001bc0: 382c 3633 3720 726f 6f74 2020 2020 2020  8,637 root      
+00001bd0: 2020 2049 4e46 4f20 2020 2020 5371 7561     INFO     Squa
+00001be0: 7368 696e 6720 6669 6c65 2027 2f74 6d70  shing file '/tmp
+00001bf0: 2f64 6f63 6b65 722d 7371 7561 7368 2d66  /docker-squash-f
+00001c00: 6278 5a7a 342f 6f6c 642f 3235 3935 3465  bxZz4/old/25954e
+00001c10: 3664 3233 3030 3036 3233 3565 6563 6237  6d230006235eecb7
+00001c20: 6630 6363 3536 3032 3634 6437 3331 3436  f0cc560264d73146
+00001c30: 3938 3563 3264 3265 3636 3362 6163 3935  985c2d2e663bac95
+00001c40: 3364 3636 3062 3837 3330 2f6c 6179 6572  3d660b8730/layer
+00001c50: 2e74 6172 272e 2e2e 0a20 2020 2032 3031  .tar'....    201
+00001c60: 362d 3034 2d30 3120 3133 3a31 313a 3038  6-04-01 13:11:08
+00001c70: 2c36 3337 2072 6f6f 7420 2020 2020 2020  ,637 root       
+00001c80: 2020 494e 464f 2020 2020 2053 7175 6173    INFO     Squas
+00001c90: 6869 6e67 2066 696c 6520 272f 746d 702f  hing file '/tmp/
+00001ca0: 646f 636b 6572 2d73 7175 6173 682d 6662  docker-squash-fb
+00001cb0: 785a 7a34 2f6f 6c64 2f35 6165 3639 6362  xZz4/old/5ae69cb
+00001cc0: 3435 3461 3561 3534 3266 3633 6531 3438  454a5a542f63e148
+00001cd0: 6365 3430 6662 3965 3031 6465 3562 6230  ce40fb9e01de5bb0
+00001ce0: 3138 3035 6234 6465 6432 3338 3834 3162  1805b4ded238841b
+00001cf0: 6332 6365 3865 3839 352f 6c61 7965 722e  c2ce8e895/layer.
+00001d00: 7461 7227 2e2e 2e0a 2020 2020 3230 3136  tar'....    2016
+00001d10: 2d30 342d 3031 2031 333a 3131 3a30 382c  -04-01 13:11:08,
+00001d20: 3633 3720 726f 6f74 2020 2020 2020 2020  637 root        
+00001d30: 2049 4e46 4f20 2020 2020 5371 7561 7368   INFO     Squash
+00001d40: 696e 6720 6669 6c65 2027 2f74 6d70 2f64  ing file '/tmp/d
+00001d50: 6f63 6b65 722d 7371 7561 7368 2d66 6278  ocker-squash-fbx
+00001d60: 5a7a 342f 6f6c 642f 6463 3234 3731 3266  Zz4/old/dc24712f
+00001d70: 3335 6334 3065 3935 3862 6538 6163 6132  35c40e958be8aca2
+00001d80: 3733 3165 3762 6638 3335 3362 3962 3138  731e7bf8353b9b18
+00001d90: 6261 6136 6139 3461 6438 3463 3639 3532  baa6a94ad84c6952
+00001da0: 6362 6337 3730 3034 2f6c 6179 6572 2e74  cbc77004/layer.t
+00001db0: 6172 272e 2e2e 0a20 2020 2032 3031 362d  ar'....    2016-
+00001dc0: 3034 2d30 3120 3133 3a31 313a 3038 2c36  04-01 13:11:08,6
+00001dd0: 3338 2072 6f6f 7420 2020 2020 2020 2020  38 root         
+00001de0: 494e 464f 2020 2020 2053 7175 6173 6869  INFO     Squashi
+00001df0: 6e67 2066 696c 6520 272f 746d 702f 646f  ng file '/tmp/do
+00001e00: 636b 6572 2d73 7175 6173 682d 6662 785a  cker-squash-fbxZ
+00001e10: 7a34 2f6f 6c64 2f64 3932 3931 3239 6434  z4/old/d929129d4
+00001e20: 6338 6536 3165 6133 3636 3165 6234 3263  c8e61ea3661eb42c
+00001e30: 3330 6430 3166 3463 3135 3234 3138 3638  30d01f4c15241868
+00001e40: 3931 3738 6166 6337 6463 3831 3835 6133  9178afc7dc8185a3
+00001e50: 3738 3134 3532 382f 6c61 7965 722e 7461  7814528/layer.ta
+00001e60: 7227 2e2e 2e0a 2020 2020 3230 3136 2d30  r'....    2016-0
+00001e70: 342d 3031 2031 333a 3131 3a30 392c 3131  4-01 13:11:09,11
+00001e80: 3320 726f 6f74 2020 2020 2020 2020 2049  3 root         I
+00001e90: 4e46 4f20 2020 2020 5371 7561 7368 696e  NFO     Squashin
+00001ea0: 6720 6669 6c65 2027 2f74 6d70 2f64 6f63  g file '/tmp/doc
+00001eb0: 6b65 722d 7371 7561 7368 2d66 6278 5a7a  ker-squash-fbxZz
+00001ec0: 342f 6f6c 642f 6238 6661 3363 6166 3764  4/old/b8fa3caf7d
+00001ed0: 3664 6332 3238 6266 3234 3939 6133 6166  6dc228bf2499a3af
+00001ee0: 3836 6535 3037 3361 6430 6331 3733 3034  86e5073ad0c17304
+00001ef0: 6333 3930 3066 6133 3431 6539 6432 6665  c3900fa341e9d2fe
+00001f00: 3465 3536 3535 2f6c 6179 6572 2e74 6172  4e5655/layer.tar
+00001f10: 272e 2e2e 0a20 2020 2032 3031 362d 3034  '....    2016-04
+00001f20: 2d30 3120 3133 3a31 313a 3039 2c31 3135  -01 13:11:09,115
+00001f30: 2072 6f6f 7420 2020 2020 2020 2020 494e   root         IN
+00001f40: 464f 2020 2020 2053 7175 6173 6869 6e67  FO     Squashing
+00001f50: 2066 696c 6520 272f 746d 702f 646f 636b   file '/tmp/dock
+00001f60: 6572 2d73 7175 6173 682d 6662 785a 7a34  er-squash-fbxZz4
+00001f70: 2f6f 6c64 2f33 3862 3866 3835 6537 3462  /old/38b8f85e74b
+00001f80: 6661 3737 3361 3061 6436 3964 6132 3230  fa773a0ad69da220
+00001f90: 3564 6330 3134 3839 3435 6536 6635 6137  5dc0148945e6f5a7
+00001fa0: 6365 6230 3466 6134 6538 3631 3965 3164  ceb04fa4e8619e1d
+00001fb0: 6534 3235 622f 6c61 7965 722e 7461 7227  e425b/layer.tar'
+00001fc0: 2e2e 2e0a 2020 2020 3230 3136 2d30 342d  ....    2016-04-
+00001fd0: 3031 2031 333a 3131 3a30 392c 3131 3520  01 13:11:09,115 
+00001fe0: 726f 6f74 2020 2020 2020 2020 2049 4e46  root         INF
+00001ff0: 4f20 2020 2020 5371 7561 7368 696e 6720  O     Squashing 
+00002000: 6669 6c65 2027 2f74 6d70 2f64 6f63 6b65  file '/tmp/docke
+00002010: 722d 7371 7561 7368 2d66 6278 5a7a 342f  r-squash-fbxZz4/
+00002020: 6f6c 642f 6165 3739 6236 3436 6239 6139  old/ae79b646b9a9
+00002030: 6132 3837 6335 6636 6130 3138 3731 6363  a287c5f6a01871cc
+00002040: 3964 3965 6535 3936 6461 6665 6532 6462  9d9ee596dafee2db
+00002050: 3934 3237 3134 6361 3364 6561 3063 3036  942714ca3dea0c06
+00002060: 6565 6633 2f6c 6179 6572 2e74 6172 272e  eef3/layer.tar'.
+00002070: 2e2e 0a20 2020 2032 3031 362d 3034 2d30  ...    2016-04-0
+00002080: 3120 3133 3a31 313a 3039 2c31 3135 2072  1 13:11:09,115 r
+00002090: 6f6f 7420 2020 2020 2020 2020 494e 464f  oot         INFO
+000020a0: 2020 2020 2053 7175 6173 6869 6e67 2066       Squashing f
+000020b0: 696c 6520 272f 746d 702f 646f 636b 6572  ile '/tmp/docker
+000020c0: 2d73 7175 6173 682d 6662 785a 7a34 2f6f  -squash-fbxZz4/o
+000020d0: 6c64 2f32 6234 3630 3664 6339 6463 3737  ld/2b4606dc9dc77
+000020e0: 3361 6132 3230 6136 3533 3531 6665 3864  3aa220a65351fe8d
+000020f0: 3534 6630 3335 3334 6335 3866 6561 3233  54f03534c58fea23
+00002100: 3039 3630 6539 3539 3135 3232 3233 3636  0960e95915222366
+00002110: 3037 342f 6c61 7965 722e 7461 7227 2e2e  074/layer.tar'..
+00002120: 2e0a 2020 2020 3230 3136 2d30 342d 3031  ..    2016-04-01
+00002130: 2031 333a 3131 3a30 392c 3131 3520 726f   13:11:09,115 ro
+00002140: 6f74 2020 2020 2020 2020 2049 4e46 4f20  ot         INFO 
+00002150: 2020 2020 5371 7561 7368 696e 6720 6669      Squashing fi
+00002160: 6c65 2027 2f74 6d70 2f64 6f63 6b65 722d  le '/tmp/docker-
+00002170: 7371 7561 7368 2d66 6278 5a7a 342f 6f6c  squash-fbxZz4/ol
+00002180: 642f 3131 3866 6139 6533 3335 3736 6563  d/118fa9e33576ec
+00002190: 6336 3235 6562 6262 6664 6632 3830 3963  c625ebbbfdf2809c
+000021a0: 3135 3237 6537 3136 6362 3466 6435 6362  1527e716cb4fd5cb
+000021b0: 3430 3534 3865 6236 6433 3530 3361 3735  40548eb6d3503a75
+000021c0: 6139 2f6c 6179 6572 2e74 6172 272e 2e2e  a9/layer.tar'...
+000021d0: 0a20 2020 2032 3031 362d 3034 2d30 3120  .    2016-04-01 
+000021e0: 3133 3a31 313a 3039 2c31 3135 2072 6f6f  13:11:09,115 roo
+000021f0: 7420 2020 2020 2020 2020 494e 464f 2020  t         INFO  
+00002200: 2020 2053 7175 6173 6869 6e67 2066 696c     Squashing fil
+00002210: 6520 272f 746d 702f 646f 636b 6572 2d73  e '/tmp/docker-s
+00002220: 7175 6173 682d 6662 785a 7a34 2f6f 6c64  quash-fbxZz4/old
+00002230: 2f35 6637 6538 6633 3663 3362 6232 3063  /5f7e8f36c3bb20c
+00002240: 3964 6237 3437 3061 3232 6638 3238 3731  9db7470a22f82871
+00002250: 3062 3464 3238 6165 6465 3634 3936 3663  0b4d28aede64966c
+00002260: 3432 3561 6464 3438 6131 6231 3466 6532  425add48a1b14fe2
+00002270: 332f 6c61 7965 722e 7461 7227 2e2e 2e0a  3/layer.tar'....
+00002280: 2020 2020 3230 3136 2d30 342d 3031 2031      2016-04-01 1
+00002290: 333a 3131 3a31 302c 3132 3720 726f 6f74  3:11:10,127 root
+000022a0: 2020 2020 2020 2020 2049 4e46 4f20 2020           INFO   
+000022b0: 2020 5371 7561 7368 696e 6720 6669 6c65    Squashing file
+000022c0: 2027 2f74 6d70 2f64 6f63 6b65 722d 7371   '/tmp/docker-sq
+000022d0: 7561 7368 2d66 6278 5a7a 342f 6f6c 642f  uash-fbxZz4/old/
+000022e0: 3364 3464 3032 3238 6631 3631 6236 3765  3d4d0228f161b67e
+000022f0: 6234 3666 6462 3432 3561 6431 3438 6333  b46fdb425ad148c3
+00002300: 3164 3939 3434 6463 6238 3232 6636 3765  1d9944dcb822f67e
+00002310: 6163 3365 3261 6332 6566 6665 6663 3733  ac3e2ac2effefc73
+00002320: 2f6c 6179 6572 2e74 6172 272e 2e2e 0a20  /layer.tar'.... 
+00002330: 2020 2032 3031 362d 3034 2d30 3120 3133     2016-04-01 13
+00002340: 3a31 313a 3130 2c31 3239 2072 6f6f 7420  :11:10,129 root 
+00002350: 2020 2020 2020 2020 494e 464f 2020 2020          INFO    
+00002360: 2053 7175 6173 6869 6e67 2066 696c 6520   Squashing file 
+00002370: 272f 746d 702f 646f 636b 6572 2d73 7175  '/tmp/docker-squ
+00002380: 6173 682d 6662 785a 7a34 2f6f 6c64 2f66  ash-fbxZz4/old/f
+00002390: 3761 6234 6561 3139 3730 3834 6162 3734  7ab4ea197084ab74
+000023a0: 3833 6132 6361 3534 3039 6264 6366 3534  83a2ca5409bdcf54
+000023b0: 3733 3134 3162 6662 3631 6238 3638 3762  73141bfb61b8687b
+000023c0: 3133 3239 3934 3333 3539 6363 3366 652f  1329943359cc3fe/
+000023d0: 6c61 7965 722e 7461 7227 2e2e 2e0a 2020  layer.tar'....  
+000023e0: 2020 3230 3136 2d30 342d 3031 2031 333a    2016-04-01 13:
+000023f0: 3131 3a31 302c 3733 3220 726f 6f74 2020  11:10,732 root  
+00002400: 2020 2020 2020 2049 4e46 4f20 2020 2020         INFO     
+00002410: 5371 7561 7368 696e 6720 6669 6e69 7368  Squashing finish
+00002420: 6564 210a 2020 2020 3230 3136 2d30 342d  ed!.    2016-04-
+00002430: 3031 2031 333a 3131 3a31 302c 3733 3720  01 13:11:10,737 
+00002440: 726f 6f74 2020 2020 2020 2020 2049 4e46  root         INF
+00002450: 4f20 2020 2020 4e65 7720 7371 7561 7368  O     New squash
+00002460: 6564 2069 6d61 6765 2049 4420 6973 2035  ed image ID is 5
+00002470: 3232 3535 6537 3564 3365 6238 3331 3233  2255e75d3eb83123
+00002480: 6530 3734 6638 3937 6538 6339 3731 6465  e074f897e8c971de
+00002490: 6339 6431 3136 3861 3563 3832 6437 6331  c9d1168a5c82d7c1
+000024a0: 3439 3661 3139 3064 6132 6534 3065 660a  496a190da2e40ef.
+000024b0: 2020 2020 3230 3136 2d30 342d 3031 2031      2016-04-01 1
+000024c0: 333a 3131 3a31 342c 3536 3320 726f 6f74  3:11:14,563 root
+000024d0: 2020 2020 2020 2020 2049 4e46 4f20 2020           INFO   
+000024e0: 2020 496d 6167 6520 7265 6769 7374 6572    Image register
+000024f0: 6564 2069 6e20 446f 636b 6572 2064 6165  ed in Docker dae
+00002500: 6d6f 6e20 6173 206a 626f 7373 2f77 696c  mon as jboss/wil
+00002510: 6466 6c79 3a73 7175 6173 6865 640a 2020  dfly:squashed.  
+00002520: 2020 3230 3136 2d30 342d 3031 2031 333a    2016-04-01 13:
+00002530: 3131 3a31 342c 3635 3220 726f 6f74 2020  11:14,652 root  
+00002540: 2020 2020 2020 2049 4e46 4f20 2020 2020         INFO     
+00002550: 446f 6e65 0a0a 5765 2063 616e 206e 6f77  Done..We can now
+00002560: 2063 6f6e 6669 726d 2074 6865 206c 6179   confirm the lay
+00002570: 6572 2073 7472 7563 7475 7265 3a0a 0a3a  er structure:..:
+00002580: 3a0a 0a20 2020 2024 2064 6f63 6b65 7220  :..    $ docker 
+00002590: 6869 7374 6f72 7920 6a62 6f73 732f 7769  history jboss/wi
+000025a0: 6c64 666c 793a 7371 7561 7368 6564 0a20  ldfly:squashed. 
+000025b0: 2020 2049 4d41 4745 2020 2020 2020 2020     IMAGE        
+000025c0: 2020 2020 2020 2043 5245 4154 4544 2020         CREATED  
+000025d0: 2020 2020 2020 2020 2020 2043 5245 4154             CREAT
+000025e0: 4544 2042 5920 2020 2020 2020 2020 2020  ED BY           
+000025f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002600: 2020 2020 2020 2020 2020 2053 495a 4520             SIZE 
+00002610: 2020 2020 2020 2020 2020 2020 2020 2043                 C
+00002620: 4f4d 4d45 4e54 0a20 2020 2035 3232 3535  OMMENT.    52255
+00002630: 6537 3564 3365 6220 2020 2020 2020 2034  e75d3eb        4
+00002640: 3020 7365 636f 6e64 7320 6167 6f20 2020  0 seconds ago   
+00002650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002680: 2020 2033 3538 2e32 204d 420a 2020 2020     358.2 MB.    
+00002690: 3462 6231 3566 3362 3639 3737 2020 2020  4bb15f3b6977    
+000026a0: 2020 2020 3320 7765 656b 7320 6167 6f20      3 weeks ago 
+000026b0: 2020 2020 2020 2020 2f62 696e 2f73 6820          /bin/sh 
+000026c0: 2d63 2023 286e 6f70 2920 5553 4552 205b  -c #(nop) USER [
+000026d0: 6a62 6f73 735d 2020 2020 2020 2020 2020  jboss]          
+000026e0: 2020 2020 2020 2020 3020 420a 2020 2020          0 B.    
+000026f0: 3564 6331 6534 3966 3433 3631 2020 2020  5dc1e49f4361    
+00002700: 2020 2020 3320 7765 656b 7320 6167 6f20      3 weeks ago 
+00002710: 2020 2020 2020 2020 2f62 696e 2f73 6820          /bin/sh 
+00002720: 2d63 2023 286e 6f70 2920 574f 524b 4449  -c #(nop) WORKDI
+00002730: 5220 2f6f 7074 2f6a 626f 7373 2020 2020  R /opt/jboss    
+00002740: 2020 2020 2020 2020 3020 420a 2020 2020          0 B.    
+00002750: 3766 3066 3965 6233 3131 3734 2020 2020  7f0f9eb31174    
+00002760: 2020 2020 3320 7765 656b 7320 6167 6f20      3 weeks ago 
+00002770: 2020 2020 2020 2020 2f62 696e 2f73 6820          /bin/sh 
+00002780: 2d63 2067 726f 7570 6164 6420 2d72 206a  -c groupadd -r j
+00002790: 626f 7373 202d 6720 3130 3030 2026 2620  boss -g 1000 && 
+000027a0: 7573 6572 6120 2020 342e 3334 3920 6b42  usera   4.349 kB
+000027b0: 0a20 2020 2062 6435 3135 6630 3434 6166  .    bd515f044af
+000027c0: 3720 2020 2020 2020 2033 2077 6565 6b73  7        3 weeks
+000027d0: 2061 676f 2020 2020 2020 2020 202f 6269   ago         /bi
+000027e0: 6e2f 7368 202d 6320 7975 6d20 7570 6461  n/sh -c yum upda
+000027f0: 7465 202d 7920 2626 2079 756d 202d 7920  te -y && yum -y 
+00002800: 696e 7374 616c 6c20 786d 2020 2032 352e  install xm   25.
+00002810: 3138 204d 420a 2020 2020 6237 3833 3336  18 MB.    b78336
+00002820: 3039 3930 3435 2020 2020 2020 2020 3320  099045        3 
+00002830: 7765 656b 7320 6167 6f20 2020 2020 2020  weeks ago       
+00002840: 2020 2f62 696e 2f73 6820 2d63 2023 286e    /bin/sh -c #(n
+00002850: 6f70 2920 4d41 494e 5441 494e 4552 204d  op) MAINTAINER M
+00002860: 6172 656b 2047 6f6c 646d 616e 6e20 3c20  arek Goldmann < 
+00002870: 2020 3020 420a 2020 2020 3438 3136 6132    0 B.    4816a2
+00002880: 3938 3534 3863 2020 2020 2020 2020 3320  98548c        3 
+00002890: 7765 656b 7320 6167 6f20 2020 2020 2020  weeks ago       
+000028a0: 2020 2f62 696e 2f73 6820 2d63 2023 286e    /bin/sh -c #(n
+000028b0: 6f70 2920 434d 4420 5b22 2f62 696e 2f62  op) CMD ["/bin/b
+000028c0: 6173 6822 5d20 2020 2020 2020 2020 2020  ash"]           
+000028d0: 2020 3020 420a 2020 2020 3665 6532 3335    0 B.    6ee235
+000028e0: 6366 3434 3733 2020 2020 2020 2020 3320  cf4473        3 
+000028f0: 7765 656b 7320 6167 6f20 2020 2020 2020  weeks ago       
+00002900: 2020 2f62 696e 2f73 6820 2d63 2023 286e    /bin/sh -c #(n
+00002910: 6f70 2920 4c41 4245 4c20 6e61 6d65 3d43  op) LABEL name=C
+00002920: 656e 744f 5320 4261 7365 2049 6d61 6720  entOS Base Imag 
+00002930: 2020 3020 420a 2020 2020 3437 3463 3265    0 B.    474c2e
+00002940: 6537 3766 6133 2020 2020 2020 2020 3320  e77fa3        3 
+00002950: 7765 656b 7320 6167 6f20 2020 2020 2020  weeks ago       
+00002960: 2020 2f62 696e 2f73 6820 2d63 2023 286e    /bin/sh -c #(n
+00002970: 6f70 2920 4144 4420 6669 6c65 3a37 3238  op) ADD file:728
+00002980: 3532 6663 3736 3236 6432 3333 3334 3320  52fc7626d233343 
+00002990: 2020 3139 362e 3620 4d42 0a20 2020 2031    196.6 MB.    1
+000029a0: 3534 3430 3834 6661 6438 3120 2020 2020  544084fad81     
+000029b0: 2020 2036 206d 6f6e 7468 7320 6167 6f20     6 months ago 
+000029c0: 2020 2020 2020 202f 6269 6e2f 7368 202d         /bin/sh -
+000029d0: 6320 2328 6e6f 7029 204d 4149 4e54 4149  c #(nop) MAINTAI
+000029e0: 4e45 5220 5468 6520 4365 6e74 4f53 2050  NER The CentOS P
+000029f0: 726f 6a65 2020 2030 2042 0a0a 4f74 6865  roje   0 B..Othe
+00002a00: 7220 6f70 7469 6f6e 2069 7320 746f 2073  r option is to s
+00002a10: 7065 6369 6679 2068 6f77 206d 616e 7920  pecify how many 
+00002a20: 6c61 7965 7273 2028 636f 756e 7469 6e67  layers (counting
+00002a30: 2066 726f 6d20 7468 6520 6e65 7765 7374   from the newest
+00002a40: 206c 6179 6572 2920 7765 2077 616e 7420   layer) we want 
+00002a50: 746f 2073 7175 6173 682e 5c0a 4c65 7427  to squash.\.Let'
+00002a60: 7320 7371 7561 7368 206c 6173 7420 3130  s squash last 10
+00002a70: 206c 6179 6572 7320 6672 6f6d 2074 6865   layers from the
+00002a80: 2060 606a 626f 7373 2f77 696c 6466 6c79   ``jboss/wildfly
+00002a90: 3a6c 6174 6573 7460 6020 696d 6167 653a  :latest`` image:
+00002aa0: 0a0a 3a3a 0a0a 2020 2020 2420 646f 636b  ..::..    $ dock
+00002ab0: 6572 2d73 7175 6173 6820 2d66 2031 3020  er-squash -f 10 
+00002ac0: 2d74 206a 626f 7373 2f77 696c 6466 6c79  -t jboss/wildfly
+00002ad0: 3a73 7175 6173 6865 6420 6a62 6f73 732f  :squashed jboss/
+00002ae0: 7769 6c64 666c 793a 6c61 7465 7374 0a20  wildfly:latest. 
+00002af0: 2020 2032 3031 362d 3034 2d30 3120 3133     2016-04-01 13
+00002b00: 3a31 353a 3036 2c34 3838 2072 6f6f 7420  :15:06,488 root 
+00002b10: 2020 2020 2020 2020 494e 464f 2020 2020          INFO    
+00002b20: 2064 6f63 6b65 722d 7363 7269 7074 7320   docker-scripts 
+00002b30: 7665 7273 696f 6e20 312e 302e 3064 6576  version 1.0.0dev
+00002b40: 2c20 446f 636b 6572 2037 3230 3636 3231  , Docker 7206621
+00002b50: 2c20 4150 4920 312e 3231 2e2e 2e0a 2020  , API 1.21....  
+00002b60: 2020 3230 3136 2d30 342d 3031 2031 333a    2016-04-01 13:
+00002b70: 3135 3a30 362c 3438 3820 726f 6f74 2020  15:06,488 root  
+00002b80: 2020 2020 2020 2049 4e46 4f20 2020 2020         INFO     
+00002b90: 5573 696e 6720 7631 2069 6d61 6765 2066  Using v1 image f
+00002ba0: 6f72 6d61 740a 2020 2020 3230 3136 2d30  ormat.    2016-0
+00002bb0: 342d 3031 2031 333a 3135 3a30 362c 3530  4-01 13:15:06,50
+00002bc0: 3420 726f 6f74 2020 2020 2020 2020 2049  4 root         I
+00002bd0: 4e46 4f20 2020 2020 4f6c 6420 696d 6167  NFO     Old imag
+00002be0: 6520 6861 7320 3231 206c 6179 6572 730a  e has 21 layers.
+00002bf0: 2020 2020 3230 3136 2d30 342d 3031 2031      2016-04-01 1
+00002c00: 333a 3135 3a30 362c 3530 3420 726f 6f74  3:15:06,504 root
+00002c10: 2020 2020 2020 2020 2049 4e46 4f20 2020           INFO   
+00002c20: 2020 4368 6563 6b69 6e67 2069 6620 7371    Checking if sq
+00002c30: 7561 7368 696e 6720 6973 206e 6563 6573  uashing is neces
+00002c40: 7361 7279 2e2e 2e0a 2020 2020 3230 3136  sary....    2016
+00002c50: 2d30 342d 3031 2031 333a 3135 3a30 362c  -04-01 13:15:06,
+00002c60: 3530 3420 726f 6f74 2020 2020 2020 2020  504 root        
+00002c70: 2049 4e46 4f20 2020 2020 4174 7465 6d70   INFO     Attemp
+00002c80: 7469 6e67 2074 6f20 7371 7561 7368 206c  ting to squash l
+00002c90: 6173 7420 3130 206c 6179 6572 732e 2e2e  ast 10 layers...
+00002ca0: 0a20 2020 2032 3031 362d 3034 2d30 3120  .    2016-04-01 
+00002cb0: 3133 3a31 353a 3036 2c35 3035 2072 6f6f  13:15:06,505 roo
+00002cc0: 7420 2020 2020 2020 2020 494e 464f 2020  t         INFO  
+00002cd0: 2020 2053 6176 696e 6720 696d 6167 6520     Saving image 
+00002ce0: 3235 3935 3465 3664 3233 3030 3036 3233  25954e6d23000623
+00002cf0: 3565 6563 6237 6630 6363 3536 3032 3634  5eecb7f0cc560264
+00002d00: 6437 3331 3436 3938 3563 3264 3265 3636  d73146985c2d2e66
+00002d10: 3362 6163 3935 3364 3636 3062 3837 3330  3bac953d660b8730
+00002d20: 2074 6f20 2f74 6d70 2f64 6f63 6b65 722d   to /tmp/docker-
+00002d30: 7371 7561 7368 2d66 7538 3043 582f 6f6c  squash-fu80CX/ol
+00002d40: 642f 696d 6167 652e 7461 7220 6669 6c65  d/image.tar file
+00002d50: 2e2e 2e0a 2020 2020 3230 3136 2d30 342d  ....    2016-04-
+00002d60: 3031 2031 333a 3135 3a31 322c 3133 3620  01 13:15:12,136 
+00002d70: 726f 6f74 2020 2020 2020 2020 2049 4e46  root         INF
+00002d80: 4f20 2020 2020 496d 6167 6520 7361 7665  O     Image save
+00002d90: 6421 0a20 2020 2032 3031 362d 3034 2d30  d!.    2016-04-0
+00002da0: 3120 3133 3a31 353a 3132 2c31 3637 2072  1 13:15:12,167 r
+00002db0: 6f6f 7420 2020 2020 2020 2020 494e 464f  oot         INFO
+00002dc0: 2020 2020 2055 6e70 6163 6b69 6e67 202f       Unpacking /
+00002dd0: 746d 702f 646f 636b 6572 2d73 7175 6173  tmp/docker-squas
+00002de0: 682d 6675 3830 4358 2f6f 6c64 2f69 6d61  h-fu80CX/old/ima
+00002df0: 6765 2e74 6172 2074 6172 2066 696c 6520  ge.tar tar file 
+00002e00: 746f 202f 746d 702f 646f 636b 6572 2d73  to /tmp/docker-s
+00002e10: 7175 6173 682d 6675 3830 4358 2f6f 6c64  quash-fu80CX/old
+00002e20: 2064 6972 6563 746f 7279 0a20 2020 2032   directory.    2
+00002e30: 3031 362d 3034 2d30 3120 3133 3a31 353a  016-04-01 13:15:
+00002e40: 3132 2c37 3036 2072 6f6f 7420 2020 2020  12,706 root     
+00002e50: 2020 2020 494e 464f 2020 2020 2041 7263      INFO     Arc
+00002e60: 6869 7665 2075 6e70 6163 6b65 6421 0a20  hive unpacked!. 
+00002e70: 2020 2032 3031 362d 3034 2d30 3120 3133     2016-04-01 13
+00002e80: 3a31 353a 3132 2c37 3536 2072 6f6f 7420  :15:12,756 root 
+00002e90: 2020 2020 2020 2020 494e 464f 2020 2020          INFO    
+00002ea0: 2053 7175 6173 6869 6e67 2069 6d61 6765   Squashing image
+00002eb0: 2027 6a62 6f73 732f 7769 6c64 666c 793a   'jboss/wildfly:
+00002ec0: 6c61 7465 7374 272e 2e2e 0a20 2020 2032  latest'....    2
+00002ed0: 3031 362d 3034 2d30 3120 3133 3a31 353a  016-04-01 13:15:
+00002ee0: 3132 2c37 3536 2072 6f6f 7420 2020 2020  12,756 root     
+00002ef0: 2020 2020 494e 464f 2020 2020 2053 7461      INFO     Sta
+00002f00: 7274 696e 6720 7371 7561 7368 696e 672e  rting squashing.
+00002f10: 2e2e 0a20 2020 2032 3031 362d 3034 2d30  ...    2016-04-0
+00002f20: 3120 3133 3a31 353a 3132 2c37 3536 2072  1 13:15:12,756 r
+00002f30: 6f6f 7420 2020 2020 2020 2020 494e 464f  oot         INFO
+00002f40: 2020 2020 2053 7175 6173 6869 6e67 2066       Squashing f
+00002f50: 696c 6520 272f 746d 702f 646f 636b 6572  ile '/tmp/docker
+00002f60: 2d73 7175 6173 682d 6675 3830 4358 2f6f  -squash-fu80CX/o
+00002f70: 6c64 2f32 3539 3534 6536 6432 3330 3030  ld/25954e6d23000
+00002f80: 3632 3335 6565 6362 3766 3063 6335 3630  6235eecb7f0cc560
+00002f90: 3236 3464 3733 3134 3639 3835 6332 6432  264d73146985c2d2
+00002fa0: 6536 3633 6261 6339 3533 6436 3630 6238  e663bac953d660b8
+00002fb0: 3733 302f 6c61 7965 722e 7461 7227 2e2e  730/layer.tar'..
+00002fc0: 2e0a 2020 2020 3230 3136 2d30 342d 3031  ..    2016-04-01
+00002fd0: 2031 333a 3135 3a31 322c 3735 3720 726f   13:15:12,757 ro
+00002fe0: 6f74 2020 2020 2020 2020 2049 4e46 4f20  ot         INFO 
+00002ff0: 2020 2020 5371 7561 7368 696e 6720 6669      Squashing fi
+00003000: 6c65 2027 2f74 6d70 2f64 6f63 6b65 722d  le '/tmp/docker-
+00003010: 7371 7561 7368 2d66 7538 3043 582f 6f6c  squash-fu80CX/ol
+00003020: 642f 3561 6536 3963 6234 3534 6135 6135  d/5ae69cb454a5a5
+00003030: 3432 6636 3365 3134 3863 6534 3066 6239  42f63e148ce40fb9
+00003040: 6530 3164 6535 6262 3031 3830 3562 3464  e01de5bb01805b4d
+00003050: 6564 3233 3838 3431 6263 3263 6538 6538  ed238841bc2ce8e8
+00003060: 3935 2f6c 6179 6572 2e74 6172 272e 2e2e  95/layer.tar'...
+00003070: 0a20 2020 2032 3031 362d 3034 2d30 3120  .    2016-04-01 
+00003080: 3133 3a31 353a 3132 2c37 3537 2072 6f6f  13:15:12,757 roo
+00003090: 7420 2020 2020 2020 2020 494e 464f 2020  t         INFO  
+000030a0: 2020 2053 7175 6173 6869 6e67 2066 696c     Squashing fil
+000030b0: 6520 272f 746d 702f 646f 636b 6572 2d73  e '/tmp/docker-s
+000030c0: 7175 6173 682d 6675 3830 4358 2f6f 6c64  quash-fu80CX/old
+000030d0: 2f64 6332 3437 3132 6633 3563 3430 6539  /dc24712f35c40e9
+000030e0: 3538 6265 3861 6361 3237 3331 6537 6266  58be8aca2731e7bf
+000030f0: 3833 3533 6239 6231 3862 6161 3661 3934  8353b9b18baa6a94
+00003100: 6164 3834 6336 3935 3263 6263 3737 3030  ad84c6952cbc7700
+00003110: 342f 6c61 7965 722e 7461 7227 2e2e 2e0a  4/layer.tar'....
+00003120: 2020 2020 3230 3136 2d30 342d 3031 2031      2016-04-01 1
+00003130: 333a 3135 3a31 322c 3735 3720 726f 6f74  3:15:12,757 root
+00003140: 2020 2020 2020 2020 2049 4e46 4f20 2020           INFO   
+00003150: 2020 5371 7561 7368 696e 6720 6669 6c65    Squashing file
+00003160: 2027 2f74 6d70 2f64 6f63 6b65 722d 7371   '/tmp/docker-sq
+00003170: 7561 7368 2d66 7538 3043 582f 6f6c 642f  uash-fu80CX/old/
+00003180: 6439 3239 3132 3964 3463 3865 3631 6561  d929129d4c8e61ea
+00003190: 3336 3631 6562 3432 6333 3064 3031 6634  3661eb42c30d01f4
+000031a0: 6331 3532 3431 3836 3839 3137 3861 6663  c152418689178afc
+000031b0: 3764 6338 3138 3561 3337 3831 3435 3238  7dc8185a37814528
+000031c0: 2f6c 6179 6572 2e74 6172 272e 2e2e 0a20  /layer.tar'.... 
+000031d0: 2020 2032 3031 362d 3034 2d30 3120 3133     2016-04-01 13
+000031e0: 3a31 353a 3133 2c32 3334 2072 6f6f 7420  :15:13,234 root 
+000031f0: 2020 2020 2020 2020 494e 464f 2020 2020          INFO    
+00003200: 2053 7175 6173 6869 6e67 2066 696c 6520   Squashing file 
+00003210: 272f 746d 702f 646f 636b 6572 2d73 7175  '/tmp/docker-squ
+00003220: 6173 682d 6675 3830 4358 2f6f 6c64 2f62  ash-fu80CX/old/b
+00003230: 3866 6133 6361 6637 6436 6463 3232 3862  8fa3caf7d6dc228b
+00003240: 6632 3439 3961 3361 6638 3665 3530 3733  f2499a3af86e5073
+00003250: 6164 3063 3137 3330 3463 3339 3030 6661  ad0c17304c3900fa
+00003260: 3334 3165 3964 3266 6534 6535 3635 352f  341e9d2fe4e5655/
+00003270: 6c61 7965 722e 7461 7227 2e2e 2e0a 2020  layer.tar'....  
+00003280: 2020 3230 3136 2d30 342d 3031 2031 333a    2016-04-01 13:
+00003290: 3135 3a31 332c 3233 3520 726f 6f74 2020  15:13,235 root  
+000032a0: 2020 2020 2020 2049 4e46 4f20 2020 2020         INFO     
+000032b0: 5371 7561 7368 696e 6720 6669 6c65 2027  Squashing file '
+000032c0: 2f74 6d70 2f64 6f63 6b65 722d 7371 7561  /tmp/docker-squa
+000032d0: 7368 2d66 7538 3043 582f 6f6c 642f 3338  sh-fu80CX/old/38
+000032e0: 6238 6638 3565 3734 6266 6137 3733 6130  b8f85e74bfa773a0
+000032f0: 6164 3639 6461 3232 3035 6463 3031 3438  ad69da2205dc0148
+00003300: 3934 3565 3666 3561 3763 6562 3034 6661  945e6f5a7ceb04fa
+00003310: 3465 3836 3139 6531 6465 3432 3562 2f6c  4e8619e1de425b/l
+00003320: 6179 6572 2e74 6172 272e 2e2e 0a20 2020  ayer.tar'....   
+00003330: 2032 3031 362d 3034 2d30 3120 3133 3a31   2016-04-01 13:1
+00003340: 353a 3133 2c32 3335 2072 6f6f 7420 2020  5:13,235 root   
+00003350: 2020 2020 2020 494e 464f 2020 2020 2053        INFO     S
+00003360: 7175 6173 6869 6e67 2066 696c 6520 272f  quashing file '/
+00003370: 746d 702f 646f 636b 6572 2d73 7175 6173  tmp/docker-squas
+00003380: 682d 6675 3830 4358 2f6f 6c64 2f61 6537  h-fu80CX/old/ae7
+00003390: 3962 3634 3662 3961 3961 3238 3763 3566  9b646b9a9a287c5f
+000033a0: 3661 3031 3837 3163 6339 6439 6565 3539  6a01871cc9d9ee59
+000033b0: 3664 6166 6565 3264 6239 3432 3731 3463  6dafee2db942714c
+000033c0: 6133 6465 6130 6330 3665 6566 332f 6c61  a3dea0c06eef3/la
+000033d0: 7965 722e 7461 7227 2e2e 2e0a 2020 2020  yer.tar'....    
+000033e0: 3230 3136 2d30 342d 3031 2031 333a 3135  2016-04-01 13:15
+000033f0: 3a31 332c 3233 3520 726f 6f74 2020 2020  :13,235 root    
+00003400: 2020 2020 2049 4e46 4f20 2020 2020 5371       INFO     Sq
+00003410: 7561 7368 696e 6720 6669 6c65 2027 2f74  uashing file '/t
+00003420: 6d70 2f64 6f63 6b65 722d 7371 7561 7368  mp/docker-squash
+00003430: 2d66 7538 3043 582f 6f6c 642f 3262 3436  -fu80CX/old/2b46
+00003440: 3036 6463 3964 6337 3733 6161 3232 3061  06dc9dc773aa220a
+00003450: 3635 3335 3166 6538 6435 3466 3033 3533  65351fe8d54f0353
+00003460: 3463 3538 6665 6132 3330 3936 3065 3935  4c58fea230960e95
+00003470: 3931 3532 3232 3336 3630 3734 2f6c 6179  915222366074/lay
+00003480: 6572 2e74 6172 272e 2e2e 0a20 2020 2032  er.tar'....    2
+00003490: 3031 362d 3034 2d30 3120 3133 3a31 353a  016-04-01 13:15:
+000034a0: 3133 2c32 3336 2072 6f6f 7420 2020 2020  13,236 root     
+000034b0: 2020 2020 494e 464f 2020 2020 2053 7175      INFO     Squ
+000034c0: 6173 6869 6e67 2066 696c 6520 272f 746d  ashing file '/tm
+000034d0: 702f 646f 636b 6572 2d73 7175 6173 682d  p/docker-squash-
+000034e0: 6675 3830 4358 2f6f 6c64 2f31 3138 6661  fu80CX/old/118fa
+000034f0: 3965 3333 3537 3665 6363 3632 3565 6262  9e33576ecc625ebb
+00003500: 6266 6466 3238 3039 6331 3532 3765 3731  bfdf2809c1527e71
+00003510: 3663 6234 6664 3563 6234 3035 3438 6562  6cb4fd5cb40548eb
+00003520: 3664 3335 3033 6137 3561 392f 6c61 7965  6d3503a75a9/laye
+00003530: 722e 7461 7227 2e2e 2e0a 2020 2020 3230  r.tar'....    20
+00003540: 3136 2d30 342d 3031 2031 333a 3135 3a31  16-04-01 13:15:1
+00003550: 332c 3233 3620 726f 6f74 2020 2020 2020  3,236 root      
+00003560: 2020 2049 4e46 4f20 2020 2020 5371 7561     INFO     Squa
+00003570: 7368 696e 6720 6669 6c65 2027 2f74 6d70  shing file '/tmp
+00003580: 2f64 6f63 6b65 722d 7371 7561 7368 2d66  /docker-squash-f
+00003590: 7538 3043 582f 6f6c 642f 3566 3765 3866  u80CX/old/5f7e8f
+000035a0: 3336 6333 6262 3230 6339 6462 3734 3730  36c3bb20c9db7470
+000035b0: 6132 3266 3832 3837 3130 6234 6432 3861  a22f828710b4d28a
+000035c0: 6564 6536 3439 3636 6334 3235 6164 6434  ede64966c425add4
+000035d0: 3861 3162 3134 6665 3233 2f6c 6179 6572  8a1b14fe23/layer
+000035e0: 2e74 6172 272e 2e2e 0a20 2020 2032 3031  .tar'....    201
+000035f0: 362d 3034 2d30 3120 3133 3a31 353a 3134  6-04-01 13:15:14
+00003600: 2c38 3438 2072 6f6f 7420 2020 2020 2020  ,848 root       
+00003610: 2020 494e 464f 2020 2020 2053 7175 6173    INFO     Squas
+00003620: 6869 6e67 2066 696e 6973 6865 6421 0a20  hing finished!. 
+00003630: 2020 2032 3031 362d 3034 2d30 3120 3133     2016-04-01 13
+00003640: 3a31 353a 3134 2c38 3533 2072 6f6f 7420  :15:14,853 root 
+00003650: 2020 2020 2020 2020 494e 464f 2020 2020          INFO    
+00003660: 204e 6577 2073 7175 6173 6865 6420 696d   New squashed im
+00003670: 6167 6520 4944 2069 7320 6664 6537 6564  age ID is fde7ed
+00003680: 6432 6535 3638 3363 3937 6265 6466 3963  d2e5683c97bedf9c
+00003690: 3062 6635 3261 6435 3135 3064 6235 3635  0bf52ad5150db565
+000036a0: 3065 3432 3164 6533 6439 3239 3363 6535  0e421de3d9293ce5
+000036b0: 3232 3362 3235 3634 3535 0a20 2020 2032  223b256455.    2
+000036c0: 3031 362d 3034 2d30 3120 3133 3a31 353a  016-04-01 13:15:
+000036d0: 3138 2c39 3633 2072 6f6f 7420 2020 2020  18,963 root     
+000036e0: 2020 2020 494e 464f 2020 2020 2049 6d61      INFO     Ima
+000036f0: 6765 2072 6567 6973 7465 7265 6420 696e  ge registered in
+00003700: 2044 6f63 6b65 7220 6461 656d 6f6e 2061   Docker daemon a
+00003710: 7320 6a62 6f73 732f 7769 6c64 666c 793a  s jboss/wildfly:
+00003720: 7371 7561 7368 6564 0a20 2020 2032 3031  squashed.    201
+00003730: 362d 3034 2d30 3120 3133 3a31 353a 3139  6-04-01 13:15:19
+00003740: 2c30 3539 2072 6f6f 7420 2020 2020 2020  ,059 root       
+00003750: 2020 494e 464f 2020 2020 2044 6f6e 650a    INFO     Done.
+00003760: 0a4c 6574 2773 2063 6f6e 6669 726d 2074  .Let's confirm t
+00003770: 6865 2069 6d61 6765 2073 7472 7563 7475  he image structu
+00003780: 7265 206e 6f77 3a0a 0a3a 3a0a 0a20 2020  re now:..::..   
+00003790: 2024 2064 6f63 6b65 7220 6869 7374 6f72   $ docker histor
+000037a0: 7920 6a62 6f73 732f 7769 6c64 666c 793a  y jboss/wildfly:
+000037b0: 7371 7561 7368 6564 0a20 2020 2049 4d41  squashed.    IMA
+000037c0: 4745 2020 2020 2020 2020 2020 2020 2020  GE              
+000037d0: 2043 5245 4154 4544 2020 2020 2020 2020   CREATED        
+000037e0: 2020 2020 2043 5245 4154 4544 2042 5920       CREATED BY 
+000037f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003800: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003810: 2020 2020 2053 495a 4520 2020 2020 2020       SIZE       
+00003820: 2020 2020 2020 2020 2043 4f4d 4d45 4e54           COMMENT
+00003830: 0a20 2020 2066 6465 3765 6464 3265 3536  .    fde7edd2e56
+00003840: 3820 2020 2020 2020 2033 3220 7365 636f  8        32 seco
+00003850: 6e64 7320 6167 6f20 2020 2020 2020 2020  nds ago         
+00003860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003880: 2020 2020 2020 2020 2020 2020 2033 3538               358
+00003890: 2e32 204d 420a 2020 2020 3364 3464 3032  .2 MB.    3d4d02
+000038a0: 3238 6631 3631 2020 2020 2020 2020 3320  28f161        3 
+000038b0: 7765 656b 7320 6167 6f20 2020 2020 2020  weeks ago       
+000038c0: 2020 2f62 696e 2f73 6820 2d63 2023 286e    /bin/sh -c #(n
+000038d0: 6f70 2920 5553 4552 205b 726f 6f74 5d20  op) USER [root] 
+000038e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000038f0: 2020 3020 420a 2020 2020 6637 6162 3465    0 B.    f7ab4e
+00003900: 6131 3937 3038 2020 2020 2020 2020 3320  a19708        3 
+00003910: 7765 656b 7320 6167 6f20 2020 2020 2020  weeks ago       
+00003920: 2020 2f62 696e 2f73 6820 2d63 2023 286e    /bin/sh -c #(n
+00003930: 6f70 2920 4d41 494e 5441 494e 4552 204d  op) MAINTAINER M
+00003940: 6172 656b 2047 6f6c 646d 616e 6e20 3c20  arek Goldmann < 
+00003950: 2020 3020 420a 2020 2020 3462 6231 3566    0 B.    4bb15f
+00003960: 3362 3639 3737 2020 2020 2020 2020 3320  3b6977        3 
+00003970: 7765 656b 7320 6167 6f20 2020 2020 2020  weeks ago       
+00003980: 2020 2f62 696e 2f73 6820 2d63 2023 286e    /bin/sh -c #(n
+00003990: 6f70 2920 5553 4552 205b 6a62 6f73 735d  op) USER [jboss]
+000039a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000039b0: 2020 3020 420a 2020 2020 3564 6331 6534    0 B.    5dc1e4
+000039c0: 3966 3433 3631 2020 2020 2020 2020 3320  9f4361        3 
+000039d0: 7765 656b 7320 6167 6f20 2020 2020 2020  weeks ago       
+000039e0: 2020 2f62 696e 2f73 6820 2d63 2023 286e    /bin/sh -c #(n
+000039f0: 6f70 2920 574f 524b 4449 5220 2f6f 7074  op) WORKDIR /opt
+00003a00: 2f6a 626f 7373 2020 2020 2020 2020 2020  /jboss          
+00003a10: 2020 3020 420a 2020 2020 3766 3066 3965    0 B.    7f0f9e
+00003a20: 6233 3131 3734 2020 2020 2020 2020 3320  b31174        3 
+00003a30: 7765 656b 7320 6167 6f20 2020 2020 2020  weeks ago       
+00003a40: 2020 2f62 696e 2f73 6820 2d63 2067 726f    /bin/sh -c gro
+00003a50: 7570 6164 6420 2d72 206a 626f 7373 202d  upadd -r jboss -
+00003a60: 6720 3130 3030 2026 2620 7573 6572 6120  g 1000 && usera 
+00003a70: 2020 342e 3334 3920 6b42 0a20 2020 2062    4.349 kB.    b
+00003a80: 6435 3135 6630 3434 6166 3720 2020 2020  d515f044af7     
 00003a90: 2020 2033 2077 6565 6b73 2061 676f 2020     3 weeks ago  
 00003aa0: 2020 2020 2020 202f 6269 6e2f 7368 202d         /bin/sh -
-00003ab0: 6320 2328 6e6f 7029 204c 4142 454c 206e  c #(nop) LABEL n
-00003ac0: 616d 653d 4365 6e74 4f53 2042 6173 6520  ame=CentOS Base 
-00003ad0: 496d 6167 2020 2030 2042 2020 2020 2020  Imag   0 B      
-00003ae0: 2020 2020 2020 2020 2020 200a 2020 2020             .    
-00003af0: 3437 3463 3265 6537 3766 6133 2020 2020  474c2ee77fa3    
-00003b00: 2020 2020 3320 7765 656b 7320 6167 6f20      3 weeks ago 
-00003b10: 2020 2020 2020 2020 2f62 696e 2f73 6820          /bin/sh 
-00003b20: 2d63 2023 286e 6f70 2920 4144 4420 6669  -c #(nop) ADD fi
-00003b30: 6c65 3a37 3238 3532 6663 3736 3236 6432  le:72852fc7626d2
-00003b40: 3333 3334 3320 2020 3139 362e 3620 4d42  33343   196.6 MB
-00003b50: 2020 2020 2020 2020 2020 2020 0a20 2020              .   
-00003b60: 2031 3534 3430 3834 6661 6438 3120 2020   1544084fad81   
-00003b70: 2020 2020 2036 206d 6f6e 7468 7320 6167       6 months ag
-00003b80: 6f20 2020 2020 2020 202f 6269 6e2f 7368  o        /bin/sh
-00003b90: 202d 6320 2328 6e6f 7029 204d 4149 4e54   -c #(nop) MAINT
-00003ba0: 4149 4e45 5220 5468 6520 4365 6e74 4f53  AINER The CentOS
-00003bb0: 2050 726f 6a65 2020 2030 2042 0a0a        Proje   0 B..
+00003ab0: 6320 7975 6d20 7570 6461 7465 202d 7920  c yum update -y 
+00003ac0: 2626 2079 756d 202d 7920 696e 7374 616c  && yum -y instal
+00003ad0: 6c20 786d 2020 2032 352e 3138 204d 420a  l xm   25.18 MB.
+00003ae0: 2020 2020 6237 3833 3336 3039 3930 3435      b78336099045
+00003af0: 2020 2020 2020 2020 3320 7765 656b 7320          3 weeks 
+00003b00: 6167 6f20 2020 2020 2020 2020 2f62 696e  ago         /bin
+00003b10: 2f73 6820 2d63 2023 286e 6f70 2920 4d41  /sh -c #(nop) MA
+00003b20: 494e 5441 494e 4552 204d 6172 656b 2047  INTAINER Marek G
+00003b30: 6f6c 646d 616e 6e20 3c20 2020 3020 420a  oldmann <   0 B.
+00003b40: 2020 2020 3438 3136 6132 3938 3534 3863      4816a298548c
+00003b50: 2020 2020 2020 2020 3320 7765 656b 7320          3 weeks 
+00003b60: 6167 6f20 2020 2020 2020 2020 2f62 696e  ago         /bin
+00003b70: 2f73 6820 2d63 2023 286e 6f70 2920 434d  /sh -c #(nop) CM
+00003b80: 4420 5b22 2f62 696e 2f62 6173 6822 5d20  D ["/bin/bash"] 
+00003b90: 2020 2020 2020 2020 2020 2020 3020 420a              0 B.
+00003ba0: 2020 2020 3665 6532 3335 6366 3434 3733      6ee235cf4473
+00003bb0: 2020 2020 2020 2020 3320 7765 656b 7320          3 weeks 
+00003bc0: 6167 6f20 2020 2020 2020 2020 2f62 696e  ago         /bin
+00003bd0: 2f73 6820 2d63 2023 286e 6f70 2920 4c41  /sh -c #(nop) LA
+00003be0: 4245 4c20 6e61 6d65 3d43 656e 744f 5320  BEL name=CentOS 
+00003bf0: 4261 7365 2049 6d61 6720 2020 3020 420a  Base Imag   0 B.
+00003c00: 2020 2020 3437 3463 3265 6537 3766 6133      474c2ee77fa3
+00003c10: 2020 2020 2020 2020 3320 7765 656b 7320          3 weeks 
+00003c20: 6167 6f20 2020 2020 2020 2020 2f62 696e  ago         /bin
+00003c30: 2f73 6820 2d63 2023 286e 6f70 2920 4144  /sh -c #(nop) AD
+00003c40: 4420 6669 6c65 3a37 3238 3532 6663 3736  D file:72852fc76
+00003c50: 3236 6432 3333 3334 3320 2020 3139 362e  26d233343   196.
+00003c60: 3620 4d42 0a20 2020 2031 3534 3430 3834  6 MB.    1544084
+00003c70: 6661 6438 3120 2020 2020 2020 2036 206d  fad81        6 m
+00003c80: 6f6e 7468 7320 6167 6f20 2020 2020 2020  onths ago       
+00003c90: 202f 6269 6e2f 7368 202d 6320 2328 6e6f   /bin/sh -c #(no
+00003ca0: 7029 204d 4149 4e54 4149 4e45 5220 5468  p) MAINTAINER Th
+00003cb0: 6520 4365 6e74 4f53 2050 726f 6a65 2020  e CentOS Proje  
+00003cc0: 2030 2042 0a                              0 B.
```

### Comparing `docker-squash-1.0.9/docker_squash/cli.py` & `docker-squash-1.1.0/docker_squash/cli.py`

 * *Files 26% similar despite different names*

```diff
@@ -13,97 +13,146 @@
 class SingleLevelFilter(logging.Filter):
     def __init__(self, passlevel, reject):
         self.passlevel = passlevel
         self.reject = reject
 
     def filter(self, record):
         if self.reject:
-            return (record.levelno != self.passlevel)
+            return record.levelno != self.passlevel
         else:
-            return (record.levelno == self.passlevel)
+            return record.levelno == self.passlevel
 
 
 class MyParser(argparse.ArgumentParser):
+    # noinspection PyMethodMayBeStatic
+    def str2bool(self, v: str) -> bool:
+        if isinstance(v, bool):
+            return v
+        if v.lower() in ("yes", "true", "t", "y", "1"):
+            return True
+        elif v.lower() in ("no", "false", "f", "n", "0"):
+            return False
+        else:
+            raise argparse.ArgumentTypeError("Boolean value expected.")
 
     def error(self, message):
         self.print_help()
-        sys.stderr.write('\nError: %s\n' % message)
+        sys.stderr.write("\nError: %s\n" % message)
         sys.exit(2)
 
 
 class CLI(object):
-
     def __init__(self):
         handler_out = logging.StreamHandler(sys.stdout)
         handler_err = logging.StreamHandler(sys.stderr)
 
         handler_out.addFilter(SingleLevelFilter(logging.INFO, False))
         handler_err.addFilter(SingleLevelFilter(logging.INFO, True))
 
         self.log = logging.getLogger()
         formatter = logging.Formatter(
-            '%(asctime)s %(name)-12s %(levelname)-8s %(message)s')
+            "%(asctime)s %(name)-12s %(levelname)-8s %(message)s"
+        )
 
         handler_out.setFormatter(formatter)
         handler_err.setFormatter(formatter)
 
         self.log.addHandler(handler_out)
         self.log.addHandler(handler_err)
 
     def run(self):
-        parser = MyParser(
-            description='Docker layer squashing tool')
+        parser = MyParser(description="Docker layer squashing tool")
 
         parser.add_argument(
-            '-v', '--verbose', action='store_true', help='Verbose output')
+            "-v", "--verbose", action="store_true", help="Verbose output"
+        )
 
         parser.add_argument(
-            '--version', action='version', help='Show version and exit', version=version)
-
-        parser.add_argument('image', help='Image to be squashed')
-        parser.add_argument(
-            '-d', '--development', action='store_true', help='Does not clean up after failure for easier debugging')
-        parser.add_argument(
-            '-f', '--from-layer', help='Number of layers to squash or ID of the layer (or image ID or image name) to squash from. In case the provided value is an integer, specified number of layers will be squashed. Every layer in the image will be squashed if the parameter is not provided.')
-        parser.add_argument(
-            '-t', '--tag', help="Specify the tag to be used for the new image. If not specified no tag will be applied")
-        parser.add_argument(
-            '-m', '--message', help="Specify a commit message (comment) for the new image.")
-        parser.add_argument(
-            '-c', '--cleanup', action='store_true', help="Remove source image from Docker after squashing")
-        parser.add_argument(
-            '--tmp-dir', help='Temporary directory to be created and used')
-        parser.add_argument(
-            '--output-path', help='Path where the image should be stored after squashing. If not provided, image will be loaded into Docker daemon')
+            "--version", action="version", help="Show version and exit", version=version
+        )
+
+        parser.add_argument("image", help="Image to be squashed")
+        parser.add_argument(
+            "-d",
+            "--development",
+            action="store_true",
+            help="Does not clean up after failure for easier debugging",
+        )
+        parser.add_argument(
+            "-f",
+            "--from-layer",
+            help="Number of layers to squash or ID of the layer (or image ID or image name) to squash from. In case the provided value is an integer, specified number of layers will be squashed. Every layer in the image will be squashed if the parameter is not provided.",
+        )
+        parser.add_argument(
+            "-t",
+            "--tag",
+            help="Specify the tag to be used for the new image. If not specified no tag will be applied",
+        )
+        parser.add_argument(
+            "-m",
+            "--message",
+            help="Specify a commit message (comment) for the new image.",
+        )
+        parser.add_argument(
+            "-c",
+            "--cleanup",
+            action="store_true",
+            help="Remove source image from Docker after squashing",
+        )
+        parser.add_argument(
+            "--tmp-dir", help="Temporary directory to be created and used"
+        )
+        parser.add_argument(
+            "--output-path",
+            help="Path where the image may be stored after squashing.",
+        )
+        parser.add_argument(
+            "--load-image",
+            type=parser.str2bool,
+            const=True,
+            nargs="?",
+            default=True,
+            help="Whether to load the image into Docker daemon after squashing",
+        )
 
         args = parser.parse_args()
 
         if args.verbose:
             self.log.setLevel(logging.DEBUG)
         else:
             self.log.setLevel(logging.INFO)
 
         self.log.debug("Running version %s", version)
-
         try:
-            squash.Squash(log=self.log, image=args.image,
-                          from_layer=args.from_layer, tag=args.tag, comment=args.message, output_path=args.output_path, tmp_dir=args.tmp_dir, development=args.development, cleanup=args.cleanup).run()
+            squash.Squash(
+                log=self.log,
+                image=args.image,
+                from_layer=args.from_layer,
+                tag=args.tag,
+                comment=args.message,
+                output_path=args.output_path,
+                load_image=args.load_image,
+                tmp_dir=args.tmp_dir,
+                development=args.development,
+                cleanup=args.cleanup,
+            ).run()
         except KeyboardInterrupt:
             self.log.error("Program interrupted by user, exiting...")
             sys.exit(1)
-        except:
+        except Exception:
             e = sys.exc_info()[1]
 
             if args.development or args.verbose:
                 self.log.exception(e)
             else:
                 self.log.error(str(e))
 
             self.log.error(
-                "Execution failed, consult logs above. If you think this is our fault, please file an issue: https://github.com/goldmann/docker-squash/issues, thanks!")
+                "Execution failed, consult logs above. If you think this is our fault, please file an issue: https://github.com/goldmann/docker-squash/issues, thanks!"
+            )
 
             if isinstance(e, SquashError):
                 sys.exit(e.code)
 
             sys.exit(1)
```

### Comparing `docker-squash-1.0.9/docker_squash/image.py` & `docker-squash-1.1.0/docker_squash/image.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,30 +1,29 @@
-
 import datetime
-import docker
 import hashlib
+import itertools
 import json
 import logging
 import os
+import pathlib
 import re
 import shutil
-import six
 import tarfile
 import tempfile
 import threading
+from typing import List
 
-from docker_squash.errors import SquashError, SquashUnnecessaryError
+import docker
 
-if not six.PY3:
-    import docker_squash.lib.xtarfile
+from docker_squash.errors import SquashError, SquashUnnecessaryError
 
 
 class Chdir(object):
 
-    """ Context manager for changing the current working directory """
+    """Context manager for changing the current working directory"""
 
     def __init__(self, newPath):
         self.newPath = os.path.expanduser(newPath)
 
     def __enter__(self):
         self.savedPath = os.getcwd()
         os.chdir(self.newPath)
@@ -40,15 +39,17 @@
 
     This class should not be used directly.
     """
 
     FORMAT = None
     """ Image format version """
 
-    def __init__(self, log, docker, image, from_layer, tmp_dir=None, tag=None, comment=""):
+    def __init__(
+        self, log, docker, image, from_layer, tmp_dir=None, tag=None, comment=""
+    ):
         self.log = log
         self.debug = self.log.isEnabledFor(logging.DEBUG)
         self.docker = docker
         self.image = image
         self.from_layer = from_layer
         self.tag = tag
         self.comment = comment
@@ -60,15 +61,16 @@
         #
         # Golang doesn't add padding to microseconds when marshaling
         # microseconds in date into JSON. Python does.
         # We need to produce same output as Docker's to not generate
         # different metadata. That's why we need to strip all zeros at the
         # end of the date string...
         self.date = re.sub(
-            r'0*Z$', 'Z', datetime.datetime.utcnow().strftime('%Y-%m-%dT%H:%M:%S.%fZ'))
+            r"0*Z$", "Z", datetime.datetime.utcnow().strftime("%Y-%m-%dT%H:%M:%S.%fZ")
+        )
         """ Date used in metadata, already formatted using the `%Y-%m-%dT%H:%M:%S.%fZ` format """
 
         self.tmp_dir = tmp_dir
         """ Main temporary directory to save all working files. This is the root directory for all other temporary files. """
 
     def squash(self):
         self._before_squashing()
@@ -77,24 +79,24 @@
 
         return ret
 
     def _squash(self):
         pass
 
     def cleanup(self):
-        """ Cleanup the temporary directory """
+        """Cleanup the temporary directory"""
 
         self.log.debug("Cleaning up %s temporary directory" % self.tmp_dir)
         shutil.rmtree(self.tmp_dir, ignore_errors=True)
 
     def _initialize_directories(self):
         # Prepare temporary directory where all the work will be executed
         try:
             self.tmp_dir = self._prepare_tmp_directory(self.tmp_dir)
-        except:
+        except Exception:
             raise SquashError("Preparing temporary directory failed")
 
         # Temporary location on the disk of the old, unpacked *image*
         self.old_image_dir = os.path.join(self.tmp_dir, "old")
         # Temporary location on the disk of the new, unpacked, squashed *image*
         self.new_image_dir = os.path.join(self.tmp_dir, "new")
         # Temporary location on the disk of the squashed *layer*
@@ -102,114 +104,128 @@
 
         for d in self.old_image_dir, self.new_image_dir:
             os.makedirs(d)
 
     def _squash_id(self, layer):
         if layer == "<missing>":
             self.log.warning(
-                "You try to squash from layer that does not have it's own ID, we'll try to find it later")
+                "You try to squash from layer that does not have it's own ID, we'll try to find it later"
+            )
             return None
 
         try:
-            squash_id = self.docker.inspect_image(layer)['Id']
-        except:
+            squash_id = self.docker.inspect_image(layer)["Id"]
+        except Exception:
             raise SquashError(
-                "Could not get the layer ID to squash, please check provided 'layer' argument: %s" % layer)
+                "Could not get the layer ID to squash, please check provided 'layer' argument: %s"
+                % layer
+            )
 
         if squash_id not in self.old_image_layers:
             raise SquashError(
-                "Couldn't find the provided layer (%s) in the %s image" % (layer, self.image))
+                "Couldn't find the provided layer (%s) in the %s image"
+                % (layer, self.image)
+            )
 
         self.log.debug("Layer ID to squash from: %s" % squash_id)
 
         return squash_id
 
     def _validate_number_of_layers(self, number_of_layers):
         """
         Makes sure that the specified number of layers to squash
         is a valid number
         """
 
         # Only positive numbers are correct
         if number_of_layers <= 0:
             raise SquashError(
-                "Number of layers to squash cannot be less or equal 0, provided: %s" % number_of_layers)
+                "Number of layers to squash cannot be less or equal 0, provided: %s"
+                % number_of_layers
+            )
 
         # Do not squash if provided number of layer to squash is bigger
         # than number of actual layers in the image
         if number_of_layers > len(self.old_image_layers):
             raise SquashError(
-                "Cannot squash %s layers, the %s image contains only %s layers" % (number_of_layers, self.image, len(self.old_image_layers)))
+                "Cannot squash %s layers, the %s image contains only %s layers"
+                % (number_of_layers, self.image, len(self.old_image_layers))
+            )
 
     def _before_squashing(self):
         self._initialize_directories()
 
         # Location of the tar archive with squashed layers
         self.squashed_tar = os.path.join(self.squashed_dir, "layer.tar")
 
         if self.tag:
             self.image_name, self.image_tag = self._parse_image_name(self.tag)
 
         # The image id or name of the image to be squashed
         try:
-            self.old_image_id = self.docker.inspect_image(self.image)['Id']
+            self.old_image_id = self.docker.inspect_image(self.image)["Id"]
         except SquashError:
             raise SquashError(
-                "Could not get the image ID to squash, please check provided 'image' argument: %s" % self.image)
+                "Could not get the image ID to squash, please check provided 'image' argument: %s"
+                % self.image
+            )
 
         self.old_image_layers = []
 
         # Read all layers in the image
         self._read_layers(self.old_image_layers, self.old_image_id)
 
         self.old_image_layers.reverse()
 
         self.log.info("Old image has %s layers", len(self.old_image_layers))
         self.log.debug("Old layers: %s", self.old_image_layers)
 
         # By default - squash all layers.
-        if self.from_layer == None:
+        if self.from_layer is None:
             self.from_layer = len(self.old_image_layers)
 
         try:
             number_of_layers = int(self.from_layer)
 
-            self.log.debug(
-                "We detected number of layers as the argument to squash")
+            self.log.debug("We detected number of layers as the argument to squash")
         except ValueError:
             self.log.debug("We detected layer as the argument to squash")
 
             squash_id = self._squash_id(self.from_layer)
 
             if not squash_id:
                 raise SquashError(
-                    "The %s layer could not be found in the %s image" % (self.from_layer, self.image))
-
-            number_of_layers = len(self.old_image_layers) - \
-                self.old_image_layers.index(squash_id) - 1
+                    "The %s layer could not be found in the %s image"
+                    % (self.from_layer, self.image)
+                )
+
+            number_of_layers = (
+                len(self.old_image_layers) - self.old_image_layers.index(squash_id) - 1
+            )
 
         self._validate_number_of_layers(number_of_layers)
 
         marker = len(self.old_image_layers) - number_of_layers
 
         self.layers_to_squash = self.old_image_layers[marker:]
         self.layers_to_move = self.old_image_layers[:marker]
 
         self.log.info("Checking if squashing is necessary...")
 
         if len(self.layers_to_squash) < 1:
             raise SquashError(
-                "Invalid number of layers to squash: %s" % len(self.layers_to_squash))
+                "Invalid number of layers to squash: %s" % len(self.layers_to_squash)
+            )
 
         if len(self.layers_to_squash) == 1:
             raise SquashUnnecessaryError(
-                "Single layer marked to squash, no squashing is required")
+                "Single layer marked to squash, no squashing is required"
+            )
 
-        self.log.info("Attempting to squash last %s layers...",
-                      number_of_layers)
+        self.log.info("Attempting to squash last %s layers...", number_of_layers)
         self.log.debug("Layers to squash: %s", self.layers_to_squash)
         self.log.debug("Layers to move: %s", self.layers_to_move)
 
         # Fetch the image and unpack it on the fly to the old image directory
         self._save_image(self.old_image_id, self.old_image_dir)
 
         self.size_before = self._dir_size(self.old_image_dir)
@@ -218,25 +234,29 @@
 
     def _after_squashing(self):
         self.log.debug("Removing from disk already squashed layers...")
         shutil.rmtree(self.old_image_dir, ignore_errors=True)
 
         self.size_after = self._dir_size(self.new_image_dir)
 
-        size_before_mb = float(self.size_before)/1024/1024
-        size_after_mb = float(self.size_after)/1024/1024
+        size_before_mb = float(self.size_before) / 1024 / 1024
+        size_after_mb = float(self.size_after) / 1024 / 1024
 
         self.log.info("Original image size: %.2f MB" % size_before_mb)
         self.log.info("Squashed image size: %.2f MB" % size_after_mb)
 
-        if (size_after_mb >= size_before_mb):
-            self.log.info("If the squashed image is larger than original it means that there were no meaningful files to squash and it just added metadata. Are you sure you specified correct parameters?")
+        if size_after_mb >= size_before_mb:
+            self.log.info(
+                "If the squashed image is larger than original it means that there were no meaningful files to squash and it just added metadata. Are you sure you specified correct parameters?"
+            )
         else:
-            self.log.info("Image size decreased by %.2f %%" % float(
-                ((size_before_mb-size_after_mb)/size_before_mb)*100))
+            self.log.info(
+                "Image size decreased by %.2f %%"
+                % float(((size_before_mb - size_after_mb) / size_before_mb) * 100)
+            )
 
     def _dir_size(self, directory):
         size = 0
 
         for path, dirs, files in os.walk(directory):
             for f in files:
                 size += os.path.getsize(os.path.join(path, f))
@@ -253,129 +273,131 @@
         self._tar_image(target_tar_file, self.new_image_dir)
         self.log.info("Image available at '%s'" % target_tar_file)
 
     def load_squashed_image(self):
         self._load_image(self.new_image_dir)
 
         if self.tag:
-            self.log.info("Image registered in Docker daemon as %s:%s" %
-                          (self.image_name, self.image_tag))
+            self.log.info(
+                "Image registered in Docker daemon as %s:%s"
+                % (self.image_name, self.image_tag)
+            )
 
     def _files_in_layers(self, layers, directory):
         """
         Prepare a list of files in all layers
         """
         files = {}
 
         for layer in layers:
             self.log.debug("Generating list of files in layer '%s'..." % layer)
             tar_file = os.path.join(directory, layer, "layer.tar")
-            with tarfile.open(tar_file, 'r', format=tarfile.PAX_FORMAT) as tar:
-                files[layer] = [self._normalize_path(
-                    x) for x in tar.getnames()]
+            with tarfile.open(tar_file, "r", format=tarfile.PAX_FORMAT) as tar:
+                files[layer] = [self._normalize_path(x) for x in tar.getnames()]
             self.log.debug("Done, found %s files" % len(files[layer]))
 
         return files
 
     def _prepare_tmp_directory(self, tmp_dir):
-        """ Creates temporary directory that is used to work on layers """
+        """Creates temporary directory that is used to work on layers"""
 
         if tmp_dir:
             if os.path.exists(tmp_dir):
                 raise SquashError(
-                    "The '%s' directory already exists, please remove it before you proceed" % tmp_dir)
+                    "The '%s' directory already exists, please remove it before you proceed"
+                    % tmp_dir
+                )
             os.makedirs(tmp_dir)
         else:
             tmp_dir = tempfile.mkdtemp(prefix="docker-squash-")
 
         self.log.debug("Using %s as the temporary directory" % tmp_dir)
 
         return tmp_dir
 
     def _load_image(self, directory):
-
         tar_file = os.path.join(self.tmp_dir, "image.tar")
 
         self._tar_image(tar_file, directory)
 
-        with open(tar_file, 'rb') as f:
+        with open(tar_file, "rb") as f:
             self.log.debug("Loading squashed image...")
             self.docker.load_image(f)
             self.log.debug("Image loaded!")
 
         os.remove(tar_file)
 
     def _tar_image(self, target_tar_file, directory):
-        with tarfile.open(target_tar_file, 'w', format=tarfile.PAX_FORMAT) as tar:
+        with tarfile.open(target_tar_file, "w", format=tarfile.PAX_FORMAT) as tar:
             self.log.debug("Generating tar archive for the squashed image...")
             with Chdir(directory):
                 # docker produces images like this:
                 #   repositories
                 #   <layer>/json
                 # and not:
                 #   ./
                 #   ./repositories
                 #   ./<layer>/json
                 for f in os.listdir("."):
                     tar.add(f)
             self.log.debug("Archive generated")
 
     def _layers_to_squash(self, layers, from_layer):
-        """ Prepares a list of layer IDs that should be squashed """
+        """Prepares a list of layer IDs that should be squashed"""
         to_squash = []
         to_leave = []
         should_squash = True
 
-        for l in reversed(layers):
-            if l == from_layer:
+        for reversed_layer in reversed(layers):
+            if reversed_layer == from_layer:
                 should_squash = False
 
             if should_squash:
-                to_squash.append(l)
+                to_squash.append(reversed_layer)
             else:
-                to_leave.append(l)
+                to_leave.append(reversed_layer)
 
         to_squash.reverse()
         to_leave.reverse()
 
         return to_squash, to_leave
 
     def _extract_tar(self, fileobj, directory):
-        with tarfile.open(fileobj=fileobj, mode='r|') as tar:
+        with tarfile.open(fileobj=fileobj, mode="r|") as tar:
             tar.extractall(path=directory)
 
     def _save_image(self, image_id, directory):
-        """ Saves the image as a tar archive under specified name """
+        """Saves the image as a tar archive under specified name"""
 
         for x in [0, 1, 2]:
-            self.log.info("Saving image %s to %s directory..." %
-                          (image_id, directory))
+            self.log.info("Saving image %s to %s directory..." % (image_id, directory))
             self.log.debug("Try #%s..." % (x + 1))
 
             try:
                 image = self.docker.get_image(image_id)
 
-                if docker.version_info[0] < 3:
+                if int(docker.__version__.split(".")[0]) < 3:
                     # Docker library prior to 3.0.0 returned the requests
                     # object directly which cold be used to read from
                     self.log.debug(
-                        "Extracting image using HTTPResponse object directly")
+                        "Extracting image using HTTPResponse object directly"
+                    )
                     self._extract_tar(image, directory)
                 else:
                     # Docker library >=3.0.0 returns iterator over raw data
-                    self.log.debug(
-                        "Extracting image using iterator over raw data")
+                    self.log.debug("Extracting image using iterator over raw data")
 
                     fd_r, fd_w = os.pipe()
 
-                    r = os.fdopen(fd_r, 'rb')
-                    w = os.fdopen(fd_w, 'wb')
+                    r = os.fdopen(fd_r, "rb")
+                    w = os.fdopen(fd_w, "wb")
 
                     extracter = threading.Thread(
-                        target=self._extract_tar, args=(r, directory))
+                        target=self._extract_tar, args=(r, directory)
+                    )
                     extracter.start()
 
                     for chunk in image:
                         w.write(chunk)
 
                     w.flush()
                     w.close()
@@ -383,113 +405,114 @@
                     extracter.join()
                     r.close()
                 self.log.info("Image saved!")
                 return True
             except Exception as e:
                 self.log.exception(e)
                 self.log.warning(
-                    "An error occured while saving the %s image, retrying..." % image_id)
+                    "An error occured while saving the %s image, retrying..." % image_id
+                )
 
         raise SquashError("Couldn't save %s image!" % image_id)
 
     def _unpack(self, tar_file, directory):
-        """ Unpacks tar archive to selected directory """
+        """Unpacks tar archive to selected directory"""
 
-        self.log.info("Unpacking %s tar file to %s directory" %
-                      (tar_file, directory))
+        self.log.info("Unpacking %s tar file to %s directory" % (tar_file, directory))
 
-        with tarfile.open(tar_file, 'r') as tar:
+        with tarfile.open(tar_file, "r") as tar:
             tar.extractall(path=directory)
 
         self.log.info("Archive unpacked!")
 
     def _read_layers(self, layers, image_id):
-        """ Reads the JSON metadata for specified layer / image id """
+        """Reads the JSON metadata for specified layer / image id"""
 
         for layer in self.docker.history(image_id):
-            layers.append(layer['Id'])
+            layers.append(layer["Id"])
 
     def _parse_image_name(self, image):
         """
         Parses the provided image name and splits it in the
         name and tag part, if possible. If no tag is provided
         'latest' is used.
         """
-        if ':' in image and '/' not in image.split(':')[-1]:
-            image_tag = image.split(':')[-1]
-            image_name = image[:-(len(image_tag) + 1)]
+        if ":" in image and "/" not in image.split(":")[-1]:
+            image_tag = image.split(":")[-1]
+            image_name = image[: -(len(image_tag) + 1)]
         else:
             image_tag = "latest"
             image_name = image
 
         return (image_name, image_tag)
 
     def _dump_json(self, data, new_line=False):
         """
         Helper function to marshal object into JSON string.
         Additionally a sha256sum of the created JSON string is generated.
         """
 
         # We do not want any spaces between keys and values in JSON
-        json_data = json.dumps(data, separators=(',', ':'))
+        json_data = json.dumps(data, separators=(",", ":"))
 
         if new_line:
             json_data = "%s\n" % json_data
 
         # Generate sha256sum of the JSON data, may be handy
-        sha = hashlib.sha256(json_data.encode('utf-8')).hexdigest()
+        sha = hashlib.sha256(json_data.encode("utf-8")).hexdigest()
 
         return json_data, sha
 
     def _generate_repositories_json(self, repositories_file, image_id, name, tag):
         if not image_id:
             raise SquashError("Provided image id cannot be null")
 
-        if name == tag == None:
+        if name is None and tag is None:
             self.log.debug(
-                "No name and tag provided for the image, skipping generating repositories file")
+                "No name and tag provided for the image, skipping generating repositories file"
+            )
             return
 
         repos = {}
         repos[name] = {}
         repos[name][tag] = image_id
 
-        data = json.dumps(repos, separators=(',', ':'))
+        data = json.dumps(repos, separators=(",", ":"))
 
-        with open(repositories_file, 'w') as f:
+        with open(repositories_file, "w") as f:
             f.write(data)
             f.write("\n")
 
     def _write_version_file(self, squashed_dir):
         version_file = os.path.join(squashed_dir, "VERSION")
 
-        with open(version_file, 'w') as f:
+        with open(version_file, "w") as f:
             f.write("1.0")
 
     def _write_json_metadata(self, metadata, metadata_file):
-        with open(metadata_file, 'w') as f:
+        with open(metadata_file, "w") as f:
             f.write(metadata)
 
     def _read_old_metadata(self, old_json_file):
         self.log.debug("Reading JSON metadata file '%s'..." % old_json_file)
 
         # Read original metadata
-        with open(old_json_file, 'r') as f:
+        with open(old_json_file, "r") as f:
             metadata = json.load(f)
 
         return metadata
 
     def _move_layers(self, layers, src, dest):
         """
         This moves all the layers that should be copied as-is.
         In other words - all layers that are not meant to be squashed will be
         moved from the old image to the new image untouched.
         """
         for layer in layers:
-            layer_id = layer.replace('sha256:', '')
+            layer_id = layer.replace("sha256:", "")
 
             self.log.debug("Moving unmodified layer '%s'..." % layer_id)
             shutil.move(os.path.join(src, layer_id), dest)
 
     def _file_should_be_skipped(self, file_name, file_paths):
         # file_paths is now array of array with files to be skipped.
         # First level are layers, second are files in these layers.
@@ -510,19 +533,18 @@
 
         Docker marker files are files taht have the .wh. prefix in the name.
         These files mark the corresponding file to be removed (hidden) when
         we start a container from the image.
         """
         marker_files = {}
 
-        self.log.debug(
-            "Searching for marker files in '%s' archive..." % tar.name)
+        self.log.debug("Searching for marker files in '%s' archive..." % tar.name)
 
         for member in members:
-            if '.wh.' in member.name:
+            if ".wh." in member.name:
                 self.log.debug("Found '%s' marker file" % member.name)
                 marker_files[member] = tar.extractfile(member)
 
         self.log.debug("Done, found %s files" % len(marker_files))
 
         return marker_files
 
@@ -530,114 +552,129 @@
         """
         This method is responsible for adding back all markers that were not
         added to the squashed layer AND files they refer to can be found in layers
         we do not squash.
         """
 
         if markers:
-            self.log.debug("Marker files to add: %s" %
-                           [o.name for o in markers.keys()])
+            self.log.debug("Marker files to add: %s" % [o.name for o in markers.keys()])
         else:
             # No marker files to add
             return
 
         # https://github.com/goldmann/docker-squash/issues/108
         # Some tar archives do have the filenames prefixed with './'
         # which does not have any effect when we unpack the tar achive,
         # but when processing tar content - we see this.
         tar_files = [self._normalize_path(x) for x in tar.getnames()]
 
-        for marker, marker_file in six.iteritems(markers):
-            actual_file = marker.name.replace('.wh.', '')
+        for marker, marker_file in markers.items():
+            actual_file = marker.name.replace(".wh.", "")
             normalized_file = self._normalize_path(actual_file)
 
             should_be_added_back = False
 
             if self._file_should_be_skipped(normalized_file, added_symlinks):
                 self.log.debug(
-                    "Skipping '%s' marker file, this file is on a symlink path" % normalized_file)
+                    "Skipping '%s' marker file, this file is on a symlink path"
+                    % normalized_file
+                )
                 continue
 
             if normalized_file in tar_files:
                 self.log.debug(
-                    "Skipping '%s' marker file, this file was added earlier for some reason..." % normalized_file)
+                    "Skipping '%s' marker file, this file was added earlier for some reason..."
+                    % normalized_file
+                )
                 continue
 
             if files_in_layers:
                 for files in files_in_layers.values():
                     if normalized_file in files:
                         should_be_added_back = True
                         break
             else:
                 # There are no previous layers, so we need to add it back
                 # In fact this shouldn't happen since having a marker file
                 # where there is no previous layer does not make sense.
                 should_be_added_back = True
 
             if should_be_added_back:
-                self.log.debug(
-                    "Adding '%s' marker file back..." % marker.name)
+                self.log.debug("Adding '%s' marker file back..." % marker.name)
                 # Marker files on AUFS are hardlinks, we need to create
                 # regular files, therefore we need to recreate the tarinfo
                 # object
                 tar.addfile(tarfile.TarInfo(name=marker.name), marker_file)
                 # Add the file name to the list too to avoid re-reading all files
                 # in tar archive
                 tar_files.append(normalized_file)
             else:
-                self.log.debug(
-                    "Skipping '%s' marker file..." % marker.name)
+                self.log.debug("Skipping '%s' marker file..." % marker.name)
 
     def _normalize_path(self, path):
         return os.path.normpath(os.path.join("/", path))
 
     def _add_hardlinks(self, squashed_tar, squashed_files, to_skip, skipped_hard_links):
         for layer, hardlinks_in_layer in enumerate(skipped_hard_links):
             # We need to start from 1, that's why we bump it here
             current_layer = layer + 1
-            for member in six.itervalues(hardlinks_in_layer):
+            for member in hardlinks_in_layer.values():
                 normalized_name = self._normalize_path(member.name)
                 normalized_linkname = self._normalize_path(member.linkname)
 
                 # Find out if the name is on the list of files to skip - if it is - get the layer number
                 # where it was found
-                layer_skip_name = self._file_should_be_skipped(
-                    normalized_name, to_skip)
+                layer_skip_name = self._file_should_be_skipped(normalized_name, to_skip)
                 # Do the same for linkname
                 layer_skip_linkname = self._file_should_be_skipped(
-                    normalized_linkname, to_skip)
+                    normalized_linkname, to_skip
+                )
 
                 # We need to check if we should skip adding back the hard link
                 # This can happen in the following situations:
                 # 1. hard link is on the list of files to skip
                 # 2. hard link target is on the list of files to skip
                 # 3. hard link is already in squashed files
                 # 4. hard link target is NOT in already squashed files
-                if layer_skip_name and current_layer > layer_skip_name or layer_skip_linkname and current_layer > layer_skip_linkname or normalized_name in squashed_files or normalized_linkname not in squashed_files:
-                    self.log.debug("Found a hard link '%s' to a file which is marked to be skipped: '%s', skipping link too" % (
-                        normalized_name, normalized_linkname))
+                if (
+                    layer_skip_name
+                    and current_layer > layer_skip_name
+                    or layer_skip_linkname
+                    and current_layer > layer_skip_linkname
+                    or normalized_name in squashed_files
+                    or normalized_linkname not in squashed_files
+                ):
+                    self.log.debug(
+                        "Found a hard link '%s' to a file which is marked to be skipped: '%s', skipping link too"
+                        % (normalized_name, normalized_linkname)
+                    )
                 else:
                     if self.debug:
-                        self.log.debug("Adding hard link '%s' pointing to '%s' back..." % (
-                            normalized_name, normalized_linkname))
+                        self.log.debug(
+                            "Adding hard link '%s' pointing to '%s' back..."
+                            % (normalized_name, normalized_linkname)
+                        )
 
                     squashed_files.append(normalized_name)
                     squashed_tar.addfile(member)
 
     def _add_file(self, member, content, squashed_tar, squashed_files, to_skip):
         normalized_name = self._normalize_path(member.name)
 
         if normalized_name in squashed_files:
             self.log.debug(
-                "Skipping file '%s' because it is already squashed" % normalized_name)
+                "Skipping file '%s' because it is already squashed" % normalized_name
+            )
             return
 
         if self._file_should_be_skipped(normalized_name, to_skip):
             self.log.debug(
-                "Skipping '%s' file because it's on the list to skip files" % normalized_name)
+                "Skipping '%s' file because it's on the list to skip files"
+                % normalized_name
+            )
             return
 
         if content:
             squashed_tar.addfile(member, content)
         else:
             # Special case: other(?) files, we skip the file
             # itself
@@ -647,50 +684,62 @@
         squashed_files.append(normalized_name)
 
     def _add_symlinks(self, squashed_tar, squashed_files, to_skip, skipped_sym_links):
         added_symlinks = []
         for layer, symlinks_in_layer in enumerate(skipped_sym_links):
             # We need to start from 1, that's why we bump it here
             current_layer = layer + 1
-            for member in six.itervalues(symlinks_in_layer):
-
+            for member in symlinks_in_layer.values():
                 # Handling symlinks. This is similar to hard links with one
                 # difference. Sometimes we do want to have broken symlinks
-                # be addedeither case because these can point to locations
-                # that will become avaialble after adding volumes for example.
+                # be added because these can point to locations
+                # that will become available after adding volumes for example.
                 normalized_name = self._normalize_path(member.name)
                 normalized_linkname = self._normalize_path(member.linkname)
 
                 # File is already in squashed files, skipping
                 if normalized_name in squashed_files:
                     self.log.debug(
-                        "Found a symbolic link '%s' which is already squashed, skipping" % (normalized_name))
+                        "Found a symbolic link '%s' which is already squashed, skipping"
+                        % (normalized_name)
+                    )
                     continue
 
                 if self._file_should_be_skipped(normalized_name, added_symlinks):
                     self.log.debug(
-                        "Found a symbolic link '%s' which is on a path to previously squashed symlink, skipping" % (normalized_name))
+                        "Found a symbolic link '%s' which is on a path to previously squashed symlink, skipping"
+                        % (normalized_name)
+                    )
                     continue
                 # Find out if the name is on the list of files to skip - if it is - get the layer number
                 # where it was found
-                layer_skip_name = self._file_should_be_skipped(
-                    normalized_name, to_skip)
+                layer_skip_name = self._file_should_be_skipped(normalized_name, to_skip)
                 # Do the same for linkname
                 layer_skip_linkname = self._file_should_be_skipped(
-                    normalized_linkname, to_skip)
+                    normalized_linkname, to_skip
+                )
 
                 # If name or linkname was found in the lists of files to be
                 # skipped or it's not found in the squashed files
-                if layer_skip_name and current_layer > layer_skip_name or layer_skip_linkname and current_layer > layer_skip_linkname:
-                    self.log.debug("Found a symbolic link '%s' to a file which is marked to be skipped: '%s', skipping link too" % (
-                        normalized_name, normalized_linkname))
+                if (
+                    layer_skip_name
+                    and current_layer > layer_skip_name
+                    or layer_skip_linkname
+                    and current_layer > layer_skip_linkname
+                ):
+                    self.log.debug(
+                        "Found a symbolic link '%s' to a file which is marked to be skipped: '%s', skipping link too"
+                        % (normalized_name, normalized_linkname)
+                    )
                 else:
                     if self.debug:
-                        self.log.debug("Adding symbolic link '%s' pointing to '%s' back..." % (
-                            normalized_name, normalized_linkname))
+                        self.log.debug(
+                            "Adding symbolic link '%s' pointing to '%s' back..."
+                            % (normalized_name, normalized_linkname)
+                        )
 
                     added_symlinks.append([normalized_name])
 
                     squashed_files.append(normalized_name)
                     squashed_tar.addfile(member)
 
         return added_symlinks
@@ -700,170 +749,198 @@
 
         # Reverse the layers to squash - we begin with the newest one
         # to make the tar lighter
         layers_to_squash.reverse()
 
         # Find all files in layers that we don't squash
         files_in_layers_to_move = self._files_in_layers(
-            layers_to_move, self.old_image_dir)
+            layers_to_move, self.old_image_dir
+        )
 
-        with tarfile.open(self.squashed_tar, 'w', format=tarfile.PAX_FORMAT) as squashed_tar:
+        with tarfile.open(
+            self.squashed_tar, "w", format=tarfile.PAX_FORMAT
+        ) as squashed_tar:
             to_skip = []
             skipped_markers = {}
             skipped_hard_links = []
             skipped_sym_links = []
             skipped_files = []
             # List of filenames in the squashed archive
             squashed_files = []
             # List of opaque directories in the image
             opaque_dirs = []
+            reading_layers: List[tarfile.TarFile] = []
 
             for layer_id in layers_to_squash:
-                layer_tar_file = os.path.join(
-                    self.old_image_dir, layer_id, "layer.tar")
+                layer_tar_file = os.path.join(self.old_image_dir, layer_id, "layer.tar")
 
                 self.log.info("Squashing file '%s'..." % layer_tar_file)
 
                 # Open the exiting layer to squash
-                with tarfile.open(layer_tar_file, 'r', format=tarfile.PAX_FORMAT) as layer_tar:
-                    # Find all marker files for all layers
-                    # We need the list of marker files upfront, so we can
-                    # skip unnecessary files
-                    members = layer_tar.getmembers()
-                    markers = self._marker_files(layer_tar, members)
-
-                    skipped_sym_link_files = {}
-                    skipped_hard_link_files = {}
-                    skipped_files_in_layer = {}
-
-                    files_to_skip = []
-                    # List of opaque directories found in this layer
-                    layer_opaque_dirs = []
-
-                    # Add it as early as possible, we will be populating
-                    # 'skipped_sym_link_files' array later
-                    skipped_sym_links.append(skipped_sym_link_files)
-
-                    # Add it as early as possible, we will be populating
-                    # 'files_to_skip' array later
-                    to_skip.append(files_to_skip)
-
-                    # Iterate over marker files found for this particular
-                    # layer and if a file in the squashed layers file corresponding
-                    # to the marker file is found, then skip both files
-                    for marker, marker_file in six.iteritems(markers):
-                        # We have a opaque directory marker file
-                        # https://github.com/opencontainers/image-spec/blob/master/layer.md#opaque-whiteout
-                        if marker.name.endswith('.wh..wh..opq'):
-                            opaque_dir = os.path.dirname(marker.name)
-
-                            self.log.debug(
-                                "Found opaque directory: '%s'" % opaque_dir)
-
-                            layer_opaque_dirs.append(opaque_dir)
-                        else:
-                            files_to_skip.append(
-                                self._normalize_path(marker.name.replace('.wh.', '')))
-
-                            skipped_markers[marker] = marker_file
-
-                    # Copy all the files to the new tar
-                    for member in members:
-                        normalized_name = self._normalize_path(member.name)
-
-                        if self._is_in_opaque_dir(member, opaque_dirs):
-                            self.log.debug(
-                                "Skipping file '%s' because it is in an opaque directory" % normalized_name)
-                            continue
-
-                        # Skip all symlinks, we'll investigate them later
-                        if member.issym():
-                            skipped_sym_link_files[normalized_name] = member
-                            continue
-
-                        if member in six.iterkeys(skipped_markers):
-                            self.log.debug(
-                                "Skipping '%s' marker file, at the end of squashing we'll see if it's necessary to add it back" % normalized_name)
-                            continue
-
-                        if self._file_should_be_skipped(normalized_name, skipped_sym_links):
-                            self.log.debug(
-                                "Skipping '%s' file because it's on a symlink path, at the end of squashing we'll see if it's necessary to add it back" % normalized_name)
-
-                            if member.isfile():
-                                f = (member, layer_tar.extractfile(member))
-                            else:
-                                f = (member, None)
-
-                            skipped_files_in_layer[normalized_name] = f
-                            continue
-
-                        # Skip files that are marked to be skipped
-                        if self._file_should_be_skipped(normalized_name, to_skip):
-                            self.log.debug(
-                                "Skipping '%s' file because it's on the list to skip files" % normalized_name)
-                            continue
-
-                        # Check if file is already added to the archive
-                        if normalized_name in squashed_files:
-                            # File already exist in the squashed archive, skip it because
-                            # file want to add is older than the one already in the archive.
-                            # This is true because we do reverse squashing - from
-                            # newer to older layer
-                            self.log.debug(
-                                "Skipping '%s' file because it's older than file already added to the archive" % normalized_name)
-                            continue
-
-                        # Hard links are processed after everything else
-                        if member.islnk():
-                            skipped_hard_link_files[normalized_name] = member
-                            continue
-
-                        content = None
+                layer_tar: tarfile.TarFile = tarfile.open(
+                    layer_tar_file, "r", format=tarfile.PAX_FORMAT
+                )
+                reading_layers.append(layer_tar)
+                # Find all marker files for all layers
+                # We need the list of marker files upfront, so we can
+                # skip unnecessary files
+                members = layer_tar.getmembers()
+                markers = self._marker_files(layer_tar, members)
+
+                skipped_sym_link_files = {}
+                skipped_hard_link_files = {}
+                skipped_files_in_layer = {}
+
+                files_to_skip = []
+                # List of opaque directories found in this layer
+                layer_opaque_dirs = []
+
+                # Add it as early as possible, we will be populating
+                # 'skipped_sym_link_files' array later
+                skipped_sym_links.append(skipped_sym_link_files)
+
+                # Add it as early as possible, we will be populating
+                # 'files_to_skip' array later
+                to_skip.append(files_to_skip)
+
+                # Iterate over marker files found for this particular
+                # layer and if a file in the squashed layers file corresponding
+                # to the marker file is found, then skip both files
+                for marker, marker_file in markers.items():
+                    # We have a opaque directory marker file
+                    # https://github.com/opencontainers/image-spec/blob/master/layer.md#opaque-whiteout
+                    if marker.name.endswith(".wh..wh..opq"):
+                        opaque_dir = os.path.dirname(marker.name)
+
+                        self.log.debug("Found opaque directory: '%s'" % opaque_dir)
+
+                        layer_opaque_dirs.append(opaque_dir)
+                    else:
+                        files_to_skip.append(
+                            self._normalize_path(marker.name.replace(".wh.", ""))
+                        )
+                        skipped_markers[marker] = marker_file
+
+                # Copy all the files to the new tar
+                for member in members:
+                    normalized_name = self._normalize_path(member.name)
+
+                    if self._is_in_opaque_dir(member, opaque_dirs):
+                        self.log.debug(
+                            "Skipping file '%s' because it is in an opaque directory"
+                            % normalized_name
+                        )
+                        continue
+
+                    # Skip all symlinks, we'll investigate them later
+                    if member.issym():
+                        skipped_sym_link_files[normalized_name] = member
+                        continue
+
+                    if member in skipped_markers.keys():
+                        self.log.debug(
+                            "Skipping '%s' marker file, at the end of squashing we'll see if it's necessary to add it back"
+                            % normalized_name
+                        )
+                        continue
+
+                    if self._file_should_be_skipped(normalized_name, skipped_sym_links):
+                        self.log.debug(
+                            "Skipping '%s' file because it's on a symlink path, at the end of squashing we'll see if it's necessary to add it back"
+                            % normalized_name
+                        )
 
                         if member.isfile():
-                            content = layer_tar.extractfile(member)
-
-                        self._add_file(member, content,
-                                       squashed_tar, squashed_files, to_skip)
+                            f = (member, layer_tar.extractfile(member))
+                        else:
+                            f = (member, None)
 
-                    skipped_hard_links.append(skipped_hard_link_files)
-                    skipped_files.append(skipped_files_in_layer)
-                    opaque_dirs += layer_opaque_dirs
+                        skipped_files_in_layer[normalized_name] = f
+                        continue
 
-            self._add_hardlinks(squashed_tar, squashed_files,
-                                to_skip, skipped_hard_links)
+                    # Skip files that are marked to be skipped
+                    if self._file_should_be_skipped(normalized_name, to_skip):
+                        self.log.debug(
+                            "Skipping '%s' file because it's on the list to skip files"
+                            % normalized_name
+                        )
+                        continue
+
+                    # Check if file is already added to the archive
+                    if normalized_name in squashed_files:
+                        # File already exist in the squashed archive, skip it because
+                        # file want to add is older than the one already in the archive.
+                        # This is true because we do reverse squashing - from
+                        # newer to older layer
+                        self.log.debug(
+                            "Skipping '%s' file because it's older than file already added to the archive"
+                            % normalized_name
+                        )
+                        continue
+
+                    # Hard links are processed after everything else
+                    if member.islnk():
+                        skipped_hard_link_files[normalized_name] = member
+                        continue
+
+                    content = None
+
+                    if member.isfile():
+                        content = layer_tar.extractfile(member)
+
+                    self._add_file(
+                        member, content, squashed_tar, squashed_files, to_skip
+                    )
+
+                skipped_hard_links.append(skipped_hard_link_files)
+                skipped_files.append(skipped_files_in_layer)
+                opaque_dirs += layer_opaque_dirs
+
+            self._add_hardlinks(
+                squashed_tar, squashed_files, to_skip, skipped_hard_links
+            )
             added_symlinks = self._add_symlinks(
-                squashed_tar, squashed_files, to_skip, skipped_sym_links)
+                squashed_tar, squashed_files, to_skip, skipped_sym_links
+            )
 
             for layer in skipped_files:
-                for member, content in six.itervalues(layer):
-                    self._add_file(member, content, squashed_tar,
-                                   squashed_files, added_symlinks)
+                for member, content in layer.values():
+                    self._add_file(
+                        member, content, squashed_tar, squashed_files, added_symlinks
+                    )
 
             if files_in_layers_to_move:
                 self._reduce(skipped_markers)
 
-                self._add_markers(skipped_markers, squashed_tar,
-                                  files_in_layers_to_move, added_symlinks)
-
+                self._add_markers(
+                    skipped_markers,
+                    squashed_tar,
+                    files_in_layers_to_move,
+                    added_symlinks,
+                )
+
+            tar: tarfile.TarFile
+            for tar in reading_layers:
+                tar.close()
         self.log.info("Squashing finished!")
 
     def _is_in_opaque_dir(self, member, dirs):
         """
         If the member we investigate is an opaque directory
         or if the member is located inside of the opaque directory,
         we copy these files as-is. Any other layer that has content
         on the opaque directory will be ignored!
         """
 
         for opaque_dir in dirs:
             if member.name == opaque_dir or member.name.startswith("%s/" % opaque_dir):
-                self.log.debug("Member '%s' found to be part of opaque directory '%s'" % (
-                    member.name, opaque_dir))
+                self.log.debug(
+                    "Member '%s' found to be part of opaque directory '%s'"
+                    % (member.name, opaque_dir)
+                )
                 return True
 
         return False
 
     def _reduce(self, markers):
         """
         This function is responsible for reducing marker files
@@ -885,32 +962,38 @@
             markers (dict): Dictionary of markers scheduled to be added.
         """
 
         self.log.debug("Reducing marker files to be added back...")
 
         # Prepare a list of files (or directories) based on the marker
         # files scheduled to be added
-        marked_files = list(map(lambda x: self._normalize_path(
-            x.name.replace('.wh.', '')), markers.keys()))
+        marked_files = list(
+            map(
+                lambda x: self._normalize_path(x.name.replace(".wh.", "")),
+                markers.keys(),
+            )
+        )
 
         # List of markers that should be not added back to tar file
         to_remove = []
 
         for marker in markers.keys():
-            self.log.debug(
-                "Investigating '{}' marker file".format(marker.name))
+            self.log.debug("Investigating '{}' marker file".format(marker.name))
 
-            path = self._normalize_path(marker.name.replace('.wh.', ''))
+            path = self._normalize_path(marker.name.replace(".wh.", ""))
             # Iterate over the path hierarchy, but starting with the
             # root directory. This will make it possible to remove
             # marker files based on the highest possible directory level
-            for directory in reversed(self._path_hierarchy(path)):
+            for directory in self._path_hierarchy(path):
                 if directory in marked_files:
                     self.log.debug(
-                        "Marker file '{}' is superseded by higher-level marker file: '{}'".format(marker.name, directory))
+                        "Marker file '{}' is superseded by higher-level marker file: '{}'".format(
+                            marker.name, directory
+                        )
+                    )
                     to_remove.append(marker)
                     break
 
         self.log.debug("Removing {} marker files".format(len(to_remove)))
 
         if to_remove:
             for marker in to_remove:
@@ -920,31 +1003,29 @@
         self.log.debug("Marker files reduced")
 
     def _path_hierarchy(self, path):
         """
         Creates a full hierarchy of directories for a given path.
 
         For a particular path, a list will be returned
-        containing paths from the path specified, through all levels
-        up to the root directory.
+        containing paths from the root directory, through all
+        levels up to the path specified.
 
         Example:
             Path '/opt/testing/some/dir/structure/file'
 
             will return:
 
-            ['/opt/testing/some/dir/structure', '/opt/testing/some/dir', '/opt/testing/some', '/opt/testing', '/opt', '/']
+            ['/', '/opt', '/opt/testing', '/opt/testing/some', '/opt/testing/some/dir', '/opt/testing/some/dir/structure']
         """
         if not path:
             raise SquashError("No path provided to create the hierarchy for")
 
-        hierarchy = []
-
-        dirname = os.path.dirname(path)
-
-        hierarchy.append(dirname)
+        if not isinstance(path, pathlib.PurePath):
+            path = pathlib.PurePath(path)
 
-        # If we are already at root level, stop
-        if dirname != '/':
-            hierarchy.extend(self._path_hierarchy(dirname))
+        if len(path.parts) == 1:
+            return path.parts
 
-        return hierarchy
+        return itertools.accumulate(
+            path.parts[:-1], func=lambda head, tail: str(path.__class__(head, tail))
+        )
```

### Comparing `docker-squash-1.0.9/docker_squash/lib/common.py` & `docker-squash-1.1.0/docker_squash/lib/common.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # -*- coding: utf-8 -*-
 
-import docker
 import os
+
+import docker
 import requests
 
 from docker_squash.errors import Error
 
 # First try to import Docker client using the API
 # available in version 2 of the library and fall
 # back to version 1
@@ -18,22 +19,26 @@
 
 
 def docker_client(log):
     log.debug("Preparing Docker client...")
 
     # Default timeout 10 minutes
     try:
-        timeout = int(os.getenv('DOCKER_TIMEOUT', 600))
-    except ValueError as e:
-        raise Error("Provided timeout value: %s cannot be parsed as integer, exiting." %
-                    os.getenv('DOCKER_TIMEOUT'))
+        timeout = int(os.getenv("DOCKER_TIMEOUT", 600))
+    except ValueError:
+        raise Error(
+            "Provided timeout value: %s cannot be parsed as integer, exiting."
+            % os.getenv("DOCKER_TIMEOUT")
+        )
 
     if not timeout > 0:
         raise Error(
-            "Provided timeout value needs to be greater than zero, currently: %s, exiting." % timeout)
+            "Provided timeout value needs to be greater than zero, currently: %s, exiting."
+            % timeout
+        )
 
     # backwards compat
     try:
         os.environ["DOCKER_HOST"] = os.environ["DOCKER_CONNECTION"]
         log.warn("DOCKER_CONNECTION is deprecated, please use DOCKER_HOST instead")
     except KeyError:
         pass
@@ -42,27 +47,30 @@
     params.update(docker.utils.kwargs_from_env())
     params["timeout"] = timeout
 
     try:
         client = APIClientClass(**params)
     except docker.errors.DockerException as e:
         log.error(
-            "Could not create Docker client, please make sure that you specified valid parameters in the 'DOCKER_HOST' environment variable.")
+            "Could not create Docker client, please make sure that you specified valid parameters in the 'DOCKER_HOST' environment variable."
+        )
         raise Error("Error while creating the Docker client: %s" % e)
 
     if client and valid_docker_connection(client):
         log.debug("Docker client ready")
         return client
     else:
         log.error(
-            "Could not connect to the Docker daemon, please make sure the Docker daemon is running.")
+            "Could not connect to the Docker daemon, please make sure the Docker daemon is running."
+        )
 
-        if os.environ.get('DOCKER_HOST'):
+        if os.environ.get("DOCKER_HOST"):
             log.error(
-                "If Docker daemon is running, please make sure that you specified valid parameters in the 'DOCKER_HOST' environment variable.")
+                "If Docker daemon is running, please make sure that you specified valid parameters in the 'DOCKER_HOST' environment variable."
+            )
 
         raise Error("Cannot connect to Docker daemon")
 
 
 def valid_docker_connection(client):
     try:
         return client.ping()
```

### Comparing `docker-squash-1.0.9/docker_squash/squash.py` & `docker-squash-1.1.0/docker_squash/squash.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,36 @@
 # -*- coding: utf-8 -*-
 
 import os
+from distutils.version import StrictVersion
 
 import docker
 
-from distutils.version import StrictVersion
-
+from docker_squash.errors import SquashError
+from docker_squash.lib import common
 from docker_squash.v1_image import V1Image
 from docker_squash.v2_image import V2Image
-from docker_squash.lib import common
-from docker_squash.errors import SquashError
 from docker_squash.version import version
 
 
 class Squash(object):
-
-    def __init__(self, log, image, docker=None, from_layer=None, tag=None, comment="", tmp_dir=None,
-                 output_path=None, load_image=True, development=False, cleanup=False):
+    def __init__(
+        self,
+        log,
+        image,
+        docker=None,
+        from_layer=None,
+        tag=None,
+        comment="",
+        tmp_dir=None,
+        output_path=None,
+        load_image=True,
+        development=False,
+        cleanup=False,
+    ):
         self.log = log
         self.docker = docker
         self.image = image
         self.from_layer = from_layer
         self.tag = tag
         self.comment = comment
         self.tmp_dir = tmp_dir
@@ -30,70 +40,93 @@
         self.cleanup = cleanup
 
         if not docker:
             self.docker = common.docker_client(self.log)
 
     def run(self):
         docker_version = self.docker.version()
-        self.log.info("docker-squash version %s, Docker %s, API %s..." %
-                      (version, docker_version['GitCommit'], docker_version['ApiVersion']))
+        self.log.info(
+            "docker-squash version %s, Docker %s, API %s..."
+            % (version, docker_version["Version"], docker_version["ApiVersion"])
+        )
 
         if self.image is None:
             raise SquashError("Image is not provided")
 
         if not (self.output_path or self.load_image):
             self.log.warning(
-                "No output path specified and loading into Docker is not selected either; squashed image would not accessible, proceeding with squashing doesn't make sense")
+                "No output path specified and loading into Docker is not selected either; squashed image would not accessible, proceeding with squashing doesn't make sense"
+            )
             return
 
         if self.output_path and os.path.exists(self.output_path):
             self.log.warning(
-                "Path '%s' specified as output path where the squashed image should be saved already exists, it'll be overriden" % self.output_path)
-
-        if StrictVersion(docker_version['ApiVersion']) >= StrictVersion("1.22"):
-            image = V2Image(self.log, self.docker, self.image,
-                            self.from_layer, self.tmp_dir, self.tag, self.comment)
+                "Path '%s' specified as output path where the squashed image should be saved already exists, it'll be overriden"
+                % self.output_path
+            )
+
+        if StrictVersion(docker_version["ApiVersion"]) >= StrictVersion("1.22"):
+            image = V2Image(
+                self.log,
+                self.docker,
+                self.image,
+                self.from_layer,
+                self.tmp_dir,
+                self.tag,
+                self.comment,
+            )
         else:
-            image = V1Image(self.log, self.docker, self.image,
-                            self.from_layer, self.tmp_dir, self.tag)
+            image = V1Image(
+                self.log,
+                self.docker,
+                self.image,
+                self.from_layer,
+                self.tmp_dir,
+                self.tag,
+            )
 
         self.log.info("Using %s image format" % image.FORMAT)
 
         try:
             return self.squash(image)
-        except:
+        except Exception:
             # https://github.com/goldmann/docker-scripts/issues/44
             # If development mode is not enabled, make sure we clean up the
             # temporary directory
             if not self.development:
                 image.cleanup()
 
             raise
 
     def _cleanup(self):
         try:
-            image_id = self.docker.inspect_image(self.image)['Id']
+            image_id = self.docker.inspect_image(self.image)["Id"]
         except docker.errors.APIError as ex:
             self.log.warning(
                 "Could not get the image ID for {} image: {}, skipping cleanup after squashing".format(
-                    self.image, str(ex)))
+                    self.image, str(ex)
+                )
+            )
             return
 
         self.log.info("Removing old {} image...".format(self.image))
 
         try:
             self.docker.remove_image(image_id, force=False, noprune=False)
             self.log.info("Image {} removed!".format(self.image))
         except docker.errors.APIError as ex:
             self.log.warning(
-                "Could not remove image {}: {}, skipping cleanup after squashing".format(self.image, str(ex)))
+                "Could not remove image {}: {}, skipping cleanup after squashing".format(
+                    self.image, str(ex)
+                )
+            )
 
     def squash(self, image):
         # Do the actual squashing
-        new_image_id=image.squash()
+        new_image_id = image.squash()
 
         self.log.info("New squashed image ID is %s" % new_image_id)
 
         if self.output_path:
             # Move the tar archive to the specified path
             image.export_tar_archive(self.output_path)
```

### Comparing `docker-squash-1.0.9/docker_squash/v1_image.py` & `docker-squash-1.1.0/docker_squash/v1_image.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,20 +3,21 @@
 import random
 import shutil
 
 from docker_squash.image import Image
 
 
 class V1Image(Image):
-    FORMAT = 'v1'
+    FORMAT = "v1"
 
     def _generate_image_id(self):
         while True:
             image_id = hashlib.sha256(
-                str(random.getrandbits(128)).encode('utf8')).hexdigest()
+                str(random.getrandbits(128)).encode("utf8")
+            ).hexdigest()
 
             try:
                 int(image_id[0:10])
             except ValueError:
                 # All good!
                 return image_id
 
@@ -28,62 +29,59 @@
 
     def _squash(self):
         # Prepare the directory
         os.makedirs(self.squashed_dir)
         self._squash_layers(self.layers_to_squash, self.layers_to_move)
         self._write_version_file(self.squashed_dir)
         # Move all the layers that should be untouched
-        self._move_layers(self.layers_to_move,
-                          self.old_image_dir, self.new_image_dir)
+        self._move_layers(self.layers_to_move, self.old_image_dir, self.new_image_dir)
 
-        config_file = os.path.join(
-            self.old_image_dir, self.old_image_id, "json")
+        config_file = os.path.join(self.old_image_dir, self.old_image_id, "json")
 
-        image_id = self._update_squashed_layer_metadata(
-            config_file, self.squashed_dir)
-        shutil.move(self.squashed_dir, os.path.join(
-            self.new_image_dir, image_id))
+        image_id = self._update_squashed_layer_metadata(config_file, self.squashed_dir)
+        shutil.move(self.squashed_dir, os.path.join(self.new_image_dir, image_id))
         repositories_file = os.path.join(self.new_image_dir, "repositories")
         self._generate_repositories_json(
-            repositories_file, image_id, self.image_name, self.image_tag)
+            repositories_file, image_id, self.image_name, self.image_tag
+        )
 
         return image_id
 
     def _update_squashed_layer_metadata(self, old_json_file, squashed_dir):
         image_id = self._generate_image_id()
 
         metadata = self._read_old_metadata(old_json_file)
 
         # Modify common metadata fields
         if self.squash_id:
-            metadata['config']['Image'] = self.squash_id
+            metadata["config"]["Image"] = self.squash_id
         else:
-            metadata['config'].pop('Image', None)
+            metadata["config"].pop("Image", None)
 
-        if 'parent_id' in metadata and self.squash_id:
-            metadata['parent_id'] = "sha256:%s" % self.squash_id
+        if "parent_id" in metadata and self.squash_id:
+            metadata["parent_id"] = "sha256:%s" % self.squash_id
         else:
-            metadata.pop('parent_id', None)
+            metadata.pop("parent_id", None)
 
-        metadata.pop('layer_id', None)
+        metadata.pop("layer_id", None)
 
-        metadata['created'] = self.date
+        metadata["created"] = self.date
 
         # Remove unnecessary fields
-        del metadata['container_config']
-        del metadata['container']
-        del metadata['config']['Hostname']
+        del metadata["container_config"]
+        del metadata["container"]
+        del metadata["config"]["Hostname"]
 
         if self.squash_id:
-            metadata['parent'] = self.squash_id
+            metadata["parent"] = self.squash_id
         else:
-            metadata.pop('parent', None)
+            metadata.pop("parent", None)
 
-        metadata['id'] = image_id
-        metadata['Size'] = os.path.getsize(
-            os.path.join(squashed_dir, "layer.tar"))
+        metadata["id"] = image_id
+        metadata["Size"] = os.path.getsize(os.path.join(squashed_dir, "layer.tar"))
         json_metadata = self._dump_json(metadata)[0]
 
         self._write_json_metadata(
-            "%s" % json_metadata, os.path.join(squashed_dir, "json"))
+            "%s" % json_metadata, os.path.join(squashed_dir, "json")
+        )
 
         return image_id
```

### Comparing `docker-squash-1.0.9/docker_squash/v2_image.py` & `docker-squash-1.1.0/docker_squash/v2_image.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,47 +1,48 @@
-
 import hashlib
 import json
 import os
 import shutil
-
 from collections import OrderedDict
+
 from docker_squash.image import Image
 
 
 class V2Image(Image):
-    FORMAT = 'v2'
+    FORMAT = "v2"
 
     def _before_squashing(self):
         super(V2Image, self)._before_squashing()
 
         # Read old image manifest file
         self.old_image_manifest = self._read_json_file(
-            os.path.join(self.old_image_dir, "manifest.json"))[0]
+            os.path.join(self.old_image_dir, "manifest.json")
+        )[0]
 
         # Read old image config file
-        self.old_image_config = self._read_json_file(os.path.join(
-            self.old_image_dir, self.old_image_manifest['Config']))
+        self.old_image_config = self._read_json_file(
+            os.path.join(self.old_image_dir, self.old_image_manifest["Config"])
+        )
 
         # Read layer paths inside of the tar archive
         # We split it into layers that needs to be squashed
         # and layers that needs to be moved as-is
         self.layer_paths_to_squash, self.layer_paths_to_move = self._read_layer_paths(
-            self.old_image_config, self.old_image_manifest, self.layers_to_move)
+            self.old_image_config, self.old_image_manifest, self.layers_to_move
+        )
 
         if self.layer_paths_to_move:
             self.squash_id = self.layer_paths_to_move[-1]
 
     def _squash(self):
         if self.layer_paths_to_squash:
             # Prepare the directory
             os.makedirs(self.squashed_dir)
             # Merge data layers
-            self._squash_layers(self.layer_paths_to_squash,
-                                self.layer_paths_to_move)
+            self._squash_layers(self.layer_paths_to_squash, self.layer_paths_to_move)
 
         self.diff_ids = self._generate_diff_ids()
         self.chain_ids = self._generate_chain_ids(self.diff_ids)
 
         metadata = self._generate_image_metadata()
         image_id = self._write_image_metadata(metadata)
 
@@ -49,48 +50,57 @@
 
         if self.layer_paths_to_squash:
             # Compute layer id to use to name the directory where
             # we store the layer data inside of the tar archive
             layer_path_id = self._generate_squashed_layer_path_id()
 
             metadata = self._generate_last_layer_metadata(
-                layer_path_id, self.layer_paths_to_squash[0])
+                layer_path_id, self.layer_paths_to_squash[0]
+            )
             self._write_squashed_layer_metadata(metadata)
 
             # Write version file to the squashed layer
             # Even Docker doesn't know why it's needed...
             self._write_version_file(self.squashed_dir)
 
             # Move the temporary squashed layer directory to the correct one
-            shutil.move(self.squashed_dir, os.path.join(
-                self.new_image_dir, layer_path_id))
+            shutil.move(
+                self.squashed_dir, os.path.join(self.new_image_dir, layer_path_id)
+            )
 
         manifest = self._generate_manifest_metadata(
-            image_id, self.image_name, self.image_tag, self.old_image_manifest, self.layer_paths_to_move, layer_path_id)
+            image_id,
+            self.image_name,
+            self.image_tag,
+            self.old_image_manifest,
+            self.layer_paths_to_move,
+            layer_path_id,
+        )
 
         self._write_manifest_metadata(manifest)
 
         repository_image_id = manifest[0]["Layers"][-1].split("/")[0]
 
         # Move all the layers that should be untouched
-        self._move_layers(self.layer_paths_to_move,
-                          self.old_image_dir, self.new_image_dir)
+        self._move_layers(
+            self.layer_paths_to_move, self.old_image_dir, self.new_image_dir
+        )
 
         repositories_file = os.path.join(self.new_image_dir, "repositories")
         self._generate_repositories_json(
-            repositories_file, repository_image_id, self.image_name, self.image_tag)
+            repositories_file, repository_image_id, self.image_name, self.image_tag
+        )
 
         return image_id
 
     def _write_image_metadata(self, metadata):
         # Create JSON from the metadata
         # Docker adds new line at the end
         json_metadata, image_id = self._dump_json(metadata, True)
-        image_metadata_file = os.path.join(
-            self.new_image_dir, "%s.json" % image_id)
+        image_metadata_file = os.path.join(self.new_image_dir, "%s.json" % image_id)
 
         self._write_json_metadata(json_metadata, image_metadata_file)
 
         return image_id
 
     def _write_squashed_layer_metadata(self, metadata):
         layer_metadata_file = os.path.join(self.squashed_dir, "json")
@@ -100,35 +110,42 @@
 
     def _write_manifest_metadata(self, manifest):
         manifest_file = os.path.join(self.new_image_dir, "manifest.json")
         json_manifest = self._dump_json(manifest, True)[0]
 
         self._write_json_metadata(json_manifest, manifest_file)
 
-    def _generate_manifest_metadata(self, image_id, image_name, image_tag, old_image_manifest, layer_paths_to_move, layer_path_id=None):
+    def _generate_manifest_metadata(
+        self,
+        image_id,
+        image_name,
+        image_tag,
+        old_image_manifest,
+        layer_paths_to_move,
+        layer_path_id=None,
+    ):
         manifest = OrderedDict()
-        manifest['Config'] = "%s.json" % image_id
+        manifest["Config"] = "%s.json" % image_id
 
         if image_name and image_tag:
-            manifest['RepoTags'] = ["%s:%s" % (image_name, image_tag)]
+            manifest["RepoTags"] = ["%s:%s" % (image_name, image_tag)]
 
-        manifest['Layers'] = old_image_manifest[
-            'Layers'][:len(layer_paths_to_move)]
+        manifest["Layers"] = old_image_manifest["Layers"][: len(layer_paths_to_move)]
 
         if layer_path_id:
-            manifest['Layers'].append("%s/layer.tar" % layer_path_id)
+            manifest["Layers"].append("%s/layer.tar" % layer_path_id)
 
         return [manifest]
 
     def _read_json_file(self, json_file):
-        """ Helper function to read JSON file as OrderedDict """
+        """Helper function to read JSON file as OrderedDict"""
 
         self.log.debug("Reading '%s' JSON file..." % json_file)
 
-        with open(json_file, 'r') as f:
+        with open(json_file, "r") as f:
             return json.load(f, object_pairs_hook=OrderedDict)
 
     def _read_layer_paths(self, old_image_config, old_image_manifest, layers_to_move):
         """
         In case of v2 format, layer id's are not the same as the id's
         used in the exported tar archive to name directories for layers.
         These id's can be found in the configuration files saved with
@@ -139,72 +156,74 @@
         # but only layers that do contain some data.
         current_manifest_layer = 0
 
         layer_paths_to_move = []
         layer_paths_to_squash = []
 
         # Iterate over image history, from base image to top layer
-        for i, layer in enumerate(old_image_config['history']):
-
+        for i, layer in enumerate(old_image_config["history"]):
             # If it's not an empty layer get the id
             # (directory name) where the layer's data is
             # stored
-            if not layer.get('empty_layer', False):
-                layer_id = old_image_manifest['Layers'][
-                    current_manifest_layer].rsplit('/')[0]
+            if not layer.get("empty_layer", False):
+                layer_id = old_image_manifest["Layers"][current_manifest_layer].rsplit(
+                    "/"
+                )[0]
 
                 # Check if this layer should be moved or squashed
                 if len(layers_to_move) > i:
                     layer_paths_to_move.append(layer_id)
                 else:
                     layer_paths_to_squash.append(layer_id)
 
                 current_manifest_layer += 1
 
         return layer_paths_to_squash, layer_paths_to_move
 
     def _generate_chain_id(self, chain_ids, diff_ids, parent_chain_id):
-        if parent_chain_id == None:
+        if parent_chain_id is None:
             return self._generate_chain_id(chain_ids, diff_ids[1:], diff_ids[0])
 
         chain_ids.append(parent_chain_id)
 
         if len(diff_ids) == 0:
             return parent_chain_id
 
         # This probably should not be hardcoded
         to_hash = "sha256:%s sha256:%s" % (parent_chain_id, diff_ids[0])
-        digest = hashlib.sha256(str(to_hash).encode('utf8')).hexdigest()
+        digest = hashlib.sha256(str(to_hash).encode("utf8")).hexdigest()
 
         return self._generate_chain_id(chain_ids, diff_ids[1:], digest)
 
     def _generate_chain_ids(self, diff_ids):
         chain_ids = []
 
         self._generate_chain_id(chain_ids, diff_ids, None)
 
         return chain_ids
 
     def _generate_diff_ids(self):
         diff_ids = []
 
         for path in self.layer_paths_to_move:
-            sha256 = self._compute_sha256(os.path.join(self.old_image_dir, path, "layer.tar"))
+            sha256 = self._compute_sha256(
+                os.path.join(self.old_image_dir, path, "layer.tar")
+            )
             diff_ids.append(sha256)
 
         if self.layer_paths_to_squash:
             sha256 = self._compute_sha256(os.path.join(self.squashed_dir, "layer.tar"))
             diff_ids.append(sha256)
 
         return diff_ids
 
     def _compute_sha256(self, layer_tar):
         sha256 = hashlib.sha256()
 
-        with open(layer_tar, 'rb') as f:
+        with open(layer_tar, "rb") as f:
             while True:
                 # Read in 10MB chunks
                 data = f.read(10485760)
 
                 if not data:
                     break
 
@@ -223,115 +242,114 @@
         as https://github.com/docker/docker/blob/v1.10.0-rc1/image/v1/imagev1.go#L64
         """
 
         # Using OrderedDict, because order of JSON elements is important
         v1_metadata = OrderedDict(self.old_image_config)
 
         # Update image creation date
-        v1_metadata['created'] = self.date
+        v1_metadata["created"] = self.date
 
         # Remove unnecessary elements
         # Do not fail if key is not found
-        for key in 'history', 'rootfs', 'container':
+        for key in "history", "rootfs", "container":
             v1_metadata.pop(key, None)
 
         # Docker internally changes the order of keys between
         # exported metadata (why oh why?!). We need to add 'os'
         # element after 'layer_id'
-        operating_system = v1_metadata.pop('os', None)
+        operating_system = v1_metadata.pop("os", None)
 
         # The 'layer_id' element is the chain_id of the
         # squashed layer
-        v1_metadata['layer_id'] = "sha256:%s" % self.chain_ids[-1]
+        v1_metadata["layer_id"] = "sha256:%s" % self.chain_ids[-1]
 
         # Add back 'os' element
         if operating_system:
-            v1_metadata['os'] = operating_system
+            v1_metadata["os"] = operating_system
 
         # The 'parent' element is the name of the directory (inside the
         # exported tar archive) of the last layer that we move
         # (layer below squashed layer)
 
         if self.layer_paths_to_move:
             if self.layer_paths_to_squash:
                 parent = self.layer_paths_to_move[-1]
             else:
                 parent = self.layer_paths_to_move[0]
 
-            v1_metadata['parent'] = "sha256:%s" % parent
+            v1_metadata["parent"] = "sha256:%s" % parent
 
         # The 'Image' element is the id of the layer from which we squash
         if self.squash_id:
             # Update image id, should be one layer below squashed layer
-            v1_metadata['config']['Image'] = self.squash_id
+            v1_metadata["config"]["Image"] = self.squash_id
         else:
-            v1_metadata['config']['Image'] = ""
+            v1_metadata["config"]["Image"] = ""
 
         # Get the sha256sum of the JSON exported metadata,
         # we do not care about the metadata anymore
         sha = self._dump_json(v1_metadata)[1]
 
         return sha
 
     def _generate_last_layer_metadata(self, layer_path_id, old_layer_path=None):
         if not old_layer_path:
             old_layer_path = layer_path_id
 
-        config_file = os.path.join(
-            self.old_image_dir, old_layer_path, "json")
+        config_file = os.path.join(self.old_image_dir, old_layer_path, "json")
 
-        with open(config_file, 'r') as f:
+        with open(config_file, "r") as f:
             config = json.load(f, object_pairs_hook=OrderedDict)
 
-        config['created'] = self.date
+        config["created"] = self.date
 
         if self.squash_id:
             # Update image id, should be one layer below squashed layer
-            config['config']['Image'] = self.squash_id
+            config["config"]["Image"] = self.squash_id
         else:
-            config['config']['Image'] = ""
+            config["config"]["Image"] = ""
 
         # Update 'parent' - it should be path to the last layer to move
         if self.layer_paths_to_move:
-            config['parent'] = self.layer_paths_to_move[-1]
+            config["parent"] = self.layer_paths_to_move[-1]
         else:
             config.pop("parent", None)
         # Update 'id' - it should be the path to the layer
-        config['id'] = layer_path_id
+        config["id"] = layer_path_id
         config.pop("container", None)
         return config
 
     def _generate_image_metadata(self):
         # First - read old image config, we'll update it instead of
         # generating one from scratch
         metadata = OrderedDict(self.old_image_config)
         # Update image creation date
-        metadata['created'] = self.date
+        metadata["created"] = self.date
 
         # Remove unnecessary or old fields
         metadata.pop("container", None)
 
         # Remove squashed layers from history
-        metadata['history'] = metadata['history'][:len(self.layers_to_move)]
+        metadata["history"] = metadata["history"][: len(self.layers_to_move)]
         # Remove diff_ids for squashed layers
-        metadata['rootfs']['diff_ids'] = metadata['rootfs'][
-            'diff_ids'][:len(self.layer_paths_to_move)]
+        metadata["rootfs"]["diff_ids"] = metadata["rootfs"]["diff_ids"][
+            : len(self.layer_paths_to_move)
+        ]
 
-        history = {'comment': self.comment, 'created': self.date}
+        history = {"comment": self.comment, "created": self.date}
 
         if self.layer_paths_to_squash:
             # Add diff_ids for the squashed layer
-            metadata['rootfs']['diff_ids'].append(
-                "sha256:%s" % self.diff_ids[-1])
+            metadata["rootfs"]["diff_ids"].append("sha256:%s" % self.diff_ids[-1])
         else:
-            history['empty_layer'] = True
+            history["empty_layer"] = True
 
         # Add new entry for squashed layer to history
-        metadata['history'].append(history)
+        metadata["history"].append(history)
 
         if self.squash_id:
             # Update image id, should be one layer below squashed layer
-            metadata['config']['Image'] = self.squash_id
+            metadata["config"]["Image"] = self.squash_id
         else:
-            metadata['config']['Image'] = ""
+            metadata["config"]["Image"] = ""
 
         return metadata
```

### Comparing `docker-squash-1.0.9/docker_squash.egg-info/PKG-INFO` & `docker-squash-1.1.0/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,979 +1,952 @@
-00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
-00000010: 3a20 322e 310a 4e61 6d65 3a20 646f 636b  : 2.1.Name: dock
-00000020: 6572 2d73 7175 6173 680a 5665 7273 696f  er-squash.Versio
-00000030: 6e3a 2031 2e30 2e39 0a53 756d 6d61 7279  n: 1.0.9.Summary
-00000040: 3a20 446f 636b 6572 206c 6179 6572 2073  : Docker layer s
-00000050: 7175 6173 6869 6e67 2074 6f6f 6c0a 486f  quashing tool.Ho
-00000060: 6d65 2d70 6167 653a 2068 7474 7073 3a2f  me-page: https:/
-00000070: 2f67 6974 6875 622e 636f 6d2f 676f 6c64  /github.com/gold
-00000080: 6d61 6e6e 2f64 6f63 6b65 722d 7371 7561  mann/docker-squa
-00000090: 7368 0a41 7574 686f 723a 204d 6172 656b  sh.Author: Marek
-000000a0: 2047 6f6c 646d 616e 6e0a 4175 7468 6f72   Goldmann.Author
-000000b0: 2d65 6d61 696c 3a20 6d61 7265 6b2e 676f  -email: marek.go
-000000c0: 6c64 6d61 6e6e 4067 6d61 696c 2e63 6f6d  ldmann@gmail.com
-000000d0: 0a4c 6963 656e 7365 3a20 4d49 540a 446f  .License: MIT.Do
-000000e0: 776e 6c6f 6164 2d55 524c 3a20 6874 7470  wnload-URL: http
-000000f0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f67  s://github.com/g
-00000100: 6f6c 646d 616e 6e2f 646f 636b 6572 2d73  oldmann/docker-s
-00000110: 7175 6173 682f 6172 6368 6976 652f 312e  quash/archive/1.
-00000120: 302e 392e 7461 722e 677a 0a4b 6579 776f  0.9.tar.gz.Keywo
-00000130: 7264 733a 2064 6f63 6b65 720a 506c 6174  rds: docker.Plat
-00000140: 666f 726d 3a20 554e 4b4e 4f57 4e0a 4c69  form: UNKNOWN.Li
-00000150: 6365 6e73 652d 4669 6c65 3a20 4c49 4345  cense-File: LICE
-00000160: 4e53 450a 0a60 6064 6f63 6b65 722d 7371  NSE..``docker-sq
-00000170: 7561 7368 6060 0a3d 3d3d 3d3d 3d3d 3d3d  uash``.=========
-00000180: 3d3d 3d3d 3d3d 3d3d 3d0a 0a2e 2e20 696d  =========.... im
-00000190: 6167 653a 3a20 6874 7470 733a 2f2f 6769  age:: https://gi
-000001a0: 7468 7562 2e63 6f6d 2f67 6f6c 646d 616e  thub.com/goldman
-000001b0: 6e2f 646f 636b 6572 2d73 7175 6173 682f  n/docker-squash/
-000001c0: 6163 7469 6f6e 732f 776f 726b 666c 6f77  actions/workflow
-000001d0: 732f 7371 7561 7368 2e79 6d6c 2f62 6164  s/squash.yml/bad
-000001e0: 6765 2e73 7667 0a20 2020 203a 7461 7267  ge.svg.    :targ
-000001f0: 6574 3a20 6874 7470 733a 2f2f 6769 7468  et: https://gith
-00000200: 7562 2e63 6f6d 2f67 6f6c 646d 616e 6e2f  ub.com/goldmann/
-00000210: 646f 636b 6572 2d73 7175 6173 682f 6163  docker-squash/ac
-00000220: 7469 6f6e 732f 776f 726b 666c 6f77 732f  tions/workflows/
-00000230: 7371 7561 7368 2e79 6d6c 0a0a 5468 6520  squash.yml..The 
-00000240: 7072 6f62 6c65 6d0a 2d2d 2d2d 2d2d 2d2d  problem.--------
-00000250: 2d2d 2d0a 0a44 6f63 6b65 7220 6372 6561  ---..Docker crea
-00000260: 7465 7320 6d61 6e79 206c 6179 6572 7320  tes many layers 
-00000270: 7768 696c 6520 6275 696c 6469 6e67 2074  while building t
-00000280: 6865 2069 6d61 6765 2e20 536f 6d65 7469  he image. Someti
-00000290: 6d65 7320 6974 2773 206e 6f74 206e 6563  mes it's not nec
-000002a0: 6573 7361 7279 206f 7220 6465 7369 7265  essary or desire
-000002b0: 6162 6c65 0a74 6f20 6861 7665 2074 6865  able.to have the
-000002c0: 6d20 696e 2074 6865 2069 6d61 6765 2e20  m in the image. 
-000002d0: 466f 7220 6578 616d 706c 6520 6120 446f  For example a Do
-000002e0: 636b 6572 6669 6c65 2060 4144 4460 2069  ckerfile `ADD` i
-000002f0: 6e73 7472 7563 7469 6f6e 2063 7265 6174  nstruction creat
-00000300: 6573 2061 2073 696e 676c 6520 6c61 7965  es a single laye
-00000310: 720a 7769 7468 2066 696c 6573 2079 6f75  r.with files you
-00000320: 2077 616e 7420 746f 206d 616b 6520 6176   want to make av
-00000330: 6169 6c61 626c 6520 696e 2074 6865 2069  ailable in the i
-00000340: 6d61 6765 2e20 5468 6520 7072 6f62 6c65  mage. The proble
-00000350: 6d20 6172 6973 6573 2077 6865 6e20 7468  m arises when th
-00000360: 6573 6520 6669 6c65 7320 6172 650a 6f6e  ese files are.on
-00000370: 6c79 2074 656d 706f 7261 7279 2066 696c  ly temporary fil
-00000380: 6573 2028 666f 7220 6578 616d 706c 6520  es (for example 
-00000390: 7072 6f64 7563 7420 6469 7374 7269 6275  product distribu
-000003a0: 7469 6f6e 2074 6861 7420 796f 7520 7761  tion that you wa
-000003b0: 6e74 2074 6f20 756e 7061 636b 292e 2044  nt to unpack). D
-000003c0: 6f63 6b65 7220 7769 6c6c 0a63 6172 7279  ocker will.carry
-000003d0: 2074 6869 7320 756e 6e65 6365 7373 6172   this unnecessar
-000003e0: 7920 6c61 7965 7220 616c 7761 7973 2077  y layer always w
-000003f0: 6974 6820 7468 6520 696d 6167 652c 2065  ith the image, e
-00000400: 7665 6e20 6966 2079 6f75 2064 656c 6574  ven if you delet
-00000410: 6520 7468 6573 6520 6669 6c65 7320 696e  e these files in
-00000420: 206e 6578 740a 6c61 7965 722e 2054 6869   next.layer. Thi
-00000430: 7320 6120 7761 7374 6520 6f66 2074 696d  s a waste of tim
-00000440: 6520 286d 6f72 6520 6461 7461 2074 6f20  e (more data to 
-00000450: 7075 7368 2f6c 6f61 642f 7361 7665 2920  push/load/save) 
-00000460: 616e 6420 7265 736f 7572 6365 7320 2862  and resources (b
-00000470: 6967 6765 7220 696d 6167 6529 2e0a 0a53  igger image)...S
-00000480: 7175 6173 6869 6e67 2068 656c 7073 2077  quashing helps w
-00000490: 6974 6820 6f72 6761 6e69 7a69 6e67 2069  ith organizing i
-000004a0: 6d61 6765 7320 696e 206c 6f67 6963 616c  mages in logical
-000004b0: 206c 6179 6572 732e 2049 6e73 7465 6164   layers. Instead
-000004c0: 206f 660a 6861 7669 6e67 2061 6e20 696d   of.having an im
-000004d0: 6167 6520 7769 7468 206d 756c 7469 706c  age with multipl
-000004e0: 6520 2869 6e20 616c 6d6f 7374 2061 6c6c  e (in almost all
-000004f0: 2063 6173 6573 2920 756e 6e65 6365 7373   cases) unnecess
-00000500: 6172 7920 6c61 7965 7273 202d 0a77 6520  ary layers -.we 
-00000510: 6361 6e20 636f 6e74 726f 6c20 7468 6520  can control the 
-00000520: 7374 7275 6374 7572 6520 6f66 2074 6865  structure of the
-00000530: 2069 6d61 6765 2e0a 0a46 6561 7475 7265   image...Feature
-00000540: 730a 2d2d 2d2d 2d2d 2d2d 0a0a 2d20 4361  s.--------..- Ca
-00000550: 6e20 7371 7561 7368 206c 6173 7420 6e20  n squash last n 
-00000560: 6c61 7965 7273 2066 726f 6d20 616e 2069  layers from an i
-00000570: 6d61 6765 0a2d 2043 616e 2073 7175 6173  mage.- Can squas
-00000580: 6820 6672 6f6d 2061 2073 656c 6563 7465  h from a selecte
-00000590: 6420 6c61 7965 7220 746f 2074 6865 2065  d layer to the e
-000005a0: 6e64 2028 6e6f 7420 616c 7761 7973 2070  nd (not always p
-000005b0: 6f73 7369 626c 652c 2064 6570 656e 6473  ossible, depends
-000005c0: 206f 6e20 7468 6520 696d 6167 6529 0a2d   on the image).-
-000005d0: 2053 7570 706f 7274 2066 6f72 2044 6f63   Support for Doc
-000005e0: 6b65 7220 312e 3920 6f72 206e 6577 6572  ker 1.9 or newer
-000005f0: 2028 6f6c 6465 7220 7265 6c65 6173 6573   (older releases
-00000600: 206d 6179 2072 756e 2070 6572 6665 6374   may run perfect
-00000610: 6c79 2066 696e 6520 746f 6f2c 2074 7279  ly fine too, try
-00000620: 2069 7421 290a 2d20 5371 7561 7368 6564   it!).- Squashed
-00000630: 2069 6d61 6765 2063 616e 2062 6520 6c6f   image can be lo
-00000640: 6164 6564 2062 6163 6b20 746f 2074 6865  aded back to the
-00000650: 2044 6f63 6b65 7220 6461 656d 6f6e 206f   Docker daemon o
-00000660: 7220 7374 6f72 6564 2061 7320 7461 7220  r stored as tar 
-00000670: 6172 6368 6976 6520 736f 6d65 7768 6572  archive somewher
-00000680: 650a 0a49 6e73 7461 6c6c 6174 696f 6e0a  e..Installation.
-00000690: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a0a 4672  ------------..Fr
-000006a0: 6f6d 2073 6f75 7263 6520 636f 6465 0a0a  om source code..
-000006b0: 3a3a 0a0a 2020 2020 2420 7069 7020 696e  ::..    $ pip in
-000006c0: 7374 616c 6c20 2d2d 7573 6572 2068 7474  stall --user htt
-000006d0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-000006e0: 676f 6c64 6d61 6e6e 2f64 6f63 6b65 722d  goldmann/docker-
-000006f0: 7371 7561 7368 2f61 7263 6869 7665 2f6d  squash/archive/m
-00000700: 6173 7465 722e 7a69 700a 0a46 726f 6d20  aster.zip..From 
-00000710: 5079 5069 0a0a 3a3a 0a0a 2020 2020 2420  PyPi..::..    $ 
-00000720: 7069 7020 696e 7374 616c 6c20 646f 636b  pip install dock
-00000730: 6572 2d73 7175 6173 680a 0a55 7361 6765  er-squash..Usage
-00000740: 0a2d 2d2d 2d2d 0a0a 3a3a 0a0a 2020 2020  .-----..::..    
-00000750: 2420 646f 636b 6572 2d73 7175 6173 6820  $ docker-squash 
-00000760: 2d68 0a20 2020 2075 7361 6765 3a20 636c  -h.    usage: cl
-00000770: 692e 7079 205b 2d68 5d20 5b2d 765d 205b  i.py [-h] [-v] [
-00000780: 2d2d 7665 7273 696f 6e5d 205b 2d64 5d20  --version] [-d] 
-00000790: 5b2d 6620 4652 4f4d 5f4c 4159 4552 5d20  [-f FROM_LAYER] 
-000007a0: 5b2d 7420 5441 475d 0a20 2020 2020 2020  [-t TAG].       
-000007b0: 2020 2020 2020 2020 2020 205b 2d2d 746d             [--tm
-000007c0: 702d 6469 7220 544d 505f 4449 525d 205b  p-dir TMP_DIR] [
-000007d0: 2d2d 6f75 7470 7574 2d70 6174 6820 4f55  --output-path OU
-000007e0: 5450 5554 5f50 4154 485d 0a20 2020 2020  TPUT_PATH].     
-000007f0: 2020 2020 2020 2020 2020 2020 2069 6d61               ima
-00000800: 6765 0a0a 2020 2020 446f 636b 6572 206c  ge..    Docker l
-00000810: 6179 6572 2073 7175 6173 6869 6e67 2074  ayer squashing t
-00000820: 6f6f 6c0a 0a20 2020 2070 6f73 6974 696f  ool..    positio
-00000830: 6e61 6c20 6172 6775 6d65 6e74 733a 0a20  nal arguments:. 
-00000840: 2020 2020 2069 6d61 6765 2020 2020 2020       image      
-00000850: 2020 2020 2020 2020 2020 2049 6d61 6765             Image
-00000860: 2074 6f20 6265 2073 7175 6173 6865 640a   to be squashed.
-00000870: 0a20 2020 206f 7074 696f 6e61 6c20 6172  .    optional ar
-00000880: 6775 6d65 6e74 733a 0a20 2020 2020 202d  guments:.      -
-00000890: 682c 202d 2d68 656c 7020 2020 2020 2020  h, --help       
-000008a0: 2020 2020 2073 686f 7720 7468 6973 2068       show this h
-000008b0: 656c 7020 6d65 7373 6167 6520 616e 6420  elp message and 
-000008c0: 6578 6974 0a20 2020 2020 202d 762c 202d  exit.      -v, -
-000008d0: 2d76 6572 626f 7365 2020 2020 2020 2020  -verbose        
-000008e0: 2056 6572 626f 7365 206f 7574 7075 740a   Verbose output.
-000008f0: 2020 2020 2020 2d2d 7665 7273 696f 6e20        --version 
-00000900: 2020 2020 2020 2020 2020 2020 5368 6f77              Show
-00000910: 2076 6572 7369 6f6e 2061 6e64 2065 7869   version and exi
-00000920: 740a 2020 2020 2020 2d64 2c20 2d2d 6465  t.      -d, --de
-00000930: 7665 6c6f 706d 656e 7420 2020 2020 446f  velopment     Do
-00000940: 6573 206e 6f74 2063 6c65 616e 2075 7020  es not clean up 
-00000950: 6166 7465 7220 6661 696c 7572 6520 666f  after failure fo
-00000960: 7220 6561 7369 6572 2064 6562 7567 6769  r easier debuggi
-00000970: 6e67 0a20 2020 2020 202d 6620 4652 4f4d  ng.      -f FROM
-00000980: 5f4c 4159 4552 2c20 2d2d 6672 6f6d 2d6c  _LAYER, --from-l
-00000990: 6179 6572 2046 524f 4d5f 4c41 5945 520a  ayer FROM_LAYER.
-000009a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000009b0: 2020 2020 2020 2020 2020 2020 4944 206f              ID o
-000009c0: 6620 7468 6520 6c61 7965 7220 6f72 2069  f the layer or i
-000009d0: 6d61 6765 2049 4420 6f72 2069 6d61 6765  mage ID or image
-000009e0: 206e 616d 652e 2049 6620 6e6f 740a 2020   name. If not.  
-000009f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000a00: 2020 2020 2020 2020 2020 7370 6563 6966            specif
-00000a10: 6965 6420 7769 6c6c 2073 7175 6173 6820  ied will squash 
-00000a20: 616c 6c20 6c61 7965 7273 2069 6e20 7468  all layers in th
-00000a30: 6520 696d 6167 650a 2020 2020 2020 2d74  e image.      -t
-00000a40: 2054 4147 2c20 2d2d 7461 6720 5441 4720   TAG, --tag TAG 
-00000a50: 2020 2020 5370 6563 6966 7920 7468 6520      Specify the 
-00000a60: 7461 6720 746f 2062 6520 7573 6564 2066  tag to be used f
-00000a70: 6f72 2074 6865 206e 6577 2069 6d61 6765  or the new image
-00000a80: 2e20 4279 0a20 2020 2020 2020 2020 2020  . By.           
-00000a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000aa0: 2064 6566 6175 6c74 2069 7427 6c6c 2062   default it'll b
-00000ab0: 6520 7365 7420 746f 2027 696d 6167 6527  e set to 'image'
-00000ac0: 2061 7267 756d 656e 740a 2020 2020 2020   argument.      
-00000ad0: 2d2d 746d 702d 6469 7220 544d 505f 4449  --tmp-dir TMP_DI
-00000ae0: 5220 2020 2020 5465 6d70 6f72 6172 7920  R     Temporary 
-00000af0: 6469 7265 6374 6f72 7920 746f 2062 6520  directory to be 
-00000b00: 6372 6561 7465 6420 616e 6420 7573 6564  created and used
-00000b10: 0a20 2020 2020 202d 2d6f 7574 7075 742d  .      --output-
-00000b20: 7061 7468 204f 5554 5055 545f 5041 5448  path OUTPUT_PATH
-00000b30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000b40: 2020 2020 2020 2020 2020 2020 2050 6174               Pat
-00000b50: 6820 7768 6572 6520 7468 6520 696d 6167  h where the imag
-00000b60: 6520 7368 6f75 6c64 2062 6520 7374 6f72  e should be stor
-00000b70: 6564 2061 6674 6572 2073 7175 6173 6869  ed after squashi
-00000b80: 6e67 2e0a 2020 2020 2020 2020 2020 2020  ng..            
-00000b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000ba0: 4966 206e 6f74 2070 726f 7669 6465 642c  If not provided,
-00000bb0: 2069 6d61 6765 2077 696c 6c20 6265 206c   image will be l
-00000bc0: 6f61 6465 6420 696e 746f 2044 6f63 6b65  oaded into Docke
-00000bd0: 720a 2020 2020 2020 2020 2020 2020 2020  r.              
-00000be0: 2020 2020 2020 2020 2020 2020 2020 6461                da
-00000bf0: 656d 6f6e 0a0a 4c69 6365 6e73 650a 2d2d  emon..License.--
-00000c00: 2d2d 2d2d 2d0a 0a4d 4954 0a0a 4578 616d  -----..MIT..Exam
-00000c10: 706c 6573 0a2d 2d2d 2d2d 2d2d 2d0a 0a57  ples.--------..W
-00000c20: 6520 7374 6172 7420 7769 7468 2069 6d61  e start with ima
-00000c30: 6765 206c 696b 6520 7468 6973 3a0a 0a3a  ge like this:..:
-00000c40: 3a0a 0a20 2020 2024 2064 6f63 6b65 7220  :..    $ docker 
-00000c50: 6869 7374 6f72 7920 6a62 6f73 732f 7769  history jboss/wi
-00000c60: 6c64 666c 793a 6c61 7465 7374 0a20 2020  ldfly:latest.   
-00000c70: 2049 4d41 4745 2020 2020 2020 2020 2020   IMAGE          
-00000c80: 2020 2020 2043 5245 4154 4544 2020 2020       CREATED    
-00000c90: 2020 2020 2020 2020 2043 5245 4154 4544           CREATED
-00000ca0: 2042 5920 2020 2020 2020 2020 2020 2020   BY             
-00000cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000cc0: 2020 2020 2020 2020 2053 495a 4520 2020           SIZE   
-00000cd0: 2020 2020 2020 2020 2020 2020 2043 4f4d               COM
-00000ce0: 4d45 4e54 0a20 2020 2032 3539 3534 6536  MENT.    25954e6
-00000cf0: 6432 3330 3020 2020 2020 2020 2033 2077  d2300        3 w
-00000d00: 6565 6b73 2061 676f 2020 2020 2020 2020  eeks ago        
-00000d10: 202f 6269 6e2f 7368 202d 6320 2328 6e6f   /bin/sh -c #(no
-00000d20: 7029 2043 4d44 205b 222f 6f70 742f 6a62  p) CMD ["/opt/jb
-00000d30: 6f73 732f 7769 6c64 666c 792f 6269 2020  oss/wildfly/bi  
-00000d40: 2030 2042 2020 2020 2020 2020 2020 2020   0 B            
-00000d50: 2020 2020 200a 2020 2020 3561 6536 3963       .    5ae69c
-00000d60: 6234 3534 6135 2020 2020 2020 2020 3320  b454a5        3 
-00000d70: 7765 656b 7320 6167 6f20 2020 2020 2020  weeks ago       
-00000d80: 2020 2f62 696e 2f73 6820 2d63 2023 286e    /bin/sh -c #(n
-00000d90: 6f70 2920 4558 504f 5345 2038 3038 302f  op) EXPOSE 8080/
-00000da0: 7463 7020 2020 2020 2020 2020 2020 2020  tcp             
-00000db0: 2020 3020 4220 2020 2020 2020 2020 2020    0 B           
-00000dc0: 2020 2020 2020 0a20 2020 2064 6332 3437        .    dc247
-00000dd0: 3132 6633 3563 3420 2020 2020 2020 2033  12f35c4        3
-00000de0: 2077 6565 6b73 2061 676f 2020 2020 2020   weeks ago      
-00000df0: 2020 202f 6269 6e2f 7368 202d 6320 2328     /bin/sh -c #(
-00000e00: 6e6f 7029 2045 4e56 204c 4155 4e43 485f  nop) ENV LAUNCH_
-00000e10: 4a42 4f53 535f 494e 5f42 4143 4b47 524f  JBOSS_IN_BACKGRO
-00000e20: 2020 2030 2042 2020 2020 2020 2020 2020     0 B          
-00000e30: 2020 2020 2020 200a 2020 2020 6439 3239         .    d929
-00000e40: 3132 3964 3463 3865 2020 2020 2020 2020  129d4c8e        
-00000e50: 3320 7765 656b 7320 6167 6f20 2020 2020  3 weeks ago     
-00000e60: 2020 2020 2f62 696e 2f73 6820 2d63 2063      /bin/sh -c c
-00000e70: 6420 2448 4f4d 4520 2020 2020 2626 2063  d $HOME     && c
-00000e80: 7572 6c20 2d4f 2068 7474 7073 3a2f 2f64  url -O https://d
-00000e90: 6f20 2020 3136 302e 3820 4d42 2020 2020  o   160.8 MB    
-00000ea0: 2020 2020 2020 2020 0a20 2020 2062 3866          .    b8f
-00000eb0: 6133 6361 6637 6436 6420 2020 2020 2020  a3caf7d6d       
-00000ec0: 2033 2077 6565 6b73 2061 676f 2020 2020   3 weeks ago    
-00000ed0: 2020 2020 202f 6269 6e2f 7368 202d 6320       /bin/sh -c 
-00000ee0: 2328 6e6f 7029 2045 4e56 204a 424f 5353  #(nop) ENV JBOSS
-00000ef0: 5f48 4f4d 453d 2f6f 7074 2f6a 626f 7373  _HOME=/opt/jboss
-00000f00: 2f77 2020 2030 2042 2020 2020 2020 2020  /w   0 B        
-00000f10: 2020 2020 2020 2020 200a 2020 2020 3338           .    38
-00000f20: 6238 6638 3565 3734 6266 2020 2020 2020  b8f85e74bf      
-00000f30: 2020 3320 7765 656b 7320 6167 6f20 2020    3 weeks ago   
-00000f40: 2020 2020 2020 2f62 696e 2f73 6820 2d63        /bin/sh -c
-00000f50: 2023 286e 6f70 2920 454e 5620 5749 4c44   #(nop) ENV WILD
-00000f60: 464c 595f 5348 4131 3d63 3064 6437 3535  FLY_SHA1=c0dd755
-00000f70: 3263 3520 2020 3020 4220 2020 2020 2020  2c5   0 B       
-00000f80: 2020 2020 2020 2020 2020 0a20 2020 2061            .    a
-00000f90: 6537 3962 3634 3662 3961 3920 2020 2020  e79b646b9a9     
-00000fa0: 2020 2033 2077 6565 6b73 2061 676f 2020     3 weeks ago  
-00000fb0: 2020 2020 2020 202f 6269 6e2f 7368 202d         /bin/sh -
-00000fc0: 6320 2328 6e6f 7029 2045 4e56 2057 494c  c #(nop) ENV WIL
-00000fd0: 4446 4c59 5f56 4552 5349 4f4e 3d31 302e  DFLY_VERSION=10.
-00000fe0: 302e 302e 2020 2030 2042 2020 2020 2020  0.0.   0 B      
-00000ff0: 2020 2020 2020 2020 2020 200a 2020 2020             .    
-00001000: 3262 3436 3036 6463 3964 6337 2020 2020  2b4606dc9dc7    
-00001010: 2020 2020 3320 7765 656b 7320 6167 6f20      3 weeks ago 
-00001020: 2020 2020 2020 2020 2f62 696e 2f73 6820          /bin/sh 
-00001030: 2d63 2023 286e 6f70 2920 454e 5620 4a41  -c #(nop) ENV JA
-00001040: 5641 5f48 4f4d 453d 2f75 7372 2f6c 6962  VA_HOME=/usr/lib
-00001050: 2f6a 766d 2f20 2020 3020 4220 2020 2020  /jvm/   0 B     
-00001060: 2020 2020 2020 2020 2020 2020 0a20 2020              .   
-00001070: 2031 3138 6661 3965 3333 3537 3620 2020   118fa9e33576   
-00001080: 2020 2020 2033 2077 6565 6b73 2061 676f       3 weeks ago
-00001090: 2020 2020 2020 2020 202f 6269 6e2f 7368           /bin/sh
-000010a0: 202d 6320 2328 6e6f 7029 2055 5345 5220   -c #(nop) USER 
-000010b0: 5b6a 626f 7373 5d20 2020 2020 2020 2020  [jboss]         
-000010c0: 2020 2020 2020 2020 2030 2042 2020 2020           0 B    
-000010d0: 2020 2020 2020 2020 2020 2020 200a 2020               .  
-000010e0: 2020 3566 3765 3866 3336 6333 6262 2020    5f7e8f36c3bb  
-000010f0: 2020 2020 2020 3320 7765 656b 7320 6167        3 weeks ag
-00001100: 6f20 2020 2020 2020 2020 2f62 696e 2f73  o         /bin/s
-00001110: 6820 2d63 2079 756d 202d 7920 696e 7374  h -c yum -y inst
-00001120: 616c 6c20 6a61 7661 2d31 2e38 2e30 2d6f  all java-1.8.0-o
-00001130: 7065 6e6a 646b 2d20 2020 3139 372e 3420  penjdk-   197.4 
-00001140: 4d42 2020 2020 2020 2020 2020 2020 0a20  MB            . 
-00001150: 2020 2033 6434 6430 3232 3866 3136 3120     3d4d0228f161 
-00001160: 2020 2020 2020 2033 2077 6565 6b73 2061         3 weeks a
-00001170: 676f 2020 2020 2020 2020 202f 6269 6e2f  go         /bin/
-00001180: 7368 202d 6320 2328 6e6f 7029 2055 5345  sh -c #(nop) USE
-00001190: 5220 5b72 6f6f 745d 2020 2020 2020 2020  R [root]        
-000011a0: 2020 2020 2020 2020 2020 2030 2042 2020             0 B  
-000011b0: 2020 2020 2020 2020 2020 2020 2020 200a                 .
-000011c0: 2020 2020 6637 6162 3465 6131 3937 3038      f7ab4ea19708
-000011d0: 2020 2020 2020 2020 3320 7765 656b 7320          3 weeks 
-000011e0: 6167 6f20 2020 2020 2020 2020 2f62 696e  ago         /bin
-000011f0: 2f73 6820 2d63 2023 286e 6f70 2920 4d41  /sh -c #(nop) MA
-00001200: 494e 5441 494e 4552 204d 6172 656b 2047  INTAINER Marek G
-00001210: 6f6c 646d 616e 6e20 3c20 2020 3020 4220  oldmann <   0 B 
-00001220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001230: 0a20 2020 2034 6262 3135 6633 6236 3937  .    4bb15f3b697
-00001240: 3720 2020 2020 2020 2033 2077 6565 6b73  7        3 weeks
-00001250: 2061 676f 2020 2020 2020 2020 202f 6269   ago         /bi
-00001260: 6e2f 7368 202d 6320 2328 6e6f 7029 2055  n/sh -c #(nop) U
-00001270: 5345 5220 5b6a 626f 7373 5d20 2020 2020  SER [jboss]     
-00001280: 2020 2020 2020 2020 2020 2020 2030 2042               0 B
-00001290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000012a0: 200a 2020 2020 3564 6331 6534 3966 3433   .    5dc1e49f43
-000012b0: 3631 2020 2020 2020 2020 3320 7765 656b  61        3 week
-000012c0: 7320 6167 6f20 2020 2020 2020 2020 2f62  s ago         /b
-000012d0: 696e 2f73 6820 2d63 2023 286e 6f70 2920  in/sh -c #(nop) 
-000012e0: 574f 524b 4449 5220 2f6f 7074 2f6a 626f  WORKDIR /opt/jbo
-000012f0: 7373 2020 2020 2020 2020 2020 2020 3020  ss            0 
-00001300: 4220 2020 2020 2020 2020 2020 2020 2020  B               
-00001310: 2020 0a20 2020 2037 6630 6639 6562 3331    .    7f0f9eb31
-00001320: 3137 3420 2020 2020 2020 2033 2077 6565  174        3 wee
-00001330: 6b73 2061 676f 2020 2020 2020 2020 202f  ks ago         /
-00001340: 6269 6e2f 7368 202d 6320 6772 6f75 7061  bin/sh -c groupa
-00001350: 6464 202d 7220 6a62 6f73 7320 2d67 2031  dd -r jboss -g 1
-00001360: 3030 3020 2626 2075 7365 7261 2020 2034  000 && usera   4
-00001370: 2e33 3439 206b 4220 2020 2020 2020 2020  .349 kB         
-00001380: 2020 200a 2020 2020 6264 3531 3566 3034     .    bd515f04
-00001390: 3461 6637 2020 2020 2020 2020 3320 7765  4af7        3 we
-000013a0: 656b 7320 6167 6f20 2020 2020 2020 2020  eks ago         
-000013b0: 2f62 696e 2f73 6820 2d63 2079 756d 2075  /bin/sh -c yum u
-000013c0: 7064 6174 6520 2d79 2026 2620 7975 6d20  pdate -y && yum 
-000013d0: 2d79 2069 6e73 7461 6c6c 2078 6d20 2020  -y install xm   
-000013e0: 3235 2e31 3820 4d42 2020 2020 2020 2020  25.18 MB        
-000013f0: 2020 2020 0a20 2020 2062 3738 3333 3630      .    b783360
-00001400: 3939 3034 3520 2020 2020 2020 2033 2077  99045        3 w
-00001410: 6565 6b73 2061 676f 2020 2020 2020 2020  eeks ago        
-00001420: 202f 6269 6e2f 7368 202d 6320 2328 6e6f   /bin/sh -c #(no
-00001430: 7029 204d 4149 4e54 4149 4e45 5220 4d61  p) MAINTAINER Ma
-00001440: 7265 6b20 476f 6c64 6d61 6e6e 203c 2020  rek Goldmann <  
-00001450: 2030 2042 2020 2020 2020 2020 2020 2020   0 B            
-00001460: 2020 2020 200a 2020 2020 3438 3136 6132       .    4816a2
-00001470: 3938 3534 3863 2020 2020 2020 2020 3320  98548c        3 
-00001480: 7765 656b 7320 6167 6f20 2020 2020 2020  weeks ago       
-00001490: 2020 2f62 696e 2f73 6820 2d63 2023 286e    /bin/sh -c #(n
-000014a0: 6f70 2920 434d 4420 5b22 2f62 696e 2f62  op) CMD ["/bin/b
-000014b0: 6173 6822 5d20 2020 2020 2020 2020 2020  ash"]           
-000014c0: 2020 3020 4220 2020 2020 2020 2020 2020    0 B           
-000014d0: 2020 2020 2020 0a20 2020 2036 6565 3233        .    6ee23
-000014e0: 3563 6634 3437 3320 2020 2020 2020 2033  5cf4473        3
-000014f0: 2077 6565 6b73 2061 676f 2020 2020 2020   weeks ago      
-00001500: 2020 202f 6269 6e2f 7368 202d 6320 2328     /bin/sh -c #(
-00001510: 6e6f 7029 204c 4142 454c 206e 616d 653d  nop) LABEL name=
-00001520: 4365 6e74 4f53 2042 6173 6520 496d 6167  CentOS Base Imag
-00001530: 2020 2030 2042 2020 2020 2020 2020 2020     0 B          
-00001540: 2020 2020 2020 200a 2020 2020 3437 3463         .    474c
-00001550: 3265 6537 3766 6133 2020 2020 2020 2020  2ee77fa3        
-00001560: 3320 7765 656b 7320 6167 6f20 2020 2020  3 weeks ago     
-00001570: 2020 2020 2f62 696e 2f73 6820 2d63 2023      /bin/sh -c #
-00001580: 286e 6f70 2920 4144 4420 6669 6c65 3a37  (nop) ADD file:7
-00001590: 3238 3532 6663 3736 3236 6432 3333 3334  2852fc7626d23334
-000015a0: 3320 2020 3139 362e 3620 4d42 2020 2020  3   196.6 MB    
-000015b0: 2020 2020 2020 2020 0a20 2020 2031 3534          .    154
-000015c0: 3430 3834 6661 6438 3120 2020 2020 2020  4084fad81       
-000015d0: 2036 206d 6f6e 7468 7320 6167 6f20 2020   6 months ago   
-000015e0: 2020 2020 202f 6269 6e2f 7368 202d 6320       /bin/sh -c 
-000015f0: 2328 6e6f 7029 204d 4149 4e54 4149 4e45  #(nop) MAINTAINE
-00001600: 5220 5468 6520 4365 6e74 4f53 2050 726f  R The CentOS Pro
-00001610: 6a65 2020 2030 2042 0a0a 416e 6420 7765  je   0 B..And we
-00001620: 2077 616e 7420 746f 2073 7175 6173 6820   want to squash 
-00001630: 616c 6c20 7468 6520 6c61 7965 7273 2064  all the layers d
-00001640: 6f77 6e20 746f 206c 6179 6572 2060 6034  own to layer ``4
-00001650: 6262 3135 6633 6236 3937 3760 602e 0a0a  bb15f3b6977``...
-00001660: 3a3a 0a0a 2020 2020 2420 646f 636b 6572  ::..    $ docker
-00001670: 2d73 7175 6173 6820 2d66 2034 6262 3135  -squash -f 4bb15
-00001680: 6633 6236 3937 3720 2d74 206a 626f 7373  f3b6977 -t jboss
-00001690: 2f77 696c 6466 6c79 3a73 7175 6173 6865  /wildfly:squashe
-000016a0: 6420 6a62 6f73 732f 7769 6c64 666c 793a  d jboss/wildfly:
-000016b0: 6c61 7465 7374 0a20 2020 2032 3031 362d  latest.    2016-
-000016c0: 3034 2d30 3120 3133 3a31 313a 3032 2c33  04-01 13:11:02,3
-000016d0: 3538 2072 6f6f 7420 2020 2020 2020 2020  58 root         
-000016e0: 494e 464f 2020 2020 2064 6f63 6b65 722d  INFO     docker-
-000016f0: 7363 7269 7074 7320 7665 7273 696f 6e20  scripts version 
-00001700: 312e 302e 3064 6576 2c20 446f 636b 6572  1.0.0dev, Docker
-00001710: 2037 3230 3636 3231 2c20 4150 4920 312e   7206621, API 1.
-00001720: 3231 2e2e 2e0a 2020 2020 3230 3136 2d30  21....    2016-0
-00001730: 342d 3031 2031 333a 3131 3a30 322c 3335  4-01 13:11:02,35
-00001740: 3820 726f 6f74 2020 2020 2020 2020 2049  8 root         I
-00001750: 4e46 4f20 2020 2020 5573 696e 6720 7631  NFO     Using v1
-00001760: 2069 6d61 6765 2066 6f72 6d61 740a 2020   image format.  
-00001770: 2020 3230 3136 2d30 342d 3031 2031 333a    2016-04-01 13:
-00001780: 3131 3a30 322c 3337 3420 726f 6f74 2020  11:02,374 root  
-00001790: 2020 2020 2020 2049 4e46 4f20 2020 2020         INFO     
-000017a0: 4f6c 6420 696d 6167 6520 6861 7320 3231  Old image has 21
-000017b0: 206c 6179 6572 730a 2020 2020 3230 3136   layers.    2016
-000017c0: 2d30 342d 3031 2031 333a 3131 3a30 322c  -04-01 13:11:02,
-000017d0: 3337 3820 726f 6f74 2020 2020 2020 2020  378 root        
-000017e0: 2049 4e46 4f20 2020 2020 4368 6563 6b69   INFO     Checki
-000017f0: 6e67 2069 6620 7371 7561 7368 696e 6720  ng if squashing 
-00001800: 6973 206e 6563 6573 7361 7279 2e2e 2e0a  is necessary....
-00001810: 2020 2020 3230 3136 2d30 342d 3031 2031      2016-04-01 1
-00001820: 333a 3131 3a30 322c 3337 3820 726f 6f74  3:11:02,378 root
-00001830: 2020 2020 2020 2020 2049 4e46 4f20 2020           INFO   
-00001840: 2020 4174 7465 6d70 7469 6e67 2074 6f20    Attempting to 
-00001850: 7371 7561 7368 206c 6173 7420 3132 206c  squash last 12 l
-00001860: 6179 6572 732e 2e2e 0a20 2020 2032 3031  ayers....    201
-00001870: 362d 3034 2d30 3120 3133 3a31 313a 3032  6-04-01 13:11:02
-00001880: 2c33 3738 2072 6f6f 7420 2020 2020 2020  ,378 root       
-00001890: 2020 494e 464f 2020 2020 2053 6176 696e    INFO     Savin
-000018a0: 6720 696d 6167 6520 3235 3935 3465 3664  g image 25954e6d
-000018b0: 3233 3030 3036 3233 3565 6563 6237 6630  230006235eecb7f0
-000018c0: 6363 3536 3032 3634 6437 3331 3436 3938  cc560264d7314698
-000018d0: 3563 3264 3265 3636 3362 6163 3935 3364  5c2d2e663bac953d
-000018e0: 3636 3062 3837 3330 2074 6f20 2f74 6d70  660b8730 to /tmp
-000018f0: 2f64 6f63 6b65 722d 7371 7561 7368 2d66  /docker-squash-f
-00001900: 6278 5a7a 342f 6f6c 642f 696d 6167 652e  bxZz4/old/image.
-00001910: 7461 7220 6669 6c65 2e2e 2e0a 2020 2020  tar file....    
-00001920: 3230 3136 2d30 342d 3031 2031 333a 3131  2016-04-01 13:11
-00001930: 3a30 382c 3030 3320 726f 6f74 2020 2020  :08,003 root    
-00001940: 2020 2020 2049 4e46 4f20 2020 2020 496d       INFO     Im
-00001950: 6167 6520 7361 7665 6421 0a20 2020 2032  age saved!.    2
-00001960: 3031 362d 3034 2d30 3120 3133 3a31 313a  016-04-01 13:11:
-00001970: 3038 2c30 3331 2072 6f6f 7420 2020 2020  08,031 root     
-00001980: 2020 2020 494e 464f 2020 2020 2055 6e70      INFO     Unp
-00001990: 6163 6b69 6e67 202f 746d 702f 646f 636b  acking /tmp/dock
-000019a0: 6572 2d73 7175 6173 682d 6662 785a 7a34  er-squash-fbxZz4
-000019b0: 2f6f 6c64 2f69 6d61 6765 2e74 6172 2074  /old/image.tar t
-000019c0: 6172 2066 696c 6520 746f 202f 746d 702f  ar file to /tmp/
-000019d0: 646f 636b 6572 2d73 7175 6173 682d 6662  docker-squash-fb
-000019e0: 785a 7a34 2f6f 6c64 2064 6972 6563 746f  xZz4/old directo
-000019f0: 7279 0a20 2020 2032 3031 362d 3034 2d30  ry.    2016-04-0
-00001a00: 3120 3133 3a31 313a 3038 2c35 3838 2072  1 13:11:08,588 r
-00001a10: 6f6f 7420 2020 2020 2020 2020 494e 464f  oot         INFO
-00001a20: 2020 2020 2041 7263 6869 7665 2075 6e70       Archive unp
-00001a30: 6163 6b65 6421 0a20 2020 2032 3031 362d  acked!.    2016-
-00001a40: 3034 2d30 3120 3133 3a31 313a 3038 2c36  04-01 13:11:08,6
-00001a50: 3336 2072 6f6f 7420 2020 2020 2020 2020  36 root         
-00001a60: 494e 464f 2020 2020 2053 7175 6173 6869  INFO     Squashi
-00001a70: 6e67 2069 6d61 6765 2027 6a62 6f73 732f  ng image 'jboss/
-00001a80: 7769 6c64 666c 793a 6c61 7465 7374 272e  wildfly:latest'.
-00001a90: 2e2e 0a20 2020 2032 3031 362d 3034 2d30  ...    2016-04-0
-00001aa0: 3120 3133 3a31 313a 3038 2c36 3337 2072  1 13:11:08,637 r
-00001ab0: 6f6f 7420 2020 2020 2020 2020 494e 464f  oot         INFO
-00001ac0: 2020 2020 2053 7461 7274 696e 6720 7371       Starting sq
-00001ad0: 7561 7368 696e 672e 2e2e 0a20 2020 2032  uashing....    2
-00001ae0: 3031 362d 3034 2d30 3120 3133 3a31 313a  016-04-01 13:11:
-00001af0: 3038 2c36 3337 2072 6f6f 7420 2020 2020  08,637 root     
-00001b00: 2020 2020 494e 464f 2020 2020 2053 7175      INFO     Squ
-00001b10: 6173 6869 6e67 2066 696c 6520 272f 746d  ashing file '/tm
-00001b20: 702f 646f 636b 6572 2d73 7175 6173 682d  p/docker-squash-
-00001b30: 6662 785a 7a34 2f6f 6c64 2f32 3539 3534  fbxZz4/old/25954
-00001b40: 6536 6432 3330 3030 3632 3335 6565 6362  e6d230006235eecb
-00001b50: 3766 3063 6335 3630 3236 3464 3733 3134  7f0cc560264d7314
-00001b60: 3639 3835 6332 6432 6536 3633 6261 6339  6985c2d2e663bac9
-00001b70: 3533 6436 3630 6238 3733 302f 6c61 7965  53d660b8730/laye
-00001b80: 722e 7461 7227 2e2e 2e0a 2020 2020 3230  r.tar'....    20
-00001b90: 3136 2d30 342d 3031 2031 333a 3131 3a30  16-04-01 13:11:0
-00001ba0: 382c 3633 3720 726f 6f74 2020 2020 2020  8,637 root      
-00001bb0: 2020 2049 4e46 4f20 2020 2020 5371 7561     INFO     Squa
-00001bc0: 7368 696e 6720 6669 6c65 2027 2f74 6d70  shing file '/tmp
-00001bd0: 2f64 6f63 6b65 722d 7371 7561 7368 2d66  /docker-squash-f
-00001be0: 6278 5a7a 342f 6f6c 642f 3561 6536 3963  bxZz4/old/5ae69c
-00001bf0: 6234 3534 6135 6135 3432 6636 3365 3134  b454a5a542f63e14
-00001c00: 3863 6534 3066 6239 6530 3164 6535 6262  8ce40fb9e01de5bb
-00001c10: 3031 3830 3562 3464 6564 3233 3838 3431  01805b4ded238841
-00001c20: 6263 3263 6538 6538 3935 2f6c 6179 6572  bc2ce8e895/layer
-00001c30: 2e74 6172 272e 2e2e 0a20 2020 2032 3031  .tar'....    201
-00001c40: 362d 3034 2d30 3120 3133 3a31 313a 3038  6-04-01 13:11:08
-00001c50: 2c36 3337 2072 6f6f 7420 2020 2020 2020  ,637 root       
-00001c60: 2020 494e 464f 2020 2020 2053 7175 6173    INFO     Squas
-00001c70: 6869 6e67 2066 696c 6520 272f 746d 702f  hing file '/tmp/
-00001c80: 646f 636b 6572 2d73 7175 6173 682d 6662  docker-squash-fb
-00001c90: 785a 7a34 2f6f 6c64 2f64 6332 3437 3132  xZz4/old/dc24712
-00001ca0: 6633 3563 3430 6539 3538 6265 3861 6361  f35c40e958be8aca
-00001cb0: 3237 3331 6537 6266 3833 3533 6239 6231  2731e7bf8353b9b1
-00001cc0: 3862 6161 3661 3934 6164 3834 6336 3935  8baa6a94ad84c695
-00001cd0: 3263 6263 3737 3030 342f 6c61 7965 722e  2cbc77004/layer.
-00001ce0: 7461 7227 2e2e 2e0a 2020 2020 3230 3136  tar'....    2016
-00001cf0: 2d30 342d 3031 2031 333a 3131 3a30 382c  -04-01 13:11:08,
-00001d00: 3633 3820 726f 6f74 2020 2020 2020 2020  638 root        
-00001d10: 2049 4e46 4f20 2020 2020 5371 7561 7368   INFO     Squash
-00001d20: 696e 6720 6669 6c65 2027 2f74 6d70 2f64  ing file '/tmp/d
-00001d30: 6f63 6b65 722d 7371 7561 7368 2d66 6278  ocker-squash-fbx
-00001d40: 5a7a 342f 6f6c 642f 6439 3239 3132 3964  Zz4/old/d929129d
-00001d50: 3463 3865 3631 6561 3336 3631 6562 3432  4c8e61ea3661eb42
-00001d60: 6333 3064 3031 6634 6331 3532 3431 3836  c30d01f4c1524186
-00001d70: 3839 3137 3861 6663 3764 6338 3138 3561  89178afc7dc8185a
-00001d80: 3337 3831 3435 3238 2f6c 6179 6572 2e74  37814528/layer.t
-00001d90: 6172 272e 2e2e 0a20 2020 2032 3031 362d  ar'....    2016-
-00001da0: 3034 2d30 3120 3133 3a31 313a 3039 2c31  04-01 13:11:09,1
-00001db0: 3133 2072 6f6f 7420 2020 2020 2020 2020  13 root         
-00001dc0: 494e 464f 2020 2020 2053 7175 6173 6869  INFO     Squashi
-00001dd0: 6e67 2066 696c 6520 272f 746d 702f 646f  ng file '/tmp/do
-00001de0: 636b 6572 2d73 7175 6173 682d 6662 785a  cker-squash-fbxZ
-00001df0: 7a34 2f6f 6c64 2f62 3866 6133 6361 6637  z4/old/b8fa3caf7
-00001e00: 6436 6463 3232 3862 6632 3439 3961 3361  d6dc228bf2499a3a
-00001e10: 6638 3665 3530 3733 6164 3063 3137 3330  f86e5073ad0c1730
-00001e20: 3463 3339 3030 6661 3334 3165 3964 3266  4c3900fa341e9d2f
-00001e30: 6534 6535 3635 352f 6c61 7965 722e 7461  e4e5655/layer.ta
-00001e40: 7227 2e2e 2e0a 2020 2020 3230 3136 2d30  r'....    2016-0
-00001e50: 342d 3031 2031 333a 3131 3a30 392c 3131  4-01 13:11:09,11
-00001e60: 3520 726f 6f74 2020 2020 2020 2020 2049  5 root         I
-00001e70: 4e46 4f20 2020 2020 5371 7561 7368 696e  NFO     Squashin
-00001e80: 6720 6669 6c65 2027 2f74 6d70 2f64 6f63  g file '/tmp/doc
-00001e90: 6b65 722d 7371 7561 7368 2d66 6278 5a7a  ker-squash-fbxZz
-00001ea0: 342f 6f6c 642f 3338 6238 6638 3565 3734  4/old/38b8f85e74
-00001eb0: 6266 6137 3733 6130 6164 3639 6461 3232  bfa773a0ad69da22
-00001ec0: 3035 6463 3031 3438 3934 3565 3666 3561  05dc0148945e6f5a
-00001ed0: 3763 6562 3034 6661 3465 3836 3139 6531  7ceb04fa4e8619e1
-00001ee0: 6465 3432 3562 2f6c 6179 6572 2e74 6172  de425b/layer.tar
-00001ef0: 272e 2e2e 0a20 2020 2032 3031 362d 3034  '....    2016-04
-00001f00: 2d30 3120 3133 3a31 313a 3039 2c31 3135  -01 13:11:09,115
-00001f10: 2072 6f6f 7420 2020 2020 2020 2020 494e   root         IN
-00001f20: 464f 2020 2020 2053 7175 6173 6869 6e67  FO     Squashing
-00001f30: 2066 696c 6520 272f 746d 702f 646f 636b   file '/tmp/dock
-00001f40: 6572 2d73 7175 6173 682d 6662 785a 7a34  er-squash-fbxZz4
-00001f50: 2f6f 6c64 2f61 6537 3962 3634 3662 3961  /old/ae79b646b9a
-00001f60: 3961 3238 3763 3566 3661 3031 3837 3163  9a287c5f6a01871c
-00001f70: 6339 6439 6565 3539 3664 6166 6565 3264  c9d9ee596dafee2d
-00001f80: 6239 3432 3731 3463 6133 6465 6130 6330  b942714ca3dea0c0
-00001f90: 3665 6566 332f 6c61 7965 722e 7461 7227  6eef3/layer.tar'
-00001fa0: 2e2e 2e0a 2020 2020 3230 3136 2d30 342d  ....    2016-04-
-00001fb0: 3031 2031 333a 3131 3a30 392c 3131 3520  01 13:11:09,115 
-00001fc0: 726f 6f74 2020 2020 2020 2020 2049 4e46  root         INF
-00001fd0: 4f20 2020 2020 5371 7561 7368 696e 6720  O     Squashing 
-00001fe0: 6669 6c65 2027 2f74 6d70 2f64 6f63 6b65  file '/tmp/docke
-00001ff0: 722d 7371 7561 7368 2d66 6278 5a7a 342f  r-squash-fbxZz4/
-00002000: 6f6c 642f 3262 3436 3036 6463 3964 6337  old/2b4606dc9dc7
-00002010: 3733 6161 3232 3061 3635 3335 3166 6538  73aa220a65351fe8
-00002020: 6435 3466 3033 3533 3463 3538 6665 6132  d54f03534c58fea2
-00002030: 3330 3936 3065 3935 3931 3532 3232 3336  30960e9591522236
-00002040: 3630 3734 2f6c 6179 6572 2e74 6172 272e  6074/layer.tar'.
-00002050: 2e2e 0a20 2020 2032 3031 362d 3034 2d30  ...    2016-04-0
-00002060: 3120 3133 3a31 313a 3039 2c31 3135 2072  1 13:11:09,115 r
-00002070: 6f6f 7420 2020 2020 2020 2020 494e 464f  oot         INFO
-00002080: 2020 2020 2053 7175 6173 6869 6e67 2066       Squashing f
-00002090: 696c 6520 272f 746d 702f 646f 636b 6572  ile '/tmp/docker
-000020a0: 2d73 7175 6173 682d 6662 785a 7a34 2f6f  -squash-fbxZz4/o
-000020b0: 6c64 2f31 3138 6661 3965 3333 3537 3665  ld/118fa9e33576e
-000020c0: 6363 3632 3565 6262 6266 6466 3238 3039  cc625ebbbfdf2809
-000020d0: 6331 3532 3765 3731 3663 6234 6664 3563  c1527e716cb4fd5c
-000020e0: 6234 3035 3438 6562 3664 3335 3033 6137  b40548eb6d3503a7
-000020f0: 3561 392f 6c61 7965 722e 7461 7227 2e2e  5a9/layer.tar'..
-00002100: 2e0a 2020 2020 3230 3136 2d30 342d 3031  ..    2016-04-01
-00002110: 2031 333a 3131 3a30 392c 3131 3520 726f   13:11:09,115 ro
-00002120: 6f74 2020 2020 2020 2020 2049 4e46 4f20  ot         INFO 
-00002130: 2020 2020 5371 7561 7368 696e 6720 6669      Squashing fi
-00002140: 6c65 2027 2f74 6d70 2f64 6f63 6b65 722d  le '/tmp/docker-
-00002150: 7371 7561 7368 2d66 6278 5a7a 342f 6f6c  squash-fbxZz4/ol
-00002160: 642f 3566 3765 3866 3336 6333 6262 3230  d/5f7e8f36c3bb20
-00002170: 6339 6462 3734 3730 6132 3266 3832 3837  c9db7470a22f8287
-00002180: 3130 6234 6432 3861 6564 6536 3439 3636  10b4d28aede64966
-00002190: 6334 3235 6164 6434 3861 3162 3134 6665  c425add48a1b14fe
-000021a0: 3233 2f6c 6179 6572 2e74 6172 272e 2e2e  23/layer.tar'...
-000021b0: 0a20 2020 2032 3031 362d 3034 2d30 3120  .    2016-04-01 
-000021c0: 3133 3a31 313a 3130 2c31 3237 2072 6f6f  13:11:10,127 roo
-000021d0: 7420 2020 2020 2020 2020 494e 464f 2020  t         INFO  
-000021e0: 2020 2053 7175 6173 6869 6e67 2066 696c     Squashing fil
-000021f0: 6520 272f 746d 702f 646f 636b 6572 2d73  e '/tmp/docker-s
-00002200: 7175 6173 682d 6662 785a 7a34 2f6f 6c64  quash-fbxZz4/old
-00002210: 2f33 6434 6430 3232 3866 3136 3162 3637  /3d4d0228f161b67
-00002220: 6562 3436 6664 6234 3235 6164 3134 3863  eb46fdb425ad148c
-00002230: 3331 6439 3934 3464 6362 3832 3266 3637  31d9944dcb822f67
-00002240: 6561 6333 6532 6163 3265 6666 6566 6337  eac3e2ac2effefc7
-00002250: 332f 6c61 7965 722e 7461 7227 2e2e 2e0a  3/layer.tar'....
-00002260: 2020 2020 3230 3136 2d30 342d 3031 2031      2016-04-01 1
-00002270: 333a 3131 3a31 302c 3132 3920 726f 6f74  3:11:10,129 root
-00002280: 2020 2020 2020 2020 2049 4e46 4f20 2020           INFO   
-00002290: 2020 5371 7561 7368 696e 6720 6669 6c65    Squashing file
-000022a0: 2027 2f74 6d70 2f64 6f63 6b65 722d 7371   '/tmp/docker-sq
-000022b0: 7561 7368 2d66 6278 5a7a 342f 6f6c 642f  uash-fbxZz4/old/
-000022c0: 6637 6162 3465 6131 3937 3038 3461 6237  f7ab4ea197084ab7
-000022d0: 3438 3361 3263 6135 3430 3962 6463 6635  483a2ca5409bdcf5
-000022e0: 3437 3331 3431 6266 6236 3162 3836 3837  473141bfb61b8687
-000022f0: 6231 3332 3939 3433 3335 3963 6333 6665  b1329943359cc3fe
-00002300: 2f6c 6179 6572 2e74 6172 272e 2e2e 0a20  /layer.tar'.... 
-00002310: 2020 2032 3031 362d 3034 2d30 3120 3133     2016-04-01 13
-00002320: 3a31 313a 3130 2c37 3332 2072 6f6f 7420  :11:10,732 root 
-00002330: 2020 2020 2020 2020 494e 464f 2020 2020          INFO    
-00002340: 2053 7175 6173 6869 6e67 2066 696e 6973   Squashing finis
-00002350: 6865 6421 0a20 2020 2032 3031 362d 3034  hed!.    2016-04
-00002360: 2d30 3120 3133 3a31 313a 3130 2c37 3337  -01 13:11:10,737
-00002370: 2072 6f6f 7420 2020 2020 2020 2020 494e   root         IN
-00002380: 464f 2020 2020 204e 6577 2073 7175 6173  FO     New squas
-00002390: 6865 6420 696d 6167 6520 4944 2069 7320  hed image ID is 
-000023a0: 3532 3235 3565 3735 6433 6562 3833 3132  52255e75d3eb8312
-000023b0: 3365 3037 3466 3839 3765 3863 3937 3164  3e074f897e8c971d
-000023c0: 6563 3964 3131 3638 6135 6338 3264 3763  ec9d1168a5c82d7c
-000023d0: 3134 3936 6131 3930 6461 3265 3430 6566  1496a190da2e40ef
-000023e0: 0a20 2020 2032 3031 362d 3034 2d30 3120  .    2016-04-01 
-000023f0: 3133 3a31 313a 3134 2c35 3633 2072 6f6f  13:11:14,563 roo
-00002400: 7420 2020 2020 2020 2020 494e 464f 2020  t         INFO  
-00002410: 2020 2049 6d61 6765 2072 6567 6973 7465     Image registe
-00002420: 7265 6420 696e 2044 6f63 6b65 7220 6461  red in Docker da
-00002430: 656d 6f6e 2061 7320 6a62 6f73 732f 7769  emon as jboss/wi
-00002440: 6c64 666c 793a 7371 7561 7368 6564 0a20  ldfly:squashed. 
-00002450: 2020 2032 3031 362d 3034 2d30 3120 3133     2016-04-01 13
-00002460: 3a31 313a 3134 2c36 3532 2072 6f6f 7420  :11:14,652 root 
-00002470: 2020 2020 2020 2020 494e 464f 2020 2020          INFO    
-00002480: 2044 6f6e 650a 0a57 6520 6361 6e20 6e6f   Done..We can no
-00002490: 7720 636f 6e66 6972 6d20 7468 6520 6c61  w confirm the la
-000024a0: 7965 7220 7374 7275 6374 7572 653a 0a0a  yer structure:..
-000024b0: 3a3a 0a0a 2020 2020 2420 646f 636b 6572  ::..    $ docker
-000024c0: 2068 6973 746f 7279 206a 626f 7373 2f77   history jboss/w
-000024d0: 696c 6466 6c79 3a73 7175 6173 6865 640a  ildfly:squashed.
-000024e0: 2020 2020 494d 4147 4520 2020 2020 2020      IMAGE       
-000024f0: 2020 2020 2020 2020 4352 4541 5445 4420          CREATED 
-00002500: 2020 2020 2020 2020 2020 2020 4352 4541              CREA
-00002510: 5445 4420 4259 2020 2020 2020 2020 2020  TED BY          
+00000000: 6060 646f 636b 6572 2d73 7175 6173 6860  ``docker-squash`
+00000010: 600a 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  `.==============
+00000020: 3d3d 3d3d 0a0a 2e2e 2069 6d61 6765 3a3a  ====.... image::
+00000030: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
+00000040: 636f 6d2f 676f 6c64 6d61 6e6e 2f64 6f63  com/goldmann/doc
+00000050: 6b65 722d 7371 7561 7368 2f61 6374 696f  ker-squash/actio
+00000060: 6e73 2f77 6f72 6b66 6c6f 7773 2f73 7175  ns/workflows/squ
+00000070: 6173 682e 796d 6c2f 6261 6467 652e 7376  ash.yml/badge.sv
+00000080: 670a 2020 2020 3a74 6172 6765 743a 2068  g.    :target: h
+00000090: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+000000a0: 6d2f 676f 6c64 6d61 6e6e 2f64 6f63 6b65  m/goldmann/docke
+000000b0: 722d 7371 7561 7368 2f61 6374 696f 6e73  r-squash/actions
+000000c0: 2f77 6f72 6b66 6c6f 7773 2f73 7175 6173  /workflows/squas
+000000d0: 682e 796d 6c0a 0a54 6865 2070 726f 626c  h.yml..The probl
+000000e0: 656d 0a2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a0a  em.-----------..
+000000f0: 446f 636b 6572 2063 7265 6174 6573 206d  Docker creates m
+00000100: 616e 7920 6c61 7965 7273 2077 6869 6c65  any layers while
+00000110: 2062 7569 6c64 696e 6720 7468 6520 696d   building the im
+00000120: 6167 652e 2053 6f6d 6574 696d 6573 2069  age. Sometimes i
+00000130: 7427 7320 6e6f 7420 6e65 6365 7373 6172  t's not necessar
+00000140: 7920 6f72 2064 6573 6972 6561 626c 650a  y or desireable.
+00000150: 746f 2068 6176 6520 7468 656d 2069 6e20  to have them in 
+00000160: 7468 6520 696d 6167 652e 2046 6f72 2065  the image. For e
+00000170: 7861 6d70 6c65 2061 2044 6f63 6b65 7266  xample a Dockerf
+00000180: 696c 6520 6041 4444 6020 696e 7374 7275  ile `ADD` instru
+00000190: 6374 696f 6e20 6372 6561 7465 7320 6120  ction creates a 
+000001a0: 7369 6e67 6c65 206c 6179 6572 0a77 6974  single layer.wit
+000001b0: 6820 6669 6c65 7320 796f 7520 7761 6e74  h files you want
+000001c0: 2074 6f20 6d61 6b65 2061 7661 696c 6162   to make availab
+000001d0: 6c65 2069 6e20 7468 6520 696d 6167 652e  le in the image.
+000001e0: 2054 6865 2070 726f 626c 656d 2061 7269   The problem ari
+000001f0: 7365 7320 7768 656e 2074 6865 7365 2066  ses when these f
+00000200: 696c 6573 2061 7265 0a6f 6e6c 7920 7465  iles are.only te
+00000210: 6d70 6f72 6172 7920 6669 6c65 7320 2866  mporary files (f
+00000220: 6f72 2065 7861 6d70 6c65 2070 726f 6475  or example produ
+00000230: 6374 2064 6973 7472 6962 7574 696f 6e20  ct distribution 
+00000240: 7468 6174 2079 6f75 2077 616e 7420 746f  that you want to
+00000250: 2075 6e70 6163 6b29 2e20 446f 636b 6572   unpack). Docker
+00000260: 2077 696c 6c0a 6361 7272 7920 7468 6973   will.carry this
+00000270: 2075 6e6e 6563 6573 7361 7279 206c 6179   unnecessary lay
+00000280: 6572 2061 6c77 6179 7320 7769 7468 2074  er always with t
+00000290: 6865 2069 6d61 6765 2c20 6576 656e 2069  he image, even i
+000002a0: 6620 796f 7520 6465 6c65 7465 2074 6865  f you delete the
+000002b0: 7365 2066 696c 6573 2069 6e20 6e65 7874  se files in next
+000002c0: 0a6c 6179 6572 2e20 5468 6973 2061 2077  .layer. This a w
+000002d0: 6173 7465 206f 6620 7469 6d65 2028 6d6f  aste of time (mo
+000002e0: 7265 2064 6174 6120 746f 2070 7573 682f  re data to push/
+000002f0: 6c6f 6164 2f73 6176 6529 2061 6e64 2072  load/save) and r
+00000300: 6573 6f75 7263 6573 2028 6269 6767 6572  esources (bigger
+00000310: 2069 6d61 6765 292e 0a0a 5371 7561 7368   image)...Squash
+00000320: 696e 6720 6865 6c70 7320 7769 7468 206f  ing helps with o
+00000330: 7267 616e 697a 696e 6720 696d 6167 6573  rganizing images
+00000340: 2069 6e20 6c6f 6769 6361 6c20 6c61 7965   in logical laye
+00000350: 7273 2e20 496e 7374 6561 6420 6f66 0a68  rs. Instead of.h
+00000360: 6176 696e 6720 616e 2069 6d61 6765 2077  aving an image w
+00000370: 6974 6820 6d75 6c74 6970 6c65 2028 696e  ith multiple (in
+00000380: 2061 6c6d 6f73 7420 616c 6c20 6361 7365   almost all case
+00000390: 7329 2075 6e6e 6563 6573 7361 7279 206c  s) unnecessary l
+000003a0: 6179 6572 7320 2d0a 7765 2063 616e 2063  ayers -.we can c
+000003b0: 6f6e 7472 6f6c 2074 6865 2073 7472 7563  ontrol the struc
+000003c0: 7475 7265 206f 6620 7468 6520 696d 6167  ture of the imag
+000003d0: 652e 0a0a 4665 6174 7572 6573 0a2d 2d2d  e...Features.---
+000003e0: 2d2d 2d2d 2d0a 0a2d 2043 616e 2073 7175  -----..- Can squ
+000003f0: 6173 6820 6c61 7374 206e 206c 6179 6572  ash last n layer
+00000400: 7320 6672 6f6d 2061 6e20 696d 6167 650a  s from an image.
+00000410: 2d20 4361 6e20 7371 7561 7368 2066 726f  - Can squash fro
+00000420: 6d20 6120 7365 6c65 6374 6564 206c 6179  m a selected lay
+00000430: 6572 2074 6f20 7468 6520 656e 6420 286e  er to the end (n
+00000440: 6f74 2061 6c77 6179 7320 706f 7373 6962  ot always possib
+00000450: 6c65 2c20 6465 7065 6e64 7320 6f6e 2074  le, depends on t
+00000460: 6865 2069 6d61 6765 290a 2d20 5375 7070  he image).- Supp
+00000470: 6f72 7420 666f 7220 446f 636b 6572 2031  ort for Docker 1
+00000480: 2e39 206f 7220 6e65 7765 7220 286f 6c64  .9 or newer (old
+00000490: 6572 2072 656c 6561 7365 7320 6d61 7920  er releases may 
+000004a0: 7275 6e20 7065 7266 6563 746c 7920 6669  run perfectly fi
+000004b0: 6e65 2074 6f6f 2c20 7472 7920 6974 2129  ne too, try it!)
+000004c0: 0a2d 2053 7175 6173 6865 6420 696d 6167  .- Squashed imag
+000004d0: 6520 6361 6e20 6265 206c 6f61 6465 6420  e can be loaded 
+000004e0: 6261 636b 2074 6f20 7468 6520 446f 636b  back to the Dock
+000004f0: 6572 2064 6165 6d6f 6e20 6f72 2073 746f  er daemon or sto
+00000500: 7265 6420 6173 2074 6172 2061 7263 6869  red as tar archi
+00000510: 7665 2073 6f6d 6577 6865 7265 0a0a 496e  ve somewhere..In
+00000520: 7374 616c 6c61 7469 6f6e 0a2d 2d2d 2d2d  stallation.-----
+00000530: 2d2d 2d2d 2d2d 2d0a 0a46 726f 6d20 736f  -------..From so
+00000540: 7572 6365 2063 6f64 650a 0a3a 3a0a 0a20  urce code..::.. 
+00000550: 2020 2024 2070 6970 2069 6e73 7461 6c6c     $ pip install
+00000560: 202d 2d75 7365 7220 6874 7470 733a 2f2f   --user https://
+00000570: 6769 7468 7562 2e63 6f6d 2f67 6f6c 646d  github.com/goldm
+00000580: 616e 6e2f 646f 636b 6572 2d73 7175 6173  ann/docker-squas
+00000590: 682f 6172 6368 6976 652f 6d61 7374 6572  h/archive/master
+000005a0: 2e7a 6970 0a0a 4672 6f6d 2050 7950 690a  .zip..From PyPi.
+000005b0: 0a3a 3a0a 0a20 2020 2024 2070 6970 2069  .::..    $ pip i
+000005c0: 6e73 7461 6c6c 2064 6f63 6b65 722d 7371  nstall docker-sq
+000005d0: 7561 7368 0a0a 4974 2069 7320 7375 7070  uash..It is supp
+000005e0: 6f72 7465 6420 6f6e 2050 7974 686f 6e20  orted on Python 
+000005f0: 332e 3620 616e 6420 6162 6f76 652e 0a0a  3.6 and above...
+00000600: 5573 6167 650a 2d2d 2d2d 2d0a 0a3a 3a0a  Usage.-----..::.
+00000610: 0a20 2020 2024 2064 6f63 6b65 722d 7371  .    $ docker-sq
+00000620: 7561 7368 202d 680a 2020 2020 7573 6167  uash -h.    usag
+00000630: 653a 2063 6c69 2e70 7920 5b2d 685d 205b  e: cli.py [-h] [
+00000640: 2d76 5d20 5b2d 2d76 6572 7369 6f6e 5d20  -v] [--version] 
+00000650: 5b2d 645d 205b 2d66 2046 524f 4d5f 4c41  [-d] [-f FROM_LA
+00000660: 5945 525d 205b 2d74 2054 4147 5d0a 2020  YER] [-t TAG].  
+00000670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000680: 5b2d 2d74 6d70 2d64 6972 2054 4d50 5f44  [--tmp-dir TMP_D
+00000690: 4952 5d20 5b2d 2d6f 7574 7075 742d 7061  IR] [--output-pa
+000006a0: 7468 204f 5554 5055 545f 5041 5448 5d0a  th OUTPUT_PATH].
+000006b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000006c0: 2020 696d 6167 650a 0a20 2020 2044 6f63    image..    Doc
+000006d0: 6b65 7220 6c61 7965 7220 7371 7561 7368  ker layer squash
+000006e0: 696e 6720 746f 6f6c 0a0a 2020 2020 706f  ing tool..    po
+000006f0: 7369 7469 6f6e 616c 2061 7267 756d 656e  sitional argumen
+00000700: 7473 3a0a 2020 2020 2020 696d 6167 6520  ts:.      image 
+00000710: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000720: 496d 6167 6520 746f 2062 6520 7371 7561  Image to be squa
+00000730: 7368 6564 0a0a 2020 2020 6f70 7469 6f6e  shed..    option
+00000740: 616c 2061 7267 756d 656e 7473 3a0a 2020  al arguments:.  
+00000750: 2020 2020 2d68 2c20 2d2d 6865 6c70 2020      -h, --help  
+00000760: 2020 2020 2020 2020 2020 7368 6f77 2074            show t
+00000770: 6869 7320 6865 6c70 206d 6573 7361 6765  his help message
+00000780: 2061 6e64 2065 7869 740a 2020 2020 2020   and exit.      
+00000790: 2d76 2c20 2d2d 7665 7262 6f73 6520 2020  -v, --verbose   
+000007a0: 2020 2020 2020 5665 7262 6f73 6520 6f75        Verbose ou
+000007b0: 7470 7574 0a20 2020 2020 202d 2d76 6572  tput.      --ver
+000007c0: 7369 6f6e 2020 2020 2020 2020 2020 2020  sion            
+000007d0: 2053 686f 7720 7665 7273 696f 6e20 616e   Show version an
+000007e0: 6420 6578 6974 0a20 2020 2020 202d 642c  d exit.      -d,
+000007f0: 202d 2d64 6576 656c 6f70 6d65 6e74 2020   --development  
+00000800: 2020 2044 6f65 7320 6e6f 7420 636c 6561     Does not clea
+00000810: 6e20 7570 2061 6674 6572 2066 6169 6c75  n up after failu
+00000820: 7265 2066 6f72 2065 6173 6965 7220 6465  re for easier de
+00000830: 6275 6767 696e 670a 2020 2020 2020 2d66  bugging.      -f
+00000840: 2046 524f 4d5f 4c41 5945 522c 202d 2d66   FROM_LAYER, --f
+00000850: 726f 6d2d 6c61 7965 7220 4652 4f4d 5f4c  rom-layer FROM_L
+00000860: 4159 4552 0a20 2020 2020 2020 2020 2020  AYER.           
+00000870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000880: 204e 756d 6265 7220 6f66 206c 6179 6572   Number of layer
+00000890: 7320 746f 2073 7175 6173 6820 6f72 2049  s to squash or I
+000008a0: 4420 6f66 2074 6865 206c 6179 6572 2028  D of the layer (
+000008b0: 6f72 2069 6d61 6765 2049 4420 6f72 2069  or image ID or i
+000008c0: 6d61 6765 206e 616d 6529 2074 6f20 7371  mage name) to sq
+000008d0: 7561 7368 2066 726f 6d2e 0a20 2020 2020  uash from..     
+000008e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000008f0: 2020 2020 2020 2049 6e20 6361 7365 2074         In case t
+00000900: 6865 2070 726f 7669 6465 6420 7661 6c75  he provided valu
+00000910: 6520 6973 2061 6e20 696e 7465 6765 722c  e is an integer,
+00000920: 2073 7065 6369 6669 6564 206e 756d 6265   specified numbe
+00000930: 7220 6f66 206c 6179 6572 7320 7769 6c6c  r of layers will
+00000940: 2062 6520 7371 7561 7368 6564 2e0a 2020   be squashed..  
+00000950: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000960: 2020 2020 2020 2020 2020 4576 6572 7920            Every 
+00000970: 6c61 7965 7220 696e 2074 6865 2069 6d61  layer in the ima
+00000980: 6765 2077 696c 6c20 6265 2073 7175 6173  ge will be squas
+00000990: 6865 6420 6966 2074 6865 2070 6172 616d  hed if the param
+000009a0: 6574 6572 2069 7320 6e6f 7420 7072 6f76  eter is not prov
+000009b0: 6964 6564 2e0a 2020 2020 2020 2d74 2054  ided..      -t T
+000009c0: 4147 2c20 2d2d 7461 6720 5441 4720 2020  AG, --tag TAG   
+000009d0: 2020 5370 6563 6966 7920 7468 6520 7461    Specify the ta
+000009e0: 6720 746f 2062 6520 7573 6564 2066 6f72  g to be used for
+000009f0: 2074 6865 206e 6577 2069 6d61 6765 2e20   the new image. 
+00000a00: 4966 206e 6f74 2073 7065 6369 6669 6564  If not specified
+00000a10: 206e 6f20 7461 6720 7769 6c6c 2062 6520   no tag will be 
+00000a20: 6170 706c 6965 640a 2020 2020 2020 2d6d  applied.      -m
+00000a30: 204d 4553 5341 4745 2c20 2d2d 6d65 7373   MESSAGE, --mess
+00000a40: 6167 6520 4d45 5353 4147 450a 2020 2020  age MESSAGE.    
+00000a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000a60: 2020 2020 2020 2020 5370 6563 6966 7920          Specify 
+00000a70: 6120 636f 6d6d 6974 206d 6573 7361 6765  a commit message
+00000a80: 2028 636f 6d6d 656e 7429 2066 6f72 2074   (comment) for t
+00000a90: 6865 206e 6577 2069 6d61 6765 2e0a 2020  he new image..  
+00000aa0: 2020 2020 2d63 2c20 2d2d 636c 6561 6e75      -c, --cleanu
+00000ab0: 7020 2020 2020 2020 2020 5265 6d6f 7665  p         Remove
+00000ac0: 2073 6f75 7263 6520 696d 6167 6520 6672   source image fr
+00000ad0: 6f6d 2044 6f63 6b65 7220 6166 7465 7220  om Docker after 
+00000ae0: 7371 7561 7368 696e 670a 2020 2020 2020  squashing.      
+00000af0: 2d2d 746d 702d 6469 7220 544d 505f 4449  --tmp-dir TMP_DI
+00000b00: 5220 2020 2020 5465 6d70 6f72 6172 7920  R     Temporary 
+00000b10: 6469 7265 6374 6f72 7920 746f 2062 6520  directory to be 
+00000b20: 6372 6561 7465 6420 616e 6420 7573 6564  created and used
+00000b30: 0a20 2020 2020 202d 2d6f 7574 7075 742d  .      --output-
+00000b40: 7061 7468 204f 5554 5055 545f 5041 5448  path OUTPUT_PATH
+00000b50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000b60: 2020 2020 2020 2020 2020 2020 2050 6174               Pat
+00000b70: 6820 7768 6572 6520 7468 6520 696d 6167  h where the imag
+00000b80: 6520 6d61 7920 6265 2073 746f 7265 6420  e may be stored 
+00000b90: 6166 7465 7220 7371 7561 7368 696e 672e  after squashing.
+00000ba0: 0a20 2020 2020 202d 2d6c 6f61 642d 696d  .      --load-im
+00000bb0: 6167 6520 5b4c 4f41 445f 494d 4147 455d  age [LOAD_IMAGE]
+00000bc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000bd0: 2020 2020 2020 2020 2020 2020 2057 6865               Whe
+00000be0: 7468 6572 2074 6f20 6c6f 6164 2074 6865  ther to load the
+00000bf0: 2069 6d61 6765 2069 6e74 6f20 446f 636b   image into Dock
+00000c00: 6572 2064 6165 6d6f 6e20 6166 7465 7220  er daemon after 
+00000c10: 7371 7561 7368 696e 670a 2020 2020 2020  squashing.      
+00000c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000c30: 2020 2020 2020 4465 6661 756c 743a 2074        Default: t
+00000c40: 7275 650a 0a4e 6f74 6520 7468 6174 2065  rue..Note that e
+00000c50: 6e76 6972 6f6e 6d65 6e74 2076 6172 6961  nvironment varia
+00000c60: 626c 6573 206d 6179 2062 6520 7365 7420  bles may be set 
+00000c70: 6173 2064 6f63 756d 656e 7465 6420 696e  as documented in
+00000c80: 2060 6865 7265 203c 646f 6373 2f65 6e76   `here <docs/env
+00000c90: 6972 6f6e 6d65 6e74 5f76 6172 6961 626c  ironment_variabl
+00000ca0: 6573 2e61 646f 633e 605f 2e0a 0a4c 6963  es.adoc>`_...Lic
+00000cb0: 656e 7365 0a2d 2d2d 2d2d 2d2d 0a0a 4d49  ense.-------..MI
+00000cc0: 540a 0a45 7861 6d70 6c65 730a 2d2d 2d2d  T..Examples.----
+00000cd0: 2d2d 2d2d 0a0a 5765 2073 7461 7274 2077  ----..We start w
+00000ce0: 6974 6820 696d 6167 6520 6c69 6b65 2074  ith image like t
+00000cf0: 6869 733a 0a0a 3a3a 0a0a 2020 2020 2420  his:..::..    $ 
+00000d00: 646f 636b 6572 2068 6973 746f 7279 206a  docker history j
+00000d10: 626f 7373 2f77 696c 6466 6c79 3a6c 6174  boss/wildfly:lat
+00000d20: 6573 740a 2020 2020 494d 4147 4520 2020  est.    IMAGE   
+00000d30: 2020 2020 2020 2020 2020 2020 4352 4541              CREA
+00000d40: 5445 4420 2020 2020 2020 2020 2020 2020  TED             
+00000d50: 4352 4541 5445 4420 4259 2020 2020 2020  CREATED BY      
+00000d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000d80: 5349 5a45 2020 2020 2020 2020 2020 2020  SIZE            
+00000d90: 2020 2020 434f 4d4d 454e 540a 2020 2020      COMMENT.    
+00000da0: 3235 3935 3465 3664 3233 3030 2020 2020  25954e6d2300    
+00000db0: 2020 2020 3320 7765 656b 7320 6167 6f20      3 weeks ago 
+00000dc0: 2020 2020 2020 2020 2f62 696e 2f73 6820          /bin/sh 
+00000dd0: 2d63 2023 286e 6f70 2920 434d 4420 5b22  -c #(nop) CMD ["
+00000de0: 2f6f 7074 2f6a 626f 7373 2f77 696c 6466  /opt/jboss/wildf
+00000df0: 6c79 2f62 6920 2020 3020 420a 2020 2020  ly/bi   0 B.    
+00000e00: 3561 6536 3963 6234 3534 6135 2020 2020  5ae69cb454a5    
+00000e10: 2020 2020 3320 7765 656b 7320 6167 6f20      3 weeks ago 
+00000e20: 2020 2020 2020 2020 2f62 696e 2f73 6820          /bin/sh 
+00000e30: 2d63 2023 286e 6f70 2920 4558 504f 5345  -c #(nop) EXPOSE
+00000e40: 2038 3038 302f 7463 7020 2020 2020 2020   8080/tcp       
+00000e50: 2020 2020 2020 2020 3020 420a 2020 2020          0 B.    
+00000e60: 6463 3234 3731 3266 3335 6334 2020 2020  dc24712f35c4    
+00000e70: 2020 2020 3320 7765 656b 7320 6167 6f20      3 weeks ago 
+00000e80: 2020 2020 2020 2020 2f62 696e 2f73 6820          /bin/sh 
+00000e90: 2d63 2023 286e 6f70 2920 454e 5620 4c41  -c #(nop) ENV LA
+00000ea0: 554e 4348 5f4a 424f 5353 5f49 4e5f 4241  UNCH_JBOSS_IN_BA
+00000eb0: 434b 4752 4f20 2020 3020 420a 2020 2020  CKGRO   0 B.    
+00000ec0: 6439 3239 3132 3964 3463 3865 2020 2020  d929129d4c8e    
+00000ed0: 2020 2020 3320 7765 656b 7320 6167 6f20      3 weeks ago 
+00000ee0: 2020 2020 2020 2020 2f62 696e 2f73 6820          /bin/sh 
+00000ef0: 2d63 2063 6420 2448 4f4d 4520 2020 2020  -c cd $HOME     
+00000f00: 2626 2063 7572 6c20 2d4f 2068 7474 7073  && curl -O https
+00000f10: 3a2f 2f64 6f20 2020 3136 302e 3820 4d42  ://do   160.8 MB
+00000f20: 0a20 2020 2062 3866 6133 6361 6637 6436  .    b8fa3caf7d6
+00000f30: 6420 2020 2020 2020 2033 2077 6565 6b73  d        3 weeks
+00000f40: 2061 676f 2020 2020 2020 2020 202f 6269   ago         /bi
+00000f50: 6e2f 7368 202d 6320 2328 6e6f 7029 2045  n/sh -c #(nop) E
+00000f60: 4e56 204a 424f 5353 5f48 4f4d 453d 2f6f  NV JBOSS_HOME=/o
+00000f70: 7074 2f6a 626f 7373 2f77 2020 2030 2042  pt/jboss/w   0 B
+00000f80: 0a20 2020 2033 3862 3866 3835 6537 3462  .    38b8f85e74b
+00000f90: 6620 2020 2020 2020 2033 2077 6565 6b73  f        3 weeks
+00000fa0: 2061 676f 2020 2020 2020 2020 202f 6269   ago         /bi
+00000fb0: 6e2f 7368 202d 6320 2328 6e6f 7029 2045  n/sh -c #(nop) E
+00000fc0: 4e56 2057 494c 4446 4c59 5f53 4841 313d  NV WILDFLY_SHA1=
+00000fd0: 6330 6464 3735 3532 6335 2020 2030 2042  c0dd7552c5   0 B
+00000fe0: 0a20 2020 2061 6537 3962 3634 3662 3961  .    ae79b646b9a
+00000ff0: 3920 2020 2020 2020 2033 2077 6565 6b73  9        3 weeks
+00001000: 2061 676f 2020 2020 2020 2020 202f 6269   ago         /bi
+00001010: 6e2f 7368 202d 6320 2328 6e6f 7029 2045  n/sh -c #(nop) E
+00001020: 4e56 2057 494c 4446 4c59 5f56 4552 5349  NV WILDFLY_VERSI
+00001030: 4f4e 3d31 302e 302e 302e 2020 2030 2042  ON=10.0.0.   0 B
+00001040: 0a20 2020 2032 6234 3630 3664 6339 6463  .    2b4606dc9dc
+00001050: 3720 2020 2020 2020 2033 2077 6565 6b73  7        3 weeks
+00001060: 2061 676f 2020 2020 2020 2020 202f 6269   ago         /bi
+00001070: 6e2f 7368 202d 6320 2328 6e6f 7029 2045  n/sh -c #(nop) E
+00001080: 4e56 204a 4156 415f 484f 4d45 3d2f 7573  NV JAVA_HOME=/us
+00001090: 722f 6c69 622f 6a76 6d2f 2020 2030 2042  r/lib/jvm/   0 B
+000010a0: 0a20 2020 2031 3138 6661 3965 3333 3537  .    118fa9e3357
+000010b0: 3620 2020 2020 2020 2033 2077 6565 6b73  6        3 weeks
+000010c0: 2061 676f 2020 2020 2020 2020 202f 6269   ago         /bi
+000010d0: 6e2f 7368 202d 6320 2328 6e6f 7029 2055  n/sh -c #(nop) U
+000010e0: 5345 5220 5b6a 626f 7373 5d20 2020 2020  SER [jboss]     
+000010f0: 2020 2020 2020 2020 2020 2020 2030 2042               0 B
+00001100: 0a20 2020 2035 6637 6538 6633 3663 3362  .    5f7e8f36c3b
+00001110: 6220 2020 2020 2020 2033 2077 6565 6b73  b        3 weeks
+00001120: 2061 676f 2020 2020 2020 2020 202f 6269   ago         /bi
+00001130: 6e2f 7368 202d 6320 7975 6d20 2d79 2069  n/sh -c yum -y i
+00001140: 6e73 7461 6c6c 206a 6176 612d 312e 382e  nstall java-1.8.
+00001150: 302d 6f70 656e 6a64 6b2d 2020 2031 3937  0-openjdk-   197
+00001160: 2e34 204d 420a 2020 2020 3364 3464 3032  .4 MB.    3d4d02
+00001170: 3238 6631 3631 2020 2020 2020 2020 3320  28f161        3 
+00001180: 7765 656b 7320 6167 6f20 2020 2020 2020  weeks ago       
+00001190: 2020 2f62 696e 2f73 6820 2d63 2023 286e    /bin/sh -c #(n
+000011a0: 6f70 2920 5553 4552 205b 726f 6f74 5d20  op) USER [root] 
+000011b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000011c0: 2020 3020 420a 2020 2020 6637 6162 3465    0 B.    f7ab4e
+000011d0: 6131 3937 3038 2020 2020 2020 2020 3320  a19708        3 
+000011e0: 7765 656b 7320 6167 6f20 2020 2020 2020  weeks ago       
+000011f0: 2020 2f62 696e 2f73 6820 2d63 2023 286e    /bin/sh -c #(n
+00001200: 6f70 2920 4d41 494e 5441 494e 4552 204d  op) MAINTAINER M
+00001210: 6172 656b 2047 6f6c 646d 616e 6e20 3c20  arek Goldmann < 
+00001220: 2020 3020 420a 2020 2020 3462 6231 3566    0 B.    4bb15f
+00001230: 3362 3639 3737 2020 2020 2020 2020 3320  3b6977        3 
+00001240: 7765 656b 7320 6167 6f20 2020 2020 2020  weeks ago       
+00001250: 2020 2f62 696e 2f73 6820 2d63 2023 286e    /bin/sh -c #(n
+00001260: 6f70 2920 5553 4552 205b 6a62 6f73 735d  op) USER [jboss]
+00001270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001280: 2020 3020 420a 2020 2020 3564 6331 6534    0 B.    5dc1e4
+00001290: 3966 3433 3631 2020 2020 2020 2020 3320  9f4361        3 
+000012a0: 7765 656b 7320 6167 6f20 2020 2020 2020  weeks ago       
+000012b0: 2020 2f62 696e 2f73 6820 2d63 2023 286e    /bin/sh -c #(n
+000012c0: 6f70 2920 574f 524b 4449 5220 2f6f 7074  op) WORKDIR /opt
+000012d0: 2f6a 626f 7373 2020 2020 2020 2020 2020  /jboss          
+000012e0: 2020 3020 420a 2020 2020 3766 3066 3965    0 B.    7f0f9e
+000012f0: 6233 3131 3734 2020 2020 2020 2020 3320  b31174        3 
+00001300: 7765 656b 7320 6167 6f20 2020 2020 2020  weeks ago       
+00001310: 2020 2f62 696e 2f73 6820 2d63 2067 726f    /bin/sh -c gro
+00001320: 7570 6164 6420 2d72 206a 626f 7373 202d  upadd -r jboss -
+00001330: 6720 3130 3030 2026 2620 7573 6572 6120  g 1000 && usera 
+00001340: 2020 342e 3334 3920 6b42 0a20 2020 2062    4.349 kB.    b
+00001350: 6435 3135 6630 3434 6166 3720 2020 2020  d515f044af7     
+00001360: 2020 2033 2077 6565 6b73 2061 676f 2020     3 weeks ago  
+00001370: 2020 2020 2020 202f 6269 6e2f 7368 202d         /bin/sh -
+00001380: 6320 7975 6d20 7570 6461 7465 202d 7920  c yum update -y 
+00001390: 2626 2079 756d 202d 7920 696e 7374 616c  && yum -y instal
+000013a0: 6c20 786d 2020 2032 352e 3138 204d 420a  l xm   25.18 MB.
+000013b0: 2020 2020 6237 3833 3336 3039 3930 3435      b78336099045
+000013c0: 2020 2020 2020 2020 3320 7765 656b 7320          3 weeks 
+000013d0: 6167 6f20 2020 2020 2020 2020 2f62 696e  ago         /bin
+000013e0: 2f73 6820 2d63 2023 286e 6f70 2920 4d41  /sh -c #(nop) MA
+000013f0: 494e 5441 494e 4552 204d 6172 656b 2047  INTAINER Marek G
+00001400: 6f6c 646d 616e 6e20 3c20 2020 3020 420a  oldmann <   0 B.
+00001410: 2020 2020 3438 3136 6132 3938 3534 3863      4816a298548c
+00001420: 2020 2020 2020 2020 3320 7765 656b 7320          3 weeks 
+00001430: 6167 6f20 2020 2020 2020 2020 2f62 696e  ago         /bin
+00001440: 2f73 6820 2d63 2023 286e 6f70 2920 434d  /sh -c #(nop) CM
+00001450: 4420 5b22 2f62 696e 2f62 6173 6822 5d20  D ["/bin/bash"] 
+00001460: 2020 2020 2020 2020 2020 2020 3020 420a              0 B.
+00001470: 2020 2020 3665 6532 3335 6366 3434 3733      6ee235cf4473
+00001480: 2020 2020 2020 2020 3320 7765 656b 7320          3 weeks 
+00001490: 6167 6f20 2020 2020 2020 2020 2f62 696e  ago         /bin
+000014a0: 2f73 6820 2d63 2023 286e 6f70 2920 4c41  /sh -c #(nop) LA
+000014b0: 4245 4c20 6e61 6d65 3d43 656e 744f 5320  BEL name=CentOS 
+000014c0: 4261 7365 2049 6d61 6720 2020 3020 420a  Base Imag   0 B.
+000014d0: 2020 2020 3437 3463 3265 6537 3766 6133      474c2ee77fa3
+000014e0: 2020 2020 2020 2020 3320 7765 656b 7320          3 weeks 
+000014f0: 6167 6f20 2020 2020 2020 2020 2f62 696e  ago         /bin
+00001500: 2f73 6820 2d63 2023 286e 6f70 2920 4144  /sh -c #(nop) AD
+00001510: 4420 6669 6c65 3a37 3238 3532 6663 3736  D file:72852fc76
+00001520: 3236 6432 3333 3334 3320 2020 3139 362e  26d233343   196.
+00001530: 3620 4d42 0a20 2020 2031 3534 3430 3834  6 MB.    1544084
+00001540: 6661 6438 3120 2020 2020 2020 2036 206d  fad81        6 m
+00001550: 6f6e 7468 7320 6167 6f20 2020 2020 2020  onths ago       
+00001560: 202f 6269 6e2f 7368 202d 6320 2328 6e6f   /bin/sh -c #(no
+00001570: 7029 204d 4149 4e54 4149 4e45 5220 5468  p) MAINTAINER Th
+00001580: 6520 4365 6e74 4f53 2050 726f 6a65 2020  e CentOS Proje  
+00001590: 2030 2042 0a0a 416e 6420 7765 2077 616e   0 B..And we wan
+000015a0: 7420 746f 2073 7175 6173 6820 616c 6c20  t to squash all 
+000015b0: 7468 6520 6c61 7965 7273 2064 6f77 6e20  the layers down 
+000015c0: 746f 206c 6179 6572 2060 6034 6262 3135  to layer ``4bb15
+000015d0: 6633 6236 3937 3760 602e 0a0a 3a3a 0a0a  f3b6977``...::..
+000015e0: 2020 2020 2420 646f 636b 6572 2d73 7175      $ docker-squ
+000015f0: 6173 6820 2d66 2034 6262 3135 6633 6236  ash -f 4bb15f3b6
+00001600: 3937 3720 2d74 206a 626f 7373 2f77 696c  977 -t jboss/wil
+00001610: 6466 6c79 3a73 7175 6173 6865 6420 6a62  dfly:squashed jb
+00001620: 6f73 732f 7769 6c64 666c 793a 6c61 7465  oss/wildfly:late
+00001630: 7374 0a20 2020 2032 3031 362d 3034 2d30  st.    2016-04-0
+00001640: 3120 3133 3a31 313a 3032 2c33 3538 2072  1 13:11:02,358 r
+00001650: 6f6f 7420 2020 2020 2020 2020 494e 464f  oot         INFO
+00001660: 2020 2020 2064 6f63 6b65 722d 7363 7269       docker-scri
+00001670: 7074 7320 7665 7273 696f 6e20 312e 302e  pts version 1.0.
+00001680: 3064 6576 2c20 446f 636b 6572 2037 3230  0dev, Docker 720
+00001690: 3636 3231 2c20 4150 4920 312e 3231 2e2e  6621, API 1.21..
+000016a0: 2e0a 2020 2020 3230 3136 2d30 342d 3031  ..    2016-04-01
+000016b0: 2031 333a 3131 3a30 322c 3335 3820 726f   13:11:02,358 ro
+000016c0: 6f74 2020 2020 2020 2020 2049 4e46 4f20  ot         INFO 
+000016d0: 2020 2020 5573 696e 6720 7631 2069 6d61      Using v1 ima
+000016e0: 6765 2066 6f72 6d61 740a 2020 2020 3230  ge format.    20
+000016f0: 3136 2d30 342d 3031 2031 333a 3131 3a30  16-04-01 13:11:0
+00001700: 322c 3337 3420 726f 6f74 2020 2020 2020  2,374 root      
+00001710: 2020 2049 4e46 4f20 2020 2020 4f6c 6420     INFO     Old 
+00001720: 696d 6167 6520 6861 7320 3231 206c 6179  image has 21 lay
+00001730: 6572 730a 2020 2020 3230 3136 2d30 342d  ers.    2016-04-
+00001740: 3031 2031 333a 3131 3a30 322c 3337 3820  01 13:11:02,378 
+00001750: 726f 6f74 2020 2020 2020 2020 2049 4e46  root         INF
+00001760: 4f20 2020 2020 4368 6563 6b69 6e67 2069  O     Checking i
+00001770: 6620 7371 7561 7368 696e 6720 6973 206e  f squashing is n
+00001780: 6563 6573 7361 7279 2e2e 2e0a 2020 2020  ecessary....    
+00001790: 3230 3136 2d30 342d 3031 2031 333a 3131  2016-04-01 13:11
+000017a0: 3a30 322c 3337 3820 726f 6f74 2020 2020  :02,378 root    
+000017b0: 2020 2020 2049 4e46 4f20 2020 2020 4174       INFO     At
+000017c0: 7465 6d70 7469 6e67 2074 6f20 7371 7561  tempting to squa
+000017d0: 7368 206c 6173 7420 3132 206c 6179 6572  sh last 12 layer
+000017e0: 732e 2e2e 0a20 2020 2032 3031 362d 3034  s....    2016-04
+000017f0: 2d30 3120 3133 3a31 313a 3032 2c33 3738  -01 13:11:02,378
+00001800: 2072 6f6f 7420 2020 2020 2020 2020 494e   root         IN
+00001810: 464f 2020 2020 2053 6176 696e 6720 696d  FO     Saving im
+00001820: 6167 6520 3235 3935 3465 3664 3233 3030  age 25954e6d2300
+00001830: 3036 3233 3565 6563 6237 6630 6363 3536  06235eecb7f0cc56
+00001840: 3032 3634 6437 3331 3436 3938 3563 3264  0264d73146985c2d
+00001850: 3265 3636 3362 6163 3935 3364 3636 3062  2e663bac953d660b
+00001860: 3837 3330 2074 6f20 2f74 6d70 2f64 6f63  8730 to /tmp/doc
+00001870: 6b65 722d 7371 7561 7368 2d66 6278 5a7a  ker-squash-fbxZz
+00001880: 342f 6f6c 642f 696d 6167 652e 7461 7220  4/old/image.tar 
+00001890: 6669 6c65 2e2e 2e0a 2020 2020 3230 3136  file....    2016
+000018a0: 2d30 342d 3031 2031 333a 3131 3a30 382c  -04-01 13:11:08,
+000018b0: 3030 3320 726f 6f74 2020 2020 2020 2020  003 root        
+000018c0: 2049 4e46 4f20 2020 2020 496d 6167 6520   INFO     Image 
+000018d0: 7361 7665 6421 0a20 2020 2032 3031 362d  saved!.    2016-
+000018e0: 3034 2d30 3120 3133 3a31 313a 3038 2c30  04-01 13:11:08,0
+000018f0: 3331 2072 6f6f 7420 2020 2020 2020 2020  31 root         
+00001900: 494e 464f 2020 2020 2055 6e70 6163 6b69  INFO     Unpacki
+00001910: 6e67 202f 746d 702f 646f 636b 6572 2d73  ng /tmp/docker-s
+00001920: 7175 6173 682d 6662 785a 7a34 2f6f 6c64  quash-fbxZz4/old
+00001930: 2f69 6d61 6765 2e74 6172 2074 6172 2066  /image.tar tar f
+00001940: 696c 6520 746f 202f 746d 702f 646f 636b  ile to /tmp/dock
+00001950: 6572 2d73 7175 6173 682d 6662 785a 7a34  er-squash-fbxZz4
+00001960: 2f6f 6c64 2064 6972 6563 746f 7279 0a20  /old directory. 
+00001970: 2020 2032 3031 362d 3034 2d30 3120 3133     2016-04-01 13
+00001980: 3a31 313a 3038 2c35 3838 2072 6f6f 7420  :11:08,588 root 
+00001990: 2020 2020 2020 2020 494e 464f 2020 2020          INFO    
+000019a0: 2041 7263 6869 7665 2075 6e70 6163 6b65   Archive unpacke
+000019b0: 6421 0a20 2020 2032 3031 362d 3034 2d30  d!.    2016-04-0
+000019c0: 3120 3133 3a31 313a 3038 2c36 3336 2072  1 13:11:08,636 r
+000019d0: 6f6f 7420 2020 2020 2020 2020 494e 464f  oot         INFO
+000019e0: 2020 2020 2053 7175 6173 6869 6e67 2069       Squashing i
+000019f0: 6d61 6765 2027 6a62 6f73 732f 7769 6c64  mage 'jboss/wild
+00001a00: 666c 793a 6c61 7465 7374 272e 2e2e 0a20  fly:latest'.... 
+00001a10: 2020 2032 3031 362d 3034 2d30 3120 3133     2016-04-01 13
+00001a20: 3a31 313a 3038 2c36 3337 2072 6f6f 7420  :11:08,637 root 
+00001a30: 2020 2020 2020 2020 494e 464f 2020 2020          INFO    
+00001a40: 2053 7461 7274 696e 6720 7371 7561 7368   Starting squash
+00001a50: 696e 672e 2e2e 0a20 2020 2032 3031 362d  ing....    2016-
+00001a60: 3034 2d30 3120 3133 3a31 313a 3038 2c36  04-01 13:11:08,6
+00001a70: 3337 2072 6f6f 7420 2020 2020 2020 2020  37 root         
+00001a80: 494e 464f 2020 2020 2053 7175 6173 6869  INFO     Squashi
+00001a90: 6e67 2066 696c 6520 272f 746d 702f 646f  ng file '/tmp/do
+00001aa0: 636b 6572 2d73 7175 6173 682d 6662 785a  cker-squash-fbxZ
+00001ab0: 7a34 2f6f 6c64 2f32 3539 3534 6536 6432  z4/old/25954e6d2
+00001ac0: 3330 3030 3632 3335 6565 6362 3766 3063  30006235eecb7f0c
+00001ad0: 6335 3630 3236 3464 3733 3134 3639 3835  c560264d73146985
+00001ae0: 6332 6432 6536 3633 6261 6339 3533 6436  c2d2e663bac953d6
+00001af0: 3630 6238 3733 302f 6c61 7965 722e 7461  60b8730/layer.ta
+00001b00: 7227 2e2e 2e0a 2020 2020 3230 3136 2d30  r'....    2016-0
+00001b10: 342d 3031 2031 333a 3131 3a30 382c 3633  4-01 13:11:08,63
+00001b20: 3720 726f 6f74 2020 2020 2020 2020 2049  7 root         I
+00001b30: 4e46 4f20 2020 2020 5371 7561 7368 696e  NFO     Squashin
+00001b40: 6720 6669 6c65 2027 2f74 6d70 2f64 6f63  g file '/tmp/doc
+00001b50: 6b65 722d 7371 7561 7368 2d66 6278 5a7a  ker-squash-fbxZz
+00001b60: 342f 6f6c 642f 3561 6536 3963 6234 3534  4/old/5ae69cb454
+00001b70: 6135 6135 3432 6636 3365 3134 3863 6534  a5a542f63e148ce4
+00001b80: 3066 6239 6530 3164 6535 6262 3031 3830  0fb9e01de5bb0180
+00001b90: 3562 3464 6564 3233 3838 3431 6263 3263  5b4ded238841bc2c
+00001ba0: 6538 6538 3935 2f6c 6179 6572 2e74 6172  e8e895/layer.tar
+00001bb0: 272e 2e2e 0a20 2020 2032 3031 362d 3034  '....    2016-04
+00001bc0: 2d30 3120 3133 3a31 313a 3038 2c36 3337  -01 13:11:08,637
+00001bd0: 2072 6f6f 7420 2020 2020 2020 2020 494e   root         IN
+00001be0: 464f 2020 2020 2053 7175 6173 6869 6e67  FO     Squashing
+00001bf0: 2066 696c 6520 272f 746d 702f 646f 636b   file '/tmp/dock
+00001c00: 6572 2d73 7175 6173 682d 6662 785a 7a34  er-squash-fbxZz4
+00001c10: 2f6f 6c64 2f64 6332 3437 3132 6633 3563  /old/dc24712f35c
+00001c20: 3430 6539 3538 6265 3861 6361 3237 3331  40e958be8aca2731
+00001c30: 6537 6266 3833 3533 6239 6231 3862 6161  e7bf8353b9b18baa
+00001c40: 3661 3934 6164 3834 6336 3935 3263 6263  6a94ad84c6952cbc
+00001c50: 3737 3030 342f 6c61 7965 722e 7461 7227  77004/layer.tar'
+00001c60: 2e2e 2e0a 2020 2020 3230 3136 2d30 342d  ....    2016-04-
+00001c70: 3031 2031 333a 3131 3a30 382c 3633 3820  01 13:11:08,638 
+00001c80: 726f 6f74 2020 2020 2020 2020 2049 4e46  root         INF
+00001c90: 4f20 2020 2020 5371 7561 7368 696e 6720  O     Squashing 
+00001ca0: 6669 6c65 2027 2f74 6d70 2f64 6f63 6b65  file '/tmp/docke
+00001cb0: 722d 7371 7561 7368 2d66 6278 5a7a 342f  r-squash-fbxZz4/
+00001cc0: 6f6c 642f 6439 3239 3132 3964 3463 3865  old/d929129d4c8e
+00001cd0: 3631 6561 3336 3631 6562 3432 6333 3064  61ea3661eb42c30d
+00001ce0: 3031 6634 6331 3532 3431 3836 3839 3137  01f4c15241868917
+00001cf0: 3861 6663 3764 6338 3138 3561 3337 3831  8afc7dc8185a3781
+00001d00: 3435 3238 2f6c 6179 6572 2e74 6172 272e  4528/layer.tar'.
+00001d10: 2e2e 0a20 2020 2032 3031 362d 3034 2d30  ...    2016-04-0
+00001d20: 3120 3133 3a31 313a 3039 2c31 3133 2072  1 13:11:09,113 r
+00001d30: 6f6f 7420 2020 2020 2020 2020 494e 464f  oot         INFO
+00001d40: 2020 2020 2053 7175 6173 6869 6e67 2066       Squashing f
+00001d50: 696c 6520 272f 746d 702f 646f 636b 6572  ile '/tmp/docker
+00001d60: 2d73 7175 6173 682d 6662 785a 7a34 2f6f  -squash-fbxZz4/o
+00001d70: 6c64 2f62 3866 6133 6361 6637 6436 6463  ld/b8fa3caf7d6dc
+00001d80: 3232 3862 6632 3439 3961 3361 6638 3665  228bf2499a3af86e
+00001d90: 3530 3733 6164 3063 3137 3330 3463 3339  5073ad0c17304c39
+00001da0: 3030 6661 3334 3165 3964 3266 6534 6535  00fa341e9d2fe4e5
+00001db0: 3635 352f 6c61 7965 722e 7461 7227 2e2e  655/layer.tar'..
+00001dc0: 2e0a 2020 2020 3230 3136 2d30 342d 3031  ..    2016-04-01
+00001dd0: 2031 333a 3131 3a30 392c 3131 3520 726f   13:11:09,115 ro
+00001de0: 6f74 2020 2020 2020 2020 2049 4e46 4f20  ot         INFO 
+00001df0: 2020 2020 5371 7561 7368 696e 6720 6669      Squashing fi
+00001e00: 6c65 2027 2f74 6d70 2f64 6f63 6b65 722d  le '/tmp/docker-
+00001e10: 7371 7561 7368 2d66 6278 5a7a 342f 6f6c  squash-fbxZz4/ol
+00001e20: 642f 3338 6238 6638 3565 3734 6266 6137  d/38b8f85e74bfa7
+00001e30: 3733 6130 6164 3639 6461 3232 3035 6463  73a0ad69da2205dc
+00001e40: 3031 3438 3934 3565 3666 3561 3763 6562  0148945e6f5a7ceb
+00001e50: 3034 6661 3465 3836 3139 6531 6465 3432  04fa4e8619e1de42
+00001e60: 3562 2f6c 6179 6572 2e74 6172 272e 2e2e  5b/layer.tar'...
+00001e70: 0a20 2020 2032 3031 362d 3034 2d30 3120  .    2016-04-01 
+00001e80: 3133 3a31 313a 3039 2c31 3135 2072 6f6f  13:11:09,115 roo
+00001e90: 7420 2020 2020 2020 2020 494e 464f 2020  t         INFO  
+00001ea0: 2020 2053 7175 6173 6869 6e67 2066 696c     Squashing fil
+00001eb0: 6520 272f 746d 702f 646f 636b 6572 2d73  e '/tmp/docker-s
+00001ec0: 7175 6173 682d 6662 785a 7a34 2f6f 6c64  quash-fbxZz4/old
+00001ed0: 2f61 6537 3962 3634 3662 3961 3961 3238  /ae79b646b9a9a28
+00001ee0: 3763 3566 3661 3031 3837 3163 6339 6439  7c5f6a01871cc9d9
+00001ef0: 6565 3539 3664 6166 6565 3264 6239 3432  ee596dafee2db942
+00001f00: 3731 3463 6133 6465 6130 6330 3665 6566  714ca3dea0c06eef
+00001f10: 332f 6c61 7965 722e 7461 7227 2e2e 2e0a  3/layer.tar'....
+00001f20: 2020 2020 3230 3136 2d30 342d 3031 2031      2016-04-01 1
+00001f30: 333a 3131 3a30 392c 3131 3520 726f 6f74  3:11:09,115 root
+00001f40: 2020 2020 2020 2020 2049 4e46 4f20 2020           INFO   
+00001f50: 2020 5371 7561 7368 696e 6720 6669 6c65    Squashing file
+00001f60: 2027 2f74 6d70 2f64 6f63 6b65 722d 7371   '/tmp/docker-sq
+00001f70: 7561 7368 2d66 6278 5a7a 342f 6f6c 642f  uash-fbxZz4/old/
+00001f80: 3262 3436 3036 6463 3964 6337 3733 6161  2b4606dc9dc773aa
+00001f90: 3232 3061 3635 3335 3166 6538 6435 3466  220a65351fe8d54f
+00001fa0: 3033 3533 3463 3538 6665 6132 3330 3936  03534c58fea23096
+00001fb0: 3065 3935 3931 3532 3232 3336 3630 3734  0e95915222366074
+00001fc0: 2f6c 6179 6572 2e74 6172 272e 2e2e 0a20  /layer.tar'.... 
+00001fd0: 2020 2032 3031 362d 3034 2d30 3120 3133     2016-04-01 13
+00001fe0: 3a31 313a 3039 2c31 3135 2072 6f6f 7420  :11:09,115 root 
+00001ff0: 2020 2020 2020 2020 494e 464f 2020 2020          INFO    
+00002000: 2053 7175 6173 6869 6e67 2066 696c 6520   Squashing file 
+00002010: 272f 746d 702f 646f 636b 6572 2d73 7175  '/tmp/docker-squ
+00002020: 6173 682d 6662 785a 7a34 2f6f 6c64 2f31  ash-fbxZz4/old/1
+00002030: 3138 6661 3965 3333 3537 3665 6363 3632  18fa9e33576ecc62
+00002040: 3565 6262 6266 6466 3238 3039 6331 3532  5ebbbfdf2809c152
+00002050: 3765 3731 3663 6234 6664 3563 6234 3035  7e716cb4fd5cb405
+00002060: 3438 6562 3664 3335 3033 6137 3561 392f  48eb6d3503a75a9/
+00002070: 6c61 7965 722e 7461 7227 2e2e 2e0a 2020  layer.tar'....  
+00002080: 2020 3230 3136 2d30 342d 3031 2031 333a    2016-04-01 13:
+00002090: 3131 3a30 392c 3131 3520 726f 6f74 2020  11:09,115 root  
+000020a0: 2020 2020 2020 2049 4e46 4f20 2020 2020         INFO     
+000020b0: 5371 7561 7368 696e 6720 6669 6c65 2027  Squashing file '
+000020c0: 2f74 6d70 2f64 6f63 6b65 722d 7371 7561  /tmp/docker-squa
+000020d0: 7368 2d66 6278 5a7a 342f 6f6c 642f 3566  sh-fbxZz4/old/5f
+000020e0: 3765 3866 3336 6333 6262 3230 6339 6462  7e8f36c3bb20c9db
+000020f0: 3734 3730 6132 3266 3832 3837 3130 6234  7470a22f828710b4
+00002100: 6432 3861 6564 6536 3439 3636 6334 3235  d28aede64966c425
+00002110: 6164 6434 3861 3162 3134 6665 3233 2f6c  add48a1b14fe23/l
+00002120: 6179 6572 2e74 6172 272e 2e2e 0a20 2020  ayer.tar'....   
+00002130: 2032 3031 362d 3034 2d30 3120 3133 3a31   2016-04-01 13:1
+00002140: 313a 3130 2c31 3237 2072 6f6f 7420 2020  1:10,127 root   
+00002150: 2020 2020 2020 494e 464f 2020 2020 2053        INFO     S
+00002160: 7175 6173 6869 6e67 2066 696c 6520 272f  quashing file '/
+00002170: 746d 702f 646f 636b 6572 2d73 7175 6173  tmp/docker-squas
+00002180: 682d 6662 785a 7a34 2f6f 6c64 2f33 6434  h-fbxZz4/old/3d4
+00002190: 6430 3232 3866 3136 3162 3637 6562 3436  d0228f161b67eb46
+000021a0: 6664 6234 3235 6164 3134 3863 3331 6439  fdb425ad148c31d9
+000021b0: 3934 3464 6362 3832 3266 3637 6561 6333  944dcb822f67eac3
+000021c0: 6532 6163 3265 6666 6566 6337 332f 6c61  e2ac2effefc73/la
+000021d0: 7965 722e 7461 7227 2e2e 2e0a 2020 2020  yer.tar'....    
+000021e0: 3230 3136 2d30 342d 3031 2031 333a 3131  2016-04-01 13:11
+000021f0: 3a31 302c 3132 3920 726f 6f74 2020 2020  :10,129 root    
+00002200: 2020 2020 2049 4e46 4f20 2020 2020 5371       INFO     Sq
+00002210: 7561 7368 696e 6720 6669 6c65 2027 2f74  uashing file '/t
+00002220: 6d70 2f64 6f63 6b65 722d 7371 7561 7368  mp/docker-squash
+00002230: 2d66 6278 5a7a 342f 6f6c 642f 6637 6162  -fbxZz4/old/f7ab
+00002240: 3465 6131 3937 3038 3461 6237 3438 3361  4ea197084ab7483a
+00002250: 3263 6135 3430 3962 6463 6635 3437 3331  2ca5409bdcf54731
+00002260: 3431 6266 6236 3162 3836 3837 6231 3332  41bfb61b8687b132
+00002270: 3939 3433 3335 3963 6333 6665 2f6c 6179  9943359cc3fe/lay
+00002280: 6572 2e74 6172 272e 2e2e 0a20 2020 2032  er.tar'....    2
+00002290: 3031 362d 3034 2d30 3120 3133 3a31 313a  016-04-01 13:11:
+000022a0: 3130 2c37 3332 2072 6f6f 7420 2020 2020  10,732 root     
+000022b0: 2020 2020 494e 464f 2020 2020 2053 7175      INFO     Squ
+000022c0: 6173 6869 6e67 2066 696e 6973 6865 6421  ashing finished!
+000022d0: 0a20 2020 2032 3031 362d 3034 2d30 3120  .    2016-04-01 
+000022e0: 3133 3a31 313a 3130 2c37 3337 2072 6f6f  13:11:10,737 roo
+000022f0: 7420 2020 2020 2020 2020 494e 464f 2020  t         INFO  
+00002300: 2020 204e 6577 2073 7175 6173 6865 6420     New squashed 
+00002310: 696d 6167 6520 4944 2069 7320 3532 3235  image ID is 5225
+00002320: 3565 3735 6433 6562 3833 3132 3365 3037  5e75d3eb83123e07
+00002330: 3466 3839 3765 3863 3937 3164 6563 3964  4f897e8c971dec9d
+00002340: 3131 3638 6135 6338 3264 3763 3134 3936  1168a5c82d7c1496
+00002350: 6131 3930 6461 3265 3430 6566 0a20 2020  a190da2e40ef.   
+00002360: 2032 3031 362d 3034 2d30 3120 3133 3a31   2016-04-01 13:1
+00002370: 313a 3134 2c35 3633 2072 6f6f 7420 2020  1:14,563 root   
+00002380: 2020 2020 2020 494e 464f 2020 2020 2049        INFO     I
+00002390: 6d61 6765 2072 6567 6973 7465 7265 6420  mage registered 
+000023a0: 696e 2044 6f63 6b65 7220 6461 656d 6f6e  in Docker daemon
+000023b0: 2061 7320 6a62 6f73 732f 7769 6c64 666c   as jboss/wildfl
+000023c0: 793a 7371 7561 7368 6564 0a20 2020 2032  y:squashed.    2
+000023d0: 3031 362d 3034 2d30 3120 3133 3a31 313a  016-04-01 13:11:
+000023e0: 3134 2c36 3532 2072 6f6f 7420 2020 2020  14,652 root     
+000023f0: 2020 2020 494e 464f 2020 2020 2044 6f6e      INFO     Don
+00002400: 650a 0a57 6520 6361 6e20 6e6f 7720 636f  e..We can now co
+00002410: 6e66 6972 6d20 7468 6520 6c61 7965 7220  nfirm the layer 
+00002420: 7374 7275 6374 7572 653a 0a0a 3a3a 0a0a  structure:..::..
+00002430: 2020 2020 2420 646f 636b 6572 2068 6973      $ docker his
+00002440: 746f 7279 206a 626f 7373 2f77 696c 6466  tory jboss/wildf
+00002450: 6c79 3a73 7175 6173 6865 640a 2020 2020  ly:squashed.    
+00002460: 494d 4147 4520 2020 2020 2020 2020 2020  IMAGE           
+00002470: 2020 2020 4352 4541 5445 4420 2020 2020      CREATED     
+00002480: 2020 2020 2020 2020 4352 4541 5445 4420          CREATED 
+00002490: 4259 2020 2020 2020 2020 2020 2020 2020  BY              
+000024a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000024b0: 2020 2020 2020 2020 5349 5a45 2020 2020          SIZE    
+000024c0: 2020 2020 2020 2020 2020 2020 434f 4d4d              COMM
+000024d0: 454e 540a 2020 2020 3532 3235 3565 3735  ENT.    52255e75
+000024e0: 6433 6562 2020 2020 2020 2020 3430 2073  d3eb        40 s
+000024f0: 6563 6f6e 6473 2061 676f 2020 2020 2020  econds ago      
+00002500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002510: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00002520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002530: 2020 2020 2020 2020 2020 2020 5349 5a45              SIZE
-00002540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002550: 434f 4d4d 454e 540a 2020 2020 3532 3235  COMMENT.    5225
-00002560: 3565 3735 6433 6562 2020 2020 2020 2020  5e75d3eb        
-00002570: 3430 2073 6563 6f6e 6473 2061 676f 2020  40 seconds ago  
-00002580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000025a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000025b0: 2020 2020 3335 382e 3220 4d42 2020 2020      358.2 MB    
-000025c0: 2020 2020 2020 2020 0a20 2020 2034 6262          .    4bb
-000025d0: 3135 6633 6236 3937 3720 2020 2020 2020  15f3b6977       
-000025e0: 2033 2077 6565 6b73 2061 676f 2020 2020   3 weeks ago    
-000025f0: 2020 2020 202f 6269 6e2f 7368 202d 6320       /bin/sh -c 
-00002600: 2328 6e6f 7029 2055 5345 5220 5b6a 626f  #(nop) USER [jbo
-00002610: 7373 5d20 2020 2020 2020 2020 2020 2020  ss]             
-00002620: 2020 2020 2030 2042 2020 2020 2020 2020       0 B        
-00002630: 2020 2020 2020 2020 200a 2020 2020 3564           .    5d
-00002640: 6331 6534 3966 3433 3631 2020 2020 2020  c1e49f4361      
-00002650: 2020 3320 7765 656b 7320 6167 6f20 2020    3 weeks ago   
-00002660: 2020 2020 2020 2f62 696e 2f73 6820 2d63        /bin/sh -c
-00002670: 2023 286e 6f70 2920 574f 524b 4449 5220   #(nop) WORKDIR 
-00002680: 2f6f 7074 2f6a 626f 7373 2020 2020 2020  /opt/jboss      
-00002690: 2020 2020 2020 3020 4220 2020 2020 2020        0 B       
-000026a0: 2020 2020 2020 2020 2020 0a20 2020 2037            .    7
-000026b0: 6630 6639 6562 3331 3137 3420 2020 2020  f0f9eb31174     
-000026c0: 2020 2033 2077 6565 6b73 2061 676f 2020     3 weeks ago  
-000026d0: 2020 2020 2020 202f 6269 6e2f 7368 202d         /bin/sh -
-000026e0: 6320 6772 6f75 7061 6464 202d 7220 6a62  c groupadd -r jb
-000026f0: 6f73 7320 2d67 2031 3030 3020 2626 2075  oss -g 1000 && u
-00002700: 7365 7261 2020 2034 2e33 3439 206b 4220  sera   4.349 kB 
-00002710: 2020 2020 2020 2020 2020 200a 2020 2020             .    
-00002720: 6264 3531 3566 3034 3461 6637 2020 2020  bd515f044af7    
-00002730: 2020 2020 3320 7765 656b 7320 6167 6f20      3 weeks ago 
-00002740: 2020 2020 2020 2020 2f62 696e 2f73 6820          /bin/sh 
-00002750: 2d63 2079 756d 2075 7064 6174 6520 2d79  -c yum update -y
-00002760: 2026 2620 7975 6d20 2d79 2069 6e73 7461   && yum -y insta
-00002770: 6c6c 2078 6d20 2020 3235 2e31 3820 4d42  ll xm   25.18 MB
-00002780: 2020 2020 2020 2020 2020 2020 0a20 2020              .   
-00002790: 2062 3738 3333 3630 3939 3034 3520 2020   b78336099045   
-000027a0: 2020 2020 2033 2077 6565 6b73 2061 676f       3 weeks ago
-000027b0: 2020 2020 2020 2020 202f 6269 6e2f 7368           /bin/sh
-000027c0: 202d 6320 2328 6e6f 7029 204d 4149 4e54   -c #(nop) MAINT
-000027d0: 4149 4e45 5220 4d61 7265 6b20 476f 6c64  AINER Marek Gold
-000027e0: 6d61 6e6e 203c 2020 2030 2042 2020 2020  mann <   0 B    
-000027f0: 2020 2020 2020 2020 2020 2020 200a 2020               .  
-00002800: 2020 3438 3136 6132 3938 3534 3863 2020    4816a298548c  
-00002810: 2020 2020 2020 3320 7765 656b 7320 6167        3 weeks ag
-00002820: 6f20 2020 2020 2020 2020 2f62 696e 2f73  o         /bin/s
-00002830: 6820 2d63 2023 286e 6f70 2920 434d 4420  h -c #(nop) CMD 
-00002840: 5b22 2f62 696e 2f62 6173 6822 5d20 2020  ["/bin/bash"]   
-00002850: 2020 2020 2020 2020 2020 3020 4220 2020            0 B   
-00002860: 2020 2020 2020 2020 2020 2020 2020 0a20                . 
-00002870: 2020 2036 6565 3233 3563 6634 3437 3320     6ee235cf4473 
-00002880: 2020 2020 2020 2033 2077 6565 6b73 2061         3 weeks a
-00002890: 676f 2020 2020 2020 2020 202f 6269 6e2f  go         /bin/
-000028a0: 7368 202d 6320 2328 6e6f 7029 204c 4142  sh -c #(nop) LAB
-000028b0: 454c 206e 616d 653d 4365 6e74 4f53 2042  EL name=CentOS B
-000028c0: 6173 6520 496d 6167 2020 2030 2042 2020  ase Imag   0 B  
-000028d0: 2020 2020 2020 2020 2020 2020 2020 200a                 .
-000028e0: 2020 2020 3437 3463 3265 6537 3766 6133      474c2ee77fa3
-000028f0: 2020 2020 2020 2020 3320 7765 656b 7320          3 weeks 
-00002900: 6167 6f20 2020 2020 2020 2020 2f62 696e  ago         /bin
-00002910: 2f73 6820 2d63 2023 286e 6f70 2920 4144  /sh -c #(nop) AD
-00002920: 4420 6669 6c65 3a37 3238 3532 6663 3736  D file:72852fc76
-00002930: 3236 6432 3333 3334 3320 2020 3139 362e  26d233343   196.
-00002940: 3620 4d42 2020 2020 2020 2020 2020 2020  6 MB            
-00002950: 0a20 2020 2031 3534 3430 3834 6661 6438  .    1544084fad8
-00002960: 3120 2020 2020 2020 2036 206d 6f6e 7468  1        6 month
-00002970: 7320 6167 6f20 2020 2020 2020 202f 6269  s ago        /bi
-00002980: 6e2f 7368 202d 6320 2328 6e6f 7029 204d  n/sh -c #(nop) M
-00002990: 4149 4e54 4149 4e45 5220 5468 6520 4365  AINTAINER The Ce
-000029a0: 6e74 4f53 2050 726f 6a65 2020 2030 2042  ntOS Proje   0 B
-000029b0: 0a0a 4f74 6865 7220 6f70 7469 6f6e 2069  ..Other option i
-000029c0: 7320 746f 2073 7065 6369 6679 2068 6f77  s to specify how
-000029d0: 206d 616e 7920 6c61 7965 7273 2028 636f   many layers (co
-000029e0: 756e 7469 6e67 2066 726f 6d20 7468 6520  unting from the 
-000029f0: 6e65 7765 7374 206c 6179 6572 2920 7765  newest layer) we
-00002a00: 2077 616e 7420 746f 2073 7175 6173 682e   want to squash.
-00002a10: 5c0a 4c65 7427 7320 7371 7561 7368 206c  \.Let's squash l
-00002a20: 6173 7420 3130 206c 6179 6572 7320 6672  ast 10 layers fr
-00002a30: 6f6d 2074 6865 2060 606a 626f 7373 2f77  om the ``jboss/w
-00002a40: 696c 6466 6c79 3a6c 6174 6573 7460 6020  ildfly:latest`` 
-00002a50: 696d 6167 653a 0a0a 3a3a 0a0a 2020 2020  image:..::..    
-00002a60: 2420 646f 636b 6572 2d73 7175 6173 6820  $ docker-squash 
-00002a70: 2d66 2031 3020 2d74 206a 626f 7373 2f77  -f 10 -t jboss/w
-00002a80: 696c 6466 6c79 3a73 7175 6173 6865 6420  ildfly:squashed 
-00002a90: 6a62 6f73 732f 7769 6c64 666c 793a 6c61  jboss/wildfly:la
-00002aa0: 7465 7374 0a20 2020 2032 3031 362d 3034  test.    2016-04
-00002ab0: 2d30 3120 3133 3a31 353a 3036 2c34 3838  -01 13:15:06,488
-00002ac0: 2072 6f6f 7420 2020 2020 2020 2020 494e   root         IN
-00002ad0: 464f 2020 2020 2064 6f63 6b65 722d 7363  FO     docker-sc
-00002ae0: 7269 7074 7320 7665 7273 696f 6e20 312e  ripts version 1.
-00002af0: 302e 3064 6576 2c20 446f 636b 6572 2037  0.0dev, Docker 7
-00002b00: 3230 3636 3231 2c20 4150 4920 312e 3231  206621, API 1.21
-00002b10: 2e2e 2e0a 2020 2020 3230 3136 2d30 342d  ....    2016-04-
-00002b20: 3031 2031 333a 3135 3a30 362c 3438 3820  01 13:15:06,488 
-00002b30: 726f 6f74 2020 2020 2020 2020 2049 4e46  root         INF
-00002b40: 4f20 2020 2020 5573 696e 6720 7631 2069  O     Using v1 i
-00002b50: 6d61 6765 2066 6f72 6d61 740a 2020 2020  mage format.    
-00002b60: 3230 3136 2d30 342d 3031 2031 333a 3135  2016-04-01 13:15
-00002b70: 3a30 362c 3530 3420 726f 6f74 2020 2020  :06,504 root    
-00002b80: 2020 2020 2049 4e46 4f20 2020 2020 4f6c       INFO     Ol
-00002b90: 6420 696d 6167 6520 6861 7320 3231 206c  d image has 21 l
-00002ba0: 6179 6572 730a 2020 2020 3230 3136 2d30  ayers.    2016-0
-00002bb0: 342d 3031 2031 333a 3135 3a30 362c 3530  4-01 13:15:06,50
-00002bc0: 3420 726f 6f74 2020 2020 2020 2020 2049  4 root         I
-00002bd0: 4e46 4f20 2020 2020 4368 6563 6b69 6e67  NFO     Checking
-00002be0: 2069 6620 7371 7561 7368 696e 6720 6973   if squashing is
-00002bf0: 206e 6563 6573 7361 7279 2e2e 2e0a 2020   necessary....  
-00002c00: 2020 3230 3136 2d30 342d 3031 2031 333a    2016-04-01 13:
-00002c10: 3135 3a30 362c 3530 3420 726f 6f74 2020  15:06,504 root  
-00002c20: 2020 2020 2020 2049 4e46 4f20 2020 2020         INFO     
-00002c30: 4174 7465 6d70 7469 6e67 2074 6f20 7371  Attempting to sq
-00002c40: 7561 7368 206c 6173 7420 3130 206c 6179  uash last 10 lay
-00002c50: 6572 732e 2e2e 0a20 2020 2032 3031 362d  ers....    2016-
-00002c60: 3034 2d30 3120 3133 3a31 353a 3036 2c35  04-01 13:15:06,5
-00002c70: 3035 2072 6f6f 7420 2020 2020 2020 2020  05 root         
-00002c80: 494e 464f 2020 2020 2053 6176 696e 6720  INFO     Saving 
-00002c90: 696d 6167 6520 3235 3935 3465 3664 3233  image 25954e6d23
-00002ca0: 3030 3036 3233 3565 6563 6237 6630 6363  0006235eecb7f0cc
-00002cb0: 3536 3032 3634 6437 3331 3436 3938 3563  560264d73146985c
-00002cc0: 3264 3265 3636 3362 6163 3935 3364 3636  2d2e663bac953d66
-00002cd0: 3062 3837 3330 2074 6f20 2f74 6d70 2f64  0b8730 to /tmp/d
-00002ce0: 6f63 6b65 722d 7371 7561 7368 2d66 7538  ocker-squash-fu8
-00002cf0: 3043 582f 6f6c 642f 696d 6167 652e 7461  0CX/old/image.ta
-00002d00: 7220 6669 6c65 2e2e 2e0a 2020 2020 3230  r file....    20
-00002d10: 3136 2d30 342d 3031 2031 333a 3135 3a31  16-04-01 13:15:1
-00002d20: 322c 3133 3620 726f 6f74 2020 2020 2020  2,136 root      
-00002d30: 2020 2049 4e46 4f20 2020 2020 496d 6167     INFO     Imag
-00002d40: 6520 7361 7665 6421 0a20 2020 2032 3031  e saved!.    201
-00002d50: 362d 3034 2d30 3120 3133 3a31 353a 3132  6-04-01 13:15:12
-00002d60: 2c31 3637 2072 6f6f 7420 2020 2020 2020  ,167 root       
-00002d70: 2020 494e 464f 2020 2020 2055 6e70 6163    INFO     Unpac
-00002d80: 6b69 6e67 202f 746d 702f 646f 636b 6572  king /tmp/docker
-00002d90: 2d73 7175 6173 682d 6675 3830 4358 2f6f  -squash-fu80CX/o
-00002da0: 6c64 2f69 6d61 6765 2e74 6172 2074 6172  ld/image.tar tar
-00002db0: 2066 696c 6520 746f 202f 746d 702f 646f   file to /tmp/do
-00002dc0: 636b 6572 2d73 7175 6173 682d 6675 3830  cker-squash-fu80
-00002dd0: 4358 2f6f 6c64 2064 6972 6563 746f 7279  CX/old directory
-00002de0: 0a20 2020 2032 3031 362d 3034 2d30 3120  .    2016-04-01 
-00002df0: 3133 3a31 353a 3132 2c37 3036 2072 6f6f  13:15:12,706 roo
-00002e00: 7420 2020 2020 2020 2020 494e 464f 2020  t         INFO  
-00002e10: 2020 2041 7263 6869 7665 2075 6e70 6163     Archive unpac
-00002e20: 6b65 6421 0a20 2020 2032 3031 362d 3034  ked!.    2016-04
-00002e30: 2d30 3120 3133 3a31 353a 3132 2c37 3536  -01 13:15:12,756
-00002e40: 2072 6f6f 7420 2020 2020 2020 2020 494e   root         IN
-00002e50: 464f 2020 2020 2053 7175 6173 6869 6e67  FO     Squashing
-00002e60: 2069 6d61 6765 2027 6a62 6f73 732f 7769   image 'jboss/wi
-00002e70: 6c64 666c 793a 6c61 7465 7374 272e 2e2e  ldfly:latest'...
-00002e80: 0a20 2020 2032 3031 362d 3034 2d30 3120  .    2016-04-01 
-00002e90: 3133 3a31 353a 3132 2c37 3536 2072 6f6f  13:15:12,756 roo
-00002ea0: 7420 2020 2020 2020 2020 494e 464f 2020  t         INFO  
-00002eb0: 2020 2053 7461 7274 696e 6720 7371 7561     Starting squa
-00002ec0: 7368 696e 672e 2e2e 0a20 2020 2032 3031  shing....    201
-00002ed0: 362d 3034 2d30 3120 3133 3a31 353a 3132  6-04-01 13:15:12
-00002ee0: 2c37 3536 2072 6f6f 7420 2020 2020 2020  ,756 root       
-00002ef0: 2020 494e 464f 2020 2020 2053 7175 6173    INFO     Squas
-00002f00: 6869 6e67 2066 696c 6520 272f 746d 702f  hing file '/tmp/
-00002f10: 646f 636b 6572 2d73 7175 6173 682d 6675  docker-squash-fu
-00002f20: 3830 4358 2f6f 6c64 2f32 3539 3534 6536  80CX/old/25954e6
-00002f30: 6432 3330 3030 3632 3335 6565 6362 3766  d230006235eecb7f
-00002f40: 3063 6335 3630 3236 3464 3733 3134 3639  0cc560264d731469
-00002f50: 3835 6332 6432 6536 3633 6261 6339 3533  85c2d2e663bac953
-00002f60: 6436 3630 6238 3733 302f 6c61 7965 722e  d660b8730/layer.
-00002f70: 7461 7227 2e2e 2e0a 2020 2020 3230 3136  tar'....    2016
-00002f80: 2d30 342d 3031 2031 333a 3135 3a31 322c  -04-01 13:15:12,
-00002f90: 3735 3720 726f 6f74 2020 2020 2020 2020  757 root        
-00002fa0: 2049 4e46 4f20 2020 2020 5371 7561 7368   INFO     Squash
-00002fb0: 696e 6720 6669 6c65 2027 2f74 6d70 2f64  ing file '/tmp/d
-00002fc0: 6f63 6b65 722d 7371 7561 7368 2d66 7538  ocker-squash-fu8
-00002fd0: 3043 582f 6f6c 642f 3561 6536 3963 6234  0CX/old/5ae69cb4
-00002fe0: 3534 6135 6135 3432 6636 3365 3134 3863  54a5a542f63e148c
-00002ff0: 6534 3066 6239 6530 3164 6535 6262 3031  e40fb9e01de5bb01
-00003000: 3830 3562 3464 6564 3233 3838 3431 6263  805b4ded238841bc
-00003010: 3263 6538 6538 3935 2f6c 6179 6572 2e74  2ce8e895/layer.t
-00003020: 6172 272e 2e2e 0a20 2020 2032 3031 362d  ar'....    2016-
-00003030: 3034 2d30 3120 3133 3a31 353a 3132 2c37  04-01 13:15:12,7
-00003040: 3537 2072 6f6f 7420 2020 2020 2020 2020  57 root         
-00003050: 494e 464f 2020 2020 2053 7175 6173 6869  INFO     Squashi
-00003060: 6e67 2066 696c 6520 272f 746d 702f 646f  ng file '/tmp/do
-00003070: 636b 6572 2d73 7175 6173 682d 6675 3830  cker-squash-fu80
-00003080: 4358 2f6f 6c64 2f64 6332 3437 3132 6633  CX/old/dc24712f3
-00003090: 3563 3430 6539 3538 6265 3861 6361 3237  5c40e958be8aca27
-000030a0: 3331 6537 6266 3833 3533 6239 6231 3862  31e7bf8353b9b18b
-000030b0: 6161 3661 3934 6164 3834 6336 3935 3263  aa6a94ad84c6952c
-000030c0: 6263 3737 3030 342f 6c61 7965 722e 7461  bc77004/layer.ta
-000030d0: 7227 2e2e 2e0a 2020 2020 3230 3136 2d30  r'....    2016-0
-000030e0: 342d 3031 2031 333a 3135 3a31 322c 3735  4-01 13:15:12,75
-000030f0: 3720 726f 6f74 2020 2020 2020 2020 2049  7 root         I
-00003100: 4e46 4f20 2020 2020 5371 7561 7368 696e  NFO     Squashin
-00003110: 6720 6669 6c65 2027 2f74 6d70 2f64 6f63  g file '/tmp/doc
-00003120: 6b65 722d 7371 7561 7368 2d66 7538 3043  ker-squash-fu80C
-00003130: 582f 6f6c 642f 6439 3239 3132 3964 3463  X/old/d929129d4c
-00003140: 3865 3631 6561 3336 3631 6562 3432 6333  8e61ea3661eb42c3
-00003150: 3064 3031 6634 6331 3532 3431 3836 3839  0d01f4c152418689
-00003160: 3137 3861 6663 3764 6338 3138 3561 3337  178afc7dc8185a37
-00003170: 3831 3435 3238 2f6c 6179 6572 2e74 6172  814528/layer.tar
-00003180: 272e 2e2e 0a20 2020 2032 3031 362d 3034  '....    2016-04
-00003190: 2d30 3120 3133 3a31 353a 3133 2c32 3334  -01 13:15:13,234
-000031a0: 2072 6f6f 7420 2020 2020 2020 2020 494e   root         IN
-000031b0: 464f 2020 2020 2053 7175 6173 6869 6e67  FO     Squashing
-000031c0: 2066 696c 6520 272f 746d 702f 646f 636b   file '/tmp/dock
-000031d0: 6572 2d73 7175 6173 682d 6675 3830 4358  er-squash-fu80CX
-000031e0: 2f6f 6c64 2f62 3866 6133 6361 6637 6436  /old/b8fa3caf7d6
-000031f0: 6463 3232 3862 6632 3439 3961 3361 6638  dc228bf2499a3af8
-00003200: 3665 3530 3733 6164 3063 3137 3330 3463  6e5073ad0c17304c
-00003210: 3339 3030 6661 3334 3165 3964 3266 6534  3900fa341e9d2fe4
-00003220: 6535 3635 352f 6c61 7965 722e 7461 7227  e5655/layer.tar'
-00003230: 2e2e 2e0a 2020 2020 3230 3136 2d30 342d  ....    2016-04-
-00003240: 3031 2031 333a 3135 3a31 332c 3233 3520  01 13:15:13,235 
-00003250: 726f 6f74 2020 2020 2020 2020 2049 4e46  root         INF
-00003260: 4f20 2020 2020 5371 7561 7368 696e 6720  O     Squashing 
-00003270: 6669 6c65 2027 2f74 6d70 2f64 6f63 6b65  file '/tmp/docke
-00003280: 722d 7371 7561 7368 2d66 7538 3043 582f  r-squash-fu80CX/
-00003290: 6f6c 642f 3338 6238 6638 3565 3734 6266  old/38b8f85e74bf
-000032a0: 6137 3733 6130 6164 3639 6461 3232 3035  a773a0ad69da2205
-000032b0: 6463 3031 3438 3934 3565 3666 3561 3763  dc0148945e6f5a7c
-000032c0: 6562 3034 6661 3465 3836 3139 6531 6465  eb04fa4e8619e1de
-000032d0: 3432 3562 2f6c 6179 6572 2e74 6172 272e  425b/layer.tar'.
-000032e0: 2e2e 0a20 2020 2032 3031 362d 3034 2d30  ...    2016-04-0
-000032f0: 3120 3133 3a31 353a 3133 2c32 3335 2072  1 13:15:13,235 r
-00003300: 6f6f 7420 2020 2020 2020 2020 494e 464f  oot         INFO
-00003310: 2020 2020 2053 7175 6173 6869 6e67 2066       Squashing f
-00003320: 696c 6520 272f 746d 702f 646f 636b 6572  ile '/tmp/docker
-00003330: 2d73 7175 6173 682d 6675 3830 4358 2f6f  -squash-fu80CX/o
-00003340: 6c64 2f61 6537 3962 3634 3662 3961 3961  ld/ae79b646b9a9a
-00003350: 3238 3763 3566 3661 3031 3837 3163 6339  287c5f6a01871cc9
-00003360: 6439 6565 3539 3664 6166 6565 3264 6239  d9ee596dafee2db9
-00003370: 3432 3731 3463 6133 6465 6130 6330 3665  42714ca3dea0c06e
-00003380: 6566 332f 6c61 7965 722e 7461 7227 2e2e  ef3/layer.tar'..
-00003390: 2e0a 2020 2020 3230 3136 2d30 342d 3031  ..    2016-04-01
-000033a0: 2031 333a 3135 3a31 332c 3233 3520 726f   13:15:13,235 ro
-000033b0: 6f74 2020 2020 2020 2020 2049 4e46 4f20  ot         INFO 
-000033c0: 2020 2020 5371 7561 7368 696e 6720 6669      Squashing fi
-000033d0: 6c65 2027 2f74 6d70 2f64 6f63 6b65 722d  le '/tmp/docker-
-000033e0: 7371 7561 7368 2d66 7538 3043 582f 6f6c  squash-fu80CX/ol
-000033f0: 642f 3262 3436 3036 6463 3964 6337 3733  d/2b4606dc9dc773
-00003400: 6161 3232 3061 3635 3335 3166 6538 6435  aa220a65351fe8d5
-00003410: 3466 3033 3533 3463 3538 6665 6132 3330  4f03534c58fea230
-00003420: 3936 3065 3935 3931 3532 3232 3336 3630  960e959152223660
-00003430: 3734 2f6c 6179 6572 2e74 6172 272e 2e2e  74/layer.tar'...
-00003440: 0a20 2020 2032 3031 362d 3034 2d30 3120  .    2016-04-01 
-00003450: 3133 3a31 353a 3133 2c32 3336 2072 6f6f  13:15:13,236 roo
-00003460: 7420 2020 2020 2020 2020 494e 464f 2020  t         INFO  
-00003470: 2020 2053 7175 6173 6869 6e67 2066 696c     Squashing fil
-00003480: 6520 272f 746d 702f 646f 636b 6572 2d73  e '/tmp/docker-s
-00003490: 7175 6173 682d 6675 3830 4358 2f6f 6c64  quash-fu80CX/old
-000034a0: 2f31 3138 6661 3965 3333 3537 3665 6363  /118fa9e33576ecc
-000034b0: 3632 3565 6262 6266 6466 3238 3039 6331  625ebbbfdf2809c1
-000034c0: 3532 3765 3731 3663 6234 6664 3563 6234  527e716cb4fd5cb4
-000034d0: 3035 3438 6562 3664 3335 3033 6137 3561  0548eb6d3503a75a
-000034e0: 392f 6c61 7965 722e 7461 7227 2e2e 2e0a  9/layer.tar'....
-000034f0: 2020 2020 3230 3136 2d30 342d 3031 2031      2016-04-01 1
-00003500: 333a 3135 3a31 332c 3233 3620 726f 6f74  3:15:13,236 root
-00003510: 2020 2020 2020 2020 2049 4e46 4f20 2020           INFO   
-00003520: 2020 5371 7561 7368 696e 6720 6669 6c65    Squashing file
-00003530: 2027 2f74 6d70 2f64 6f63 6b65 722d 7371   '/tmp/docker-sq
-00003540: 7561 7368 2d66 7538 3043 582f 6f6c 642f  uash-fu80CX/old/
-00003550: 3566 3765 3866 3336 6333 6262 3230 6339  5f7e8f36c3bb20c9
-00003560: 6462 3734 3730 6132 3266 3832 3837 3130  db7470a22f828710
-00003570: 6234 6432 3861 6564 6536 3439 3636 6334  b4d28aede64966c4
-00003580: 3235 6164 6434 3861 3162 3134 6665 3233  25add48a1b14fe23
-00003590: 2f6c 6179 6572 2e74 6172 272e 2e2e 0a20  /layer.tar'.... 
-000035a0: 2020 2032 3031 362d 3034 2d30 3120 3133     2016-04-01 13
-000035b0: 3a31 353a 3134 2c38 3438 2072 6f6f 7420  :15:14,848 root 
-000035c0: 2020 2020 2020 2020 494e 464f 2020 2020          INFO    
-000035d0: 2053 7175 6173 6869 6e67 2066 696e 6973   Squashing finis
-000035e0: 6865 6421 0a20 2020 2032 3031 362d 3034  hed!.    2016-04
-000035f0: 2d30 3120 3133 3a31 353a 3134 2c38 3533  -01 13:15:14,853
-00003600: 2072 6f6f 7420 2020 2020 2020 2020 494e   root         IN
-00003610: 464f 2020 2020 204e 6577 2073 7175 6173  FO     New squas
-00003620: 6865 6420 696d 6167 6520 4944 2069 7320  hed image ID is 
-00003630: 6664 6537 6564 6432 6535 3638 3363 3937  fde7edd2e5683c97
-00003640: 6265 6466 3963 3062 6635 3261 6435 3135  bedf9c0bf52ad515
-00003650: 3064 6235 3635 3065 3432 3164 6533 6439  0db5650e421de3d9
-00003660: 3239 3363 6535 3232 3362 3235 3634 3535  293ce5223b256455
-00003670: 0a20 2020 2032 3031 362d 3034 2d30 3120  .    2016-04-01 
-00003680: 3133 3a31 353a 3138 2c39 3633 2072 6f6f  13:15:18,963 roo
-00003690: 7420 2020 2020 2020 2020 494e 464f 2020  t         INFO  
-000036a0: 2020 2049 6d61 6765 2072 6567 6973 7465     Image registe
-000036b0: 7265 6420 696e 2044 6f63 6b65 7220 6461  red in Docker da
-000036c0: 656d 6f6e 2061 7320 6a62 6f73 732f 7769  emon as jboss/wi
-000036d0: 6c64 666c 793a 7371 7561 7368 6564 0a20  ldfly:squashed. 
-000036e0: 2020 2032 3031 362d 3034 2d30 3120 3133     2016-04-01 13
-000036f0: 3a31 353a 3139 2c30 3539 2072 6f6f 7420  :15:19,059 root 
-00003700: 2020 2020 2020 2020 494e 464f 2020 2020          INFO    
-00003710: 2044 6f6e 650a 0a4c 6574 2773 2063 6f6e   Done..Let's con
-00003720: 6669 726d 2074 6865 2069 6d61 6765 2073  firm the image s
-00003730: 7472 7563 7475 7265 206e 6f77 3a0a 0a3a  tructure now:..:
-00003740: 3a0a 0a20 2020 2024 2064 6f63 6b65 7220  :..    $ docker 
-00003750: 6869 7374 6f72 7920 6a62 6f73 732f 7769  history jboss/wi
-00003760: 6c64 666c 793a 7371 7561 7368 6564 0a20  ldfly:squashed. 
-00003770: 2020 2049 4d41 4745 2020 2020 2020 2020     IMAGE        
-00003780: 2020 2020 2020 2043 5245 4154 4544 2020         CREATED  
-00003790: 2020 2020 2020 2020 2020 2043 5245 4154             CREAT
-000037a0: 4544 2042 5920 2020 2020 2020 2020 2020  ED BY           
-000037b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000037c0: 2020 2020 2020 2020 2020 2053 495a 4520             SIZE 
-000037d0: 2020 2020 2020 2020 2020 2020 2020 2043                 C
-000037e0: 4f4d 4d45 4e54 0a20 2020 2066 6465 3765  OMMENT.    fde7e
-000037f0: 6464 3265 3536 3820 2020 2020 2020 2033  dd2e568        3
-00003800: 3220 7365 636f 6e64 7320 6167 6f20 2020  2 seconds ago   
-00003810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003840: 2020 2033 3538 2e32 204d 4220 2020 2020     358.2 MB     
-00003850: 2020 2020 2020 200a 2020 2020 3364 3464         .    3d4d
-00003860: 3032 3238 6631 3631 2020 2020 2020 2020  0228f161        
-00003870: 3320 7765 656b 7320 6167 6f20 2020 2020  3 weeks ago     
-00003880: 2020 2020 2f62 696e 2f73 6820 2d63 2023      /bin/sh -c #
-00003890: 286e 6f70 2920 5553 4552 205b 726f 6f74  (nop) USER [root
-000038a0: 5d20 2020 2020 2020 2020 2020 2020 2020  ]               
-000038b0: 2020 2020 3020 4220 2020 2020 2020 2020      0 B         
-000038c0: 2020 2020 2020 2020 0a20 2020 2066 3761          .    f7a
-000038d0: 6234 6561 3139 3730 3820 2020 2020 2020  b4ea19708       
-000038e0: 2033 2077 6565 6b73 2061 676f 2020 2020   3 weeks ago    
-000038f0: 2020 2020 202f 6269 6e2f 7368 202d 6320       /bin/sh -c 
-00003900: 2328 6e6f 7029 204d 4149 4e54 4149 4e45  #(nop) MAINTAINE
-00003910: 5220 4d61 7265 6b20 476f 6c64 6d61 6e6e  R Marek Goldmann
-00003920: 203c 2020 2030 2042 2020 2020 2020 2020   <   0 B        
-00003930: 2020 2020 2020 2020 200a 2020 2020 3462           .    4b
-00003940: 6231 3566 3362 3639 3737 2020 2020 2020  b15f3b6977      
-00003950: 2020 3320 7765 656b 7320 6167 6f20 2020    3 weeks ago   
-00003960: 2020 2020 2020 2f62 696e 2f73 6820 2d63        /bin/sh -c
-00003970: 2023 286e 6f70 2920 5553 4552 205b 6a62   #(nop) USER [jb
-00003980: 6f73 735d 2020 2020 2020 2020 2020 2020  oss]            
-00003990: 2020 2020 2020 3020 4220 2020 2020 2020        0 B       
-000039a0: 2020 2020 2020 2020 2020 0a20 2020 2035            .    5
-000039b0: 6463 3165 3439 6634 3336 3120 2020 2020  dc1e49f4361     
-000039c0: 2020 2033 2077 6565 6b73 2061 676f 2020     3 weeks ago  
-000039d0: 2020 2020 2020 202f 6269 6e2f 7368 202d         /bin/sh -
-000039e0: 6320 2328 6e6f 7029 2057 4f52 4b44 4952  c #(nop) WORKDIR
-000039f0: 202f 6f70 742f 6a62 6f73 7320 2020 2020   /opt/jboss     
-00003a00: 2020 2020 2020 2030 2042 2020 2020 2020         0 B      
-00003a10: 2020 2020 2020 2020 2020 200a 2020 2020             .    
-00003a20: 3766 3066 3965 6233 3131 3734 2020 2020  7f0f9eb31174    
-00003a30: 2020 2020 3320 7765 656b 7320 6167 6f20      3 weeks ago 
-00003a40: 2020 2020 2020 2020 2f62 696e 2f73 6820          /bin/sh 
-00003a50: 2d63 2067 726f 7570 6164 6420 2d72 206a  -c groupadd -r j
-00003a60: 626f 7373 202d 6720 3130 3030 2026 2620  boss -g 1000 && 
-00003a70: 7573 6572 6120 2020 342e 3334 3920 6b42  usera   4.349 kB
-00003a80: 2020 2020 2020 2020 2020 2020 0a20 2020              .   
-00003a90: 2062 6435 3135 6630 3434 6166 3720 2020   bd515f044af7   
-00003aa0: 2020 2020 2033 2077 6565 6b73 2061 676f       3 weeks ago
-00003ab0: 2020 2020 2020 2020 202f 6269 6e2f 7368           /bin/sh
-00003ac0: 202d 6320 7975 6d20 7570 6461 7465 202d   -c yum update -
-00003ad0: 7920 2626 2079 756d 202d 7920 696e 7374  y && yum -y inst
-00003ae0: 616c 6c20 786d 2020 2032 352e 3138 204d  all xm   25.18 M
-00003af0: 4220 2020 2020 2020 2020 2020 200a 2020  B            .  
-00003b00: 2020 6237 3833 3336 3039 3930 3435 2020    b78336099045  
-00003b10: 2020 2020 2020 3320 7765 656b 7320 6167        3 weeks ag
-00003b20: 6f20 2020 2020 2020 2020 2f62 696e 2f73  o         /bin/s
-00003b30: 6820 2d63 2023 286e 6f70 2920 4d41 494e  h -c #(nop) MAIN
-00003b40: 5441 494e 4552 204d 6172 656b 2047 6f6c  TAINER Marek Gol
-00003b50: 646d 616e 6e20 3c20 2020 3020 4220 2020  dmann <   0 B   
-00003b60: 2020 2020 2020 2020 2020 2020 2020 0a20                . 
-00003b70: 2020 2034 3831 3661 3239 3835 3438 6320     4816a298548c 
-00003b80: 2020 2020 2020 2033 2077 6565 6b73 2061         3 weeks a
-00003b90: 676f 2020 2020 2020 2020 202f 6269 6e2f  go         /bin/
-00003ba0: 7368 202d 6320 2328 6e6f 7029 2043 4d44  sh -c #(nop) CMD
-00003bb0: 205b 222f 6269 6e2f 6261 7368 225d 2020   ["/bin/bash"]  
-00003bc0: 2020 2020 2020 2020 2020 2030 2042 2020             0 B  
-00003bd0: 2020 2020 2020 2020 2020 2020 2020 200a                 .
-00003be0: 2020 2020 3665 6532 3335 6366 3434 3733      6ee235cf4473
-00003bf0: 2020 2020 2020 2020 3320 7765 656b 7320          3 weeks 
-00003c00: 6167 6f20 2020 2020 2020 2020 2f62 696e  ago         /bin
-00003c10: 2f73 6820 2d63 2023 286e 6f70 2920 4c41  /sh -c #(nop) LA
-00003c20: 4245 4c20 6e61 6d65 3d43 656e 744f 5320  BEL name=CentOS 
-00003c30: 4261 7365 2049 6d61 6720 2020 3020 4220  Base Imag   0 B 
-00003c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003c50: 0a20 2020 2034 3734 6332 6565 3737 6661  .    474c2ee77fa
-00003c60: 3320 2020 2020 2020 2033 2077 6565 6b73  3        3 weeks
-00003c70: 2061 676f 2020 2020 2020 2020 202f 6269   ago         /bi
-00003c80: 6e2f 7368 202d 6320 2328 6e6f 7029 2041  n/sh -c #(nop) A
-00003c90: 4444 2066 696c 653a 3732 3835 3266 6337  DD file:72852fc7
-00003ca0: 3632 3664 3233 3333 3433 2020 2031 3936  626d233343   196
-00003cb0: 2e36 204d 4220 2020 2020 2020 2020 2020  .6 MB           
-00003cc0: 200a 2020 2020 3135 3434 3038 3466 6164   .    1544084fad
-00003cd0: 3831 2020 2020 2020 2020 3620 6d6f 6e74  81        6 mont
-00003ce0: 6873 2061 676f 2020 2020 2020 2020 2f62  hs ago        /b
-00003cf0: 696e 2f73 6820 2d63 2023 286e 6f70 2920  in/sh -c #(nop) 
-00003d00: 4d41 494e 5441 494e 4552 2054 6865 2043  MAINTAINER The C
-00003d10: 656e 744f 5320 5072 6f6a 6520 2020 3020  entOS Proje   0 
-00003d20: 420a 0a0a 0a                             B....
+00002530: 3335 382e 3220 4d42 0a20 2020 2034 6262  358.2 MB.    4bb
+00002540: 3135 6633 6236 3937 3720 2020 2020 2020  15f3b6977       
+00002550: 2033 2077 6565 6b73 2061 676f 2020 2020   3 weeks ago    
+00002560: 2020 2020 202f 6269 6e2f 7368 202d 6320       /bin/sh -c 
+00002570: 2328 6e6f 7029 2055 5345 5220 5b6a 626f  #(nop) USER [jbo
+00002580: 7373 5d20 2020 2020 2020 2020 2020 2020  ss]             
+00002590: 2020 2020 2030 2042 0a20 2020 2035 6463       0 B.    5dc
+000025a0: 3165 3439 6634 3336 3120 2020 2020 2020  1e49f4361       
+000025b0: 2033 2077 6565 6b73 2061 676f 2020 2020   3 weeks ago    
+000025c0: 2020 2020 202f 6269 6e2f 7368 202d 6320       /bin/sh -c 
+000025d0: 2328 6e6f 7029 2057 4f52 4b44 4952 202f  #(nop) WORKDIR /
+000025e0: 6f70 742f 6a62 6f73 7320 2020 2020 2020  opt/jboss       
+000025f0: 2020 2020 2030 2042 0a20 2020 2037 6630       0 B.    7f0
+00002600: 6639 6562 3331 3137 3420 2020 2020 2020  f9eb31174       
+00002610: 2033 2077 6565 6b73 2061 676f 2020 2020   3 weeks ago    
+00002620: 2020 2020 202f 6269 6e2f 7368 202d 6320       /bin/sh -c 
+00002630: 6772 6f75 7061 6464 202d 7220 6a62 6f73  groupadd -r jbos
+00002640: 7320 2d67 2031 3030 3020 2626 2075 7365  s -g 1000 && use
+00002650: 7261 2020 2034 2e33 3439 206b 420a 2020  ra   4.349 kB.  
+00002660: 2020 6264 3531 3566 3034 3461 6637 2020    bd515f044af7  
+00002670: 2020 2020 2020 3320 7765 656b 7320 6167        3 weeks ag
+00002680: 6f20 2020 2020 2020 2020 2f62 696e 2f73  o         /bin/s
+00002690: 6820 2d63 2079 756d 2075 7064 6174 6520  h -c yum update 
+000026a0: 2d79 2026 2620 7975 6d20 2d79 2069 6e73  -y && yum -y ins
+000026b0: 7461 6c6c 2078 6d20 2020 3235 2e31 3820  tall xm   25.18 
+000026c0: 4d42 0a20 2020 2062 3738 3333 3630 3939  MB.    b78336099
+000026d0: 3034 3520 2020 2020 2020 2033 2077 6565  045        3 wee
+000026e0: 6b73 2061 676f 2020 2020 2020 2020 202f  ks ago         /
+000026f0: 6269 6e2f 7368 202d 6320 2328 6e6f 7029  bin/sh -c #(nop)
+00002700: 204d 4149 4e54 4149 4e45 5220 4d61 7265   MAINTAINER Mare
+00002710: 6b20 476f 6c64 6d61 6e6e 203c 2020 2030  k Goldmann <   0
+00002720: 2042 0a20 2020 2034 3831 3661 3239 3835   B.    4816a2985
+00002730: 3438 6320 2020 2020 2020 2033 2077 6565  48c        3 wee
+00002740: 6b73 2061 676f 2020 2020 2020 2020 202f  ks ago         /
+00002750: 6269 6e2f 7368 202d 6320 2328 6e6f 7029  bin/sh -c #(nop)
+00002760: 2043 4d44 205b 222f 6269 6e2f 6261 7368   CMD ["/bin/bash
+00002770: 225d 2020 2020 2020 2020 2020 2020 2030  "]             0
+00002780: 2042 0a20 2020 2036 6565 3233 3563 6634   B.    6ee235cf4
+00002790: 3437 3320 2020 2020 2020 2033 2077 6565  473        3 wee
+000027a0: 6b73 2061 676f 2020 2020 2020 2020 202f  ks ago         /
+000027b0: 6269 6e2f 7368 202d 6320 2328 6e6f 7029  bin/sh -c #(nop)
+000027c0: 204c 4142 454c 206e 616d 653d 4365 6e74   LABEL name=Cent
+000027d0: 4f53 2042 6173 6520 496d 6167 2020 2030  OS Base Imag   0
+000027e0: 2042 0a20 2020 2034 3734 6332 6565 3737   B.    474c2ee77
+000027f0: 6661 3320 2020 2020 2020 2033 2077 6565  fa3        3 wee
+00002800: 6b73 2061 676f 2020 2020 2020 2020 202f  ks ago         /
+00002810: 6269 6e2f 7368 202d 6320 2328 6e6f 7029  bin/sh -c #(nop)
+00002820: 2041 4444 2066 696c 653a 3732 3835 3266   ADD file:72852f
+00002830: 6337 3632 3664 3233 3333 3433 2020 2031  c7626d233343   1
+00002840: 3936 2e36 204d 420a 2020 2020 3135 3434  96.6 MB.    1544
+00002850: 3038 3466 6164 3831 2020 2020 2020 2020  084fad81        
+00002860: 3620 6d6f 6e74 6873 2061 676f 2020 2020  6 months ago    
+00002870: 2020 2020 2f62 696e 2f73 6820 2d63 2023      /bin/sh -c #
+00002880: 286e 6f70 2920 4d41 494e 5441 494e 4552  (nop) MAINTAINER
+00002890: 2054 6865 2043 656e 744f 5320 5072 6f6a   The CentOS Proj
+000028a0: 6520 2020 3020 420a 0a4f 7468 6572 206f  e   0 B..Other o
+000028b0: 7074 696f 6e20 6973 2074 6f20 7370 6563  ption is to spec
+000028c0: 6966 7920 686f 7720 6d61 6e79 206c 6179  ify how many lay
+000028d0: 6572 7320 2863 6f75 6e74 696e 6720 6672  ers (counting fr
+000028e0: 6f6d 2074 6865 206e 6577 6573 7420 6c61  om the newest la
+000028f0: 7965 7229 2077 6520 7761 6e74 2074 6f20  yer) we want to 
+00002900: 7371 7561 7368 2e5c 0a4c 6574 2773 2073  squash.\.Let's s
+00002910: 7175 6173 6820 6c61 7374 2031 3020 6c61  quash last 10 la
+00002920: 7965 7273 2066 726f 6d20 7468 6520 6060  yers from the ``
+00002930: 6a62 6f73 732f 7769 6c64 666c 793a 6c61  jboss/wildfly:la
+00002940: 7465 7374 6060 2069 6d61 6765 3a0a 0a3a  test`` image:..:
+00002950: 3a0a 0a20 2020 2024 2064 6f63 6b65 722d  :..    $ docker-
+00002960: 7371 7561 7368 202d 6620 3130 202d 7420  squash -f 10 -t 
+00002970: 6a62 6f73 732f 7769 6c64 666c 793a 7371  jboss/wildfly:sq
+00002980: 7561 7368 6564 206a 626f 7373 2f77 696c  uashed jboss/wil
+00002990: 6466 6c79 3a6c 6174 6573 740a 2020 2020  dfly:latest.    
+000029a0: 3230 3136 2d30 342d 3031 2031 333a 3135  2016-04-01 13:15
+000029b0: 3a30 362c 3438 3820 726f 6f74 2020 2020  :06,488 root    
+000029c0: 2020 2020 2049 4e46 4f20 2020 2020 646f       INFO     do
+000029d0: 636b 6572 2d73 6372 6970 7473 2076 6572  cker-scripts ver
+000029e0: 7369 6f6e 2031 2e30 2e30 6465 762c 2044  sion 1.0.0dev, D
+000029f0: 6f63 6b65 7220 3732 3036 3632 312c 2041  ocker 7206621, A
+00002a00: 5049 2031 2e32 312e 2e2e 0a20 2020 2032  PI 1.21....    2
+00002a10: 3031 362d 3034 2d30 3120 3133 3a31 353a  016-04-01 13:15:
+00002a20: 3036 2c34 3838 2072 6f6f 7420 2020 2020  06,488 root     
+00002a30: 2020 2020 494e 464f 2020 2020 2055 7369      INFO     Usi
+00002a40: 6e67 2076 3120 696d 6167 6520 666f 726d  ng v1 image form
+00002a50: 6174 0a20 2020 2032 3031 362d 3034 2d30  at.    2016-04-0
+00002a60: 3120 3133 3a31 353a 3036 2c35 3034 2072  1 13:15:06,504 r
+00002a70: 6f6f 7420 2020 2020 2020 2020 494e 464f  oot         INFO
+00002a80: 2020 2020 204f 6c64 2069 6d61 6765 2068       Old image h
+00002a90: 6173 2032 3120 6c61 7965 7273 0a20 2020  as 21 layers.   
+00002aa0: 2032 3031 362d 3034 2d30 3120 3133 3a31   2016-04-01 13:1
+00002ab0: 353a 3036 2c35 3034 2072 6f6f 7420 2020  5:06,504 root   
+00002ac0: 2020 2020 2020 494e 464f 2020 2020 2043        INFO     C
+00002ad0: 6865 636b 696e 6720 6966 2073 7175 6173  hecking if squas
+00002ae0: 6869 6e67 2069 7320 6e65 6365 7373 6172  hing is necessar
+00002af0: 792e 2e2e 0a20 2020 2032 3031 362d 3034  y....    2016-04
+00002b00: 2d30 3120 3133 3a31 353a 3036 2c35 3034  -01 13:15:06,504
+00002b10: 2072 6f6f 7420 2020 2020 2020 2020 494e   root         IN
+00002b20: 464f 2020 2020 2041 7474 656d 7074 696e  FO     Attemptin
+00002b30: 6720 746f 2073 7175 6173 6820 6c61 7374  g to squash last
+00002b40: 2031 3020 6c61 7965 7273 2e2e 2e0a 2020   10 layers....  
+00002b50: 2020 3230 3136 2d30 342d 3031 2031 333a    2016-04-01 13:
+00002b60: 3135 3a30 362c 3530 3520 726f 6f74 2020  15:06,505 root  
+00002b70: 2020 2020 2020 2049 4e46 4f20 2020 2020         INFO     
+00002b80: 5361 7669 6e67 2069 6d61 6765 2032 3539  Saving image 259
+00002b90: 3534 6536 6432 3330 3030 3632 3335 6565  54e6d230006235ee
+00002ba0: 6362 3766 3063 6335 3630 3236 3464 3733  cb7f0cc560264d73
+00002bb0: 3134 3639 3835 6332 6432 6536 3633 6261  146985c2d2e663ba
+00002bc0: 6339 3533 6436 3630 6238 3733 3020 746f  c953d660b8730 to
+00002bd0: 202f 746d 702f 646f 636b 6572 2d73 7175   /tmp/docker-squ
+00002be0: 6173 682d 6675 3830 4358 2f6f 6c64 2f69  ash-fu80CX/old/i
+00002bf0: 6d61 6765 2e74 6172 2066 696c 652e 2e2e  mage.tar file...
+00002c00: 0a20 2020 2032 3031 362d 3034 2d30 3120  .    2016-04-01 
+00002c10: 3133 3a31 353a 3132 2c31 3336 2072 6f6f  13:15:12,136 roo
+00002c20: 7420 2020 2020 2020 2020 494e 464f 2020  t         INFO  
+00002c30: 2020 2049 6d61 6765 2073 6176 6564 210a     Image saved!.
+00002c40: 2020 2020 3230 3136 2d30 342d 3031 2031      2016-04-01 1
+00002c50: 333a 3135 3a31 322c 3136 3720 726f 6f74  3:15:12,167 root
+00002c60: 2020 2020 2020 2020 2049 4e46 4f20 2020           INFO   
+00002c70: 2020 556e 7061 636b 696e 6720 2f74 6d70    Unpacking /tmp
+00002c80: 2f64 6f63 6b65 722d 7371 7561 7368 2d66  /docker-squash-f
+00002c90: 7538 3043 582f 6f6c 642f 696d 6167 652e  u80CX/old/image.
+00002ca0: 7461 7220 7461 7220 6669 6c65 2074 6f20  tar tar file to 
+00002cb0: 2f74 6d70 2f64 6f63 6b65 722d 7371 7561  /tmp/docker-squa
+00002cc0: 7368 2d66 7538 3043 582f 6f6c 6420 6469  sh-fu80CX/old di
+00002cd0: 7265 6374 6f72 790a 2020 2020 3230 3136  rectory.    2016
+00002ce0: 2d30 342d 3031 2031 333a 3135 3a31 322c  -04-01 13:15:12,
+00002cf0: 3730 3620 726f 6f74 2020 2020 2020 2020  706 root        
+00002d00: 2049 4e46 4f20 2020 2020 4172 6368 6976   INFO     Archiv
+00002d10: 6520 756e 7061 636b 6564 210a 2020 2020  e unpacked!.    
+00002d20: 3230 3136 2d30 342d 3031 2031 333a 3135  2016-04-01 13:15
+00002d30: 3a31 322c 3735 3620 726f 6f74 2020 2020  :12,756 root    
+00002d40: 2020 2020 2049 4e46 4f20 2020 2020 5371       INFO     Sq
+00002d50: 7561 7368 696e 6720 696d 6167 6520 276a  uashing image 'j
+00002d60: 626f 7373 2f77 696c 6466 6c79 3a6c 6174  boss/wildfly:lat
+00002d70: 6573 7427 2e2e 2e0a 2020 2020 3230 3136  est'....    2016
+00002d80: 2d30 342d 3031 2031 333a 3135 3a31 322c  -04-01 13:15:12,
+00002d90: 3735 3620 726f 6f74 2020 2020 2020 2020  756 root        
+00002da0: 2049 4e46 4f20 2020 2020 5374 6172 7469   INFO     Starti
+00002db0: 6e67 2073 7175 6173 6869 6e67 2e2e 2e0a  ng squashing....
+00002dc0: 2020 2020 3230 3136 2d30 342d 3031 2031      2016-04-01 1
+00002dd0: 333a 3135 3a31 322c 3735 3620 726f 6f74  3:15:12,756 root
+00002de0: 2020 2020 2020 2020 2049 4e46 4f20 2020           INFO   
+00002df0: 2020 5371 7561 7368 696e 6720 6669 6c65    Squashing file
+00002e00: 2027 2f74 6d70 2f64 6f63 6b65 722d 7371   '/tmp/docker-sq
+00002e10: 7561 7368 2d66 7538 3043 582f 6f6c 642f  uash-fu80CX/old/
+00002e20: 3235 3935 3465 3664 3233 3030 3036 3233  25954e6d23000623
+00002e30: 3565 6563 6237 6630 6363 3536 3032 3634  5eecb7f0cc560264
+00002e40: 6437 3331 3436 3938 3563 3264 3265 3636  d73146985c2d2e66
+00002e50: 3362 6163 3935 3364 3636 3062 3837 3330  3bac953d660b8730
+00002e60: 2f6c 6179 6572 2e74 6172 272e 2e2e 0a20  /layer.tar'.... 
+00002e70: 2020 2032 3031 362d 3034 2d30 3120 3133     2016-04-01 13
+00002e80: 3a31 353a 3132 2c37 3537 2072 6f6f 7420  :15:12,757 root 
+00002e90: 2020 2020 2020 2020 494e 464f 2020 2020          INFO    
+00002ea0: 2053 7175 6173 6869 6e67 2066 696c 6520   Squashing file 
+00002eb0: 272f 746d 702f 646f 636b 6572 2d73 7175  '/tmp/docker-squ
+00002ec0: 6173 682d 6675 3830 4358 2f6f 6c64 2f35  ash-fu80CX/old/5
+00002ed0: 6165 3639 6362 3435 3461 3561 3534 3266  ae69cb454a5a542f
+00002ee0: 3633 6531 3438 6365 3430 6662 3965 3031  63e148ce40fb9e01
+00002ef0: 6465 3562 6230 3138 3035 6234 6465 6432  de5bb01805b4ded2
+00002f00: 3338 3834 3162 6332 6365 3865 3839 352f  38841bc2ce8e895/
+00002f10: 6c61 7965 722e 7461 7227 2e2e 2e0a 2020  layer.tar'....  
+00002f20: 2020 3230 3136 2d30 342d 3031 2031 333a    2016-04-01 13:
+00002f30: 3135 3a31 322c 3735 3720 726f 6f74 2020  15:12,757 root  
+00002f40: 2020 2020 2020 2049 4e46 4f20 2020 2020         INFO     
+00002f50: 5371 7561 7368 696e 6720 6669 6c65 2027  Squashing file '
+00002f60: 2f74 6d70 2f64 6f63 6b65 722d 7371 7561  /tmp/docker-squa
+00002f70: 7368 2d66 7538 3043 582f 6f6c 642f 6463  sh-fu80CX/old/dc
+00002f80: 3234 3731 3266 3335 6334 3065 3935 3862  24712f35c40e958b
+00002f90: 6538 6163 6132 3733 3165 3762 6638 3335  e8aca2731e7bf835
+00002fa0: 3362 3962 3138 6261 6136 6139 3461 6438  3b9b18baa6a94ad8
+00002fb0: 3463 3639 3532 6362 6337 3730 3034 2f6c  4c6952cbc77004/l
+00002fc0: 6179 6572 2e74 6172 272e 2e2e 0a20 2020  ayer.tar'....   
+00002fd0: 2032 3031 362d 3034 2d30 3120 3133 3a31   2016-04-01 13:1
+00002fe0: 353a 3132 2c37 3537 2072 6f6f 7420 2020  5:12,757 root   
+00002ff0: 2020 2020 2020 494e 464f 2020 2020 2053        INFO     S
+00003000: 7175 6173 6869 6e67 2066 696c 6520 272f  quashing file '/
+00003010: 746d 702f 646f 636b 6572 2d73 7175 6173  tmp/docker-squas
+00003020: 682d 6675 3830 4358 2f6f 6c64 2f64 3932  h-fu80CX/old/d92
+00003030: 3931 3239 6434 6338 6536 3165 6133 3636  9129d4c8e61ea366
+00003040: 3165 6234 3263 3330 6430 3166 3463 3135  1eb42c30d01f4c15
+00003050: 3234 3138 3638 3931 3738 6166 6337 6463  2418689178afc7dc
+00003060: 3831 3835 6133 3738 3134 3532 382f 6c61  8185a37814528/la
+00003070: 7965 722e 7461 7227 2e2e 2e0a 2020 2020  yer.tar'....    
+00003080: 3230 3136 2d30 342d 3031 2031 333a 3135  2016-04-01 13:15
+00003090: 3a31 332c 3233 3420 726f 6f74 2020 2020  :13,234 root    
+000030a0: 2020 2020 2049 4e46 4f20 2020 2020 5371       INFO     Sq
+000030b0: 7561 7368 696e 6720 6669 6c65 2027 2f74  uashing file '/t
+000030c0: 6d70 2f64 6f63 6b65 722d 7371 7561 7368  mp/docker-squash
+000030d0: 2d66 7538 3043 582f 6f6c 642f 6238 6661  -fu80CX/old/b8fa
+000030e0: 3363 6166 3764 3664 6332 3238 6266 3234  3caf7d6dc228bf24
+000030f0: 3939 6133 6166 3836 6535 3037 3361 6430  99a3af86e5073ad0
+00003100: 6331 3733 3034 6333 3930 3066 6133 3431  c17304c3900fa341
+00003110: 6539 6432 6665 3465 3536 3535 2f6c 6179  e9d2fe4e5655/lay
+00003120: 6572 2e74 6172 272e 2e2e 0a20 2020 2032  er.tar'....    2
+00003130: 3031 362d 3034 2d30 3120 3133 3a31 353a  016-04-01 13:15:
+00003140: 3133 2c32 3335 2072 6f6f 7420 2020 2020  13,235 root     
+00003150: 2020 2020 494e 464f 2020 2020 2053 7175      INFO     Squ
+00003160: 6173 6869 6e67 2066 696c 6520 272f 746d  ashing file '/tm
+00003170: 702f 646f 636b 6572 2d73 7175 6173 682d  p/docker-squash-
+00003180: 6675 3830 4358 2f6f 6c64 2f33 3862 3866  fu80CX/old/38b8f
+00003190: 3835 6537 3462 6661 3737 3361 3061 6436  85e74bfa773a0ad6
+000031a0: 3964 6132 3230 3564 6330 3134 3839 3435  9da2205dc0148945
+000031b0: 6536 6635 6137 6365 6230 3466 6134 6538  e6f5a7ceb04fa4e8
+000031c0: 3631 3965 3164 6534 3235 622f 6c61 7965  619e1de425b/laye
+000031d0: 722e 7461 7227 2e2e 2e0a 2020 2020 3230  r.tar'....    20
+000031e0: 3136 2d30 342d 3031 2031 333a 3135 3a31  16-04-01 13:15:1
+000031f0: 332c 3233 3520 726f 6f74 2020 2020 2020  3,235 root      
+00003200: 2020 2049 4e46 4f20 2020 2020 5371 7561     INFO     Squa
+00003210: 7368 696e 6720 6669 6c65 2027 2f74 6d70  shing file '/tmp
+00003220: 2f64 6f63 6b65 722d 7371 7561 7368 2d66  /docker-squash-f
+00003230: 7538 3043 582f 6f6c 642f 6165 3739 6236  u80CX/old/ae79b6
+00003240: 3436 6239 6139 6132 3837 6335 6636 6130  46b9a9a287c5f6a0
+00003250: 3138 3731 6363 3964 3965 6535 3936 6461  1871cc9d9ee596da
+00003260: 6665 6532 6462 3934 3237 3134 6361 3364  fee2db942714ca3d
+00003270: 6561 3063 3036 6565 6633 2f6c 6179 6572  ea0c06eef3/layer
+00003280: 2e74 6172 272e 2e2e 0a20 2020 2032 3031  .tar'....    201
+00003290: 362d 3034 2d30 3120 3133 3a31 353a 3133  6-04-01 13:15:13
+000032a0: 2c32 3335 2072 6f6f 7420 2020 2020 2020  ,235 root       
+000032b0: 2020 494e 464f 2020 2020 2053 7175 6173    INFO     Squas
+000032c0: 6869 6e67 2066 696c 6520 272f 746d 702f  hing file '/tmp/
+000032d0: 646f 636b 6572 2d73 7175 6173 682d 6675  docker-squash-fu
+000032e0: 3830 4358 2f6f 6c64 2f32 6234 3630 3664  80CX/old/2b4606d
+000032f0: 6339 6463 3737 3361 6132 3230 6136 3533  c9dc773aa220a653
+00003300: 3531 6665 3864 3534 6630 3335 3334 6335  51fe8d54f03534c5
+00003310: 3866 6561 3233 3039 3630 6539 3539 3135  8fea230960e95915
+00003320: 3232 3233 3636 3037 342f 6c61 7965 722e  222366074/layer.
+00003330: 7461 7227 2e2e 2e0a 2020 2020 3230 3136  tar'....    2016
+00003340: 2d30 342d 3031 2031 333a 3135 3a31 332c  -04-01 13:15:13,
+00003350: 3233 3620 726f 6f74 2020 2020 2020 2020  236 root        
+00003360: 2049 4e46 4f20 2020 2020 5371 7561 7368   INFO     Squash
+00003370: 696e 6720 6669 6c65 2027 2f74 6d70 2f64  ing file '/tmp/d
+00003380: 6f63 6b65 722d 7371 7561 7368 2d66 7538  ocker-squash-fu8
+00003390: 3043 582f 6f6c 642f 3131 3866 6139 6533  0CX/old/118fa9e3
+000033a0: 3335 3736 6563 6336 3235 6562 6262 6664  3576ecc625ebbbfd
+000033b0: 6632 3830 3963 3135 3237 6537 3136 6362  f2809c1527e716cb
+000033c0: 3466 6435 6362 3430 3534 3865 6236 6433  4fd5cb40548eb6d3
+000033d0: 3530 3361 3735 6139 2f6c 6179 6572 2e74  503a75a9/layer.t
+000033e0: 6172 272e 2e2e 0a20 2020 2032 3031 362d  ar'....    2016-
+000033f0: 3034 2d30 3120 3133 3a31 353a 3133 2c32  04-01 13:15:13,2
+00003400: 3336 2072 6f6f 7420 2020 2020 2020 2020  36 root         
+00003410: 494e 464f 2020 2020 2053 7175 6173 6869  INFO     Squashi
+00003420: 6e67 2066 696c 6520 272f 746d 702f 646f  ng file '/tmp/do
+00003430: 636b 6572 2d73 7175 6173 682d 6675 3830  cker-squash-fu80
+00003440: 4358 2f6f 6c64 2f35 6637 6538 6633 3663  CX/old/5f7e8f36c
+00003450: 3362 6232 3063 3964 6237 3437 3061 3232  3bb20c9db7470a22
+00003460: 6638 3238 3731 3062 3464 3238 6165 6465  f828710b4d28aede
+00003470: 3634 3936 3663 3432 3561 6464 3438 6131  64966c425add48a1
+00003480: 6231 3466 6532 332f 6c61 7965 722e 7461  b14fe23/layer.ta
+00003490: 7227 2e2e 2e0a 2020 2020 3230 3136 2d30  r'....    2016-0
+000034a0: 342d 3031 2031 333a 3135 3a31 342c 3834  4-01 13:15:14,84
+000034b0: 3820 726f 6f74 2020 2020 2020 2020 2049  8 root         I
+000034c0: 4e46 4f20 2020 2020 5371 7561 7368 696e  NFO     Squashin
+000034d0: 6720 6669 6e69 7368 6564 210a 2020 2020  g finished!.    
+000034e0: 3230 3136 2d30 342d 3031 2031 333a 3135  2016-04-01 13:15
+000034f0: 3a31 342c 3835 3320 726f 6f74 2020 2020  :14,853 root    
+00003500: 2020 2020 2049 4e46 4f20 2020 2020 4e65       INFO     Ne
+00003510: 7720 7371 7561 7368 6564 2069 6d61 6765  w squashed image
+00003520: 2049 4420 6973 2066 6465 3765 6464 3265   ID is fde7edd2e
+00003530: 3536 3833 6339 3762 6564 6639 6330 6266  5683c97bedf9c0bf
+00003540: 3532 6164 3531 3530 6462 3536 3530 6534  52ad5150db5650e4
+00003550: 3231 6465 3364 3932 3933 6365 3532 3233  21de3d9293ce5223
+00003560: 6232 3536 3435 350a 2020 2020 3230 3136  b256455.    2016
+00003570: 2d30 342d 3031 2031 333a 3135 3a31 382c  -04-01 13:15:18,
+00003580: 3936 3320 726f 6f74 2020 2020 2020 2020  963 root        
+00003590: 2049 4e46 4f20 2020 2020 496d 6167 6520   INFO     Image 
+000035a0: 7265 6769 7374 6572 6564 2069 6e20 446f  registered in Do
+000035b0: 636b 6572 2064 6165 6d6f 6e20 6173 206a  cker daemon as j
+000035c0: 626f 7373 2f77 696c 6466 6c79 3a73 7175  boss/wildfly:squ
+000035d0: 6173 6865 640a 2020 2020 3230 3136 2d30  ashed.    2016-0
+000035e0: 342d 3031 2031 333a 3135 3a31 392c 3035  4-01 13:15:19,05
+000035f0: 3920 726f 6f74 2020 2020 2020 2020 2049  9 root         I
+00003600: 4e46 4f20 2020 2020 446f 6e65 0a0a 4c65  NFO     Done..Le
+00003610: 7427 7320 636f 6e66 6972 6d20 7468 6520  t's confirm the 
+00003620: 696d 6167 6520 7374 7275 6374 7572 6520  image structure 
+00003630: 6e6f 773a 0a0a 3a3a 0a0a 2020 2020 2420  now:..::..    $ 
+00003640: 646f 636b 6572 2068 6973 746f 7279 206a  docker history j
+00003650: 626f 7373 2f77 696c 6466 6c79 3a73 7175  boss/wildfly:squ
+00003660: 6173 6865 640a 2020 2020 494d 4147 4520  ashed.    IMAGE 
+00003670: 2020 2020 2020 2020 2020 2020 2020 4352                CR
+00003680: 4541 5445 4420 2020 2020 2020 2020 2020  EATED           
+00003690: 2020 4352 4541 5445 4420 4259 2020 2020    CREATED BY    
+000036a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000036b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000036c0: 2020 5349 5a45 2020 2020 2020 2020 2020    SIZE          
+000036d0: 2020 2020 2020 434f 4d4d 454e 540a 2020        COMMENT.  
+000036e0: 2020 6664 6537 6564 6432 6535 3638 2020    fde7edd2e568  
+000036f0: 2020 2020 2020 3332 2073 6563 6f6e 6473        32 seconds
+00003700: 2061 676f 2020 2020 2020 2020 2020 2020   ago            
+00003710: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003730: 2020 2020 2020 2020 2020 3335 382e 3220            358.2 
+00003740: 4d42 0a20 2020 2033 6434 6430 3232 3866  MB.    3d4d0228f
+00003750: 3136 3120 2020 2020 2020 2033 2077 6565  161        3 wee
+00003760: 6b73 2061 676f 2020 2020 2020 2020 202f  ks ago         /
+00003770: 6269 6e2f 7368 202d 6320 2328 6e6f 7029  bin/sh -c #(nop)
+00003780: 2055 5345 5220 5b72 6f6f 745d 2020 2020   USER [root]    
+00003790: 2020 2020 2020 2020 2020 2020 2020 2030                 0
+000037a0: 2042 0a20 2020 2066 3761 6234 6561 3139   B.    f7ab4ea19
+000037b0: 3730 3820 2020 2020 2020 2033 2077 6565  708        3 wee
+000037c0: 6b73 2061 676f 2020 2020 2020 2020 202f  ks ago         /
+000037d0: 6269 6e2f 7368 202d 6320 2328 6e6f 7029  bin/sh -c #(nop)
+000037e0: 204d 4149 4e54 4149 4e45 5220 4d61 7265   MAINTAINER Mare
+000037f0: 6b20 476f 6c64 6d61 6e6e 203c 2020 2030  k Goldmann <   0
+00003800: 2042 0a20 2020 2034 6262 3135 6633 6236   B.    4bb15f3b6
+00003810: 3937 3720 2020 2020 2020 2033 2077 6565  977        3 wee
+00003820: 6b73 2061 676f 2020 2020 2020 2020 202f  ks ago         /
+00003830: 6269 6e2f 7368 202d 6320 2328 6e6f 7029  bin/sh -c #(nop)
+00003840: 2055 5345 5220 5b6a 626f 7373 5d20 2020   USER [jboss]   
+00003850: 2020 2020 2020 2020 2020 2020 2020 2030                 0
+00003860: 2042 0a20 2020 2035 6463 3165 3439 6634   B.    5dc1e49f4
+00003870: 3336 3120 2020 2020 2020 2033 2077 6565  361        3 wee
+00003880: 6b73 2061 676f 2020 2020 2020 2020 202f  ks ago         /
+00003890: 6269 6e2f 7368 202d 6320 2328 6e6f 7029  bin/sh -c #(nop)
+000038a0: 2057 4f52 4b44 4952 202f 6f70 742f 6a62   WORKDIR /opt/jb
+000038b0: 6f73 7320 2020 2020 2020 2020 2020 2030  oss            0
+000038c0: 2042 0a20 2020 2037 6630 6639 6562 3331   B.    7f0f9eb31
+000038d0: 3137 3420 2020 2020 2020 2033 2077 6565  174        3 wee
+000038e0: 6b73 2061 676f 2020 2020 2020 2020 202f  ks ago         /
+000038f0: 6269 6e2f 7368 202d 6320 6772 6f75 7061  bin/sh -c groupa
+00003900: 6464 202d 7220 6a62 6f73 7320 2d67 2031  dd -r jboss -g 1
+00003910: 3030 3020 2626 2075 7365 7261 2020 2034  000 && usera   4
+00003920: 2e33 3439 206b 420a 2020 2020 6264 3531  .349 kB.    bd51
+00003930: 3566 3034 3461 6637 2020 2020 2020 2020  5f044af7        
+00003940: 3320 7765 656b 7320 6167 6f20 2020 2020  3 weeks ago     
+00003950: 2020 2020 2f62 696e 2f73 6820 2d63 2079      /bin/sh -c y
+00003960: 756d 2075 7064 6174 6520 2d79 2026 2620  um update -y && 
+00003970: 7975 6d20 2d79 2069 6e73 7461 6c6c 2078  yum -y install x
+00003980: 6d20 2020 3235 2e31 3820 4d42 0a20 2020  m   25.18 MB.   
+00003990: 2062 3738 3333 3630 3939 3034 3520 2020   b78336099045   
+000039a0: 2020 2020 2033 2077 6565 6b73 2061 676f       3 weeks ago
+000039b0: 2020 2020 2020 2020 202f 6269 6e2f 7368           /bin/sh
+000039c0: 202d 6320 2328 6e6f 7029 204d 4149 4e54   -c #(nop) MAINT
+000039d0: 4149 4e45 5220 4d61 7265 6b20 476f 6c64  AINER Marek Gold
+000039e0: 6d61 6e6e 203c 2020 2030 2042 0a20 2020  mann <   0 B.   
+000039f0: 2034 3831 3661 3239 3835 3438 6320 2020   4816a298548c   
+00003a00: 2020 2020 2033 2077 6565 6b73 2061 676f       3 weeks ago
+00003a10: 2020 2020 2020 2020 202f 6269 6e2f 7368           /bin/sh
+00003a20: 202d 6320 2328 6e6f 7029 2043 4d44 205b   -c #(nop) CMD [
+00003a30: 222f 6269 6e2f 6261 7368 225d 2020 2020  "/bin/bash"]    
+00003a40: 2020 2020 2020 2020 2030 2042 0a20 2020           0 B.   
+00003a50: 2036 6565 3233 3563 6634 3437 3320 2020   6ee235cf4473   
+00003a60: 2020 2020 2033 2077 6565 6b73 2061 676f       3 weeks ago
+00003a70: 2020 2020 2020 2020 202f 6269 6e2f 7368           /bin/sh
+00003a80: 202d 6320 2328 6e6f 7029 204c 4142 454c   -c #(nop) LABEL
+00003a90: 206e 616d 653d 4365 6e74 4f53 2042 6173   name=CentOS Bas
+00003aa0: 6520 496d 6167 2020 2030 2042 0a20 2020  e Imag   0 B.   
+00003ab0: 2034 3734 6332 6565 3737 6661 3320 2020   474c2ee77fa3   
+00003ac0: 2020 2020 2033 2077 6565 6b73 2061 676f       3 weeks ago
+00003ad0: 2020 2020 2020 2020 202f 6269 6e2f 7368           /bin/sh
+00003ae0: 202d 6320 2328 6e6f 7029 2041 4444 2066   -c #(nop) ADD f
+00003af0: 696c 653a 3732 3835 3266 6337 3632 3664  ile:72852fc7626d
+00003b00: 3233 3333 3433 2020 2031 3936 2e36 204d  233343   196.6 M
+00003b10: 420a 2020 2020 3135 3434 3038 3466 6164  B.    1544084fad
+00003b20: 3831 2020 2020 2020 2020 3620 6d6f 6e74  81        6 mont
+00003b30: 6873 2061 676f 2020 2020 2020 2020 2f62  hs ago        /b
+00003b40: 696e 2f73 6820 2d63 2023 286e 6f70 2920  in/sh -c #(nop) 
+00003b50: 4d41 494e 5441 494e 4552 2054 6865 2043  MAINTAINER The C
+00003b60: 656e 744f 5320 5072 6f6a 6520 2020 3020  entOS Proje   0 
+00003b70: 420a                                     B.
```

### Comparing `docker-squash-1.0.9/docker_squash.egg-info/SOURCES.txt` & `docker-squash-1.1.0/docker_squash.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE
 MANIFEST.in
 README.rst
 requirements.txt
+setup.cfg
 setup.py
 docker_squash/__init__.py
 docker_squash/cli.py
 docker_squash/errors.py
 docker_squash/image.py
 docker_squash/squash.py
 docker_squash/v1_image.py
@@ -14,9 +15,8 @@
 docker_squash.egg-info/PKG-INFO
 docker_squash.egg-info/SOURCES.txt
 docker_squash.egg-info/dependency_links.txt
 docker_squash.egg-info/entry_points.txt
 docker_squash.egg-info/requires.txt
 docker_squash.egg-info/top_level.txt
 docker_squash/lib/__init__.py
-docker_squash/lib/common.py
-docker_squash/lib/xtarfile.py
+docker_squash/lib/common.py
```

### Comparing `docker-squash-1.0.9/setup.py` & `docker-squash-1.1.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 #!/usr/bin/python
 
-from setuptools import setup, find_packages
-from docker_squash.version import version
-
 import codecs
 
-with open('requirements.txt') as f:
+from setuptools import find_packages, setup
+
+from docker_squash.version import version
+
+with open("requirements.txt") as f:
     requirements = f.read().splitlines()
 
 setup(
-    name = "docker-squash",
-    version = version,
-    packages = find_packages(exclude=["tests"]),
-    url = 'https://github.com/goldmann/docker-squash',
-    download_url = "https://github.com/goldmann/docker-squash/archive/%s.tar.gz" % version,
-    author = 'Marek Goldmann',
-    author_email = 'marek.goldmann@gmail.com',
-    description = 'Docker layer squashing tool',
-    license='MIT',
-    keywords = 'docker',
-    long_description = codecs.open('README.rst', encoding="utf8").read(),
-    entry_points = {
-        'console_scripts': ['docker-squash=docker_squash.cli:run'],
+    name="docker-squash",
+    version=version,
+    packages=find_packages(exclude=["tests"]),
+    url="https://github.com/goldmann/docker-squash",
+    download_url="https://github.com/goldmann/docker-squash/archive/%s.tar.gz"
+    % version,
+    author="Marek Goldmann",
+    author_email="marek.goldmann@gmail.com",
+    description="Docker layer squashing tool",
+    license="MIT",
+    keywords="docker",
+    long_description=codecs.open("README.rst", encoding="utf8").read(),
+    entry_points={
+        "console_scripts": ["docker-squash=docker_squash.cli:run"],
     },
-    tests_require = ['mock'],
-    install_requires=requirements
+    tests_require=["mock"],
+    install_requires=requirements,
 )
```

