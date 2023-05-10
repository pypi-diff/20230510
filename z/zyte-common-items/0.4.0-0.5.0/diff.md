# Comparing `tmp/zyte-common-items-0.4.0.tar.gz` & `tmp/zyte-common-items-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zyte-common-items-0.4.0.tar", last modified: Mon Mar 27 12:06:40 2023, max compression
+gzip compressed data, was "zyte-common-items-0.5.0.tar", last modified: Wed May 10 13:31:58 2023, max compression
```

## Comparing `zyte-common-items-0.4.0.tar` & `zyte-common-items-0.5.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 12:06:40.811320 zyte-common-items-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-03-27 12:06:30.000000 zyte-common-items-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-03-27 12:06:30.000000 zyte-common-items-0.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-03-27 12:06:40.811320 zyte-common-items-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-03-27 12:06:30.000000 zyte-common-items-0.4.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-03-27 12:06:30.000000 zyte-common-items-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-27 12:06:40.811320 zyte-common-items-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-03-27 12:06:30.000000 zyte-common-items-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 12:06:40.811320 zyte-common-items-0.4.0/zyte_common_items/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-27 12:06:30.000000 zyte-common-items-0.4.0/zyte_common_items/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-03-27 12:06:30.000000 zyte-common-items-0.4.0/zyte_common_items/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3686 2023-03-27 12:06:30.000000 zyte-common-items-0.4.0/zyte_common_items/adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4507 2023-03-27 12:06:30.000000 zyte-common-items-0.4.0/zyte_common_items/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7140 2023-03-27 12:06:30.000000 zyte-common-items-0.4.0/zyte_common_items/components.py
--rw-r--r--   0 runner    (1001) docker     (123)    20332 2023-03-27 12:06:30.000000 zyte-common-items-0.4.0/zyte_common_items/items.py
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-03-27 12:06:30.000000 zyte-common-items-0.4.0/zyte_common_items/pages.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 12:06:30.000000 zyte-common-items-0.4.0/zyte_common_items/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-03-27 12:06:30.000000 zyte-common-items-0.4.0/zyte_common_items/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 12:06:40.811320 zyte-common-items-0.4.0/zyte_common_items.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-03-27 12:06:40.000000 zyte-common-items-0.4.0/zyte_common_items.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-03-27 12:06:40.000000 zyte-common-items-0.4.0/zyte_common_items.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 12:06:40.000000 zyte-common-items-0.4.0/zyte_common_items.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-03-27 12:06:40.000000 zyte-common-items-0.4.0/zyte_common_items.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-03-27 12:06:40.000000 zyte-common-items-0.4.0/zyte_common_items.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:31:58.246227 zyte-common-items-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-05-10 13:31:43.000000 zyte-common-items-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-10 13:31:43.000000 zyte-common-items-0.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-05-10 13:31:58.246227 zyte-common-items-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-05-10 13:31:43.000000 zyte-common-items-0.5.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-10 13:31:43.000000 zyte-common-items-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 13:31:58.246227 zyte-common-items-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-05-10 13:31:43.000000 zyte-common-items-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:31:58.242227 zyte-common-items-0.5.0/zyte_common_items/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-10 13:31:43.000000 zyte-common-items-0.5.0/zyte_common_items/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-05-10 13:31:43.000000 zyte-common-items-0.5.0/zyte_common_items/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4158 2023-05-10 13:31:43.000000 zyte-common-items-0.5.0/zyte_common_items/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6612 2023-05-10 13:31:43.000000 zyte-common-items-0.5.0/zyte_common_items/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7567 2023-05-10 13:31:43.000000 zyte-common-items-0.5.0/zyte_common_items/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23762 2023-05-10 13:31:43.000000 zyte-common-items-0.5.0/zyte_common_items/items.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-05-10 13:31:43.000000 zyte-common-items-0.5.0/zyte_common_items/pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 13:31:43.000000 zyte-common-items-0.5.0/zyte_common_items/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-05-10 13:31:43.000000 zyte-common-items-0.5.0/zyte_common_items/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:31:58.246227 zyte-common-items-0.5.0/zyte_common_items.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-05-10 13:31:58.000000 zyte-common-items-0.5.0/zyte_common_items.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-05-10 13:31:58.000000 zyte-common-items-0.5.0/zyte_common_items.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 13:31:58.000000 zyte-common-items-0.5.0/zyte_common_items.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-10 13:31:58.000000 zyte-common-items-0.5.0/zyte_common_items.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-10 13:31:58.000000 zyte-common-items-0.5.0/zyte_common_items.egg-info/top_level.txt
```

### Comparing `zyte-common-items-0.4.0/LICENSE` & `zyte-common-items-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `zyte-common-items-0.4.0/PKG-INFO` & `zyte-common-items-0.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zyte-common-items
-Version: 0.4.0
+Version: 0.5.0
 Summary: Item definitions for Zyte API schema
 Home-page: https://github.com/zytedata/zyte-common-items
 Author: Zyte Group Ltd
 Author-email: info@zyte.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `zyte-common-items-0.4.0/README.rst` & `zyte-common-items-0.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `zyte-common-items-0.4.0/setup.py` & `zyte-common-items-0.5.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         ]
     ),
     package_data={
         "zyte_common_items": ["py.typed", "VERSION"],
     },
     install_requires=[
         "attrs>=21.3.0",
-        "itemadapter>=0.2.0",
+        "itemadapter>=0.8.0",
         "web-poet>=0.7.0",
     ],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: BSD License",
         "Natural Language :: English",
```

