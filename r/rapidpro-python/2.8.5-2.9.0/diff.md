# Comparing `tmp/rapidpro-python-2.8.5.tar.gz` & `tmp/rapidpro_python-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rapidpro-python-2.8.5.tar", max compression
+gzip compressed data, was "rapidpro_python-2.9.0.tar", max compression
```

## Comparing `rapidpro-python-2.8.5.tar` & `rapidpro_python-2.9.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1476 2022-03-31 19:16:56.871990 rapidpro-python-2.8.5/LICENSE
--rw-r--r--   0        0        0     1387 2022-03-31 19:16:56.871990 rapidpro-python-2.8.5/README.md
--rw-r--r--   0        0        0      867 2022-03-31 19:16:56.871990 rapidpro-python-2.8.5/pyproject.toml
--rw-r--r--   0        0        0      129 2022-03-31 19:16:56.871990 rapidpro-python-2.8.5/temba_client/__init__.py
--rw-r--r--   0        0        0     9211 2022-03-31 19:16:56.871990 rapidpro-python-2.8.5/temba_client/base.py
--rw-r--r--   0        0        0     1690 2022-03-31 19:16:56.871990 rapidpro-python-2.8.5/temba_client/exceptions.py
--rw-r--r--   0        0        0     4660 2022-03-31 19:16:56.871990 rapidpro-python-2.8.5/temba_client/serialization.py
--rw-r--r--   0        0        0    11762 2022-03-31 19:16:56.871990 rapidpro-python-2.8.5/temba_client/tests.py
--rw-r--r--   0        0        0      851 2022-03-31 19:16:56.871990 rapidpro-python-2.8.5/temba_client/utils.py
--rw-r--r--   0        0        0    24778 2022-03-31 19:16:56.871990 rapidpro-python-2.8.5/temba_client/v2/__init__.py
--rw-r--r--   0        0        0    54405 2022-03-31 19:16:56.871990 rapidpro-python-2.8.5/temba_client/v2/tests.py
--rw-r--r--   0        0        0     6798 2022-03-31 19:16:56.871990 rapidpro-python-2.8.5/temba_client/v2/types.py
--rw-r--r--   0        0        0     2112 2022-03-31 19:17:08.916974 rapidpro-python-2.8.5/setup.py
--rw-r--r--   0        0        0     2362 2022-03-31 19:17:08.917437 rapidpro-python-2.8.5/PKG-INFO
+-rw-r--r--   0        0        0     1476 2023-01-17 19:10:29.590880 rapidpro_python-2.9.0/LICENSE
+-rw-r--r--   0        0        0     1387 2023-01-17 19:10:29.590880 rapidpro_python-2.9.0/README.md
+-rw-r--r--   0        0        0     1236 2023-01-17 19:10:29.594880 rapidpro_python-2.9.0/pyproject.toml
+-rw-r--r--   0        0        0      129 2023-01-17 19:10:29.594880 rapidpro_python-2.9.0/temba_client/__init__.py
+-rw-r--r--   0        0        0     9211 2023-01-17 19:10:29.594880 rapidpro_python-2.9.0/temba_client/base.py
+-rw-r--r--   0        0        0     1690 2023-01-17 19:10:29.594880 rapidpro_python-2.9.0/temba_client/exceptions.py
+-rw-r--r--   0        0        0     4660 2023-01-17 19:10:29.594880 rapidpro_python-2.9.0/temba_client/serialization.py
+-rw-r--r--   0        0        0    11775 2023-01-17 19:10:29.594880 rapidpro_python-2.9.0/temba_client/tests.py
+-rw-r--r--   0        0        0      851 2023-01-17 19:10:29.594880 rapidpro_python-2.9.0/temba_client/utils.py
+-rw-r--r--   0        0        0    24731 2023-01-17 19:10:29.594880 rapidpro_python-2.9.0/temba_client/v2/__init__.py
+-rw-r--r--   0        0        0    54927 2023-01-17 19:10:29.594880 rapidpro_python-2.9.0/temba_client/v2/tests.py
+-rw-r--r--   0        0        0     7235 2023-01-17 19:10:29.594880 rapidpro_python-2.9.0/temba_client/v2/types.py
+-rw-r--r--   0        0        0     2118 1970-01-01 00:00:00.000000 rapidpro_python-2.9.0/setup.py
+-rw-r--r--   0        0        0     2311 1970-01-01 00:00:00.000000 rapidpro_python-2.9.0/PKG-INFO
```

### Comparing `rapidpro-python-2.8.5/LICENSE` & `rapidpro_python-2.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rapidpro-python-2.8.5/README.md` & `rapidpro_python-2.9.0/README.md`

 * *Files identical despite different names*

### Comparing `rapidpro-python-2.8.5/pyproject.toml` & `rapidpro_python-2.9.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rapidpro-python"
-version = "2.8.5"
+version = "2.9.0"
 description = "Python client library for the RapidPro API"
 authors = ["Nyaruka <code@nyaruka.com>"]
 readme = "README.md"
 license = "BSD-4-Clause"
 classifiers=[
     'Development Status :: 5 - Production/Stable',
     'Intended Audience :: Developers',
@@ -16,21 +16,40 @@
     { include = "temba_client" },
 ]
 
 [tool.poetry.urls]
 repository = "http://github.com/rapidpro/rapidpro-python"
 
 [tool.poetry.dependencies]
