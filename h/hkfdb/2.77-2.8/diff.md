# Comparing `tmp/hkfdb-2.77.tar.gz` & `tmp/hkfdb-2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hkfdb-2.77.tar", last modified: Tue May  2 16:14:02 2023, max compression
+gzip compressed data, was "hkfdb-2.8.tar", last modified: Wed May 10 16:06:40 2023, max compression
```

## Comparing `hkfdb-2.77.tar` & `hkfdb-2.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 16:14:02.933984 hkfdb-2.77/
--rw-rw-rw-   0        0        0    35149 2021-07-30 00:33:11.000000 hkfdb-2.77/LICENSE
--rw-rw-rw-   0        0        0     1652 2023-05-02 16:14:02.933984 hkfdb-2.77/PKG-INFO
--rw-rw-rw-   0        0        0     1243 2023-03-30 03:29:25.000000 hkfdb-2.77/README.md
-drwxrwxrwx   0        0        0        0 2023-05-02 16:14:02.933984 hkfdb-2.77/hkfdb/
--rw-rw-rw-   0        0        0    91011 2023-05-02 16:13:10.000000 hkfdb-2.77/hkfdb/Database.py
--rw-rw-rw-   0        0        0       23 2021-09-12 13:30:45.000000 hkfdb-2.77/hkfdb/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-02 16:14:02.933984 hkfdb-2.77/hkfdb.egg-info/
--rw-rw-rw-   0        0        0     1652 2023-05-02 16:14:02.000000 hkfdb-2.77/hkfdb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      206 2023-05-02 16:14:02.000000 hkfdb-2.77/hkfdb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 16:14:02.000000 hkfdb-2.77/hkfdb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-05-02 16:14:02.000000 hkfdb-2.77/hkfdb.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-02 16:14:02.000000 hkfdb-2.77/hkfdb.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-02 16:14:02.933984 hkfdb-2.77/setup.cfg
--rw-rw-rw-   0        0        0      762 2023-05-02 16:13:52.000000 hkfdb-2.77/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-10 16:06:40.725525 hkfdb-2.8/
+-rw-rw-rw-   0        0        0    35149 2021-07-30 00:33:11.000000 hkfdb-2.8/LICENSE
+-rw-rw-rw-   0        0        0     1651 2023-05-10 16:06:40.725525 hkfdb-2.8/PKG-INFO
+-rw-rw-rw-   0        0        0     1243 2023-03-30 03:29:25.000000 hkfdb-2.8/README.md
+drwxrwxrwx   0        0        0        0 2023-05-10 16:06:40.714491 hkfdb-2.8/hkfdb/
+-rw-rw-rw-   0        0        0    93244 2023-05-10 16:04:53.000000 hkfdb-2.8/hkfdb/Database.py
+-rw-rw-rw-   0        0        0       23 2021-09-12 13:30:45.000000 hkfdb-2.8/hkfdb/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-10 16:06:40.723524 hkfdb-2.8/hkfdb.egg-info/
+-rw-rw-rw-   0        0        0     1651 2023-05-10 16:06:40.000000 hkfdb-2.8/hkfdb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      206 2023-05-10 16:06:40.000000 hkfdb-2.8/hkfdb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 16:06:40.000000 hkfdb-2.8/hkfdb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-05-10 16:06:40.000000 hkfdb-2.8/hkfdb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-10 16:06:40.000000 hkfdb-2.8/hkfdb.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-10 16:06:40.725525 hkfdb-2.8/setup.cfg
+-rw-rw-rw-   0        0        0      761 2023-05-10 16:06:05.000000 hkfdb-2.8/setup.py
```

### Comparing `hkfdb-2.77/LICENSE` & `hkfdb-2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `hkfdb-2.77/PKG-INFO` & `hkfdb-2.8/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hkfdb
-Version: 2.77
+Version: 2.8
 Summary: Hong Kong Finance Database.
 Home-page: https://www.hkfdb.net
 Author: Hong Kong Finance Database Team
 Author-email: info@hkfdb.net
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `hkfdb-2.77/README.md` & `hkfdb-2.8/README.md`

 * *Files identical despite different names*

### Comparing `hkfdb-2.77/hkfdb/Database.py` & `hkfdb-2.8/hkfdb/Database.py`

 * *Files 2% similar despite different names*

```diff
@@ -318,18 +318,24 @@
 
                         if df.loc[0, 'expiry_date'] == '20130530':
                             front_cut_off_date = 20130501
 
                         if (back_cut_off_date != end_date) or (
                                 back_cut_off_date == end_date and back_cut_off_date not in expiry_date_list):
                             if '1D' not in freq:
+                                df_front = df[(df['date'] == front_cut_off_date) & (df['time'] == rolling_time)]
+                                df_back  = df[(df['date'] == back_cut_off_date) & (df['time'] == rolling_time)]
+
                                 df = df[(df['date'] > front_cut_off_date) | (
-                                            (df['date'] == front_cut_off_date) & (df['time'] >= rolling_time))]
+                                            (df['date'] == front_cut_off_date) & (df['time'] > rolling_time))]
                                 df = df[(df['date'] < back_cut_off_date) | (
                                             (df['date'] == back_cut_off_date) & (df['time'] < rolling_time))]
