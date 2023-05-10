# Comparing `tmp/async_rmq-0.2.2.tar.gz` & `tmp/async_rmq-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "async_rmq-0.2.2.tar", last modified: Thu Apr  6 09:04:58 2023, max compression
+gzip compressed data, was "async_rmq-0.2.3.tar", last modified: Wed May 10 11:00:57 2023, max compression
```

## Comparing `async_rmq-0.2.2.tar` & `async_rmq-0.2.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-06 09:04:58.695357 async_rmq-0.2.2/
--rw-rw-rw-   0        0        0      162 2023-04-06 09:04:58.695357 async_rmq-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     1039 2023-02-22 10:40:51.000000 async_rmq-0.2.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-06 09:04:58.682390 async_rmq-0.2.2/async_rmq/
--rw-rw-rw-   0        0        0        0 2023-01-30 13:24:34.000000 async_rmq-0.2.2/async_rmq/_init_.py
--rw-rw-rw-   0        0        0     2439 2023-03-15 10:40:00.000000 async_rmq-0.2.2/async_rmq/abstract_rmq_consumer.py
--rw-rw-rw-   0        0        0     1661 2023-04-06 09:04:12.000000 async_rmq-0.2.2/async_rmq/consumer_threading.py
--rw-rw-rw-   0        0        0     6522 2023-04-06 08:56:37.000000 async_rmq-0.2.2/async_rmq/rmq_functions.py
-drwxrwxrwx   0        0        0        0 2023-04-06 09:04:58.694393 async_rmq-0.2.2/async_rmq.egg-info/
--rw-rw-rw-   0        0        0      162 2023-04-06 09:04:58.000000 async_rmq-0.2.2/async_rmq.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      306 2023-04-06 09:04:58.000000 async_rmq-0.2.2/async_rmq.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-06 09:04:58.000000 async_rmq-0.2.2/async_rmq.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-02-20 13:54:08.000000 async_rmq-0.2.2/async_rmq.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       10 2023-04-06 09:04:58.000000 async_rmq-0.2.2/async_rmq.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-06 09:04:58.697393 async_rmq-0.2.2/setup.cfg
--rw-rw-rw-   0        0        0      259 2023-04-06 09:04:48.000000 async_rmq-0.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-10 11:00:57.721200 async_rmq-0.2.3/
+-rw-rw-rw-   0        0        0      162 2023-05-10 11:00:57.722195 async_rmq-0.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1039 2023-02-22 10:40:51.000000 async_rmq-0.2.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-10 11:00:57.707382 async_rmq-0.2.3/async_rmq/
+-rw-rw-rw-   0        0        0        0 2023-01-30 13:24:34.000000 async_rmq-0.2.3/async_rmq/_init_.py
+-rw-rw-rw-   0        0        0     2439 2023-03-15 10:40:00.000000 async_rmq-0.2.3/async_rmq/abstract_rmq_consumer.py
+-rw-rw-rw-   0        0        0     1390 2023-05-10 10:58:25.000000 async_rmq-0.2.3/async_rmq/consumer_threading.py
+-rw-rw-rw-   0        0        0     7642 2023-05-10 10:59:43.000000 async_rmq-0.2.3/async_rmq/rmq_functions.py
+drwxrwxrwx   0        0        0        0 2023-05-10 11:00:57.721200 async_rmq-0.2.3/async_rmq.egg-info/
+-rw-rw-rw-   0        0        0      162 2023-05-10 11:00:57.000000 async_rmq-0.2.3/async_rmq.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      306 2023-05-10 11:00:57.000000 async_rmq-0.2.3/async_rmq.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 11:00:57.000000 async_rmq-0.2.3/async_rmq.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-02-20 13:54:08.000000 async_rmq-0.2.3/async_rmq.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       10 2023-05-10 11:00:57.000000 async_rmq-0.2.3/async_rmq.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-10 11:00:57.723183 async_rmq-0.2.3/setup.cfg
+-rw-rw-rw-   0        0        0      259 2023-05-10 11:00:11.000000 async_rmq-0.2.3/setup.py
```

### Comparing `async_rmq-0.2.2/README.md` & `async_rmq-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `async_rmq-0.2.2/async_rmq/abstract_rmq_consumer.py` & `async_rmq-0.2.3/async_rmq/abstract_rmq_consumer.py`

 * *Files identical despite different names*

### Comparing `async_rmq-0.2.2/async_rmq/consumer_threading.py` & `async_rmq-0.2.3/async_rmq/consumer_threading.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,21 +12,17 @@
     def get_workers(self):
         self.workers = []
         self.consumer_classes = [workers_data["consumer_class"] for workers_data in self.consumers_conf]
         for workers_data in self.consumers_conf:
             workers_count = workers_data["workers_count"]
             consumer_class = workers_data["consumer_class"]
             consumer_settings = workers_data["consumer_settings"]
-            queue_parameters = workers_data["queue_parameters"]
-            exchange_parameters = workers_data["exchange_parameters"]
             dead_letter_params = workers_data["dead_letter_params"]
 
             consumer_functions = [run_consumer(consumer_class,
-                                               queue_parameters,
-                                               exchange_parameters,
                                                **self.credentials,
                                                **consumer_settings,
                                                **dead_letter_params) for i in range(1, workers_count + 1)]
             self.workers.extend(consumer_functions)
 
     def stop_consumers(self):
         import gc
```

