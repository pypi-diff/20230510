# Comparing `tmp/chat2plot-0.0.4.tar.gz` & `tmp/chat2plot-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chat2plot-0.0.4.tar", last modified: Tue May  9 15:17:05 2023, max compression
+gzip compressed data, was "chat2plot-0.0.5.tar", last modified: Wed May 10 14:39:51 2023, max compression
```

## Comparing `chat2plot-0.0.4.tar` & `chat2plot-0.0.5.tar`

### file list

```diff
@@ -1,26 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 15:17:05.067079 chat2plot-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-09 15:16:54.000000 chat2plot-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-09 15:16:54.000000 chat2plot-0.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-05-09 15:17:05.067079 chat2plot-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-05-09 15:16:54.000000 chat2plot-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 15:17:05.067079 chat2plot-0.0.4/chat2plot/
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-09 15:16:54.000000 chat2plot-0.0.4/chat2plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9007 2023-05-09 15:16:54.000000 chat2plot-0.0.4/chat2plot/chat2plot.py
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-09 15:16:54.000000 chat2plot-0.0.4/chat2plot/dataset_description.py
--rw-r--r--   0 runner    (1001) docker     (123)     4552 2023-05-09 15:16:54.000000 chat2plot-0.0.4/chat2plot/render.py
--rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-05-09 15:16:54.000000 chat2plot-0.0.4/chat2plot/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-05-09 15:16:54.000000 chat2plot-0.0.4/chat2plot/transform.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-09 15:16:54.000000 chat2plot-0.0.4/chat2plot/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 15:17:05.067079 chat2plot-0.0.4/chat2plot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-05-09 15:17:05.000000 chat2plot-0.0.4/chat2plot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-09 15:17:05.000000 chat2plot-0.0.4/chat2plot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 15:17:05.000000 chat2plot-0.0.4/chat2plot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-09 15:17:05.000000 chat2plot-0.0.4/chat2plot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-09 15:17:05.000000 chat2plot-0.0.4/chat2plot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-09 15:16:54.000000 chat2plot-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-09 15:16:54.000000 chat2plot-0.0.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-09 15:17:05.071079 chat2plot-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-05-09 15:16:54.000000 chat2plot-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 15:17:05.067079 chat2plot-0.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 15:16:54.000000 chat2plot-0.0.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-09 15:16:54.000000 chat2plot-0.0.4/tests/test_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:39:51.077373 chat2plot-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-10 14:39:35.000000 chat2plot-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-10 14:39:35.000000 chat2plot-0.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-05-10 14:39:51.077373 chat2plot-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-05-10 14:39:35.000000 chat2plot-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:39:51.073373 chat2plot-0.0.5/chat2plot/
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-10 14:39:35.000000 chat2plot-0.0.5/chat2plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7992 2023-05-10 14:39:35.000000 chat2plot-0.0.5/chat2plot/chat2plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-10 14:39:35.000000 chat2plot-0.0.5/chat2plot/dataset_description.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-05-10 14:39:35.000000 chat2plot-0.0.5/chat2plot/dictionary_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-05-10 14:39:35.000000 chat2plot-0.0.5/chat2plot/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-05-10 14:39:35.000000 chat2plot-0.0.5/chat2plot/render.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6794 2023-05-10 14:39:35.000000 chat2plot-0.0.5/chat2plot/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-05-10 14:39:35.000000 chat2plot-0.0.5/chat2plot/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-10 14:39:35.000000 chat2plot-0.0.5/chat2plot/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:39:51.077373 chat2plot-0.0.5/chat2plot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-05-10 14:39:51.000000 chat2plot-0.0.5/chat2plot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-05-10 14:39:51.000000 chat2plot-0.0.5/chat2plot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 14:39:51.000000 chat2plot-0.0.5/chat2plot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-10 14:39:51.000000 chat2plot-0.0.5/chat2plot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-10 14:39:51.000000 chat2plot-0.0.5/chat2plot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-10 14:39:35.000000 chat2plot-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-10 14:39:35.000000 chat2plot-0.0.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-10 14:39:51.077373 chat2plot-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-05-10 14:39:35.000000 chat2plot-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:39:51.077373 chat2plot-0.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 14:39:35.000000 chat2plot-0.0.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-10 14:39:35.000000 chat2plot-0.0.5/tests/test_schema.py
```

### Comparing `chat2plot-0.0.4/LICENSE` & `chat2plot-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `chat2plot-0.0.4/PKG-INFO` & `chat2plot-0.0.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chat2plot
-Version: 0.0.4
+Version: 0.0.5
 Summary: chat to visualization with LLM
 Home-page: https://github.com/nyanp/chat2plot
 Author: nyanp
 Author-email: Noumi.Taiga@gmail.com
 License: MIT
 Keywords: llm visualization chart gpt
 Classifier: License :: OSI Approved :: MIT License
@@ -30,20 +30,26 @@
 os.environ["OPENAI_API_KEY"] = "..."
 
 df = pd.read_csv(...)
 
 # 2. Pass a dataframe to draw
 c2p = chat2plot(df)
 
-# 3. Plot chart interactively
-c2p("average target over countries")
+# 3. Make a question about the data
+result = c2p("average target over countries")
+result.figure.show()  # draw a plot
+print(result.config)  # get a config (json / dataclass)
+print(result.explanation)  # see the explanation generated by LLM
+
+# you can make follow-up request to refine the chart
+result = c2p("change to horizontal-bar chart")
+result.figure.show()
 
-c2p("change to horizontal-bar chart")
-
-c2p("...")
+# draw a chart inside chat2plot
+_ = c2p("filter data to asia region", show_plot=True)
 ```
 
 ## Why Chat2Plpot
 
 Inside Chat2Plot, LLM does not generate Python code,
 but generates plot specifications in json.