-python = "^3.6"
+python = "^3.9"
 pytz = "*"
 requests = "^2.25.0"
 iso8601 = "^0.1.13"
 
 [tool.poetry.dev-dependencies]
-nose = "^1.3.7"
 coverage = "^5.3"
-flake8 = "^3.8.4"
 codecov = "^2.1.10"
+ruff = "^0.0.171"
+isort = "^5.10.1"
+black = "^22.10.0"
+nose2 = "^0.12.0"
+
+[tool.black]
+line-length = 119
+
+[tool.ruff]
+line-length = 120
+select = ["E", "F", "W"]
+ignore = ["E501", "F405"]
+fix = true
+
+[tool.isort]
+multi_line_output = 3
+force_grid_wrap = 0
+line_length = 119
+include_trailing_comma = true
+combine_as_imports = true
+sections = ["FUTURE", "STDLIB", "THIRDPARTY", "FIRSTPARTY", "LOCALFOLDER"]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `rapidpro-python-2.8.5/temba_client/base.py` & `rapidpro_python-2.9.0/temba_client/base.py`

 * *Files identical despite different names*

### Comparing `rapidpro-python-2.8.5/temba_client/exceptions.py` & `rapidpro_python-2.9.0/temba_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `rapidpro-python-2.8.5/temba_client/serialization.py` & `rapidpro_python-2.9.0/temba_client/serialization.py`

 * *Files identical despite different names*

### Comparing `rapidpro-python-2.8.5/temba_client/tests.py` & `rapidpro_python-2.9.0/temba_client/tests.py`

 * *Files 1% similar despite different names*

```diff
@@ -157,15 +157,16 @@
 
         self.assertRaises(TembaSerializationException, field.deserialize, 1.5)
         self.assertRaises(TembaSerializationException, field.deserialize, "")
 
     def test_object_list(self):
         field = ObjectListField(item_class=TestSubType)
         self.assertEqual(
-            field.serialize([TestSubType.create(zed="a"), TestSubType.create(zed=2)]), [{"zed": "a"}, {"zed": 2}]
+            field.serialize([TestSubType.create(zed="a"), TestSubType.create(zed=2)]),
+            [{"zed": "a"}, {"zed": 2}],
         )
 
         self.assertRaises(TembaSerializationException, field.serialize, "Not a list")
 
         obj_list = field.deserialize([{"zed": "a"}, {"zed": 2}])
         self.assertEqual(len(obj_list), 2)
         self.assertEqual(obj_list[0].zed, "a")
```

### Comparing `rapidpro-python-2.8.5/temba_client/utils.py` & `rapidpro_python-2.9.0/temba_client/utils.py`

 * *Files identical despite different names*

### Comparing `rapidpro-python-2.8.5/temba_client/v2/__init__.py` & `rapidpro_python-2.9.0/temba_client/v2/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,14 @@
     Run,
 )
 
 
 class TembaClient(BaseCursorClient):
     """
     Client for the Temba API v2
-
     :param str host: server hostname, e.g. 'rapidpro.io'
     :param str token: organization API token
     :param str user_agent: string to be included in the User-Agent header
     """
 
     def __init__(self, host, token, user_agent=None, verify_ssl=None):
         super(TembaClient, self).__init__(host, token, 2, user_agent, verify_ssl)
@@ -40,105 +39,96 @@
     # ==================================================================================================================
     # Fetch object operations
     # ==================================================================================================================
 
     def get_archives(self, archive_type=None, period=None, before=None, after=None):
         """
         Gets all matching archives
-
         :param str archive_type: "message" or "run"
         :param str period: "daily" or "monthly"
         :param datetime before: created before
         :param datetime after: created after
         :return: archive query
         """
 
         params = self._build_params(archive_type=archive_type, period=period, before=before, after=after)
         return self._get_query("archives", params, Archive)
 
     def get_boundaries(self, geometry=None):
         """
         Gets all administrative boundaries
-
         :return: boundary query
         """
         params = self._build_params(geometry=geometry)
         return self._get_query("boundaries", params, Boundary)
 
     def get_broadcasts(self, id=None, before=None, after=None):
         """
         Gets all matching broadcasts
-
         :param id: broadcast id
         :param datetime before: created before
         :param datetime after: created after
         :return: broadcast query
         """
         params = self._build_params(id=id, before=before, after=after)
         return self._get_query("broadcasts", params, Broadcast)
 
     def get_campaigns(self, uuid=None):
         """
         Gets all matching campaigns
-
         :param uuid: campaigns UUID
         :return: campaign query
         """
         params = self._build_params(uuid=uuid)
         return self._get_query("campaigns", params, Campaign)
 
     def get_campaign_events(self, uuid=None, campaign=None):
         """
         Gets all matching campaign events
-
         :param uuid: event UUID
         :param campaign: campaign object or UUID
         :return: campaign event query
         """
         params = self._build_params(uuid=uuid, campaign=campaign)
         return self._get_query("campaign_events", params, CampaignEvent)
 
     def get_channels(self, uuid=None, address=None):
         """
         Gets all matching channels
-
         :param uuid: channel UUID
         :param urn: channel address
         :return: channel query
         """
         params = self._build_params(uuid=uuid, address=address)
         return self._get_query("channels", params, Channel)
 
     def get_channel_events(self, id=None, contact=None, before=None, after=None):
         """
         Gets all matching channel events
-
         :param id: event id
         :param contact: contact object or UUID
         :param datetime before: created before
         :param datetime after: created after
         :return: channel event query
         """
         params = self._build_params(id=id, contact=contact, before=before, after=after)
         return self._get_query("channel_events", params, ChannelEvent)
 
     def get_classifiers(self, uuid=None):
         """
         Gets all matching NLU classifiers
-
         :param uuid: classifier UUID
         :return: classifier query
         """
         params = self._build_params(uuid=uuid)
         return self._get_query("classifiers", params, Classifier)
 
     def get_contacts(self, uuid=None, urn=None, group=None, deleted=None, before=None, after=None, reverse=None):
         """
         Gets all matching contacts
-
         :param uuid: contact UUID
         :param urn: contact URN
         :param group: contact group name or UUID
         :param deleted: return deleted contact only
         :param reverse: whether to return contacts ordered in reverse (oldest first).
         :param datetime before: modified before
         :param datetime after: modified after
@@ -148,82 +138,74 @@
             uuid=uuid, urn=urn, group=group, deleted=deleted, reverse=reverse, before=before, after=after
         )
         return self._get_query("contacts", params, Contact)
 
     def get_definitions(self, flows=(), campaigns=(), dependencies=None):
         """
         Gets an export of specified definitions
