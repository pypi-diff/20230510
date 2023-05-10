# Comparing `tmp/djangoldp_tzcld-1.0.4.tar.gz` & `tmp/djangoldp_tzcld-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/djangoldp_tzcld-1.0.4.tar", last modified: Wed Apr 26 15:33:53 2023, max compression
+gzip compressed data, was "dist/djangoldp_tzcld-1.0.5.tar", last modified: Wed May 10 13:52:18 2023, max compression
```

## Comparing `djangoldp_tzcld-1.0.4.tar` & `djangoldp_tzcld-1.0.5.tar`

### file list

```diff
@@ -1,40 +1,42 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 15:33:53.000000 djangoldp_tzcld-1.0.4/
--rw-rw-rw-   0 root         (0) root         (0)       65 2023-04-26 15:33:37.000000 djangoldp_tzcld-1.0.4/README.md
--rw-rw-rw-   0 root         (0) root         (0)       61 2023-04-26 15:33:37.000000 djangoldp_tzcld-1.0.4/setup.py
--rw-rw-rw-   0 root         (0) root         (0)      505 2023-04-26 15:33:53.000000 djangoldp_tzcld-1.0.4/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 15:33:53.000000 djangoldp_tzcld-1.0.4/djangoldp_tzcld.egg-info/
--rw-r--r--   0 root         (0) root         (0)      272 2023-04-26 15:33:53.000000 djangoldp_tzcld-1.0.4/djangoldp_tzcld.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 15:33:53.000000 djangoldp_tzcld-1.0.4/djangoldp_tzcld.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     1549 2023-04-26 15:33:53.000000 djangoldp_tzcld-1.0.4/djangoldp_tzcld.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-04-26 15:33:53.000000 djangoldp_tzcld-1.0.4/djangoldp_tzcld.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-04-26 15:33:53.000000 djangoldp_tzcld-1.0.4/djangoldp_tzcld.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)      272 2023-04-26 15:33:53.000000 djangoldp_tzcld-1.0.4/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 15:33:53.000000 djangoldp_tzcld-1.0.4/djangoldp_tzcld/
--rw-rw-rw-   0 root         (0) root         (0)    18055 2023-04-26 15:33:37.000000 djangoldp_tzcld-1.0.4/djangoldp_tzcld/models.py
--rw-rw-rw-   0 root         (0) root         (0)     1085 2023-04-26 15:33:37.000000 djangoldp_tzcld-1.0.4/djangoldp_tzcld/permissions.py
--rw-rw-rw-   0 root         (0) root         (0)     2347 2023-04-26 15:33:37.000000 djangoldp_tzcld-1.0.4/djangoldp_tzcld/admin.py
--rw-rw-rw-   0 root         (0) root         (0)       47 2023-04-26 15:33:51.000000 djangoldp_tzcld-1.0.4/djangoldp_tzcld/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      104 2023-04-26 15:33:37.000000 djangoldp_tzcld-1.0.4/djangoldp_tzcld/apps.py
--rw-rw-rw-   0 root         (0) root         (0)      161 2023-04-26 15:33:37.000000 djangoldp_tzcld-1.0.4/djangoldp_tzcld/settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 15:33:53.000000 djangoldp_tzcld-1.0.4/djangoldp_tzcld/migrations/
--rw-rw-rw-   0 root         (0) root         (0)     5896 2023-04-26 15:33:37.000000 djangoldp_tzcld-1.0.4/djangoldp_tzcld/migrations/0004_tzcldprofilejob_tzcldprofilejobemail_tzcldprofilejobphone.py
--rw-rw-rw-   0 root         (0) root         (0)      836 2023-04-26 15:33:37.000000 djangoldp_tzcld-1.0.4/djangoldp_tzcld/migrations/0007_auto_20230327_1451.py
--rw-rw-rw-   0 root         (0) root         (0)     9812 2023-04-26 15:33:37.000000 djangoldp_tzcld-1.0.4/djangoldp_tzcld/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)      889 2023-04-26 15:33:37.000000 djangoldp_tzcld-1.0.4/djangoldp_tzcld/migrations/0013_auto_20230330_1246.py
--rw-rw-rw-   0 root         (0) root         (0)     1889 2023-04-26 15:33:37.000000 djangoldp_tzcld-1.0.4/djangoldp_tzcld/migrations/0016_tzcldcontactmember.py
--rw-rw-rw-   0 root         (0) root         (0)      501 2023-04-26 15:33:37.000000 djangoldp_tzcld-1.0.4/djangoldp_tzcld/migrations/0014_auto_20230330_1258.py
--rw-rw-rw-   0 root         (0) root         (0)     1099 2023-04-26 15:33:37.000000 djangoldp_tzcld-1.0.4/djangoldp_tzcld/migrations/0019_auto_20230414_1634.py
--rw-rw-rw-   0 root         (0) root         (0)      431 2023-04-26 15:33:37.000000 djangoldp_tzcld-1.0.4/djangoldp_tzcld/migrations/0002_tzcldcommunity_contact_job.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-26 15:33:37.000000 djangoldp_tzcld-1.0.4/djangoldp_tzcld/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1033 2023-04-26 15:33:37.000000 djangoldp_tzcld-1.0.4/djangoldp_tzcld/migrations/0012_auto_20230330_1233.py
--rw-rw-rw-   0 root         (0) root         (0)     1774 2023-04-26 15:33:37.000000 djangoldp_tzcld-1.0.4/djangoldp_tzcld/migrations/0003_auto_20220720_1242.py
--rw-rw-rw-   0 root         (0) root         (0)    18022 2023-04-26 15:33:37.000000 djangoldp_tzcld-1.0.4/djangoldp_tzcld/migrations/0006_auto_20230327_1449.py
--rw-rw-rw-   0 root         (0) root         (0)      652 2023-04-26 15:33:37.000000 djangoldp_tzcld-1.0.4/djangoldp_tzcld/migrations/0005_auto_20230325_1335.py
--rw-rw-rw-   0 root         (0) root         (0)     4403 2023-04-26 15:33:37.000000 djangoldp_tzcld-1.0.4/djangoldp_tzcld/migrations/0011_auto_20230328_1045.py
--rw-rw-rw-   0 root         (0) root         (0)      706 2023-04-26 15:33:37.000000 djangoldp_tzcld-1.0.4/djangoldp_tzcld/migrations/0018_auto_20230406_1755.py
--rw-rw-rw-   0 root         (0) root         (0)      632 2023-04-26 15:33:37.000000 djangoldp_tzcld-1.0.4/djangoldp_tzcld/migrations/0017_tzcldcontactmember_community.py
--rw-rw-rw-   0 root         (0) root         (0)     1816 2023-04-26 15:33:37.000000 djangoldp_tzcld-1.0.4/djangoldp_tzcld/migrations/0015_auto_20230330_1439.py
--rw-rw-rw-   0 root         (0) root         (0)      653 2023-04-26 15:33:37.000000 djangoldp_tzcld-1.0.4/djangoldp_tzcld/migrations/0010_auto_20230327_1629.py
--rw-rw-rw-   0 root         (0) root         (0)     1750 2023-04-26 15:33:37.000000 djangoldp_tzcld-1.0.4/djangoldp_tzcld/migrations/0020_auto_20230417_1242.py
--rw-rw-rw-   0 root         (0) root         (0)     1270 2023-04-26 15:33:37.000000 djangoldp_tzcld-1.0.4/djangoldp_tzcld/migrations/0009_auto_20230327_1623.py
--rw-rw-rw-   0 root         (0) root         (0)      711 2023-04-26 15:33:37.000000 djangoldp_tzcld-1.0.4/djangoldp_tzcld/migrations/0008_auto_20230327_1602.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 13:52:18.000000 djangoldp_tzcld-1.0.5/
+-rw-rw-rw-   0 root         (0) root         (0)       65 2023-05-10 13:52:00.000000 djangoldp_tzcld-1.0.5/README.md
+-rw-rw-rw-   0 root         (0) root         (0)       61 2023-05-10 13:52:00.000000 djangoldp_tzcld-1.0.5/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)      505 2023-05-10 13:52:18.000000 djangoldp_tzcld-1.0.5/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 13:52:18.000000 djangoldp_tzcld-1.0.5/djangoldp_tzcld.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      272 2023-05-10 13:52:18.000000 djangoldp_tzcld-1.0.5/djangoldp_tzcld.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-10 13:52:18.000000 djangoldp_tzcld-1.0.5/djangoldp_tzcld.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     1682 2023-05-10 13:52:18.000000 djangoldp_tzcld-1.0.5/djangoldp_tzcld.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-05-10 13:52:18.000000 djangoldp_tzcld-1.0.5/djangoldp_tzcld.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-05-10 13:52:18.000000 djangoldp_tzcld-1.0.5/djangoldp_tzcld.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)      272 2023-05-10 13:52:18.000000 djangoldp_tzcld-1.0.5/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 13:52:18.000000 djangoldp_tzcld-1.0.5/djangoldp_tzcld/
+-rw-rw-rw-   0 root         (0) root         (0)    18147 2023-05-10 13:52:00.000000 djangoldp_tzcld-1.0.5/djangoldp_tzcld/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     1085 2023-05-10 13:52:00.000000 djangoldp_tzcld-1.0.5/djangoldp_tzcld/permissions.py
+-rw-rw-rw-   0 root         (0) root         (0)     2347 2023-05-10 13:52:00.000000 djangoldp_tzcld-1.0.5/djangoldp_tzcld/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)       47 2023-05-10 13:52:16.000000 djangoldp_tzcld-1.0.5/djangoldp_tzcld/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      104 2023-05-10 13:52:00.000000 djangoldp_tzcld-1.0.5/djangoldp_tzcld/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)      161 2023-05-10 13:52:00.000000 djangoldp_tzcld-1.0.5/djangoldp_tzcld/settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 13:52:18.000000 djangoldp_tzcld-1.0.5/djangoldp_tzcld/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)     5896 2023-05-10 13:52:00.000000 djangoldp_tzcld-1.0.5/djangoldp_tzcld/migrations/0004_tzcldprofilejob_tzcldprofilejobemail_tzcldprofilejobphone.py
+-rw-rw-rw-   0 root         (0) root         (0)      836 2023-05-10 13:52:00.000000 djangoldp_tzcld-1.0.5/djangoldp_tzcld/migrations/0007_auto_20230327_1451.py
+-rw-rw-rw-   0 root         (0) root         (0)     9812 2023-05-10 13:52:00.000000 djangoldp_tzcld-1.0.5/djangoldp_tzcld/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)      889 2023-05-10 13:52:00.000000 djangoldp_tzcld-1.0.5/djangoldp_tzcld/migrations/0013_auto_20230330_1246.py
+-rw-rw-rw-   0 root         (0) root         (0)     1889 2023-05-10 13:52:00.000000 djangoldp_tzcld-1.0.5/djangoldp_tzcld/migrations/0016_tzcldcontactmember.py
+-rw-rw-rw-   0 root         (0) root         (0)      501 2023-05-10 13:52:00.000000 djangoldp_tzcld-1.0.5/djangoldp_tzcld/migrations/0014_auto_20230330_1258.py
+-rw-rw-rw-   0 root         (0) root         (0)     1099 2023-05-10 13:52:00.000000 djangoldp_tzcld-1.0.5/djangoldp_tzcld/migrations/0019_auto_20230414_1634.py
+-rw-rw-rw-   0 root         (0) root         (0)      960 2023-05-10 13:52:00.000000 djangoldp_tzcld-1.0.5/djangoldp_tzcld/migrations/0021_auto_20230510_1232.py
+-rw-rw-rw-   0 root         (0) root         (0)      431 2023-05-10 13:52:00.000000 djangoldp_tzcld-1.0.5/djangoldp_tzcld/migrations/0002_tzcldcommunity_contact_job.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-10 13:52:00.000000 djangoldp_tzcld-1.0.5/djangoldp_tzcld/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1033 2023-05-10 13:52:00.000000 djangoldp_tzcld-1.0.5/djangoldp_tzcld/migrations/0012_auto_20230330_1233.py
+-rw-rw-rw-   0 root         (0) root         (0)     1774 2023-05-10 13:52:00.000000 djangoldp_tzcld-1.0.5/djangoldp_tzcld/migrations/0003_auto_20220720_1242.py
+-rw-rw-rw-   0 root         (0) root         (0)    18022 2023-05-10 13:52:00.000000 djangoldp_tzcld-1.0.5/djangoldp_tzcld/migrations/0006_auto_20230327_1449.py
+-rw-rw-rw-   0 root         (0) root         (0)      652 2023-05-10 13:52:00.000000 djangoldp_tzcld-1.0.5/djangoldp_tzcld/migrations/0005_auto_20230325_1335.py
+-rw-rw-rw-   0 root         (0) root         (0)     4403 2023-05-10 13:52:00.000000 djangoldp_tzcld-1.0.5/djangoldp_tzcld/migrations/0011_auto_20230328_1045.py
+-rw-rw-rw-   0 root         (0) root         (0)      706 2023-05-10 13:52:00.000000 djangoldp_tzcld-1.0.5/djangoldp_tzcld/migrations/0018_auto_20230406_1755.py
+-rw-rw-rw-   0 root         (0) root         (0)      459 2023-05-10 13:52:00.000000 djangoldp_tzcld-1.0.5/djangoldp_tzcld/migrations/0022_tzcldcommunity_membership_organisation_name.py
+-rw-rw-rw-   0 root         (0) root         (0)      632 2023-05-10 13:52:00.000000 djangoldp_tzcld-1.0.5/djangoldp_tzcld/migrations/0017_tzcldcontactmember_community.py
+-rw-rw-rw-   0 root         (0) root         (0)     1816 2023-05-10 13:52:00.000000 djangoldp_tzcld-1.0.5/djangoldp_tzcld/migrations/0015_auto_20230330_1439.py
+-rw-rw-rw-   0 root         (0) root         (0)      653 2023-05-10 13:52:00.000000 djangoldp_tzcld-1.0.5/djangoldp_tzcld/migrations/0010_auto_20230327_1629.py
+-rw-rw-rw-   0 root         (0) root         (0)     1750 2023-05-10 13:52:00.000000 djangoldp_tzcld-1.0.5/djangoldp_tzcld/migrations/0020_auto_20230417_1242.py
+-rw-rw-rw-   0 root         (0) root         (0)     1270 2023-05-10 13:52:00.000000 djangoldp_tzcld-1.0.5/djangoldp_tzcld/migrations/0009_auto_20230327_1623.py
+-rw-rw-rw-   0 root         (0) root         (0)      711 2023-05-10 13:52:00.000000 djangoldp_tzcld-1.0.5/djangoldp_tzcld/migrations/0008_auto_20230327_1602.py
```

### Comparing `djangoldp_tzcld-1.0.4/djangoldp_tzcld.egg-info/SOURCES.txt` & `djangoldp_tzcld-1.0.5/djangoldp_tzcld.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -28,8 +28,10 @@
 djangoldp_tzcld/migrations/0014_auto_20230330_1258.py
 djangoldp_tzcld/migrations/0015_auto_20230330_1439.py
 djangoldp_tzcld/migrations/0016_tzcldcontactmember.py
 djangoldp_tzcld/migrations/0017_tzcldcontactmember_community.py
 djangoldp_tzcld/migrations/0018_auto_20230406_1755.py
 djangoldp_tzcld/migrations/0019_auto_20230414_1634.py
 djangoldp_tzcld/migrations/0020_auto_20230417_1242.py