### Comparing `zyte-common-items-0.4.0/zyte_common_items/__init__.py` & `zyte-common-items-0.5.0/zyte_common_items/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # flake8: noqa
-from .adapter import ZyteItemAdapter
+from .adapter import ZyteItemAdapter, ZyteItemKeepEmptyAdapter
 from .base import Item, is_data_container
 from .components import (
     AdditionalProperty,
     Address,
     AggregateRating,
     Amenity,
     Brand,
@@ -12,20 +12,30 @@
     Gtin,
     Image,
     Link,
     Metadata,
     NamedLink,
     OpeningHoursItem,
     ParentPlace,
+    RealEstateArea,
     StarRating,
 )
-from .items import BusinessPlace, Product, ProductFromList, ProductList, ProductVariant
+from .items import (
+    BusinessPlace,
+    Product,
+    ProductFromList,
+    ProductList,
+    ProductVariant,
+    RealEstate,
+)
 from .pages import (
     BaseBusinessPlacePage,
     BasePage,
     BaseProductListPage,
     BaseProductPage,
+    BaseRealEstatePage,
     BusinessPlacePage,
     Page,
     ProductListPage,
     ProductPage,
+    RealEstatePage,
 )
```

### Comparing `zyte-common-items-0.4.0/zyte_common_items/adapter.py` & `zyte-common-items-0.5.0/zyte_common_items/adapter.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 """This module offers better integration with the itemadapter package."""
-
-
 from types import MappingProxyType
 from typing import Any, Collection, Iterator, KeysView
 
 from itemadapter.adapter import AttrsAdapter
 
 from zyte_common_items.base import Item
 
@@ -95,7 +93,20 @@
         ]
         fields.extend(
             attr
             for attr in self.item._unknown_fields_dict
             if not _is_empty(self.item._unknown_fields_dict[attr])
         )
         return iter(fields)
+
+
+class ZyteItemKeepEmptyAdapter(ZyteItemAdapter):
+    """Similar to :class:`~.ZyteItemAdapter` but doesn't remove empty values.
+
+    It is intended to be used in tests and other use cases where it's important
+    to differentiate between empty and missing fields.
+    """
+
+    def __iter__(self) -> Iterator:
+        fields = [attr for attr in self._fields_dict if hasattr(self.item, attr)]
+        fields.extend(self.item._unknown_fields_dict)
+        return iter(fields)
```

### Comparing `zyte-common-items-0.4.0/zyte_common_items/components.py` & `zyte-common-items-0.5.0/zyte_common_items/components.py`

 * *Files 3% similar despite different names*

```diff
@@ -263,7 +263,25 @@
     rawDayOfWeek: Optional[str] = None
 
     #: Opening time, as it appears on the page, without processing.
     rawOpens: Optional[str] = None
 
     #: Closing time, as it appears on the page, without processing.
     rawCloses: Optional[str] = None
+
+
+@attrs.define(kw_only=True)
+class RealEstateArea(Item):
+    """Area of a place, with type, units, value and raw value."""
+
+    #: Area
+    value: float
+
+    #: Unit of the value field, one of: SQMT (square meters), SQFT (square
+    #: feet), ACRE (acres).
+    unitCode: str
+
+    #: Type of area, one of: LOT, FLOOR
+    areaType: Optional[str] = None
+
+    #: Area in the raw format, as it appears on the website.
+    raw: str
```

### Comparing `zyte-common-items-0.4.0/zyte_common_items/items.py` & `zyte-common-items-0.5.0/zyte_common_items/items.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     Gtin,
     Image,
     Link,
     Metadata,
     NamedLink,
     OpeningHoursItem,
     ParentPlace,
+    RealEstateArea,
     StarRating,
 )
 from zyte_common_items.util import url_to_str
 
 
 @attrs.define(kw_only=True)
 class ProductVariant(Item):
