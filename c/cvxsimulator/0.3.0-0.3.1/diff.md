# Comparing `tmp/cvxsimulator-0.3.0.tar.gz` & `tmp/cvxsimulator-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cvxsimulator-0.3.0.tar", max compression
+gzip compressed data, was "cvxsimulator-0.3.1.tar", max compression
```

## Comparing `cvxsimulator-0.3.0.tar` & `cvxsimulator-0.3.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1102 2023-05-09 21:32:33.005040 cvxsimulator-0.3.0/LICENSE
--rw-r--r--   0        0        0     4226 2023-05-09 21:32:33.005040 cvxsimulator-0.3.0/README.md
--rw-r--r--   0        0        0        0 2023-05-09 21:32:33.073040 cvxsimulator-0.3.0/cvx/simulator/__init__.py
--rw-r--r--   0        0        0     3796 2023-05-09 21:32:33.077041 cvxsimulator-0.3.0/cvx/simulator/builder.py
--rw-r--r--   0        0        0     1163 2023-05-09 21:32:33.077041 cvxsimulator-0.3.0/cvx/simulator/metrics.py
--rw-r--r--   0        0        0     1341 2023-05-09 21:32:33.077041 cvxsimulator-0.3.0/cvx/simulator/month.py
--rw-r--r--   0        0        0     3549 2023-05-09 21:32:33.077041 cvxsimulator-0.3.0/cvx/simulator/portfolio.py
--rw-r--r--   0        0        0      464 2023-05-09 21:32:33.077041 cvxsimulator-0.3.0/cvx/simulator/trading_costs.py
--rw-r--r--   0        0        0      596 2023-05-09 21:33:27.529802 cvxsimulator-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     4795 1970-01-01 00:00:00.000000 cvxsimulator-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1102 2023-05-10 05:02:56.377078 cvxsimulator-0.3.1/LICENSE
+-rw-r--r--   0        0        0     4907 2023-05-10 05:02:56.377078 cvxsimulator-0.3.1/README.md
+-rw-r--r--   0        0        0        0 2023-05-10 05:02:56.445079 cvxsimulator-0.3.1/cvx/simulator/__init__.py
+-rw-r--r--   0        0        0     3796 2023-05-10 05:02:56.445079 cvxsimulator-0.3.1/cvx/simulator/builder.py
+-rw-r--r--   0        0        0     1163 2023-05-10 05:02:56.445079 cvxsimulator-0.3.1/cvx/simulator/metrics.py
+-rw-r--r--   0        0        0     1341 2023-05-10 05:02:56.445079 cvxsimulator-0.3.1/cvx/simulator/month.py
+-rw-r--r--   0        0        0     3549 2023-05-10 05:02:56.445079 cvxsimulator-0.3.1/cvx/simulator/portfolio.py
+-rw-r--r--   0        0        0      464 2023-05-10 05:02:56.445079 cvxsimulator-0.3.1/cvx/simulator/trading_costs.py
+-rw-r--r--   0        0        0      596 2023-05-10 05:03:54.213931 cvxsimulator-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     5476 1970-01-01 00:00:00.000000 cvxsimulator-0.3.1/PKG-INFO
```

### Comparing `cvxsimulator-0.3.0/LICENSE` & `cvxsimulator-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cvxsimulator-0.3.0/README.md` & `cvxsimulator-0.3.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -20,27 +20,29 @@
 * [Analyse results](#analyse-results)
 
 We demonstrate those steps with somewhat silly policies. They are never good strategies, but are always valid ones.
 
 ### Create the builder object
 
 The user defines a builder object by loading a frame of prices 
-and initialize the initial amount of cash used in our experiment:
+and initialize the amount of cash used in our experiment:
 
 ```python
 from pathlib import Path
 
 import pandas as pd
-from cvx.simulator.portfolio import build_portfolio
+from cvx.simulator.builder import builder
 
 prices = pd.read_csv(Path("resources") / "price.csv", index_col=0, parse_dates=True, header=0).ffill()
 b = builder(prices=prices, initial_cash=1e6)
 ```
 
-It is also possible to specify a model for trading costs.
+It is also possible to specify a model for trading costs. 
+The builder helps to fill up the frame of positions. Only once done
+we construct the actual portfolio.
 
 ### Loop through time
 
 We have overloaded the `__iter__` and `__setitem__` methods to create a custom loop. 
 Let's start with a first strategy. Each day we choose two names from the universe at random.
 Buy one (say 0.1 of your portfolio wealth) and short one the same amount.
 
@@ -51,26 +53,30 @@
     # compute the pair
     stocks = pd.Series(index=b.assets, data=0.0)
     stocks[pair] = [state.nav, -state.nav] / state.prices[pair].values
     # update the position 
     b[t[-1]] = 0.1 * stocks
 ```
 
+Here t is the growing list of timestamps, e.g. in the first iteration
+t is $t1, t2$, in the second iteration it will be $t1, t2, t3$ etc.
+
 A lot of magic is hidden in the state variable. 
 The state gives access to the currently available cash, the current prices and the current valuation of all holdings.
 
 Here's a slightly more realistic loop. Given a set of $4$ assets we want to implmenent the popular $1/n$ strategy.
 
 ```python
 for t, state in b:
     # each day we invest a quarter of the capital in the assets
     b[t[-1]] = 0.25 * state.nav / state.prices
 ```
 
-Note that we update the position at time `now` using a series of actual stocks rather than weights or cashpositions.
+Note that we update the position at the last element in the t list 
+using a series of actual stocks rather than weights or cashpositions.
 The builder class also exposes setters for such conventions.
 
 ```python
 for t, state in b:
     # each day we invest a quarter of the capital in the assets
     b.set_weights(t[-1], pd.Series(index=b.assets, data = 0.25))
 ```
@@ -79,31 +85,45 @@
 
 ```python
 portfolio = b.build()
 ```
 
 ### Analyse results
 
-The loop above is filling up the desired positions. The portfolio object is now ready for further analysis.
+The loop above is filling up the desired positions. 
+After triggering the `build()` the resulting portfolio 
+is ready for further analysis.
 It is possible dive into the data, e.g.
 
 ```python
 portfolio.nav
 portfolio.cash
 portfolio.equity
 ...
 ``` 
 
-## The dirty path
+## Bypassing the builder
 
-Some may know the positions they want to enter for eternity. 
+Some may know the positions the portfolio shall enter for eternity. 
 Running through a loop is rather non-pythonic waste of time in such a case.
 It is possible to completely bypass this step by submitting 
 a frame of positions together with a frame of prices when creating the portfolio object.
 
+```python
+from pathlib import Path
+
+import pandas as pd
+from cvx.simulator.portfolio import EquityPortfolio
+
+prices = pd.read_csv(Path("resources") / "price.csv", index_col=0, parse_dates=True, header=0).ffill()
+stocks = pd.read_csv(Path("resources") / "stock.csv", index_col=0, parse_dates=True, header=0)
+portfolio = EquityPortfolio(prices=prices, stocks=stocks, initial_cash=1e6)
+```
+
+
 ## Poetry
 
 We assume you share already the love for [Poetry](https://python-poetry.org). Once you have installed poetry you can perform
 
 ```bash
 poetry install
 ```
```

### Comparing `cvxsimulator-0.3.0/cvx/simulator/builder.py` & `cvxsimulator-0.3.1/cvx/simulator/builder.py`

 * *Files identical despite different names*

### Comparing `cvxsimulator-0.3.0/cvx/simulator/metrics.py` & `cvxsimulator-0.3.1/cvx/simulator/metrics.py`

 * *Files identical despite different names*

### Comparing `cvxsimulator-0.3.0/cvx/simulator/month.py` & `cvxsimulator-0.3.1/cvx/simulator/month.py`

 * *Files identical despite different names*

### Comparing `cvxsimulator-0.3.0/cvx/simulator/portfolio.py` & `cvxsimulator-0.3.1/cvx/simulator/portfolio.py`

 * *Files identical despite different names*

### Comparing `cvxsimulator-0.3.0/pyproject.toml` & `cvxsimulator-0.3.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cvxsimulator"
-version = "v0.3.0"
+version = "v0.3.1"
 description = "Simple simulator for investors"
 authors = ["Thomas Schmelzer"]
 readme = "README.md"
 repository = "https://github.com/cvxgrp/simulator"
 packages = [{include = "cvx"}]
 
 [tool.poetry.dependencies]
```

### Comparing `cvxsimulator-0.3.0/PKG-INFO` & `cvxsimulator-0.3.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvxsimulator
-Version: 0.3.0
+Version: 0.3.1
 Summary: Simple simulator for investors
 Home-page: https://github.com/cvxgrp/simulator
 Author: Thomas Schmelzer
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -36,27 +36,29 @@
 * [Analyse results](#analyse-results)
 
 We demonstrate those steps with somewhat silly policies. They are never good strategies, but are always valid ones.
 
 ### Create the builder object
 
 The user defines a builder object by loading a frame of prices 
-and initialize the initial amount of cash used in our experiment:
+and initialize the amount of cash used in our experiment:
 
 ```python
 from pathlib import Path
 
 import pandas as pd
-from cvx.simulator.portfolio import build_portfolio
+from cvx.simulator.builder import builder
 
 prices = pd.read_csv(Path("resources") / "price.csv", index_col=0, parse_dates=True, header=0).ffill()
 b = builder(prices=prices, initial_cash=1e6)
 ```
 
-It is also possible to specify a model for trading costs.
+It is also possible to specify a model for trading costs. 
+The builder helps to fill up the frame of positions. Only once done
+we construct the actual portfolio.
 
 ### Loop through time
 
 We have overloaded the `__iter__` and `__setitem__` methods to create a custom loop. 
 Let's start with a first strategy. Each day we choose two names from the universe at random.
 Buy one (say 0.1 of your portfolio wealth) and short one the same amount.
 
@@ -67,26 +69,30 @@
     # compute the pair
     stocks = pd.Series(index=b.assets, data=0.0)
     stocks[pair] = [state.nav, -state.nav] / state.prices[pair].values
     # update the position 
     b[t[-1]] = 0.1 * stocks
 ```
 
+Here t is the growing list of timestamps, e.g. in the first iteration
+t is $t1, t2$, in the second iteration it will be $t1, t2, t3$ etc.
+
 A lot of magic is hidden in the state variable. 
 The state gives access to the currently available cash, the current prices and the current valuation of all holdings.
 
 Here's a slightly more realistic loop. Given a set of $4$ assets we want to implmenent the popular $1/n$ strategy.
 
 ```python
 for t, state in b:
     # each day we invest a quarter of the capital in the assets
     b[t[-1]] = 0.25 * state.nav / state.prices
 ```
 
-Note that we update the position at time `now` using a series of actual stocks rather than weights or cashpositions.
+Note that we update the position at the last element in the t list 
+using a series of actual stocks rather than weights or cashpositions.
 The builder class also exposes setters for such conventions.
 
 ```python
 for t, state in b:
     # each day we invest a quarter of the capital in the assets
     b.set_weights(t[-1], pd.Series(index=b.assets, data = 0.25))
 ```
@@ -95,31 +101,45 @@
 
 ```python
 portfolio = b.build()
 ```
 
 ### Analyse results
 
-The loop above is filling up the desired positions. The portfolio object is now ready for further analysis.
+The loop above is filling up the desired positions. 
+After triggering the `build()` the resulting portfolio 
+is ready for further analysis.
 It is possible dive into the data, e.g.
 
 ```python
 portfolio.nav
 portfolio.cash
 portfolio.equity
 ...
 ``` 
 
-## The dirty path
+## Bypassing the builder
 
-Some may know the positions they want to enter for eternity. 
+Some may know the positions the portfolio shall enter for eternity. 
 Running through a loop is rather non-pythonic waste of time in such a case.
 It is possible to completely bypass this step by submitting 
 a frame of positions together with a frame of prices when creating the portfolio object.
 
+```python
+from pathlib import Path
+
+import pandas as pd
+from cvx.simulator.portfolio import EquityPortfolio
+
+prices = pd.read_csv(Path("resources") / "price.csv", index_col=0, parse_dates=True, header=0).ffill()
+stocks = pd.read_csv(Path("resources") / "stock.csv", index_col=0, parse_dates=True, header=0)
+portfolio = EquityPortfolio(prices=prices, stocks=stocks, initial_cash=1e6)
+```
+
+
 ## Poetry
 
 We assume you share already the love for [Poetry](https://python-poetry.org). Once you have installed poetry you can perform
 
 ```bash
 poetry install
 ```
```

