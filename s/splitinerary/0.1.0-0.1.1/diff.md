# Comparing `tmp/splitinerary-0.1.0.tar.gz` & `tmp/splitinerary-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "splitinerary-0.1.0.tar", last modified: Sun Mar 26 22:17:04 2023, max compression
+gzip compressed data, was "splitinerary-0.1.1.tar", last modified: Wed May 10 02:03:50 2023, max compression
```

## Comparing `splitinerary-0.1.0.tar` & `splitinerary-0.1.1.tar`

### file list

```diff
@@ -1,33 +1,44 @@
-drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-03-26 22:17:04.613031 splitinerary-0.1.0/
--rw-r--r--   0 eugene     (501) staff       (20)      300 2023-03-26 21:57:54.000000 splitinerary-0.1.0/.bumpversion.cfg
--rw-r--r--   0 eugene     (501) staff       (20)     1058 2023-03-26 21:57:54.000000 splitinerary-0.1.0/CONTRIBUTING.md
--rw-r--r--   0 eugene     (501) staff       (20)     1063 2023-02-11 01:03:45.000000 splitinerary-0.1.0/LICENSE
--rw-r--r--   0 eugene     (501) staff       (20)      425 2023-03-26 22:06:22.000000 splitinerary-0.1.0/MANIFEST.in
--rw-r--r--   0 eugene     (501) staff       (20)     2060 2023-03-26 21:57:54.000000 splitinerary-0.1.0/Makefile
--rw-r--r--   0 eugene     (501) staff       (20)      295 2023-03-26 22:17:04.612849 splitinerary-0.1.0/PKG-INFO
--rw-r--r--   0 eugene     (501) staff       (20)     2838 2023-03-26 21:57:54.000000 splitinerary-0.1.0/README.md
--rw-r--r--   0 eugene     (501) staff       (20)     1373 2023-03-26 21:57:54.000000 splitinerary-0.1.0/pyproject.toml
--rw-r--r--   0 eugene     (501) staff       (20)       38 2023-03-26 22:17:04.613087 splitinerary-0.1.0/setup.cfg
--rw-r--r--   0 eugene     (501) staff       (20)      283 2023-03-26 22:16:59.000000 splitinerary-0.1.0/setup.py
-drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-03-26 22:17:04.610468 splitinerary-0.1.0/splitinerary/
--rw-r--r--   0 eugene     (501) staff       (20)      285 2023-03-26 21:57:54.000000 splitinerary-0.1.0/splitinerary/__init__.py
--rw-r--r--   0 eugene     (501) staff       (20)      755 2023-03-26 21:57:54.000000 splitinerary-0.1.0/splitinerary/custom_event.py
--rw-r--r--   0 eugene     (501) staff       (20)     1099 2023-03-26 21:57:54.000000 splitinerary-0.1.0/splitinerary/event.py
--rw-r--r--   0 eugene     (501) staff       (20)     2478 2023-03-26 20:12:58.000000 splitinerary-0.1.0/splitinerary/transportation.py
--rw-r--r--   0 eugene     (501) staff       (20)     4617 2023-03-26 21:57:54.000000 splitinerary-0.1.0/splitinerary/trip.py
--rw-r--r--   0 eugene     (501) staff       (20)      492 2023-03-26 21:57:54.000000 splitinerary-0.1.0/splitinerary/user.py
-drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-03-26 22:17:04.611464 splitinerary-0.1.0/splitinerary.egg-info/
--rw-r--r--   0 eugene     (501) staff       (20)      295 2023-03-26 22:17:04.000000 splitinerary-0.1.0/splitinerary.egg-info/PKG-INFO
--rw-r--r--   0 eugene     (501) staff       (20)      579 2023-03-26 22:17:04.000000 splitinerary-0.1.0/splitinerary.egg-info/SOURCES.txt
--rw-r--r--   0 eugene     (501) staff       (20)        1 2023-03-26 22:17:04.000000 splitinerary-0.1.0/splitinerary.egg-info/dependency_links.txt
--rw-r--r--   0 eugene     (501) staff       (20)        1 2023-03-26 22:17:04.000000 splitinerary-0.1.0/splitinerary.egg-info/top_level.txt
-drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-03-26 22:17:04.608225 splitinerary-0.1.0/test/
-drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-03-26 22:17:04.611815 splitinerary-0.1.0/test/integration/
--rw-r--r--   0 eugene     (501) staff       (20)        0 2023-03-10 18:52:15.000000 splitinerary-0.1.0/test/integration/__init__.py
--rw-r--r--   0 eugene     (501) staff       (20)     3616 2023-03-10 18:52:15.000000 splitinerary-0.1.0/test/integration/test_integration.py
-drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-03-26 22:17:04.612596 splitinerary-0.1.0/test/unit/
--rw-r--r--   0 eugene     (501) staff       (20)        0 2023-03-10 18:52:15.000000 splitinerary-0.1.0/test/unit/__init__.py
--rw-r--r--   0 eugene     (501) staff       (20)      769 2023-03-26 21:57:54.000000 splitinerary-0.1.0/test/unit/test_event.py
--rw-r--r--   0 eugene     (501) staff       (20)    10032 2023-03-26 21:57:54.000000 splitinerary-0.1.0/test/unit/test_transportation.py
--rw-r--r--   0 eugene     (501) staff       (20)     8648 2023-03-26 21:57:54.000000 splitinerary-0.1.0/test/unit/test_trip.py
--rw-r--r--   0 eugene     (501) staff       (20)     1867 2023-03-26 21:57:54.000000 splitinerary-0.1.0/test/unit/test_user.py
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-10 02:03:50.970202 splitinerary-0.1.1/
+-rw-r--r--   0 eugene     (501) staff       (20)      300 2023-05-10 01:34:18.000000 splitinerary-0.1.1/.bumpversion.cfg
+-rw-r--r--   0 eugene     (501) staff       (20)     1058 2023-03-26 21:57:54.000000 splitinerary-0.1.1/CONTRIBUTING.md
+-rw-r--r--   0 eugene     (501) staff       (20)     1063 2023-02-11 01:03:45.000000 splitinerary-0.1.1/LICENSE
+-rw-r--r--   0 eugene     (501) staff       (20)      425 2023-03-26 22:31:52.000000 splitinerary-0.1.1/MANIFEST.in
+-rw-r--r--   0 eugene     (501) staff       (20)     2468 2023-05-10 01:14:33.000000 splitinerary-0.1.1/Makefile
+-rw-r--r--   0 eugene     (501) staff       (20)      295 2023-05-10 02:03:50.970028 splitinerary-0.1.1/PKG-INFO
+-rw-r--r--   0 eugene     (501) staff       (20)     3086 2023-05-10 01:14:33.000000 splitinerary-0.1.1/README.md
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-10 02:03:50.966332 splitinerary-0.1.1/docs/
+-rw-------   0 eugene     (501) staff       (20)        0 2023-05-10 01:14:33.000000 splitinerary-0.1.1/docs/.nojekyll
+-rw-r--r--   0 eugene     (501) staff       (20)      634 2023-05-10 01:14:33.000000 splitinerary-0.1.1/docs/Makefile
+-rw-r--r--   0 eugene     (501) staff       (20)     1386 2023-05-10 01:34:18.000000 splitinerary-0.1.1/docs/conf.py
+-rw-r--r--   0 eugene     (501) staff       (20)     4136 2023-05-10 01:34:18.000000 splitinerary-0.1.1/docs/index.md
+-rw-r--r--   0 eugene     (501) staff       (20)      800 2023-05-10 01:14:33.000000 splitinerary-0.1.1/docs/make.bat
+-rw-r--r--   0 eugene     (501) staff       (20)       77 2023-05-10 01:14:33.000000 splitinerary-0.1.1/docs/modules.rst
+-rw-r--r--   0 eugene     (501) staff       (20)       16 2023-05-10 02:00:53.000000 splitinerary-0.1.1/docs/requirements.txt
+-rw-r--r--   0 eugene     (501) staff       (20)      941 2023-05-10 01:14:33.000000 splitinerary-0.1.1/docs/splitinerary.rst
+-rw-r--r--   0 eugene     (501) staff       (20)     1373 2023-05-10 01:34:18.000000 splitinerary-0.1.1/pyproject.toml
+-rw-r--r--   0 eugene     (501) staff       (20)       38 2023-05-10 02:03:50.970259 splitinerary-0.1.1/setup.cfg
+-rw-r--r--   0 eugene     (501) staff       (20)      292 2023-05-10 01:34:18.000000 splitinerary-0.1.1/setup.py
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-10 02:03:50.967412 splitinerary-0.1.1/splitinerary/
+-rw-r--r--   0 eugene     (501) staff       (20)      342 2023-05-10 01:34:18.000000 splitinerary-0.1.1/splitinerary/__init__.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1139 2023-05-10 01:14:33.000000 splitinerary-0.1.1/splitinerary/custom_event.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1944 2023-05-10 01:14:33.000000 splitinerary-0.1.1/splitinerary/event.py
+-rw-r--r--   0 eugene     (501) staff       (20)     4291 2023-05-10 01:14:33.000000 splitinerary-0.1.1/splitinerary/transportation.py
+-rw-r--r--   0 eugene     (501) staff       (20)     5692 2023-05-10 01:34:18.000000 splitinerary-0.1.1/splitinerary/trip.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1070 2023-05-10 01:14:33.000000 splitinerary-0.1.1/splitinerary/user.py
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-10 02:03:50.968309 splitinerary-0.1.1/splitinerary.egg-info/
+-rw-------   0 eugene     (501) staff       (20)        0 2023-05-10 02:01:41.000000 splitinerary-0.1.1/splitinerary.egg-info/Icon
+-rw-r--r--   0 eugene     (501) staff       (20)      295 2023-05-10 02:03:50.000000 splitinerary-0.1.1/splitinerary.egg-info/PKG-INFO
+-rw-r--r--   0 eugene     (501) staff       (20)      769 2023-05-10 02:03:50.000000 splitinerary-0.1.1/splitinerary.egg-info/SOURCES.txt
+-rw-r--r--   0 eugene     (501) staff       (20)        1 2023-05-10 02:03:50.000000 splitinerary-0.1.1/splitinerary.egg-info/dependency_links.txt
+-rw-r--r--   0 eugene     (501) staff       (20)        1 2023-05-10 02:03:50.000000 splitinerary-0.1.1/splitinerary.egg-info/top_level.txt
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-10 02:03:50.963769 splitinerary-0.1.1/test/
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-10 02:03:50.968627 splitinerary-0.1.1/test/integration/
+-rw-------   0 eugene     (501) staff       (20)        0 2023-03-10 18:52:15.000000 splitinerary-0.1.1/test/integration/__init__.py
+-rw-r--r--   0 eugene     (501) staff       (20)     3616 2023-03-10 18:52:15.000000 splitinerary-0.1.1/test/integration/test_integration.py
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-10 02:03:50.969752 splitinerary-0.1.1/test/unit/
+-rw-------   0 eugene     (501) staff       (20)        0 2023-03-10 18:52:15.000000 splitinerary-0.1.1/test/unit/__init__.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1802 2023-05-10 01:14:33.000000 splitinerary-0.1.1/test/unit/test_custom_event.py
+-rw-r--r--   0 eugene     (501) staff       (20)      769 2023-03-26 21:57:54.000000 splitinerary-0.1.1/test/unit/test_event.py
+-rw-r--r--   0 eugene     (501) staff       (20)    10032 2023-03-26 21:57:54.000000 splitinerary-0.1.1/test/unit/test_transportation.py
+-rw-r--r--   0 eugene     (501) staff       (20)     9200 2023-05-10 01:34:18.000000 splitinerary-0.1.1/test/unit/test_trip.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1867 2023-03-26 21:57:54.000000 splitinerary-0.1.1/test/unit/test_user.py
```

### Comparing `splitinerary-0.1.0/CONTRIBUTING.md` & `splitinerary-0.1.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `splitinerary-0.1.0/LICENSE` & `splitinerary-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `splitinerary-0.1.0/Makefile` & `splitinerary-0.1.1/Makefile`

 * *Files 27% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+TMPREPO=/tmp/docs/splitinerary
+
 #########
 # BUILD #
 #########
 develop:  ## install dependencies and build library
 	python -m pip install -e .[develop]
 
 build:  ## build the python library
@@ -74,14 +76,34 @@
 #########
 deep-clean: ## clean everything from the repository
 	git clean -fdx
 
 clean: ## clean the repository
 	rm -rf .coverage coverage cover htmlcov logs build dist *.egg-info .pytest_cache
 
+########
+# DOCS #
+########
+
+docs: 
+	$(MAKE) -C docs/ clean
+	$(MAKE) -C docs/ html
+
+pages:
+	$(MAKE) -C docs/ clean
+	$(MAKE) -C docs/ html
+	rm -rf $(TMPREPO)
+	git clone -b gh-pages https://github.com/el3030/splitinerary.git $(TMPREPO)
+	rm -rf $(TMPREPO)/*
+	cp -r docs/_build/html/* $(TMPREPO)
+	cd $(TMPREPO);\
+	git add -A ;\
+	git commit -a -m 'auto-updating docs' ;\
+	git push
+
 ############################################################################################
 
 # Thanks to Francoise at marmelab.com for this
 .DEFAULT_GOAL := help
 help:
 	@grep -E '^[a-zA-Z_-]+:.*?## .*$$' $(MAKEFILE_LIST) | sort | awk 'BEGIN {FS = ":.*?## "}; {printf "\033[36m%-30s\033[0m %s\n", $$1, $$2}'
```