```

### Comparing `chat2plot-0.0.4/README.md` & `chat2plot-0.0.5/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -15,20 +15,26 @@
 os.environ["OPENAI_API_KEY"] = "..."
 
 df = pd.read_csv(...)
 
 # 2. Pass a dataframe to draw
 c2p = chat2plot(df)
 
-# 3. Plot chart interactively
-c2p("average target over countries")
+# 3. Make a question about the data
+result = c2p("average target over countries")
+result.figure.show()  # draw a plot
+print(result.config)  # get a config (json / dataclass)
+print(result.explanation)  # see the explanation generated by LLM
+
+# you can make follow-up request to refine the chart
+result = c2p("change to horizontal-bar chart")
+result.figure.show()
 
-c2p("change to horizontal-bar chart")
-
-c2p("...")
+# draw a chart inside chat2plot
+_ = c2p("filter data to asia region", show_plot=True)
 ```
 
 ## Why Chat2Plpot
 
 Inside Chat2Plot, LLM does not generate Python code,
 but generates plot specifications in json.
```

### Comparing `chat2plot-0.0.4/chat2plot/render.py` & `chat2plot-0.0.5/chat2plot/render.py`

 * *Files 13% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         ax["labels"] = labels
 
     return ax
 
 
 def draw_plotly(df: pd.DataFrame, config: PlotConfig, show: bool = True) -> Figure:
     df_filtered = filter_data(df, config.filters).copy()
-    df_filtered = transform(df_filtered, config)
+    df_filtered, config = transform(df_filtered, config)
 
     chart_type = config.chart_type
 
     if chart_type in [ChartType.BAR, ChartType.HORIZONTAL_BAR]:
         agg = groupby_agg(df_filtered, config)
         x = agg.columns[0]
         y = agg.columns[-1]
@@ -48,24 +48,24 @@
 
         if chart_type == ChartType.HORIZONTAL_BAR:
             x, y = y, x
             orientation = "h"
 
         fig = px.bar(
             agg,
-            color=config.hue.column if config.hue else None,
+            color=config.hue or None,
             orientation=orientation,
             **_ax_config(config, x, y),
         )
     elif chart_type == ChartType.SCATTER:
         assert config.x is not None
         fig = px.scatter(
             df_filtered,
-            color=config.hue.column if config.hue else None,
-            **_ax_config(config, config.x.field.column, config.y.field.column),
+            color=config.hue or None,
+            **_ax_config(config, config.x.column, config.y.column),
         )
     elif chart_type == ChartType.PIE:
         agg = groupby_agg(df_filtered, config)
         fig = px.pie(agg, names=agg.columns[0], values=agg.columns[-1])
     elif chart_type in [ChartType.LINE, ChartType.AREA]:
         func_table = {ChartType.LINE: px.line, ChartType.AREA: px.area}
 