+djangoldp_tzcld/migrations/0021_auto_20230510_1232.py
+djangoldp_tzcld/migrations/0022_tzcldcommunity_membership_organisation_name.py
 djangoldp_tzcld/migrations/__init__.py
```

### Comparing `djangoldp_tzcld-1.0.4/djangoldp_tzcld/models.py` & `djangoldp_tzcld-1.0.5/djangoldp_tzcld/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -216,15 +216,15 @@
         except:
             return self.urlid
 
     class Meta(Model.Meta):
         verbose_name = _('TZCLD Territory step state')
         verbose_name_plural = _("TZCLD Territories step states")
         anonymous_perms = ['view']
-        container_path = "tzcld--territories-step-states/"
+        container_path = "tzcld-territories-step-states/"
         serializer_fields = ['@id', 'name']
         nested_fields = []
         rdf_type = "tzcld:territoryStepState"
 
 class TzcldTerritoriesKind(Model):
     name = models.CharField(max_length=254, blank=True, null=True, default='')
 
@@ -243,17 +243,18 @@
         nested_fields = []
         rdf_type = "tzcld:territoryKind"
 
 class TzcldCommunity(Model):
     community = models.OneToOneField(Community, on_delete=models.CASCADE, related_name='tzcld_profile', null=True, blank=True)
     kind = models.ForeignKey(TzcldTerritoriesKind, on_delete=models.DO_NOTHING,related_name='kind', blank=True, null=True)
     step_state = models.ForeignKey(TzcldTerritoriesStepState, on_delete=models.DO_NOTHING,related_name='step_state', blank=False, null=True)
