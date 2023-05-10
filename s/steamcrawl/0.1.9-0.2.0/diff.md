# Comparing `tmp/steamcrawl-0.1.9.tar.gz` & `tmp/steamcrawl-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "steamcrawl-0.1.9.tar", last modified: Tue May  9 13:55:19 2023, max compression
+gzip compressed data, was "steamcrawl-0.2.0.tar", last modified: Wed May 10 13:35:58 2023, max compression
```

## Comparing `steamcrawl-0.1.9.tar` & `steamcrawl-0.2.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-09 13:55:19.595505 steamcrawl-0.1.9/
--rw-rw-rw-   0        0        0     1085 2023-05-06 17:48:49.000000 steamcrawl-0.1.9/LICENSE
--rw-rw-rw-   0        0        0     4672 2023-05-09 13:55:19.595505 steamcrawl-0.1.9/PKG-INFO
--rw-rw-rw-   0        0        0     4262 2023-05-09 13:47:51.000000 steamcrawl-0.1.9/README.md
--rw-rw-rw-   0        0        0       42 2023-05-09 13:55:19.595505 steamcrawl-0.1.9/setup.cfg
--rw-rw-rw-   0        0        0      656 2023-05-09 13:55:14.000000 steamcrawl-0.1.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-09 13:55:19.582605 steamcrawl-0.1.9/steamcrawl/
--rw-rw-rw-   0        0        0       28 2023-05-07 13:37:24.000000 steamcrawl-0.1.9/steamcrawl/__init__.py
--rw-rw-rw-   0        0        0      543 2023-05-07 15:13:15.000000 steamcrawl-0.1.9/steamcrawl/exceptions.py
--rw-rw-rw-   0        0        0    22255 2023-05-09 13:31:51.000000 steamcrawl-0.1.9/steamcrawl/request.py
-drwxrwxrwx   0        0        0        0 2023-05-09 13:55:19.594506 steamcrawl-0.1.9/steamcrawl.egg-info/
--rw-rw-rw-   0        0        0     4672 2023-05-09 13:55:19.000000 steamcrawl-0.1.9/steamcrawl.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      265 2023-05-09 13:55:19.000000 steamcrawl-0.1.9/steamcrawl.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-09 13:55:19.000000 steamcrawl-0.1.9/steamcrawl.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2023-05-09 13:55:19.000000 steamcrawl-0.1.9/steamcrawl.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-09 13:55:19.000000 steamcrawl-0.1.9/steamcrawl.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-10 13:35:58.486869 steamcrawl-0.2.0/
+-rw-rw-rw-   0        0        0     1085 2023-05-09 14:08:49.000000 steamcrawl-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0     4645 2023-05-10 13:35:58.485870 steamcrawl-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4235 2023-05-09 19:22:01.000000 steamcrawl-0.2.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-10 13:35:58.486869 steamcrawl-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      656 2023-05-10 13:30:45.000000 steamcrawl-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-10 13:35:58.463929 steamcrawl-0.2.0/steamcrawl/
+-rw-rw-rw-   0        0        0       28 2023-05-07 13:37:24.000000 steamcrawl-0.2.0/steamcrawl/__init__.py
+-rw-rw-rw-   0        0        0      543 2023-05-07 15:13:15.000000 steamcrawl-0.2.0/steamcrawl/exceptions.py
+-rw-rw-rw-   0        0        0    25429 2023-05-10 13:29:36.000000 steamcrawl-0.2.0/steamcrawl/request.py
+drwxrwxrwx   0        0        0        0 2023-05-10 13:35:58.484873 steamcrawl-0.2.0/steamcrawl.egg-info/
+-rw-rw-rw-   0        0        0     4645 2023-05-10 13:35:58.000000 steamcrawl-0.2.0/steamcrawl.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      265 2023-05-10 13:35:58.000000 steamcrawl-0.2.0/steamcrawl.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 13:35:58.000000 steamcrawl-0.2.0/steamcrawl.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2023-05-10 13:35:58.000000 steamcrawl-0.2.0/steamcrawl.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-10 13:35:58.000000 steamcrawl-0.2.0/steamcrawl.egg-info/top_level.txt
```

### Comparing `steamcrawl-0.1.9/LICENSE` & `steamcrawl-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `steamcrawl-0.1.9/PKG-INFO` & `steamcrawl-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: steamcrawl
-Version: 0.1.9
+Version: 0.2.0
 Summary: A package that helps extract Steam store and community market data as pandas DataFrame for better readabilty and usability.
 Home-page: https://github.com/Hungreeee/steamcrawl
 Author: Hungreeee
 Author-email: hungmnguyen13102003@gmail.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -15,15 +15,15 @@
 [![Repo Size](https://img.shields.io/github/repo-size/Hungreeee/steamcrawl.svg)](https://github.com/Hungreeee/steamcrawl/)
 [![GitHub follow](https://img.shields.io/github/followers/Hungreeee.svg?style=social&label=Follow&maxAge=2592000)](https://github.com/Hungreeee?tab=followers)
 
 # steamcrawl
 
 This is still a work in progress. Some functionality are available but not quite fully tested. The final version will be release as v1.0.0.
 
-A package that helps extract Steam store and community market data as pandas DataFrame for better readability and usability. The package mainly makes queries to different Steam API, clean and extract the important variables from the JSON object result and return a pandas Dataframe. 
+A package that helps extract Steam store and community market data as pandas DataFrame for better readability and usability. The package makes queries to different Steam API, clean and extract the important variables from the JSON object result and return a pandas Dataframe. 
 
 With the Steam request limit, you can make 200 requests every 5 minutes. If you exceed the limit, Steam can give you a cooldown of (possibly) a few 1,2 minutes to 6 hours (depending on the API). Please make an appropriate number of requests at a given time. It is recommended to close any Steam web and application to limit the requests you are sending.
 
 ## Installation and setup
 
 The following libraries are used in the package. Thus, the requirement of their installation must be met:
 
@@ -74,15 +74,15 @@
 # appid 730 indicates Counter-Strike: Global Offensive game. 
 # Obtain the appid for a game using get_all_appid().
 data_frame.to_csv('example.csv')
 ```
 
 The obtained result is (this is again only part of the result). 
 