-
         :param flows: flow objects or UUIDs to include
         :param campaigns: campaign objects or UUIDs to include
         :param dependencies: whether to include dependencies
         :return: definitions export
         """
         params = self._build_params(flow=flows, campaign=campaigns, dependencies=dependencies)
         return Export.deserialize(self._get_raw("definitions", params))
 
     def get_fields(self, key=None):
         """
         Gets all matching contact fields
-
         :param key: field key
         :return: field query
         """
         return self._get_query("fields", self._build_params(key=key), Field)
 
     def get_flows(self, uuid=None):
         """
         Gets all matching flows
-
         :param uuid: flow UUID
         :return: flow query
         """
         return self._get_query("flows", self._build_params(uuid=uuid), Flow)
 
     def get_flow_starts(self, uuid=None):
         """
         Gets all matching flows starts
-
         :param uuid: flow start UUID
         :return: flow start query
         """
         return self._get_query("flow_starts", self._build_params(uuid=uuid), FlowStart)
 
     def get_globals(self):
         """
         Gets all globals
-
         :return: global query
         """
         return self._get_query("globals", {}, Global)
 
     def get_groups(self, uuid=None, name=None):
         """
         Gets all matching contact groups
-
         :param uuid: group UUID
         :param name: group name
         :return: group query
         """
         return self._get_query("groups", self._build_params(uuid=uuid, name=name), Group)
 
     def get_labels(self, uuid=None, name=None):
         """
         Gets all matching message labels
-
         :param uuid: label UUID
         :param name: label name
         :return: label query
         """
         return self._get_query("labels", self._build_params(uuid=uuid, name=name), Label)
 
     def get_messages(self, id=None, broadcast=None, contact=None, folder=None, label=None, before=None, after=None):
         """
         Gets all matching messages
-
         :param id: message id
         :param broadcast: broadcast id
         :param contact: contact object or UUID
         :param folder: folder name
         :param label: message label name or UUID
         :param datetime before: created before
         :param datetime after: created after