@@ -74,16 +74,16 @@
             fig = func_table[chart_type](
                 agg, **_ax_config(config, agg.columns[0], y=agg.columns[-1])
             )
         else:
             assert config.x is not None
             fig = func_table[chart_type](
                 df_filtered,
-                color=config.hue.column if config.hue else None,
-                **_ax_config(config, config.x.field.column, config.y.field.column),
+                color=config.hue or None,
+                **_ax_config(config, config.x.column, config.y.column),
             )
     else:
         raise ValueError(f"Unknown chart_type: {chart_type}")
 
     if show:
         fig.show()
 
@@ -104,52 +104,61 @@
     if show:
         chart.show()
 
     return chart
 
 
 def groupby_agg(df: pd.DataFrame, config: PlotConfig) -> pd.DataFrame:
-    group_by = [config.x.field.column] if config.x is not None else []
+    group_by = [config.x.column] if config.x is not None else []
 
-    if config.hue and (not config.x or (config.hue.column != config.x.field.column)):
-        group_by.append(config.hue.column)
+    if config.hue and (not config.x or (config.hue != config.x.column)):
+        group_by.append(config.hue)
 
     agg_method = {
         AggregationType.AVG: "mean",
         AggregationType.SUM: "sum",
         AggregationType.COUNT: "count",
         AggregationType.DISTINCT_COUNT: "nunique",
         AggregationType.MIN: "min",
         AggregationType.MAX: "max",
     }
 
     y = config.y
-    assert y.field.aggregation is not None
+    assert y.transform.aggregation is not None
 
     if not group_by:
         return pd.DataFrame(
-            {y.field.name(): [df[y.field.column].agg(agg_method[y.field.aggregation])]}
+            {y.transformed_name(): [df[y.column].agg(agg_method[y.transform.aggregation])]}
         )
     else:
         agg = (
-            df.groupby(group_by, dropna=False)[y.field.column]
-            .agg(agg_method[y.field.aggregation])
-            .rename(y.field.name())
+            df.groupby(group_by, dropna=False)[y.column]
+            .agg(agg_method[y.transform.aggregation])
+            .rename(y.transformed_name())
         )
         ascending = config.sort_order == SortOrder.ASC
 
         if config.sort_criteria == SortingCriteria.NAME:
             agg = agg.sort_index(ascending=ascending)
         elif config.sort_criteria == SortingCriteria.VALUE:
             agg = agg.sort_values(ascending=ascending)
 
         return agg.reset_index()
 
 
 def is_aggregation(config: PlotConfig) -> bool:
-    return config.y.field.aggregation is not None
+    return config.y.transform and config.y.transform.aggregation is not None
 
 
 def filter_data(df: pd.DataFrame, filters: list[str]) -> pd.DataFrame:
     if not filters:
         return df
-    return df.query(" and ".join([Filter.parse_from_llm(f).escaped() for f in filters]))
+
+    elements = []
+    for f in filters:
+        try:
+            e = Filter.parse_from_llm(f).escaped()
+        except Exception:
+            e = f
+        elements.append(f"({e})")
+
+    return df.query(" and ".join(elements))
```

### Comparing `chat2plot-0.0.4/chat2plot/schema.py` & `chat2plot-0.0.5/chat2plot/schema.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,16 @@
-import json
 import re
 from enum import Enum
 from typing import Any, Type
 
+import jsonref
 import pydantic
 
+from chat2plot.dictionary_helper import remove_field_recursively, flatten_single_element_allof
+
 
 class SchemaWithoutTitle:
     @staticmethod
     def schema_extra(schema: dict[str, Any], _: Type[Any]) -> None:
         for prop in schema.get("properties", {}).values():
             prop.pop("title", None)
 
@@ -44,34 +46,54 @@
 
 
 class SortOrder(str, Enum):
     ASC = "asc"
     DESC = "desc"
 
 
-class Field(pydantic.BaseModel):
-    column: str = pydantic.Field(None, description="column name of the dataset")
+class TimeUnit(str, Enum):
+    YEAR= "year"
+    MONTH = "month"
+    WEEK = "week"
+    QUARTER = "quarter"
+    DAY = "day"
+
+
+class Transform(pydantic.BaseModel):
     aggregation: AggregationType | None = pydantic.Field(
-        None, description="Type of aggregation. will be ignored when it is scatter plot"
+        None,
+        description=f"Type of aggregation. It will be ignored when it is scatter plot",
+    )
+    bin_size: int | None = pydantic.Field(
+        None,
+        description="Integer value as the number of bins used to discretizes numeric values into a set of bins"
+    )
+    time_unit: TimeUnit | None = pydantic.Field(
+        None,
+        description="The time unit used to descretize date/datetime values"
     )
 