-![example2](https://github.com/Hungreeee/steamcrawl/assets/46376260/1879c84a-edcb-4c03-9f6a-b004dee69920)ources/example2.png)
+![example2](https://github.com/Hungreeee/steamcrawl/assets/46376260/1879c84a-edcb-4c03-9f6a-b004dee69920)
 
 A small note is, please do not be alerted by the popping up browser for this request, this is only the behavior of the seleniumwire package used for this function.
 
 ## Contributions:
 
 This project is created and managed by only one user Hungreeee. Therefore, errors are entirely possible to occur anywhere in the program. If you found any bug you would like to report, please open a new Issue.
```

### Comparing `steamcrawl-0.1.9/README.md` & `steamcrawl-0.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 [![Repo Size](https://img.shields.io/github/repo-size/Hungreeee/steamcrawl.svg)](https://github.com/Hungreeee/steamcrawl/)
 [![GitHub follow](https://img.shields.io/github/followers/Hungreeee.svg?style=social&label=Follow&maxAge=2592000)](https://github.com/Hungreeee?tab=followers)
 
 # steamcrawl
 
 This is still a work in progress. Some functionality are available but not quite fully tested. The final version will be release as v1.0.0.
 
-A package that helps extract Steam store and community market data as pandas DataFrame for better readability and usability. The package mainly makes queries to different Steam API, clean and extract the important variables from the JSON object result and return a pandas Dataframe. 
+A package that helps extract Steam store and community market data as pandas DataFrame for better readability and usability. The package makes queries to different Steam API, clean and extract the important variables from the JSON object result and return a pandas Dataframe. 
 
 With the Steam request limit, you can make 200 requests every 5 minutes. If you exceed the limit, Steam can give you a cooldown of (possibly) a few 1,2 minutes to 6 hours (depending on the API). Please make an appropriate number of requests at a given time. It is recommended to close any Steam web and application to limit the requests you are sending.
 
 ## Installation and setup
 
 The following libraries are used in the package. Thus, the requirement of their installation must be met:
 
@@ -62,15 +62,15 @@
 # appid 730 indicates Counter-Strike: Global Offensive game. 
 # Obtain the appid for a game using get_all_appid().
 data_frame.to_csv('example.csv')
 ```
 
 The obtained result is (this is again only part of the result). 
 
-![example2](https://github.com/Hungreeee/steamcrawl/assets/46376260/1879c84a-edcb-4c03-9f6a-b004dee69920)ources/example2.png)
+![example2](https://github.com/Hungreeee/steamcrawl/assets/46376260/1879c84a-edcb-4c03-9f6a-b004dee69920)
 
 A small note is, please do not be alerted by the popping up browser for this request, this is only the behavior of the seleniumwire package used for this function.
 
 ## Contributions:
 
 This project is created and managed by only one user Hungreeee. Therefore, errors are entirely possible to occur anywhere in the program. If you found any bug you would like to report, please open a new Issue.
```

### Comparing `steamcrawl-0.1.9/setup.py` & `steamcrawl-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name='steamcrawl',
-    version='0.1.9',
+    version='0.2.0',
     description='A package that helps extract Steam store and community market data as pandas DataFrame for better readabilty and usability.',
     packages=["steamcrawl"],
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Hungreeee',
     author_email='hungmnguyen13102003@gmail.com',
     license='MIT',
```

### Comparing `steamcrawl-0.1.9/steamcrawl/exceptions.py` & `steamcrawl-0.2.0/steamcrawl/exceptions.py`

 * *Files identical despite different names*

### Comparing `steamcrawl-0.1.9/steamcrawl/request.py` & `steamcrawl-0.2.0/steamcrawl/request.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     :return: Nothing.
     :rtype: None
     """
 
     self.headers = {
       'Cookie': ''
     }
-    self.__all_listings_api = 'https://steamcommunity.com/market/search/render/?search_descriptions=0&norender=1'
+    self.__all_listings_api = 'https://steamcommunity.com/market/search/render/?search_descriptions=0'
     self.__appid_api = 'https://api.steampowered.com/ISteamApps/GetAppList/v2/'
     self.__pricehistory_api = 'https://steamcommunity.com/market/pricehistory/'
     self.__item_overview_api = 'https://steamcommunity.com/market/priceoverview/'
     self.__listingshistory_api = 'https://steamcommunity.com/market/myhistory/render/?norender=1'
     self.__appdetails_api = 'https://store.steampowered.com/api/appdetails/'
     self.__inventory_api = 'https://steamcommunity.com/inventory/'
 
@@ -39,19 +39,21 @@
     Set the steamLoginSecure id as headers.
 
     :param steamLoginSecure: The value of your steamLoginSecure cookie.
     :type steamLoginSecure: str
     :return: Nothing.
     :rtype: None
     """
+
     exception('type', steamLoginSecure, str, "Input steamLoginSecure it not a valid string type.")
     header = 'steamLoginSecure=' + steamLoginSecure + ';'
     testApi = 'https://steamcommunity.com/market/pricehistory/?appid=730&market_hash_name=P90%20%7C%20Blind%20Spot%20(Field-Tested)'
-    requestObject = requests.get(testApi, headers={'Cookie': header}, timeout=1.0).content
-    exception('network', requestObject, [], "Input header it not an authorized cookie header.")
+    requestObject = requests.get(testApi, headers={'Cookie': header}).content
+    jsonObject = json.loads(requestObject)
+    exception('network', jsonObject, [], "Input header it not an authorized cookie header.")
     self.headers['Cookie'] = header
 
 
   def __request_helper(self, api: str, params: dict, headers: dict, index: list):
     """
     Helper function to make requests.
 
@@ -62,67 +64,140 @@
     :param headers: The headers of the request.
     :type headers: dict
     :param index: List of indices that needs to be extracted.
     :type index: list
     :return: Nothing.
     :rtype: None
     """
+
     dfGather = []
-    requestObject = requests.get(api, params=params, headers=headers, timeout=1.0)
+    requestObject = requests.get(api, params=params, headers=headers)
     contentObject = json.loads(requestObject.content)
 
     for i in index:
       if i in contentObject:
         if contentObject[i] != []:
           dfGather.append(contentObject[i])
 
+    exception('network', dfGather, [], "No information for this API call. Please double check your parameters and try again.")
+
     if 'success' in contentObject:
       isSuccess = contentObject['success']
       exception('network', isSuccess, False, "Steam cannot make this API call. Please double check your parameters and try again.")
+
+    elif 'success' in contentObject[index[0]]:
+      isSuccess = contentObject[index[0]]['success']
+      exception('network', isSuccess, False, "There is no information for this app.")
+      exception('network', isSuccess, 0, "There is no information for this app.")
     
     if 'total_count' in contentObject and 'count' in params:
       maxPage = contentObject['total_count']
       exception('exceed', params['count'], maxPage, f"{params['count']} is larger than the maximum number of count {maxPage}.")
 
+    elif 'total_inventory_count' in contentObject and 'count' in params:
+      maxPage = contentObject['total_inventory_count']
+      exception('exceed', params['count'], maxPage, f"{params['count']} is larger than the maximum number of count {maxPage}.")
+
     return dfGather
+  
+  
+  def get_all_listings(self, sortby: str='', sortdir: str='desc', count: int = 100) -> pd.DataFrame:
+    """
+    Get listings of items exactly as how they are ordered in the community market.
+
+    :param sortby: Type of listings sorting. This includes '', 'price', and 'quantity'. The default value is ''.
+    :type sortby: str
+    :param sortdir: Direction of listings sorting. This includes 'asc' and 'desc'. The default value is 'desc'.
+    :type sortby: str
+    :param count: Number of item listings from the default list to be displayed. The default value is 100.
+    :type count: int
+    :return: Listings of items (given by count).
+    :rtype: pd.DataFrame
+    """
+    exception('type', sortby, str, "Input sortby it not a valid string type.")
+    exception('type', sortdir, str, "Input sortdir it not a valid string type.")
+    exception('type', count, int, "Input count it not a valid integer type.")
+    exception('contain', sortby, ['price', 'quantity', ''], 
+      f"{sortby} is not valid as a sortby type. It should only be '', 'price', or 'quantity'.")
+    exception('contain', sortdir, ['desc', 'asc'], 
+      f"{sortdir} is not valid as a sortby type. It should only be 'desc' or 'asc'.")
+    
+    params = {
+      'sort_column': sortby,
+      'sort_dir': '',
+      'start': 0, 
+      'count': count,
+      'norender': 1
+    }
+
+    jsonObject = self.__request_helper(self.__all_listings_api, params, self.headers, ['results'])[0]
+
+    if count == 0:
+      return pd.DataFrame()
+    
+    if count <= 100: 
+      return pd.json_normalize(jsonObject)
+    
+    else:
+      remainCount = count % 100
+      params['count'] = 100
+      dfCombined = []
+
+      for i in range(0, count - remainCount, 100):
+        params['start'] = i
+
+        jsonObject = self.__request_helper(self.__all_listings_api, params, self.headers, ['results'])[0]
+        dfCombined.append(pd.json_normalize(jsonObject))
+
+      if remainCount == 0:
+        return pd.concat(dfCombined, ignore_index=True)
+      
+      else:
+        params['start'] = count - remainCount
+        params['count'] = remainCount
+        jsonObject = self.__request_helper(self.__all_listings_api, params, self.headers, ['results'])[0]
+        dfCombined.append(pd.json_normalize(jsonObject))
+        return pd.concat(dfCombined, ignore_index=True)
 
-  def get_listings(self, sortby: str='default', sortdir: str='desc', appid: str='', count: int=100) -> pd.DataFrame:
+
+  def get_app_listings(self, appid: str, sortby: str='', sortdir: str='desc', count: int=100) -> pd.DataFrame:
     """
-    Get listings of items as in the community market listing
+    Get listings of items from a specific app exactly as how they are ordered in the community market listing.
 
-    :param sortby: Type of listings sorting. This includes 'default', 'price', 'quantity', and 'name'. The default value is 'default'.
+    :param sortby: Type of listings sorting. This includes '', 'price', 'quantity', and 'name'. The default value is ''.
     :type sortby: str
     :param sortdir: Direction of listings sorting. This includes 'asc' and 'desc'. The default value is 'desc'.
     :type sortby: str
     :param appid: Filter by app, given the id.
     :type appid: str
-    :param count: Number of item listings to be displayed. The default value is 100.
+    :param count: Number of item listings from the default list to be displayed. The default value is 100.
     :type count: int
     :return: Listings of items given the chosen filters (parameters).
     :rtype: pd.DataFrame
     """
 
     exception('type', sortby, str, "Input sortby it not a valid string type.")
     exception('type', sortdir, str, "Input sortdir it not a valid string type.")
     exception('type', count, int, "Input count it not a valid integer type.")
     exception('type', appid, str, "Input appid it not a valid string type.")
-    exception('contain', sortby, ['default', 'price', 'quantity', 'name'], 
-      f"{sortby} is not valid as a sortby type. It should only be 'default', 'price', 'quantity', or 'name'.")
+    exception('contain', sortby, ['price', 'quantity', 'name', ''], 
+      f"{sortby} is not valid as a sortby type. It should only be '', 'price', 'quantity', or 'name'.")
     exception('contain', sortdir, ['desc', 'asc'], 
       f"{sortdir} is not valid as a sortby type. It should only be 'desc' or 'asc'.")
     if appid != '':
       exception('contain', int(appid), list(self.get_all_appid()['appid']), 
         f"{appid} is not a valid appid. Please check the complete list using get_all_appid().")
     
     params = {
-      'sortcolumn': sortby,
-      'sortdir': sortdir,
+      'sort_column': sortby,
+      'sort_dir': '',
       'appid': appid,
       'start': 0, 
-      'count': count
+      'count': count,
+      'norender': 1
     }
 
     jsonObject = self.__request_helper(self.__all_listings_api, params, self.headers, ['results'])[0]
 
     if count == 0:
       return pd.DataFrame()
     
@@ -177,16 +252,16 @@
       exception('contain', int(appid), list(self.get_all_appid()['appid']), 
         f"{appid} is not a valid appid. Please check the complete list using get_all_appid().")
       
     params = {
       'appids': appid
     }
 
-    jsonObject = self.__request_helper(self.__appdetails_api, params, self.headers, [appid])[0]['data']
-    return pd.json_normalize(jsonObject)
+    jsonObject = self.__request_helper(self.__appdetails_api, params, self.headers, [appid])[0]
+    return pd.json_normalize(jsonObject['data'])
   
 
   def get_item_overview(self, item_name: str, appid: str) -> pd.DataFrame:
     """
     Get the overview (median price, volume) of an item.
 
     :param item_name: The precise market name of the item.
@@ -205,19 +280,21 @@
       exception('contain', int(appid), list(self.get_all_appid()['appid']), 
         f"{appid} is not a valid appid. Please check the complete list using get_all_appid().")
 
     params = {
       'appid': appid,
       'market_hash_name': item_name
     }
-    requestObject = requests.get(self.__item_overview_api, params=params, headers=self.headers, timeout=1.0)
-    contentObject = json.loads(requestObject.content)
-    isSuccess = contentObject['success']
+
+    requestObject = requests.get(self.__item_overview_api, params=params, headers=self.headers)
+    jsonObject = json.loads(requestObject.content)
+    exception('contain', 'volume', jsonObject, "No information for this item.")
+    isSuccess = jsonObject['success']
     exception('network', isSuccess, False, "Steam cannot make this API call. Please double check your parameters and try again.")
-    return pd.json_normalize(contentObject).drop(['success'], axis=1)
+    return pd.json_normalize(jsonObject).drop(['success'], axis=1)
     
 
   def get_price_history(self, item_name: str, appid: str) -> pd.DataFrame:
     """
     Get the price history of an item.
 
     :param item_name: The precise market name of the item.
@@ -258,27 +335,29 @@
     :param col: The name of the column that needs to be moved.
     :type col: str
     :param pos: The new index that the column is going to move to.
     :type pos: int
     :return: Nothing.
     :rtype: None
     """
+    
     col = df.pop(col)
     df.insert(pos, col.name, col)
 
 
   def __market_history_helper(self, index: list) -> pd.DataFrame:
     """
     Helper function to extract market history.
 
     :param index: List of indices that needs to be extracted.
     :type index: list
     :return: The extracted data as a data frame.
     :rtype: pd.DataFrame
     """
+
     dfCombinedAssets = []
     dfCombinedEvents = []
     dfCombinedListings = []
     dfCombinedPurchases = []
 
     for key in index[0]:
       gameJsonObject = index[0][key]
@@ -295,15 +374,15 @@
     dfCombinedEvents = dfCombinedEvents.replace({'event_type': {1: 'List', 2: 'Cancel', 3: 'Sell', 4: 'Buy'}})
 
     dfCombinedEvents['time_event'] = pd.to_datetime(dfCombinedEvents['time_event'], unit='s')
 
     for key in index[2]:
       dfCombinedListings.append(pd.json_normalize(index[2][key]))
     dfCombinedListings = pd.concat(dfCombinedListings)
-    dfCombinedListings = dfCombinedListings.drop(['currencyid', 'asset.contextid', 'asset.appid', 'asset.currency', 'steam_fee', 'publisher_fee', 'publisher_fee_percent', 'publisher_fee_app', 'price', 'fee', 'asset.amount'], axis=1)
+    dfCombinedListings = dfCombinedListings.drop(['currencyid', 'asset.contextid', 'asset.appid', 'asset.currency', 'publisher_fee_percent', 'publisher_fee_app', 'price', 'asset.amount'], axis=1)
 
     if len(index) == 4:
       for key in index[3]:
         dfCombinedPurchases.append(pd.json_normalize(index[3][key]))
       dfCombinedPurchases = pd.concat(dfCombinedPurchases)
       dfCombinedPurchases = dfCombinedPurchases.drop(['currencyid', 'time_sold', 'asset.id', 'asset.appid', 'needs_rollback', 'purchaseid', 'steam_fee', 'publisher_fee', 'publisher_fee_percent', 'publisher_fee_app', 'received_currencyid', 'asset.currency', 'asset.appid', 'asset.contextid', 'asset.appid', 'asset.classid', 'asset.new_contextid', 'asset.new_id', 'asset.instanceid', 'asset.amount', 'asset.status'], axis=1)
       dfCombinedPurchases['total_paid'] = dfCombinedPurchases['paid_amount'] + dfCombinedPurchases['paid_fee'] 
@@ -386,14 +465,15 @@
         jsonObjectList = self.__request_helper(self.__listingshistory_api, params, self.headers, ['assets', 'events', 'listings', 'purchases'])
         dfCombined.append(self.__market_history_helper(jsonObjectList))
       
       if remainCount == 0:
         return pd.concat(dfCombined).reset_index(drop=True)
       
       else:
+        params['start'] = count - remainCount
         params['count'] = remainCount
         jsonObjectList = self.__request_helper(self.__listingshistory_api, params, self.headers, ['assets', 'events', 'listings', 'purchases'])
         dfCombined.append(self.__market_history_helper(jsonObjectList))
         return pd.concat(dfCombined).reset_index(drop=True)
       
   def get_buysell_orders(self, item_name: str, appid: str) -> pd.DataFrame: 
     """
@@ -421,15 +501,15 @@
 
     for request in driver.requests:
         if request.response:
           if str(request.url[34:53]) == 'itemordershistogram':
             api = request.url
             break
     exception('network', api, "", "Steam cannot make this query. Please double check the item name and try again.")
-    response = requests.get(api + '&norender=1', headers=self.headers, timeout=1.0)
+    response = requests.get(api + '&norender=1', headers=self.headers)
     exception('network', str(response.content), 'b\'null\'', "You have reached the request limit of Steam. Please try again later.")
     contentObject = json.loads(response.content)
     dfSellGraph = pd.json_normalize(contentObject, record_path=['sell_order_graph'])
     dfBuyGraph = pd.json_normalize(contentObject, record_path=['buy_order_graph'])
     
     dfSellGraph['type'] = 'sell'
     dfBuyGraph['type'] = 'buy'
```

### Comparing `steamcrawl-0.1.9/steamcrawl.egg-info/PKG-INFO` & `steamcrawl-0.2.0/steamcrawl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: steamcrawl
-Version: 0.1.9
+Version: 0.2.0
 Summary: A package that helps extract Steam store and community market data as pandas DataFrame for better readabilty and usability.
 Home-page: https://github.com/Hungreeee/steamcrawl
 Author: Hungreeee
 Author-email: hungmnguyen13102003@gmail.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -15,15 +15,15 @@
 [![Repo Size](https://img.shields.io/github/repo-size/Hungreeee/steamcrawl.svg)](https://github.com/Hungreeee/steamcrawl/)
 [![GitHub follow](https://img.shields.io/github/followers/Hungreeee.svg?style=social&label=Follow&maxAge=2592000)](https://github.com/Hungreeee?tab=followers)
 
 # steamcrawl
 
 This is still a work in progress. Some functionality are available but not quite fully tested. The final version will be release as v1.0.0.
 
-A package that helps extract Steam store and community market data as pandas DataFrame for better readability and usability. The package mainly makes queries to different Steam API, clean and extract the important variables from the JSON object result and return a pandas Dataframe. 
+A package that helps extract Steam store and community market data as pandas DataFrame for better readability and usability. The package makes queries to different Steam API, clean and extract the important variables from the JSON object result and return a pandas Dataframe. 
 
 With the Steam request limit, you can make 200 requests every 5 minutes. If you exceed the limit, Steam can give you a cooldown of (possibly) a few 1,2 minutes to 6 hours (depending on the API). Please make an appropriate number of requests at a given time. It is recommended to close any Steam web and application to limit the requests you are sending.
 
 ## Installation and setup
 
 The following libraries are used in the package. Thus, the requirement of their installation must be met:
 
@@ -74,15 +74,15 @@
 # appid 730 indicates Counter-Strike: Global Offensive game. 
 # Obtain the appid for a game using get_all_appid().
 data_frame.to_csv('example.csv')
 ```
 
 The obtained result is (this is again only part of the result). 
 
-![example2](https://github.com/Hungreeee/steamcrawl/assets/46376260/1879c84a-edcb-4c03-9f6a-b004dee69920)ources/example2.png)
+![example2](https://github.com/Hungreeee/steamcrawl/assets/46376260/1879c84a-edcb-4c03-9f6a-b004dee69920)
 
 A small note is, please do not be alerted by the popping up browser for this request, this is only the behavior of the seleniumwire package used for this function.
 
 ## Contributions:
 
 This project is created and managed by only one user Hungreeee. Therefore, errors are entirely possible to occur anywhere in the program. If you found any bug you would like to report, please open a new Issue.
```