@@ -233,67 +215,62 @@
             id=id, broadcast=broadcast, contact=contact, folder=folder, label=label, before=before, after=after
         )
         return self._get_query("messages", params, Message)
 
     def get_org(self, retry_on_rate_exceed=False):
         """
         Gets the current organization
-
         :param retry_on_rate_exceed: whether to sleep and retry if request rate limit exceeded
         :return: the org
         """
         return Org.deserialize(self._get_raw("org", {}, retry_on_rate_exceed))
 
     def get_resthooks(self):
         """
         Gets all resthooks
-
         :return: resthook query
         """
         return self._get_query("resthooks", {}, Resthook)
 
     def get_resthook_events(self, resthook=None):
         """
         Gets all resthook events
-
         :param resthook: the resthook slug
         :return: resthook event query
         """
         params = self._build_params(resthook=resthook)
         return self._get_query("resthook_events", params, ResthookEvent)
 
     def get_resthook_subscribers(self, id=None, resthook=None):
         """
         Gets all resthook subscribers
-
         :param id: subscriber id
         :param resthook: the resthook slug
         :return: resthook subscriber query
         """
         params = self._build_params(id=id, resthook=resthook)
         return self._get_query("resthook_subscribers", params, ResthookSubscriber)
 
     def get_runs(
-        self, id=None, flow=None, contact=None, responded=None, before=None, after=None, reverse=None, paths=None
+        self, uuid=None, flow=None, contact=None, responded=None, before=None, after=None, reverse=None, paths=None
     ):
         """
         Gets all matching flow runs
-
-        :param id: flow run id
+        :param uuid: flow run UUID
         :param flow: flow object or UUID
         :param contact: contact object or UUID
         :param responded: whether to limit results to runs with responses
         :param datetime before: modified before
         :param datetime after: modified after
         :param reverse: whether to return results ordered in reverse (oldest first).
         :param paths: whether to include path data
         :return: flow run query
         """
         params = self._build_params(
-            id=id,
+            uuid=uuid,
             flow=flow,
             contact=contact,
             responded=responded,
             reverse=reverse,
             before=before,
             after=after,
             paths=paths,
@@ -303,39 +280,36 @@
     # ==================================================================================================================
     # Create object operations
     # ==================================================================================================================
 
     def create_broadcast(self, text, urns=None, contacts=None, groups=None):
         """
         Creates and sends a broadcast to the given URNs, contacts or contact groups
-
         :param str text: message text
         :param list[str] urns: list of URN strings
         :param list contacts: list of contact objects or UUIDs
         :param list groups: list of group objects or UUIDs
         :return: the new broadcast
         """
         payload = self._build_params(text=text, urns=urns, contacts=contacts, groups=groups)
         return Broadcast.deserialize(self._post("broadcasts", None, payload))
 
     def create_campaign(self, name, group):
         """
         Creates a new campaign
-
         :param str name: campaign name
         :param * group: group object, UUID or name
         :return: the new campaign
         """
         payload = self._build_params(name=name, group=group)
         return Campaign.deserialize(self._post("campaigns", None, payload))
 
     def create_campaign_event(self, campaign, relative_to, offset, unit, delivery_hour, message=None, flow=None):
         """
         Creates a new campaign event
-
         :param * campaign: campaign object, UUID or name
         :param str relative_to: contact field key
         :param int offset:
         :param str unit:
         :param int delivery_hour:
         :param str message:
         :param * flow: flow object, UUID or name
@@ -351,41 +325,38 @@
             flow=flow,
         )
         return CampaignEvent.deserialize(self._post("campaign_events", None, payload))
 
     def create_contact(self, name=None, language=None, urns=None, fields=None, groups=None):
         """
         Creates a new contact
-
         :param str name: full name
         :param str language: the language code, e.g. "eng"
         :param list[str] urns: list of URN strings
         :param dict[str,str] fields: dictionary of contact field values
         :param list groups: list of group objects, UUIDs or names
         :return: the new contact
         """
         payload = self._build_params(name=name, language=language, urns=urns, fields=fields, groups=groups)
         return Contact.deserialize(self._post("contacts", None, payload))
 
     def create_field(self, label, value_type):
         """
         Creates a new contact field
-
         :param str label: field label
         :param str value_type: field value type
         :return: the new field
         """
         return Field.deserialize(self._post("fields", None, self._build_params(label=label, value_type=value_type)))
 
     def create_flow_start(
         self, flow, urns=None, contacts=None, groups=None, restart_participants=None, exclude_active=None, params=None
     ):
         """
         Creates a new flow start
-
         :param str flow: flow UUID
         :param list[str] urns: URNs of contacts to start
         :param list[str] contacts: UUIDs of contacts to start
         :param list[str] groups: UUIDs of contact groups to start
         :param bool restart_participants: whether to restart participants already in this flow
         :param bool exclude_active: whether to exclude contacts currently in other flows
         :param * params: a dictionary of parameters to pass to the flow
@@ -401,72 +372,66 @@
             params=params,
         )
         return FlowStart.deserialize(self._post("flow_starts", None, payload))
 
     def create_global(self, name, value):
         """
         Creates a new global
-
         :param str name: global name
         :param str value: global value
         :return: the new global
         """
         payload = self._build_params(name=name, value=value)
         return Global.deserialize(self._post("globals", None, payload))
 
     def create_group(self, name):
         """
         Creates a new contact group
-
         :param str name: group name
         :return: the new group
         """
         return Group.deserialize(self._post("groups", None, self._build_params(name=name)))
 
     def create_label(self, name):
         """
         Creates a new message label
-
         :param str name: label name
         :return: the new label
         """
         return Label.deserialize(self._post("labels", None, self._build_params(name=name)))
 
     def create_resthook_subscriber(self, resthook, target_url):
         """
         Creates a new resthook subscriber
-
         :param resthook: the resthook slug
         :param target_url: the target URL
         :return: the new subscriber
         """
         payload = self._build_params(resthook=resthook, target_url=target_url)
         return ResthookSubscriber.deserialize(self._post("resthook_subscribers", None, payload))
 
     # ==================================================================================================================
     # Update object operations
     # ==================================================================================================================
 
     def update_campaign(self, campaign, name, group):
         """
         Updates an existing campaign
-
         :param * campaign: campaign object, UUID or URN
         :param str name: campaign name
         :param * group: group object, UUID or name
         :return: the updated campaign
         """
         params = self._build_id_param(uuid=campaign)
         payload = self._build_params(name=name, group=group)
         return Campaign.deserialize(self._post("campaigns", params, payload))
 
     def update_campaign_event(self, event, relative_to, offset, unit, delivery_hour, message=None, flow=None):
         """
         Updates an existing campaign event
-
         :param * event: campaign event object, UUID or name
         :param str relative_to: contact field key
         :param int offset:
         :param str unit:
         :param int delivery_hour:
         :param str message:
         :param * flow: flow object, UUID or name
@@ -477,15 +442,14 @@
             relative_to=relative_to, offset=offset, unit=unit, delivery_hour=delivery_hour, message=message, flow=flow
         )
         return CampaignEvent.deserialize(self._post("campaign_events", params, payload))
 
     def update_contact(self, contact, name=None, language=None, urns=None, fields=None, groups=None):
         """
         Updates an existing contact