-    def name(self) -> str:
-        return (
-            f"{self.aggregation.value}({self.column})"
-            if self.aggregation
-            else self.column
-        )
+    def transformed_name(self, col: str) -> str:
+        dst = col
+        if self.time_unit:
+            dst = f"UNIT({col}, {self.time_unit.value})"
+        if self.bin_size:
+            dst = f"BINNING({col}, {self.bin_size})"
+        if self.aggregation:
+            dst = f"{self.aggregation.value}({col})"
+        return dst
 
     @classmethod
-    def parse_from_llm(cls, d: dict[str, str]) -> "Field":
-        return Field(
-            column=d["column"],
+    def parse_from_llm(cls, d: dict[str, str]) -> "Transform":
+        return Transform(
             aggregation=AggregationType(d["aggregation"].upper())
             if d.get("aggregation")
             else None,
+            bin_size=d.get("bin_size") or None,
+            time_unit=d.get("time_unit") or None
         )
 
     class Config(SchemaWithoutTitle):
         pass
 
 
 class Filter(pydantic.BaseModel):
@@ -100,64 +122,70 @@
                 rhs = m.group(2).strip()
                 return Filter(lhs=lhs, rhs=rhs, op=op)
 
         raise ValueError(f"Unsupported op or failed to parse: {f}")
 
 
 class Axis(pydantic.BaseModel):
-    field: Field
+    column: str = pydantic.Field(None, description="column in datasets used for the axis")
+    transform: Transform | None = pydantic.Field(None, description="transformation applied to column")
     min_value: float | None
     max_value: float | None
     label: str | None
 
+    def transformed_name(self):
+        return self.transform.transformed_name(self.column) if self.transform else self.column
+
     class Config(SchemaWithoutTitle):
         pass
 
     @classmethod
     def parse_from_llm(cls, d: dict[str, str | float | dict[str, str]]) -> "Axis":
         return Axis(
-            field=Field.parse_from_llm(d["field"]),  # type: ignore
+            column=d.get("column") or None,
+            transform=Transform.parse_from_llm(d["transform"]) if "transform" in d else None,  # type: ignore
             min_value=d.get("min_value"),  # type: ignore
             max_value=d.get("max_value"),  # type: ignore
-            label=d.get("label"),  # type: ignore
+            label=d.get("label") or None,  # type: ignore
         )
 
 
 class PlotConfig(pydantic.BaseModel):
     chart_type: ChartType = pydantic.Field(None, description="the type of the chart")
+    filters: list[str] = pydantic.Field(
+        None,
+        description="List of filter conditions, where each filter must be a legal string that can be passed to df.query(),"
+        ' such as "x >= 0". Filters will be calculated before transforming axis.',
+    )
     x: Axis | None = pydantic.Field(
         None, description="X-axis for the chart, or label column for pie chart"
     )
     y: Axis = pydantic.Field(
         None,
         description="Y-axis or measure value for the chart, or the wedge sizes for pie chart.",
     )
-    filters: list[str] = pydantic.Field(
-        None,
-        description='List of filter conditions, where each filter must be a legal string that can be passed to df.query(), such as "x >= 0".',
-    )
-    hue: Field | None = pydantic.Field(
+    hue: str | None = pydantic.Field(
         None,
-        description="Dimension used as grouping variables that will produce different colors.",
+        description="Column name used as grouping variables that will produce different colors.",
     )
     sort_criteria: SortingCriteria | None = pydantic.Field(
         None, description="The sorting criteria for x-axis"
     )
     sort_order: SortOrder | None = pydantic.Field(
         None, description="Sorting order for x-axis"
     )
 
     class Config(SchemaWithoutTitle):
         pass
 
     @property
     def required_columns(self) -> list[str]:
-        columns = [self.y.field.column]
+        columns = [self.y.column]
         if self.x:
-            columns.append(self.x.field.column)
+            columns.append(self.x.column)
         return columns
 
     @classmethod
     def from_json(cls, json_data: dict[str, Any]) -> "PlotConfig":
         assert "chart_type" in json_data
         assert "y" in json_data
 
@@ -170,72 +198,26 @@
         chart_type = ChartType(json_data["chart_type"])
 
         return cls(
             chart_type=chart_type,
             x=Axis.parse_from_llm(json_data["x"]) if json_data.get("x") else None,
             y=Axis.parse_from_llm(json_data["y"]),
             filters=wrap_if_not_list(json_data.get("filters", [])),
-            hue=Field.parse_from_llm(json_data["hue"])
-            if json_data.get("hue")
-            else None,
+            hue=json_data.get("hue") or None,
             sort_criteria=SortingCriteria(json_data["sort_criteria"])
             if json_data.get("sort_criteria")
             else None,
             sort_order=SortOrder(json_data["sort_order"])
             if json_data.get("sort_order")
             else None,
         )
 
 
-class LLMResponse(pydantic.BaseModel):
-    response_type: ResponseType
-    config: PlotConfig | None
-
-
-def inlining_refs_in_schema(
-    schema: dict[str, Any], MAX_TRIES: int = 100, not_inlining: list[str] | None = None
-) -> dict[str, Any]:
-    not_inlining = not_inlining or []
-    assert not_inlining is not None
-
-    def replace_value_in_dict(item: Any, original_schema: dict[str, Any]) -> Any:
-        if isinstance(item, list):
-            return [replace_value_in_dict(i, original_schema) for i in item]
-        elif isinstance(item, dict):
-            if list(item.keys()) == ["$ref"]:
-                definitions = item["$ref"][2:].split("/")
-                if definitions[-1] in not_inlining:  # type: ignore
-                    return item
-                res = original_schema.copy()
-                for definition in definitions:
-                    res = res[definition]
-                return res
-            else:
-                return {
-                    key: replace_value_in_dict(i, original_schema)
-                    for key, i in item.items()
-                }
-        else:
-            return item
-
-    for i in range(MAX_TRIES):
-        if "$ref" not in json.dumps(schema):
-            break
-        schema = replace_value_in_dict(schema.copy(), schema.copy())
-
-    defs = list(schema["definitions"].keys())
-    for key in defs:
-        if key not in not_inlining:
-            del schema["definitions"][key]
-
-    if not schema["definitions"]:
-        del schema["definitions"]
-
-    return schema
-
-
-def get_schema_of_chart_config(inlining_refs: bool = True) -> dict[str, Any]:
-    schema = PlotConfig.schema()
-    if inlining_refs:
-        schema = inlining_refs_in_schema(schema)
+def get_schema_of_chart_config(inlining_refs: bool = False, remove_title: bool = True) -> dict[str, Any]:
+    defs = jsonref.loads(PlotConfig.schema_json()) if inlining_refs else PlotConfig.schema()  # type: ignore
+
+    if remove_title:
+        defs = remove_field_recursively(defs, "title")
+
+    defs = flatten_single_element_allof(defs)
 
-    return schema
+    return defs
```

### Comparing `chat2plot-0.0.4/chat2plot.egg-info/PKG-INFO` & `chat2plot-0.0.5/chat2plot.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chat2plot
-Version: 0.0.4
+Version: 0.0.5
 Summary: chat to visualization with LLM
 Home-page: https://github.com/nyanp/chat2plot
 Author: nyanp
 Author-email: Noumi.Taiga@gmail.com
 License: MIT
 Keywords: llm visualization chart gpt
 Classifier: License :: OSI Approved :: MIT License
@@ -30,20 +30,26 @@
 os.environ["OPENAI_API_KEY"] = "..."
 
 df = pd.read_csv(...)
 
 # 2. Pass a dataframe to draw
 c2p = chat2plot(df)
 
-# 3. Plot chart interactively
-c2p("average target over countries")
+# 3. Make a question about the data
+result = c2p("average target over countries")
+result.figure.show()  # draw a plot
+print(result.config)  # get a config (json / dataclass)
+print(result.explanation)  # see the explanation generated by LLM
+
+# you can make follow-up request to refine the chart
+result = c2p("change to horizontal-bar chart")
+result.figure.show()
 
-c2p("change to horizontal-bar chart")
-
-c2p("...")
+# draw a chart inside chat2plot
+_ = c2p("filter data to asia region", show_plot=True)
 ```
 
 ## Why Chat2Plpot
 
 Inside Chat2Plot, LLM does not generate Python code,
 but generates plot specifications in json.
```

### Comparing `chat2plot-0.0.4/setup.cfg` & `chat2plot-0.0.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `chat2plot-0.0.4/setup.py` & `chat2plot-0.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `chat2plot-0.0.4/tests/test_schema.py` & `chat2plot-0.0.5/tests/test_schema.py`

 * *Files identical despite different names*