### Comparing `splitinerary-0.1.0/README.md` & `splitinerary-0.1.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -2,14 +2,17 @@
 
 Splitinerary is a collaborative itinerary library in Python.
 
 [![](https://img.shields.io/github/license/el3030/splitinerary)](https://opensource.org/license/mit/)
 [![](https://img.shields.io/github/issues/el3030/splitinerary)](https://github.com/el3030/splitinerary/issues)
 [![Build Status](https://github.com/el3030/splitinerary/workflows/Build%20Status/badge.svg?branch=main)](https://github.com/el3030/splitinerary/actions/workflows/build.yml)
 [![codecov](https://codecov.io/gh/el3030/splitinerary/branch/main/graph/badge.svg)](https://codecov.io/gh/el3030/splitinerary)
+[![PyPI](https://img.shields.io/pypi/v/splitinerary)](https://pypi.org/project/splitinerary/)
+[![Documentation Status](https://readthedocs.org/projects/splitinerary/badge/?version=latest)](https://el3030.github.io/splitinerary/)
+
 
 ## Overview
 
 Coordinating a group to go on a trip together is difficult because some people may fly to the same destination from different origins, some people may split off mid-trip to go somewhere else and rejoin, and some people might be staying in different places (with relatives, for example). This python program will be the core functionality for an app that allows users to work together to create a collaborative itinerary.
 
 - Trips are objects that have one or more users associated with it.
 - Each trip will have events inside of it like flights, hotels, trains, AirBnBs, concerts, etc. that each user can associate him or herself with.
@@ -63,15 +66,15 @@
 events = trip.get_all_events()
 ```
 
 For a full list of objects and functions, please see documentation.
 
 ## Documentation
 
-To be released soon!
+https://el3030.github.io/splitinerary/
 
 ## Details
 
 The source code is currently hosted on GitHub at: https://github.com/el3030/splitinerary
```

### Comparing `splitinerary-0.1.0/pyproject.toml` & `splitinerary-0.1.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 build-backend="setuptools.build_meta"
 
 [project]
 name = "splitinerary"
 authors = [{name = "Eugene Li", email = "el3030@columbia.edu"}]
 description="A collaborative itinerary for planning group trips!"
 readme = "README.md"
-version = "0.1.0"
+version = "0.1.1"
 requires-python = ">=3.8"
 
 dependencies = []
 
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "Programming Language :: Python :: Implementation :: CPython",
```

### Comparing `splitinerary-0.1.0/splitinerary/event.py` & `splitinerary-0.1.1/splitinerary/event.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,34 +1,62 @@
 class Event:
-    """
-    Event object. Sortable by datetime.
+    """Event object. Each event is sortable among other Events by datetime.
 
     Attributes:
-        datetime: datetime.datetime object of when the user wants to arrive at
-        the event, NOT NECESSARILY when the event starts (e.g. user might
-        arrive at the airport 2 hours before the flight departs)
+        datetime (datetime.datetime): when the user wants to arrive at
+            the event, NOT NECESSARILY when the event starts (e.g. user might
+            arrive at the airport 2 hours before the flight departs).
     """
 
     def __init__(self, datetime, users=None):
+        """Inits Event.
+
+        Args:
+            datetime (datetime.Datetime): datetime.Datetime object of when the
+                user gets to the event.
+            users (list of User, optional): Users participating in the Event.
+                Defaults to None.
+        """
         self.datetime = datetime
         if users is None:
             self.users = []
         else:
             self.users = users
 
     def add_user(self, user):
+        """Add user to Event.
+
+        Args:
+            user (User): User to add to Event.
+        """
         self.users.append(user)
 
     def get_users(self):
+        """Get Users participating in Event.
+
+        Returns:
+            list of User: Users participating in Event if there are any,
+                else None.
+        """
         return self.users if self.users else None
 
     def get_date(self):
+        """Get date of Event.
+
+        Returns:
+            datetime.Date: Date the event takes place on.
+        """
         return self.datetime.date()
 
     def get_time(self):
+        """Get time of Event (without the date).
+
+        Returns:
+            datetime.Time: Time the event takes place on.
+        """
         return self.datetime.time()
 
     def __lt__(self, other):
         return self.datetime < other.datetime
 
     def __eq__(self, other):
         return self.datetime == other.datetime
```

### Comparing `splitinerary-0.1.0/splitinerary/trip.py` & `splitinerary-0.1.1/splitinerary/trip.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,129 +1,137 @@
 import datetime
 from collections import defaultdict
 
 
 class Trip:
-    """
-    Trip object.
+    """Trip object that everything else in Splitinerary gets added to.
 
     Attributes:
-        dates_list (list): list (that can be sorted) of datetime.date, used to
-            keep track of which dates have events on them.
-        dates_dict (dict): {datetime.date : event.Event}
+        dates_list (list of datetime.date): sortable list of datetime.date,
+            used to keep track of which dates have events on them.
+        dates_dict (dict of datetime.date : event.Event):
             keys can be used to see if date exists in trip, values are lists
             (that can be sorted) of each day's events.
-        user_activities (dict): {user: {date: [event1, event2]}}
+        user_activities (dict of user: {date: [event1, event2]}):
+            Maps users to their activities on dates
     """
 
     def __init__(self):
+        """Inits Trip."""
         self.dates_list = []
         self.dates_dict = {}
         self.user_activities = defaultdict(lambda: defaultdict(list))
 
     def add_event(self, event):
-        """
-        Add an (already made) event to the Trip.
+        """Add an Event object to the Trip.
         This involves adding the date of the event to self.dates_list and
-            adding the event to self.dates_dict[date].
+        adding the event to self.dates_dict[date].
 
-        Parameters:
-            event (event.Event):  The event to be added to the Trip.
-        Returns:
-            None
+        Args:
+            event (Event):  The event to be added to the Trip.
         """
         date = event.get_date()
         if date not in self.dates_dict:
             self.dates_list.append(date)
             self.dates_dict[date] = []
         self.dates_dict[date].append(event)
 
         users = event.get_users()
         if users is not None:
             for user in users:
                 self.user_activities[user][date].append(event)
 
     def get_events_on_date(self, date):
-        """
-        Returns of the events on a certain day in order of start time.
+        """Returns of the events on a certain day in order of start time.
 
-        Parameters:
+        Args:
             date (datetime.date):  the date whose events are to be returned.
+
         Returns:
-            times_list (List[(datetime.time, events.Event)]): sorted list of
+            list of (datetime.time, Event): sorted list of tuples of
             events on the input date if it exists, else None.
         """
         if date not in self.dates_dict:
             return None
         else:
             self.dates_dict[date].sort()
             return self.dates_dict[date]
 
     def get_eventful_dates(self):
-        """
-        Print all of the dates that have an event on them in order of start
+        """Print all of the dates that have an event on them in order of start
             time.
 
-        Parameters:
-            None
         Returns:
-            dates_list (List[datetime.date]): sorted list of dates that have
+            list of datetime.date: sorted list of dates that have
             events on them if it exists, else None.
-
         """
         if not self.dates_list:
             return None
         self.dates_list.sort()
         return self.dates_list
 
     def get_all_events(self):
-        """
-        Returns all events in the trip in order of start time.
+        """Returns all events in the Trip in order of start time.
 
-        Parameters:
-            None
         Returns:
-            all_events (List[event.Event]): sorted list of all events in the
+            list of Event: sorted list of all events in the
             trip.
         """
         if not self.dates_dict:
             return None
         all_events = []
         for events in self.dates_dict.values():
             all_events.extend(events)
         all_events.sort()
         return all_events
 
     def get_next_event(self):
-        """
-        Returns the next event that will take place for any user.
+        """Returns the next event that will take place for any user.
 
-        Parameters:
-            None
         Returns:
-            event (event.Event): the next event that will take place for any
-            user if it exists, else None.
+            Event: the next event that will take place for any
+            User if it exists, else None.
         """
         now = datetime.datetime.now()
         all_events = self.get_all_events()
         for event in all_events:
             if event.datetime < now:
                 continue
             return event
         return None
 
     def get_users_list(self):
+        """Gets list of users participating in Trip.
+
+        Returns:
+            list of Users: A list of users participating in Trip.
+        """
         return list(self.user_activities.keys())
 
     def get_events_of_user(self, user):
+        """Gets the events of a given User.
+
+        Args:
+            user (User): A User in the Trip.
+
+        Returns:
+            dict of user: {date: [event1, event2]} : dictionary of user's
+            events for each day.
+        """
         if user not in self.user_activities:
             return None
         return self.user_activities[user]
 
     def remove_event_by_index(self, date, index):
+        """Remove an Event from a Trip given a date and index of Event on date.
+
+        Args:
+            date (datetime.Date): Date of event.
+            index (int): Index of Event on date, in order of time.
+        """
         if date not in self.dates_dict:
             return
         days_events_list = self.dates_dict[date]
         if index < 0 or index >= len(days_events_list):
             return
         removed_event = days_events_list.pop(index)
         event_date = removed_event.get_date()
@@ -135,14 +143,34 @@
         # remove event from each affected user's user_activities dict entry
         affected_users = removed_event.get_users()
         for user in affected_users:
             users_events = self.user_activities[user]
             users_events[event_date].remove(removed_event)
 
     def remove_user_from_event(self, user, event):
+        """Remove a User from an Event in the Trip.
+
+        Args:
+            user (User): User to remove from Event.
+            event (Event): Event from which User is being removed.
+        """
         event_date = event.get_date()
 
         users_events = self.user_activities[user]
         users_events[event_date].remove(event)
 
         users_list = event.get_users()
         users_list.remove(user)
+
+    def add_user_to_event(self, user, event):
+        """Add a user to an Event in the Trip.
+
+        Args:
+            user (User): User to add to the Event.
+            event (Event): Event from which User is being added.
+        """
+        event_date = event.get_date()
+
+        users_events = self.user_activities[user]
+        users_events[event_date].append(event)
+
+        event.add_user(user)
```

### Comparing `splitinerary-0.1.0/splitinerary.egg-info/SOURCES.txt` & `splitinerary-0.1.1/splitinerary.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -2,24 +2,34 @@
 CONTRIBUTING.md
 LICENSE
 MANIFEST.in
 Makefile
 README.md
 pyproject.toml
 setup.py
+docs/.nojekyll
+docs/Makefile
+docs/conf.py
+docs/index.md
+docs/make.bat
+docs/modules.rst
+docs/requirements.txt
+docs/splitinerary.rst
 splitinerary/__init__.py
 splitinerary/custom_event.py
 splitinerary/event.py
 splitinerary/transportation.py
 splitinerary/trip.py
 splitinerary/user.py
+splitinerary.egg-info/Icon
 splitinerary.egg-info/PKG-INFO
 splitinerary.egg-info/SOURCES.txt
 splitinerary.egg-info/dependency_links.txt
 splitinerary.egg-info/top_level.txt
 test/integration/__init__.py
 test/integration/test_integration.py
 test/unit/__init__.py
+test/unit/test_custom_event.py
 test/unit/test_event.py
 test/unit/test_transportation.py
 test/unit/test_trip.py
 test/unit/test_user.py
```

### Comparing `splitinerary-0.1.0/test/integration/test_integration.py` & `splitinerary-0.1.1/test/integration/test_integration.py`

 * *Files identical despite different names*

### Comparing `splitinerary-0.1.0/test/unit/test_event.py` & `splitinerary-0.1.1/test/unit/test_event.py`

 * *Files identical despite different names*

### Comparing `splitinerary-0.1.0/test/unit/test_transportation.py` & `splitinerary-0.1.1/test/unit/test_transportation.py`

 * *Files identical despite different names*

### Comparing `splitinerary-0.1.0/test/unit/test_trip.py` & `splitinerary-0.1.1/test/unit/test_trip.py`

 * *Files 2% similar despite different names*

```diff
@@ -312,7 +312,27 @@
 
         # act
         trip.remove_user_from_event(user1, event1)
 
         # assert
         event_participants = event1.get_users()
         self.assertListEqual(event_participants, [user2])
+
+
+class TestAddUserToEvent(unittest.TestCase):
+    def test_add_user_to_event_success(self):
+        # arrange
+        now = datetime.datetime.now()
+
+        user1 = User('tim', 'paine', 'tim@columbia.edu')
+        user2 = User('catelen', 'wu', 'catelen@columbia.edu')
+        event1 = Event(now, [user1])
+
+        trip = Trip()
+        trip.add_event(event1)
+
+        # act
+        trip.add_user_to_event(user2, event1)
+
+        # assert
+        event_participants = event1.get_users()
+        self.assertListEqual(event_participants, [user1, user2])
```

### Comparing `splitinerary-0.1.0/test/unit/test_user.py` & `splitinerary-0.1.1/test/unit/test_user.py`

 * *Files identical despite different names*