-
         :param * contact: contact object, UUID or URN
         :param str name: full name
         :param str language: the language code, e.g. "eng"
         :param list[str] urns: list of URN strings
         :param dict[str,str] fields: dictionary of contact field values
         :param list groups: list of group objects or UUIDs
         :return: the updated contact
@@ -494,202 +458,181 @@
         params = self._build_id_param(**{"urn" if is_urn else "uuid": contact})
         payload = self._build_params(name=name, language=language, urns=urns, fields=fields, groups=groups)
         return Contact.deserialize(self._post("contacts", params, self._build_params(**payload)))
 
     def update_field(self, field, label, value_type):
         """
         Updates an existing contact field
-
         :param * field: contact field object or key
         :param str label: field label
         :param str value_type: field value type
         :return: the updated field
         """
         params = self._build_id_param(key=field)
         payload = self._build_params(label=label, value_type=value_type)
         return Field.deserialize(self._post("fields", params, payload))
 
     def update_global(self, glbl, value):
         """
         Updates an existing global
-
         :param * glbl: global object or key
         :param str value: new value
         :return: the updated global
         """
         params = self._build_id_param(key=glbl)
         payload = self._build_params(value=value)
         return Global.deserialize(self._post("globals", params, payload))
 
     def update_group(self, group, name):
         """
         Updates an existing contact group
-
         :param * group: group object or UUID
         :param str name: group name
         :return: the updated group
         """
         return Group.deserialize(self._post("groups", self._build_id_param(uuid=group), self._build_params(name=name)))
 
     def update_label(self, label, name):
         """
         Updates an existing message label
-
         :param * label: label object or UUID
         :param str name: label name
         :return: the updated label
         """
         return Label.deserialize(self._post("labels", self._build_id_param(uuid=label), self._build_params(name=name)))
 
     # ==================================================================================================================
     # Delete object operations
     # ==================================================================================================================
 
     def delete_campaign_event(self, event):
         """
         Deletes an existing contact group
-
         :param * event: campaign event object or UUID
         """
         self._delete("campaign_events", self._build_id_param(uuid=event))
 
     def delete_contact(self, contact):
         """
         Deletes an existing contact
-
         :param * contact: contact object, UUID or URN
         """
         is_urn = isinstance(contact, str) and ":" in contact
         params = self._build_id_param(**{"urn" if is_urn else "uuid": contact})
         self._delete("contacts", params)
 
     def delete_group(self, group):
         """
         Deletes an existing contact group
-
         :param * group: group object or UUID
         """
         self._delete("groups", self._build_id_param(uuid=group))
 
     def delete_label(self, label):
         """
         Deletes an existing message label
-
         :param * label: label object or UUID
         """
         self._delete("labels", self._build_id_param(uuid=label))
 
     def delete_resthook_subscriber(self, subscriber):
         """
         Deletes an existing resthook subscriber
-
         :param * subscriber: the resthook subscriber or id
         """
         self._delete("resthook_subscribers", self._build_id_param(id=subscriber))
 
     # ==================================================================================================================
     # Bulk object operations
     # ==================================================================================================================
 
     def bulk_add_contacts(self, contacts, group):
         """
         Adds contacts to a group
-
         :param list[*] contacts: contact objects, UUIDs or URNs
         :param * group: contact group object or UUID
         """
         self._post("contact_actions", None, self._build_params(contacts=contacts, action="add", group=group))
 
     def bulk_remove_contacts(self, contacts, group):
         """
         Removes contacts from a group
-
         :param list[*] contacts: contact objects, UUIDs or URNs
         :param * group: contact group object or UUID
         """
         self._post("contact_actions", None, self._build_params(contacts=contacts, action="remove", group=group))
 
     def bulk_block_contacts(self, contacts):
         """
         Blocks contacts
-
         :param list[*] contacts: contact objects, UUIDs or URNs
         """
         self._post("contact_actions", None, self._build_params(contacts=contacts, action="block"))
 
     def bulk_unblock_contacts(self, contacts):
         """
         Un-blocks contacts
-
         :param list[*] contacts: contact objects, UUIDs or URNs
         """
         self._post("contact_actions", None, self._build_params(contacts=contacts, action="unblock"))
 
     def bulk_interrupt_contacts(self, contacts):
         """
         Interrupt active flow runs for contacts
-
         :param list[*] contacts: contact objects, UUIDs or URNs
         """
         self._post("contact_actions", None, self._build_params(contacts=contacts, action="interrupt"))
 
     def bulk_archive_contact_messages(self, contacts):
         """
         Archives all messages for contacts
-
         :param list[*] contacts: contact objects, UUIDs or URNs
         """
         self._post("contact_actions", None, self._build_params(contacts=contacts, action="archive_messages"))
 
     def bulk_delete_contacts(self, contacts):
         """
         Deletes contacts
-
         :param list[*] contacts: contact objects, UUIDs or URNs
         """
         self._post("contact_actions", None, self._build_params(contacts=contacts, action="delete"))
 
     def bulk_label_messages(self, messages, label=None, label_name=None):
         """
         Labels messages
-
         :param list[*] messages: message objects or ids
         :param * label: existing label object or UUID
         :param str label_name: label name which can be created if required
         """
         payload = self._build_params(messages=messages, action="label", label=label, label_name=label_name)
         self._post("message_actions", None, payload)
 
     def bulk_unlabel_messages(self, messages, label=None, label_name=None):
         """
         Un-labels messages
-
         :param list[*] messages: message objects or ids
         :param * label: existing label object or UUID
         :param str label_name: label name which is ignored if doesn't exist
         """
         payload = self._build_params(messages=messages, action="unlabel", label=label, label_name=label_name)
         self._post("message_actions", None, payload)
 
     def bulk_archive_messages(self, messages):
         """
         Archives messages
-
         :param list[*] messages: message objects or ids
         """
         self._post("message_actions", None, self._build_params(messages=messages, action="archive"))
 
     def bulk_restore_messages(self, messages):
         """
         Restores previously archived messages
-
         :param list[*] messages: message objects or ids
         """
         self._post("message_actions", None, self._build_params(messages=messages, action="restore"))
 
     def bulk_delete_messages(self, messages):
         """
         Deletes messages
-
         :param list[*] messages: message objects or ids
         """
         self._post("message_actions", None, self._build_params(messages=messages, action="delete"))