+
+                                df = pd.concat([df, df_front, df_back])
+
                             else:
                                 df = df[(df['date'] > front_cut_off_date) | (df['date'] == front_cut_off_date)]
                                 df = df[(df['date'] < back_cut_off_date) | (df['date'] == back_cut_off_date)]
 
                         df = df[df['date'] >= start_date]
                         df = df[df['date'] <= end_date]
                         df['date'] = df['date'].astype(str)
@@ -342,20 +348,22 @@
 
                         df = df.reset_index(drop=True)
                         date_time_list = df['datetime'].to_list()
 
                         df = df.sort_values(by='datetime')
 
                         if '1D' not in freq:
-                            if len(date_time_list_list) > 0:
-                                date_time_intersect = (set(date_time_list_list).intersection(date_time_list))
-                                if len(date_time_intersect) == 0:
-                                    df_list.append(df)
-                            else:
-                                df_list.append(df)
+                            # if len(date_time_list_list) > 0:
+                            #     date_time_intersect = (set(date_time_list_list).intersection(date_time_list))
+                            #     if len(date_time_intersect) == 0:
+                            #         df_list.append(df)
+                            # else:
+                            #     df_list.append(df)
+                            df_list.append(df)
+
                         else:
                             date_time_intersect = (set(date_time_list_list).intersection(date_time_list))
                             date_time_intersect = list(date_time_intersect)
                             if len(date_time_intersect) > 0:
                                 date_time_intersect_list.append(date_time_intersect[0])
                             df_list.append(df)
 
@@ -370,39 +378,74 @@
                 if '1D' not in freq:
                     df['datetime'] = pd.to_datetime(df['datetime'], format='%Y%m%d %H%M%S')
                     df['RTH'] = df['RTH'].astype(bool)
                 else:
                     df['datetime'] = pd.to_datetime(df['datetime'], format='%Y%m%d')
 
                 df = df[cols]
+                df['roll_diff'] = 0
+
                 if '1D' in freq:
                     drop_index_list = []
                     df = df.reset_index()
                     for date_time_intersect in date_time_intersect_list:
                         check_drop_index_row = df[df['date'] == date_time_intersect]
                         if len(check_drop_index_row) > 1:
                             index_0 = check_drop_index_row.index[0]
                             index_1 = check_drop_index_row.index[1]
                             expiry_date_0 = df.loc[index_0, 'expiry_date']
                             expiry_date_1 = df.loc[index_1, 'expiry_date']
+                            close_price_0 = df.loc[index_0, 'close']
+                            close_price_1 = df.loc[index_1, 'close']
                             if expiry_date_0 > expiry_date_1:
                                 drop_index_list.append(index_0)
+                                roll_diff = close_price_0 - close_price_1
+                                df.at[index_1,'roll_diff'] = roll_diff
                             elif expiry_date_0 < expiry_date_1:
                                 drop_index_list.append(index_1)
+                                roll_diff = close_price_1 - close_price_0
+                                roll_diff = close_price_0 - close_price_1
+                                df.at[index_0,'roll_diff'] = roll_diff
                     if len(drop_index_list) > 0:
                         df = df.drop(drop_index_list, axis=0)
                     df = df.drop('index', axis=1)
 
+                else:
+                    df = df.reset_index()
+
+                    duplicates = df[df.duplicated(subset=['datetime'], keep=False)]
+                    min_expiry_row_index_list = []
+
+                    for dt in duplicates['datetime'].unique():
+                        df2 = duplicates[duplicates['datetime'] == dt]
+                        min_expiry = df2['expiry_date'].min()
+                        max_expiry = df2['expiry_date'].max()
+                        min_expiry_row = df2.loc[df2['expiry_date'] == min_expiry]
+                        max_expiry_row = df2.loc[df2['expiry_date'] == max_expiry]
+                        min_expiry_row_index = min_expiry_row.index[0]
+                        max_expiry_row_index  = max_expiry_row.index[0]
+                        min_expiry_close = min_expiry_row['close'].values[0]
+                        max_expiry_close = max_expiry_row['close'].values[0]
+
+                        roll_diff = min_expiry_close - max_expiry_close
+
+                        min_expiry_row_index_list.append(min_expiry_row_index)
+                        df.at[max_expiry_row_index, 'roll_diff'] = roll_diff
+
+                    if len(min_expiry_row_index_list) > 0:
+                        df = df.drop(min_expiry_row_index_list, axis=0)
+                    df = df.drop('index', axis=1)
+
                 df = df.set_index(keys='datetime')
                 df = df.sort_index(ascending=True)
 
                 if '1D' not in freq and rth_only == True:
                     df = df[df['RTH'] == True]
 
-                # df = df.drop_duplicates(keep='last')
+                #df = df.drop_duplicates(keep='first')
 
                 return df
 
         else:
             err_msg = 'Error in: '
             for error in check_bool_dict:
                 if check_bool_dict[error] == False:
```

### Comparing `hkfdb-2.77/hkfdb.egg-info/PKG-INFO` & `hkfdb-2.8/hkfdb.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hkfdb
-Version: 2.77
+Version: 2.8
 Summary: Hong Kong Finance Database.
 Home-page: https://www.hkfdb.net
 Author: Hong Kong Finance Database Team
 Author-email: info@hkfdb.net
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `hkfdb-2.77/setup.py` & `hkfdb-2.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="hkfdb",
-    version="2.77",
+    version="2.8",
     author="Hong Kong Finance Database Team",
     author_email="info@hkfdb.net",
     description="Hong Kong Finance Database.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://www.hkfdb.net",
     packages=setuptools.find_packages(),
```