-    department = models.ForeignKey(TzcldTerritoryDepartment, on_delete=models.DO_NOTHING,related_name='department', blank=True, null=True)
-    region = models.ForeignKey(TzcldTerritoryRegion, on_delete=models.DO_NOTHING,related_name='region', blank=True, null=True)
+    regions = models.ManyToManyField(TzcldTerritoryRegion, related_name='community_regions', blank=True)
+    departments = models.ManyToManyField(TzcldTerritoryDepartment, related_name='community_departments', blank=True)
     membership = models.ForeignKey(TzcldProfilesMembership, on_delete=models.DO_NOTHING,related_name='membership', blank=False, null=True)
+    membership_organisation_name = models.CharField(max_length=254, blank=True, null=True, default='')
     """
     features = models.CharField(max_length=255, blank=True, null=True, default='')
     contact_mail_1 = models.CharField(max_length=255, blank=True, null=True, default='')
     contact_mail_2 = models.CharField(max_length=255, blank=True, null=True, default='')
     contact_mail_3 = models.CharField(max_length=255, blank=True, null=True, default='')
     contact_last_name = models.CharField(max_length=255, blank=True, null=True, default='')
     contact_first_name = models.CharField(max_length=255, blank=True, null=True, default='')
@@ -274,15 +275,15 @@
         permission_classes = [TzcldCommunityProfilePermissions]
         anonymous_perms = ['view']
         authenticated_perms = ['inherit', 'add']
         superuser_perms = ['view']
         ordering = ['community']
         container_path = "/tzcld-communities/"
         #serializer_fields = ['@id', 'contact_first_name', 'contact_last_name', 'contact_job', 'kind', 'features', 'region', 'contact_mail_1', 'contact_mail_2', 'contact_mail_3', 'membership', 'last_contribution_year']
-        serializer_fields = ['@id', 'community', 'kind', 'step_state', 'kind', 'department', 'region', 'locations', 'tzcld_community_contacts', 'membership']
+        serializer_fields = ['@id', 'community', 'kind', 'step_state', 'kind', 'departments', 'regions', 'locations', 'tzcld_community_contacts', 'membership', 'membership_organisation_name']
         rdf_type = "tzcld:communityProfile"
         depth = 3
 
 
 class TzcldTerritoryLocation(Model):
     name = models.CharField(max_length=255, blank=True, null=True, default='')
     address = models.CharField(max_length=255, blank=True, null=True, default='')
```

### Comparing `djangoldp_tzcld-1.0.4/djangoldp_tzcld/permissions.py` & `djangoldp_tzcld-1.0.5/djangoldp_tzcld/permissions.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-1.0.4/djangoldp_tzcld/admin.py` & `djangoldp_tzcld-1.0.5/djangoldp_tzcld/admin.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-1.0.4/djangoldp_tzcld/migrations/0004_tzcldprofilejob_tzcldprofilejobemail_tzcldprofilejobphone.py` & `djangoldp_tzcld-1.0.5/djangoldp_tzcld/migrations/0004_tzcldprofilejob_tzcldprofilejobemail_tzcldprofilejobphone.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-1.0.4/djangoldp_tzcld/migrations/0007_auto_20230327_1451.py` & `djangoldp_tzcld-1.0.5/djangoldp_tzcld/migrations/0007_auto_20230327_1451.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-1.0.4/djangoldp_tzcld/migrations/0001_initial.py` & `djangoldp_tzcld-1.0.5/djangoldp_tzcld/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-1.0.4/djangoldp_tzcld/migrations/0013_auto_20230330_1246.py` & `djangoldp_tzcld-1.0.5/djangoldp_tzcld/migrations/0013_auto_20230330_1246.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-1.0.4/djangoldp_tzcld/migrations/0016_tzcldcontactmember.py` & `djangoldp_tzcld-1.0.5/djangoldp_tzcld/migrations/0016_tzcldcontactmember.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-1.0.4/djangoldp_tzcld/migrations/0019_auto_20230414_1634.py` & `djangoldp_tzcld-1.0.5/djangoldp_tzcld/migrations/0019_auto_20230414_1634.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-1.0.4/djangoldp_tzcld/migrations/0012_auto_20230330_1233.py` & `djangoldp_tzcld-1.0.5/djangoldp_tzcld/migrations/0012_auto_20230330_1233.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-1.0.4/djangoldp_tzcld/migrations/0003_auto_20220720_1242.py` & `djangoldp_tzcld-1.0.5/djangoldp_tzcld/migrations/0003_auto_20220720_1242.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-1.0.4/djangoldp_tzcld/migrations/0006_auto_20230327_1449.py` & `djangoldp_tzcld-1.0.5/djangoldp_tzcld/migrations/0006_auto_20230327_1449.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-1.0.4/djangoldp_tzcld/migrations/0005_auto_20230325_1335.py` & `djangoldp_tzcld-1.0.5/djangoldp_tzcld/migrations/0005_auto_20230325_1335.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-1.0.4/djangoldp_tzcld/migrations/0011_auto_20230328_1045.py` & `djangoldp_tzcld-1.0.5/djangoldp_tzcld/migrations/0011_auto_20230328_1045.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-1.0.4/djangoldp_tzcld/migrations/0018_auto_20230406_1755.py` & `djangoldp_tzcld-1.0.5/djangoldp_tzcld/migrations/0018_auto_20230406_1755.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-1.0.4/djangoldp_tzcld/migrations/0017_tzcldcontactmember_community.py` & `djangoldp_tzcld-1.0.5/djangoldp_tzcld/migrations/0017_tzcldcontactmember_community.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-1.0.4/djangoldp_tzcld/migrations/0015_auto_20230330_1439.py` & `djangoldp_tzcld-1.0.5/djangoldp_tzcld/migrations/0015_auto_20230330_1439.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-1.0.4/djangoldp_tzcld/migrations/0010_auto_20230327_1629.py` & `djangoldp_tzcld-1.0.5/djangoldp_tzcld/migrations/0010_auto_20230327_1629.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-1.0.4/djangoldp_tzcld/migrations/0020_auto_20230417_1242.py` & `djangoldp_tzcld-1.0.5/djangoldp_tzcld/migrations/0020_auto_20230417_1242.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-1.0.4/djangoldp_tzcld/migrations/0009_auto_20230327_1623.py` & `djangoldp_tzcld-1.0.5/djangoldp_tzcld/migrations/0009_auto_20230327_1623.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-1.0.4/djangoldp_tzcld/migrations/0008_auto_20230327_1602.py` & `djangoldp_tzcld-1.0.5/djangoldp_tzcld/migrations/0008_auto_20230327_1602.py`

 * *Files identical despite different names*