```

### Comparing `rapidpro-python-2.8.5/temba_client/v2/tests.py` & `rapidpro_python-2.9.0/temba_client/v2/tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -262,15 +262,15 @@
         self.assertRequest(mock_request, "get", "campaign_events")
         self.assertEqual(len(results), 2)
 
         self.assertEqual(results[0].uuid, "9e6beda-0ce2-46cd-8810-91157f261cbd")
         self.assertEqual(results[0].campaign.uuid, "9ccae91f-b3f8-4c18-ad92-e795a2332c11")
         self.assertEqual(results[0].campaign.name, "Reminders")
         self.assertEqual(results[0].relative_to.key, "edd")
-        self.assertEqual(results[0].relative_to.label, "EDD")
+        self.assertEqual(results[0].relative_to.name, "EDD")
         self.assertEqual(results[0].offset, 14)
         self.assertEqual(results[0].unit, "days")
         self.assertEqual(results[0].delivery_hour, -1)
         self.assertEqual(results[0].message, None)
         self.assertEqual(results[0].flow.uuid, "70c38f94-ab42-4666-86fd-3c76139110d3")
         self.assertEqual(results[0].flow.name, "Survey Flow")
         self.assertEqual(results[0].created_on, datetime.datetime(2015, 6, 8, 12, 18, 7, 671000, pytz.utc))
@@ -389,16 +389,17 @@
         self.assertEqual(results[0].name, "Joe")
         self.assertEqual(results[0].language, "eng")
         self.assertEqual(results[0].urns, ["tel:+250973635665"])
         self.assertEqual(len(results[0].groups), 1)
         self.assertEqual(results[0].groups[0].uuid, "d29eca7c-a475-4d8d-98ca-bff968341356")
         self.assertEqual(results[0].groups[0].name, "Customers")
         self.assertEqual(results[0].fields, {"age": 34, "nickname": "Jo"})