@@ -608,7 +609,106 @@
     )
 
     #:  List of the tags associated with the place.
     tags: Optional[List[str]] = None
 
     #: Data extraction process metadata.
     metadata: Optional[BusinessPlaceMetadata] = None
+
+
+@attrs.define(slots=True, kw_only=True)
+class RealEstate(Item):
+    #: The url of the final response, after any redirects.
+    url: str = attrs.field(converter=url_to_str)
+
+    #: Webpage `breadcrumb trail`_.
+    #:
+    #: .. _Breadcrumb trail: https://en.wikipedia.org/wiki/Breadcrumb_navigation
+    breadcrumbs: Optional[List[Breadcrumb]] = None
+
+    #: The identifier of the real estate, usually assigned by the seller and unique within a website, similar to product SKU.
+    realEstateId: Optional[str] = None
+
+    #: The name of the real estate.
+    name: Optional[str] = None
+
+    #: Publication date of the real estate offer.
+    #:
+    #: Format: ISO 8601 format: "YYYY-MM-DDThh:mm:ssZ"
+    #:
+    #: With timezone, if available.
+    datePublished: Optional[str] = None
+
+    #: Same date as datePublished, but before parsing/normalization, i.e. as it appears on the website.
+    datePublishedRaw: Optional[str] = None
+
+    #: The description of the real estate.
+    #:
+    #: Format:
+    #:
+    #: - trimmed (no whitespace at the beginning or the end of the description string),
+    #:
+    #: - line breaks included,
+    #:
+    #: - no length limit,
+    #:
+    #: - no normalization of Unicode characters,
+    #:
+    #: - no concatenation of description from different parts of the page.
+    description: Optional[str] = None
+
+    #: The details of the main image of the real estate.
+    mainImage: Optional[Image] = None
+
+    #: A list of URL values of all images of the real estate.
+    images: Optional[List[Image]] = None
+
+    #: The details of the address of the real estate.
+    address: Optional[Address] = None
+
+    #: Real estate area details.
+    area: Optional[RealEstateArea] = None
+
+    #: The total number of bathrooms in the real estate.
+    numberOfBathroomsTotal: Optional[int] = None
+
+    #: The number of full bathrooms in the real estate.
+    numberOfFullBathrooms: Optional[int] = None
+
+    #: The number of partial bathrooms in the real estate.
+    numberOfPartialBathrooms: Optional[int] = None
+
+    #: The number of bedrooms in the real estate.
+    numberOfBedrooms: Optional[int] = None
+
+    #: The number of rooms (excluding bathrooms and closets) of the real estate.
+    numberOfRooms: Optional[int] = None
+
+    #: Type of a trade action: buying or renting.
+    tradeType: Optional[str] = None
+
+    #: The offer price of the real estate.
+    price: Optional[str] = None
+
+    #: The rental period to which the rental price applies, only available in case of rental. Usually weekly, monthly, quarterly, yearly.
+    rentalPeriod: Optional[str] = None
+
+    #: Currency associated with the price, as appears on the page (no post-processing).
+    currencyRaw: Optional[str] = None
+
+    #: The currency of the price, in 3-letter ISO 4217 format.
+    currency: Optional[str] = None
+
+    #: A name-value pair field holding information pertaining to specific features. Usually in a form of a specification table or freeform specification list.
+    additionalProperties: Optional[List[AdditionalProperty]] = None
+
+    #: Type of the property, e.g. flat, house, land.
+    propertyType: Optional[str] = None
+
+    #: The year the real estate was built.
+    yearBuilt: Optional[int] = None
+
+    #: The URL of the virtual tour of the real estate.
+    virtualTourUrl: Optional[str] = None
+
+    #: Contains metadata about the data extraction process.
+    metadata: Optional[Metadata] = None
```

### Comparing `zyte-common-items-0.4.0/zyte_common_items/util.py` & `zyte-common-items-0.5.0/zyte_common_items/util.py`

 * *Files 4% similar despite different names*

```diff
@@ -61,7 +61,11 @@
 
 def url_to_str(url: Union[str, _Url]) -> str:
     if not isinstance(url, (str, _Url)):
         raise ValueError(
             f"{url!r} is neither a string nor an instance of RequestURL or ResponseURL."
         )
     return str(url)
+
+
+def format_datetime(dt):
+    return f"{dt.isoformat(timespec='seconds')}Z"
```

### Comparing `zyte-common-items-0.4.0/zyte_common_items.egg-info/PKG-INFO` & `zyte-common-items-0.5.0/zyte_common_items.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zyte-common-items
-Version: 0.4.0
+Version: 0.5.0
 Summary: Item definitions for Zyte API schema
 Home-page: https://github.com/zytedata/zyte-common-items
 Author: Zyte Group Ltd
 Author-email: info@zyte.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
```