-        self.assertEqual(results[0].blocked, False)
-        self.assertEqual(results[0].stopped, False)
+        self.assertEqual(results[0].status, "active")
+        self.assertIsNone(results[0].flow)
+        self.assertIsNone(results[0].last_seen_on)
         self.assertEqual(results[0].created_on, datetime.datetime(2015, 11, 11, 8, 30, 24, 922024, pytz.utc))
         self.assertEqual(results[0].modified_on, datetime.datetime(2015, 11, 11, 8, 30, 25, 525936, pytz.utc))
 
         # check with all params
         self.client.get_contacts(
             uuid="ffce0fbb-4fe1-4052-b26a-91beb2ebae9a",
             urn="tel:+250973635665",
@@ -454,16 +455,16 @@
         # check with no params
         results = self.client.get_fields().all()
 
         self.assertRequest(mock_request, "get", "fields")
         self.assertEqual(len(results), 2)
 
         self.assertEqual(results[0].key, "chat_name")
-        self.assertEqual(results[0].label, "Chat Name")
-        self.assertEqual(results[0].value_type, "text")
+        self.assertEqual(results[0].name, "Chat Name")
+        self.assertEqual(results[0].type, "text")
 
         # check with all params
         self.client.get_fields(key="chat_name").all()
 
         self.assertRequest(mock_request, "get", "fields", params={"key": "chat_name"})
 
     def test_get_flows(self, mock_request):
@@ -608,18 +609,25 @@
         self.assertEqual(results[0].channel.name, "Nexmo")
         self.assertEqual(results[0].direction, "out")
         self.assertEqual(results[0].type, "inbox")
         self.assertEqual(results[0].status, "wired")
         self.assertEqual(results[0].visibility, "visible")
         self.assertEqual(results[0].text, "How are you?")
         self.assertEqual(results[0].labels, [])
+        self.assertEqual(results[0].attachments, [])
         self.assertEqual(results[0].created_on, datetime.datetime(2016, 1, 6, 15, 33, 0, 813162, pytz.utc))
         self.assertEqual(results[0].sent_on, datetime.datetime(2016, 1, 6, 15, 35, 3, 675716, pytz.utc))
         self.assertEqual(results[0].modified_on, None)
 
+        self.assertEqual(results[1].labels[0].uuid, "683c00e2-c130-4b40-9be9-e78c3370e583")
+        self.assertEqual(results[1].labels[0].name, "Important")
+
+        self.assertEqual(results[1].attachments[0].content_type, "audio/wav")
+        self.assertEqual(results[1].attachments[0].url, "http://domain.com/recording.wav")
+
         # check with all params
         self.client.get_messages(
             id=123456,
             broadcast=234567,
             contact="d33e9ad5-5c35-414c-abd4-e7451c69ff1d",
             folder="inbox",
             label="Spam",
@@ -716,15 +724,15 @@
         # check with no params
         query = self.client.get_runs()
         results = query.all()
 
         self.assertRequest(mock_request, "get", "runs")
         self.assertEqual(len(results), 2)
 
-        self.assertEqual(results[0].id, 4092373)
+        self.assertEqual(results[0].uuid, "0b6ed5cb-4b9f-422d-a53d-83965f93ff40")
         self.assertEqual(results[0].flow.uuid, "ffce0fbb-4fe1-4052-b26a-91beb2ebae9a")
         self.assertEqual(results[0].flow.name, "Water Survey")
         self.assertEqual(results[0].contact.uuid, "d33e9ad5-5c35-414c-abd4-e7451c69ff1d")
         self.assertEqual(results[0].contact.name, "Frank McFlow")
         self.assertEqual(results[0].start.uuid, "93a624ad-5440-415e-b49f-17bf42754acb")
         self.assertEqual(results[0].responded, True)
         self.assertEqual(len(results[0].path), 4)
@@ -744,35 +752,35 @@
             results[0].values["reason"].time, datetime.datetime(2015, 11, 11, 13, 5, 57, 576056, pytz.utc)
         )
         self.assertEqual(results[0].created_on, datetime.datetime(2015, 8, 26, 10, 4, 9, 737686, pytz.utc))
         self.assertEqual(results[0].modified_on, datetime.datetime(2015, 8, 26, 10, 5, 47, 516562, pytz.utc))
         self.assertEqual(results[0].exited_on, datetime.datetime(2015, 8, 26, 10, 5, 47, 516562, pytz.utc))
         self.assertEqual(results[0].exit_type, "completed")
 
-        self.assertEqual(query.first().id, results[0].id)
+        self.assertEqual(query.first().uuid, results[0].uuid)
         self.assertRequest(mock_request, "get", "runs")
 
         # check with all params
         self.client.get_runs(
-            id=123456,
+            uuid="3494603e-4ed9-488d-a846-bb2babf88078",
             flow="ffce0fbb-4fe1-4052-b26a-91beb2ebae9a",
             contact="d33e9ad5-5c35-414c-abd4-e7451c69ff1d",
             responded=True,
             after=datetime.datetime(2014, 12, 12, 22, 34, 36, 978123, pytz.utc),
             before=datetime.datetime(2014, 12, 12, 22, 56, 58, 917123, pytz.utc),
             reverse=False,
             paths=True,
         ).all()
 
         self.assertRequest(
             mock_request,
             "get",
             "runs",
             params={
-                "id": 123456,
+                "uuid": "3494603e-4ed9-488d-a846-bb2babf88078",
                 "flow": "ffce0fbb-4fe1-4052-b26a-91beb2ebae9a",
                 "contact": "d33e9ad5-5c35-414c-abd4-e7451c69ff1d",
                 "responded": True,
                 "after": "2014-12-12T22:34:36.978123Z",
                 "before": "2014-12-12T22:56:58.917123Z",
                 "reverse": False,
                 "paths": True,
```

### Comparing `rapidpro-python-2.8.5/temba_client/v2/types.py` & `rapidpro_python-2.9.0/temba_client/v2/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 class FieldRef(TembaObject):
     """
     Used for references to fields in other objects
     """
 
     key = SimpleField()
-    label = SimpleField()
+    name = SimpleField()
 
 
 class Archive(TembaObject):
     archive_type = SimpleField()
     start_date = DatetimeField()
     period = SimpleField()
     record_count = IntegerField()
@@ -120,52 +120,58 @@
     intents = ListField()
     created_on = DatetimeField()
 
 
 class Contact(TembaObject):
     uuid = SimpleField()
     name = SimpleField()
+    status = SimpleField()
     language = SimpleField()
     urns = ListField()
     groups = ObjectListField(item_class=ObjectRef)
+    flow = ObjectField(item_class=ObjectRef)
     fields = SimpleField()
-    blocked = BooleanField()
-    stopped = BooleanField()
     created_on = DatetimeField()
     modified_on = DatetimeField()
+    last_seen_on = DatetimeField()
 
 
 class Export(TembaObject):
     version = SimpleField()
     flows = ListField()
     campaigns = ListField()
     triggers = ListField()
+    fields = ListField()
+    groups = ListField()
 
 
 class Field(TembaObject):
     key = SimpleField()
-    label = SimpleField()
-    value_type = SimpleField()
+    name = SimpleField()
+    type = SimpleField()
 
 
 class Flow(TembaObject):
     class Runs(TembaObject):
         active = IntegerField()
+        waiting = IntegerField()
         completed = IntegerField()
         interrupted = IntegerField()
         expired = IntegerField()
+        failed = IntegerField()
 
     class FlowResult(TembaObject):
         key = SimpleField()
         name = SimpleField()
         categories = SimpleField()
         node_uuids = SimpleField()
 
     uuid = SimpleField()
     name = SimpleField()
+    type = SimpleField()
     archived = BooleanField()
     labels = ObjectListField(item_class=ObjectRef)
     expires = IntegerField()
     created_on = DatetimeField()
     runs = ObjectField(item_class=Runs)
     results = ObjectListField(item_class=FlowResult)
 
@@ -173,14 +179,15 @@
 class FlowStart(TembaObject):
     uuid = SimpleField()
     flow = ObjectField(item_class=ObjectRef)
     groups = ObjectListField(item_class=ObjectRef)
     contacts = ObjectListField(item_class=ObjectRef)
     status = SimpleField()
     restart_participants = BooleanField()
+    exclude_active = BooleanField()
     params = SimpleField()
     created_on = DatetimeField()
     modified_on = DatetimeField()
 
 
 class Global(TembaObject):
     key = SimpleField()
@@ -189,35 +196,42 @@
     modified_on = DatetimeField()
 
 
 class Group(TembaObject):
     uuid = SimpleField()
     name = SimpleField()
     query = SimpleField()
+    status = SimpleField()
+    system = BooleanField()
     count = IntegerField()
 
 
 class Label(TembaObject):
     uuid = SimpleField()
     name = SimpleField()
     count = IntegerField()
 
 
 class Message(TembaObject):
+    class AttachmentRef(TembaObject):
+        content_type = SimpleField()
+        url = SimpleField()
+
     id = IntegerField()
     broadcast = IntegerField()
     contact = ObjectField(item_class=ObjectRef)
     urn = SimpleField()
     channel = ObjectField(item_class=ObjectRef)
     direction = SimpleField()
     type = SimpleField()
     status = SimpleField()
     visibility = SimpleField()
     text = SimpleField()
     labels = ObjectListField(item_class=ObjectRef)
+    attachments = ObjectListField(item_class=AttachmentRef)
     created_on = DatetimeField()
     sent_on = DatetimeField()
     modified_on = DatetimeField()
 
 
 class Org(TembaObject):
     uuid = SimpleField()
@@ -261,15 +275,15 @@
         value = SimpleField()
         category = SimpleField()
         node = SimpleField()
         time = DatetimeField()
         name = SimpleField()
         input = SimpleField()
 
-    id = IntegerField()
+    uuid = SimpleField()
     flow = ObjectField(item_class=ObjectRef)
     contact = ObjectField(item_class=ObjectRef)
     start = ObjectField(item_class=StartRef)
     responded = BooleanField()
     path = ObjectListField(item_class=Step)
     values = ObjectDictField(item_class=Value)
     created_on = DatetimeField()
```

### Comparing `rapidpro-python-2.8.5/setup.py` & `rapidpro_python-2.9.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,23 +8,23 @@
 {'': ['*']}
 
 install_requires = \
 ['iso8601>=0.1.13,<0.2.0', 'pytz', 'requests>=2.25.0,<3.0.0']
 
 setup_kwargs = {
     'name': 'rapidpro-python',
-    'version': '2.8.5',
+    'version': '2.9.0',
     'description': 'Python client library for the RapidPro API',
     'long_description': "RapidPro Python Client\n======================\n\n[![Build Status](https://github.com/rapidpro/rapidpro-python/workflows/CI/badge.svg)](https://github.com/rapidpro/rapidpro-python/actions?query=workflow%3ACI)\n[![Coverage Status](https://codecov.io/gh/rapidpro/rapidpro-python/branch/main/graph/badge.svg)](https://codecov.io/gh/rapidpro/rapidpro-python) \n[![PyPI Release](https://img.shields.io/pypi/v/rapidpro-python.svg)](https://pypi.python.org/pypi/rapidpro-python/)\n\nOfficial Python client library for the [RapidPro](http://rapidpro.github.io/rapidpro/). Supports latest Python 3.\n\nVisit [here](http://rapidpro-python.readthedocs.org/) for complete documentation.\n\nInstallation\n------------\n\n```\npip install rapidpro-python\n```\n\nExample\n-------\n\n```python\nfrom temba_client.v2 import TembaClient\nclient = TembaClient('rapidpro.io', 'your-api-token')\nfor contact_batch in client.get_contacts(group='Reporters').iterfetches(retry_on_rate_exceed=True):\n    for contact in contact_batch:\n        print(contact.name)\n```\n\nIf you don't know your API token then visit the [API Explorer](http://rapidpro.io/api/v2/explorer)\n\nDevelopment\n-----------\n\nFor discussions about future development, see the [RapidPro Developers Group](https://groups.google.com/forum/#!forum/rapidpro-dev).\n\nTo run the tests:\n\n```\nnosetests --with-coverage --cover-erase --cover-package=temba_client --cover-html\n```\n",
     'author': 'Nyaruka',
     'author_email': 'code@nyaruka.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': None,
+    'maintainer': 'None',
+    'maintainer_email': 'None',
+    'url': 'None',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'python_requires': '>=3.6,<4.0',
+    'python_requires': '>=3.9,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `rapidpro-python-2.8.5/PKG-INFO` & `rapidpro_python-2.9.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: rapidpro-python
-Version: 2.8.5
+Version: 2.9.0
 Summary: Python client library for the RapidPro API
 License: BSD-4-Clause
 Author: Nyaruka
 Author-email: code@nyaruka.com
-Requires-Python: >=3.6,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries
 Requires-Dist: iso8601 (>=0.1.13,<0.2.0)
 Requires-Dist: pytz
 Requires-Dist: requests (>=2.25.0,<3.0.0)
 Project-URL: repository, http://github.com/rapidpro/rapidpro-python
 Description-Content-Type: text/markdown
```

