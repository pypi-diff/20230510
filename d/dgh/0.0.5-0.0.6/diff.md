# Comparing `tmp/dgh-0.0.5.tar.gz` & `tmp/dgh-0.0.6.tar.gz`

## Comparing `dgh-0.0.5.tar` & `dgh-0.0.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 dgh-0.0.5/CHANGELOG.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dgh-0.0.5/dgh/__init__.py
--rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 dgh-0.0.5/dgh/auxiliary.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 dgh-0.0.5/dgh/constants.py
--rw-r--r--   0        0        0     5481 2020-02-02 00:00:00.000000 dgh-0.0.5/dgh/dgh.py
--rw-r--r--   0        0        0     3654 2020-02-02 00:00:00.000000 dgh-0.0.5/dgh/fw.py
--rw-r--r--   0        0        0     2697 2020-02-02 00:00:00.000000 dgh-0.0.5/dgh/mappings.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 dgh-0.0.5/.gitignore
--rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 dgh-0.0.5/LICENSE
--rw-r--r--   0        0        0     2305 2020-02-02 00:00:00.000000 dgh-0.0.5/README.md
--rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 dgh-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     2798 2020-02-02 00:00:00.000000 dgh-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 dgh-0.0.6/CHANGELOG.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dgh-0.0.6/dgh/__init__.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 dgh-0.0.6/dgh/constants.py
+-rw-r--r--   0        0        0     6844 2020-02-02 00:00:00.000000 dgh-0.0.6/dgh/dgh.py
+-rw-r--r--   0        0        0     3653 2020-02-02 00:00:00.000000 dgh-0.0.6/dgh/fw.py
+-rw-r--r--   0        0        0     2698 2020-02-02 00:00:00.000000 dgh-0.0.6/dgh/mappings.py
+-rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 dgh-0.0.6/dgh/spaces.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 dgh-0.0.6/.gitignore
+-rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 dgh-0.0.6/LICENSE
+-rw-r--r--   0        0        0     2402 2020-02-02 00:00:00.000000 dgh-0.0.6/README.md
+-rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 dgh-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     2895 2020-02-02 00:00:00.000000 dgh-0.0.6/PKG-INFO
```

### Comparing `dgh-0.0.5/dgh/dgh.py` & `dgh-0.0.6/dgh/dgh.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import numpy as np
 import scipy.optimize as opt
 
-from mappings import rnd_S, center, S_to_fg, S_to_R
-from fw import make_frank_wolfe_solver
-from auxiliary import arrange_distances
-from constants import DEFAULT_SEED, MAX_C
+from .mappings import rnd_S, center, S_to_fg, S_to_R
+from .fw import make_frank_wolfe_solver
+from .spaces import diam, rad, arrange_distances
+from .constants import DEFAULT_SEED, MAX_C
 
 
 def find_c(phi, X, Y):
     """
     Find c > 1 s.t. the Hessian is at most φ away from the set of positive
     semidefinite matrices (w.r.t. normalized nuclear norm-induced distance).
 
@@ -55,33 +55,56 @@
 
     dis_S = np.abs(X__Y - S @ Y__X @ S.T + S_Y_X - S_Y_X.T).max()
 
     return dis_S
 
 
 def ub(X, Y, phi_first=.1, c_first=None, iter_budget=100, center_start=False,
-       tol=1e-8, return_fg=False, verbose=0, rnd=None):
+       lb=0, tol=1e-8, validate_tri_ineq=False, return_fg=False, verbose=0, rnd=None):
     """
     Find upper bound of dGH(X, Y) by minimizing smoothed dis(R) = dis(f, g) over
     the bi-mapping polytope 𝓢 using Frank-Wolfe.
 
     :param X: distance matrix of X (2d-array)
     :param Y: distance matrix of Y (2d-array)
     :param phi_first: upper bound of the non-convexity degree ∈ (0, ½) in the
         first minimization problem (float)
     :param c_first: exponentiation base ∈ (1, ∞) for smoothing the distortion
         in the first minimization problem (float)
     :param iter_budget: total number of Frank-Wolfe iterations (int)
     :param center_start: whether to try the center of 𝓢 as a starting point first (bool)
+    :param lb: lower bound of dGH(X, Y) to avoid redundant iterations (float)
+    :param tol: tolerance to use when evaluating convergence (float)
+    :param validate_tri_ineq: whether to validate the triangle inequality (bool)
+    :param return_fg: whether to return the optimal pair of mappings (bool)
     :param verbose: 0=no output, 1=print restart results, 2=print iterations
     :return: dGH(X, Y), f [optional], g [optional]
     """
+    # Check that the distances satisfy the metric properties minus the triangle inequality.
+    assert (X >= 0).all() and (Y >= 0).all(), 'distance matrices have negative entries'
+    assert (np.diag(X) == 0).all() and (np.diag(Y) == 0).all(),\
+        'distance matrices have non-zeros on the main diagonal'
+    assert (X == X.T).all() and (Y == Y.T).all(), 'distance matrices are not symmetric'
+    if validate_tri_ineq:
+        assert validate_tri_ineq(X) and validate_tri_ineq(Y),\
+            "triangle inequality doesn't hold"
+
+    # Initialize tools for generating starting points.
     n, m = len(X), len(Y)
     rnd = rnd or np.random.RandomState(DEFAULT_SEED)
-    assert (X == X.T).all() and (Y == Y.T).all(), 'distance matrices are not symmetric'
+
+    # Update lower bound using the radius and diameter differences.
+    diam_X, diam_Y = map(diam, [X, Y])
+    rad_X, rad_Y = map(rad, [X, Y])
+    lb = max(lb, abs(diam_X - diam_Y)/2, abs(rad_X - rad_Y)/2)
+
+    # Scale all distances to prevent overflow.
+    d_max = max(diam_X, diam_Y)
+    X, Y = map(lambda Z: Z.copy()/d_max, [X, Y])
+    lb /= d_max
 
     # Find c for the first minimization if needed.
     if c_first is not None:
         assert c_first > 1, f'starting exponentiation base must be > 1 (c_first={c_first} )'
     else:
         assert phi_first is not None, f'either phi_first or c_start must be given'
         assert 0 < phi_first < .5, f'starting non-convexity UB must be < 0.5 ' \
@@ -95,49 +118,53 @@
     while iter_budget > 0:
         # Initialize new restart.
         S = center(n, m) if restart_idx == 0 and center_start else rnd_S(n, m, rnd)
         fw_idx = 0
         c = c_first
 
         # Run a sequence of FW solvers using solutions as subsequent warm starts.
-        stopping = False
-        while not stopping:
+        solving_for_next_c = True
+        while solving_for_next_c:
             # Set up next FW solver in the sequence if needed.
             try:
                 fw = fw_seq[fw_idx]
             except IndexError:
                 fw = make_frank_wolfe_solver(
                     X, Y, c, tol=tol, verbose=verbose)
                 fw_seq.append(fw)
 
             # Solve the minimization problem.
             S, used_iter = fw(S0=S, max_iter=iter_budget)
 
             # Terminate if no iterations were made, run out of iteration budget,
             # or next c will exceed floating point arithmetic limits.
-            stopping = iter_budget == used_iter or used_iter == 0 or c > MAX_C
+            solving_for_next_c = 0 < used_iter < iter_budget and c < MAX_C
 
             # Move to the next minimization obtained by squaring c.
             iter_budget -= used_iter
             fw_idx += 1
             with np.errstate(over='ignore'):
                 c **= 2
 
         # Project the solution to the set of correspondences and find the
-        # resulting distortion.
+        # resulting distortion on the original scale.
         R = S_to_R(S, n, m)
-        dis_R = dis(R, X, Y)
+        dis_R = dis(R, X, Y) * d_max
 
         # Update the best distortion achieved from all restarts.
         if dis_R < min_dis_R:
             best_f, best_g = S_to_fg(S, n, m)
             min_dis_R = dis_R
 
         if verbose >= 1:
             print(f'finished restart {restart_idx}: ½dis(R)={dis_R/2:.4f}, '
-                  f'min ½dis(R)={min_dis_R/2:.4f}')
+                  f'min ½dis(R)={min_dis_R/2:.4f}, remaining iter={iter_budget}')
 
         restart_idx += 1
 
+        # Terminate if achieved lower bound.
+        if min_dis_R <= lb:
+            break
+
     res = (min_dis_R/2, best_f, best_g) if return_fg else min_dis_R/2
 
     return res
```

### Comparing `dgh-0.0.5/dgh/fw.py` & `dgh-0.0.6/dgh/fw.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
 from functools import partial
 
-from mappings import fg_to_R
-from auxiliary import arrange_distances
+from .mappings import fg_to_R
+from .spaces import arrange_distances
 
 
 def solve_frank_wolfe(obj, grad, find_descent_direction, minimize_obj_wrt_gamma, S0,
                       tol=1e-8, max_iter=10, verbose=0):
     """
     Minimize smoothed distortion over the bi-mapping polytope 𝓢.
```

### Comparing `dgh-0.0.5/dgh/mappings.py` & `dgh-0.0.6/dgh/mappings.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import numpy as np
 
-from constants import DEFAULT_SEED
+from .constants import DEFAULT_SEED
 
 
 def rnd_S(n, m, rnd=None):
     """
     Generates random soft mapping in X🠖Y as a point in the bi-mapping polytope 𝓢.
 
     :param n: cardinality of X (int)
```

### Comparing `dgh-0.0.5/LICENSE` & `dgh-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `dgh-0.0.5/README.md` & `dgh-0.0.6/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,50 +1,52 @@
 # dGH
 
-Computes the Gromov–Hausdorff distance $$d_\text{GH}(X, Y) = \frac{1}{2}\inf_{f:X\to Y, g:Y\to X} \text{dis}\Big(\{(x, f(x)): x \in X\} \cup \{(g(y), y): y \in Y\}\Big),$$ where $\text{dis}(R) = \sup_{(x, y), (x', y') \in R} |d_X(x, x') - d_Y(y, y')|$ for $R \subseteq X \times Y,$ by solving (a parametric family of) indefinite quadratic minimizations with affine constraints, whose solutions are guaranteed to deliver $d_\text{GH}(X, Y)$ for sufficiently large value of the parameter $c$. The minimizations are solved using the Frank-Wolfe algorithm in $O(n^3)$ time per its iteration, where $n = |X| + |Y|$ is the total number of points. Even when the algorithm fails to find a global minimum, the resulting solution provides an upper bound for $d_\text{GH}(X, Y)$.
+Computes the Gromov–Hausdorff distance $$d_\text{GH}(X, Y) = \frac{1}{2}\inf_{f:X\to Y, g:Y\to X} \text{dis}\Big(\\{(x, f(x)): x \in X\\} \cup \\{(g(y), y): y \in Y\\}\Big),$$ where $\text{dis}(R) = \sup_{(x, y), (x', y') \in R} |d_X(x, x') - d_Y(y, y')|$ for $R \subseteq X \times Y,$ by solving (a parametric family of) indefinite quadratic minimizations with affine constraints, whose solutions are guaranteed to deliver $d_\text{GH}(X, Y)$ for sufficiently large value of the parameter $c$. The minimizations are solved using the Frank-Wolfe algorithm in $O(n^3)$ time per its iteration, where $n = |X| + |Y|$ is the total number of points. Even when the algorithm fails to find a global minimum, the resulting solution provides an upper bound for $d_\text{GH}(X, Y)$.
 
 A manuscript describing the underlying theory is currently in preparation.
 
 ## Quickstart
 
 Installing the package from Python Package Index:
 
 ```$ pip install dgh```
 
-Computing $d_\text{GH}(X, Y)$ where $X$ is the vertices of the regular unit 4-simplex and $Y$ is (a shortest path-based metric representation of) the star graph of order 6:
+Computing $d_\text{GH}(X, Y)$ where $X$ is the vertices of a regular 4-simplex of diameter $\frac{3}{2}$ and $Y$ is (a shortest path-based metric representation of) the star graph of order 6:
 
 ```
 import numpy as np
-import dgh
+from dgh import dgh
 
-# Set up distance matrices.
-X = np.array([[0, 1, 1, 1, 1],
-              [0, 0, 1, 1, 1],
-              [0, 0, 0, 1, 1],
-              [0, 0, 0, 0, 1],
+# Set distance matrix for the simplex.
+X = np.array([[0, 1.5, 1.5, 1.5, 1.5],
+              [0, 0, 1.5, 1.5, 1.5],
+              [0, 0, 0, 1.5, 1.5],
+              [0, 0, 0, 0, 1.5],
               [0, 0, 0, 0, 0]])
 X += X.T
+
+# Set distance matrix for the star graph.
 Y = np.array([[0, 1, 1, 1, 1, 1],
-              [0, 0, 0, 0, 0, 0],
-              [0, 0, 0, 0, 0, 0],
-              [0, 0, 0, 0, 0, 0],
-              [0, 0, 0, 0, 0, 0],
+              [0, 0, 2, 2, 2, 2],
+              [0, 0, 0, 2, 2, 2],
+              [0, 0, 0, 0, 2, 2],
+              [0, 0, 0, 0, 0, 2],
               [0, 0, 0, 0, 0, 0]])
 Y += Y.T
 
 # Find an upper bound of the Gromov–Hausdorff distance.
 dgh.ub(X, Y)
 ```
 
-Increasing the budget of Frank-Wolfe algorithm iterations, and thus the number of restarts, allocated for the search (the default budget is 100):
+Increasing the budget of Frank-Wolfe iterations, and thus the number of restarts, allocated for the search (the default budget is 100):
 
 ```d = dgh.ub(X, Y, iter_budget=1000)```
 
 Obtaining the mappings $f:X\to Y, g:Y\to X$ (as arrays s.t. $f_i = j \Leftrightarrow f(x_i) = y_j$) that deliver the found minimum:
 
 ```d, f, g = dgh.ub(X, Y, return_fg=True)```
 
 ## Contributing
 If you found a bug or want to suggest an enhancement, you can create a [GitHub Issue](https://docs.github.com/en/issues/tracking-your-work-with-issues/creating-an-issue). Alternatively, you can email vlad.oles (at) proton (dot) me.
 
 ## License
-dGH is released under the MIT license.
+dGH is released under the MIT license.
```

### Comparing `dgh-0.0.5/pyproject.toml` & `dgh-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "dgh"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   {name="Vladyslav Oles", email="vlad.oles@proton.me"},
 ]
 description = "Computing the Gromov–Hausdorff distance"
 readme = "README.md"
 requires-python = ">=3.5"
 classifiers = [
```

### Comparing `dgh-0.0.5/PKG-INFO` & `dgh-0.0.6/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,64 +1,66 @@
 Metadata-Version: 2.1
 Name: dgh
-Version: 0.0.5
+Version: 0.0.6
 Summary: Computing the Gromov–Hausdorff distance
 Project-URL: Homepage, https://github.com/pypa/dgh
 Project-URL: Bug Tracker, https://github.com/pypa/dgh/issues
 Author-email: Vladyslav Oles <vlad.oles@proton.me>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 
 # dGH
 
-Computes the Gromov–Hausdorff distance $$d_\text{GH}(X, Y) = \frac{1}{2}\inf_{f:X\to Y, g:Y\to X} \text{dis}\Big(\{(x, f(x)): x \in X\} \cup \{(g(y), y): y \in Y\}\Big),$$ where $\text{dis}(R) = \sup_{(x, y), (x', y') \in R} |d_X(x, x') - d_Y(y, y')|$ for $R \subseteq X \times Y,$ by solving (a parametric family of) indefinite quadratic minimizations with affine constraints, whose solutions are guaranteed to deliver $d_\text{GH}(X, Y)$ for sufficiently large value of the parameter $c$. The minimizations are solved using the Frank-Wolfe algorithm in $O(n^3)$ time per its iteration, where $n = |X| + |Y|$ is the total number of points. Even when the algorithm fails to find a global minimum, the resulting solution provides an upper bound for $d_\text{GH}(X, Y)$.
+Computes the Gromov–Hausdorff distance $$d_\text{GH}(X, Y) = \frac{1}{2}\inf_{f:X\to Y, g:Y\to X} \text{dis}\Big(\\{(x, f(x)): x \in X\\} \cup \\{(g(y), y): y \in Y\\}\Big),$$ where $\text{dis}(R) = \sup_{(x, y), (x', y') \in R} |d_X(x, x') - d_Y(y, y')|$ for $R \subseteq X \times Y,$ by solving (a parametric family of) indefinite quadratic minimizations with affine constraints, whose solutions are guaranteed to deliver $d_\text{GH}(X, Y)$ for sufficiently large value of the parameter $c$. The minimizations are solved using the Frank-Wolfe algorithm in $O(n^3)$ time per its iteration, where $n = |X| + |Y|$ is the total number of points. Even when the algorithm fails to find a global minimum, the resulting solution provides an upper bound for $d_\text{GH}(X, Y)$.
 
 A manuscript describing the underlying theory is currently in preparation.
 
 ## Quickstart
 
 Installing the package from Python Package Index:
 
 ```$ pip install dgh```
 
-Computing $d_\text{GH}(X, Y)$ where $X$ is the vertices of the regular unit 4-simplex and $Y$ is (a shortest path-based metric representation of) the star graph of order 6:
+Computing $d_\text{GH}(X, Y)$ where $X$ is the vertices of a regular 4-simplex of diameter $\frac{3}{2}$ and $Y$ is (a shortest path-based metric representation of) the star graph of order 6:
 
 ```
 import numpy as np
-import dgh
+from dgh import dgh
 
-# Set up distance matrices.
-X = np.array([[0, 1, 1, 1, 1],
-              [0, 0, 1, 1, 1],
-              [0, 0, 0, 1, 1],
-              [0, 0, 0, 0, 1],
+# Set distance matrix for the simplex.
+X = np.array([[0, 1.5, 1.5, 1.5, 1.5],
+              [0, 0, 1.5, 1.5, 1.5],
+              [0, 0, 0, 1.5, 1.5],
+              [0, 0, 0, 0, 1.5],
               [0, 0, 0, 0, 0]])
 X += X.T
+
+# Set distance matrix for the star graph.
 Y = np.array([[0, 1, 1, 1, 1, 1],
-              [0, 0, 0, 0, 0, 0],
-              [0, 0, 0, 0, 0, 0],
-              [0, 0, 0, 0, 0, 0],
-              [0, 0, 0, 0, 0, 0],
+              [0, 0, 2, 2, 2, 2],
+              [0, 0, 0, 2, 2, 2],
+              [0, 0, 0, 0, 2, 2],
+              [0, 0, 0, 0, 0, 2],
               [0, 0, 0, 0, 0, 0]])
 Y += Y.T
 
 # Find an upper bound of the Gromov–Hausdorff distance.
 dgh.ub(X, Y)
 ```
 
-Increasing the budget of Frank-Wolfe algorithm iterations, and thus the number of restarts, allocated for the search (the default budget is 100):
+Increasing the budget of Frank-Wolfe iterations, and thus the number of restarts, allocated for the search (the default budget is 100):
 
 ```d = dgh.ub(X, Y, iter_budget=1000)```
 
 Obtaining the mappings $f:X\to Y, g:Y\to X$ (as arrays s.t. $f_i = j \Leftrightarrow f(x_i) = y_j$) that deliver the found minimum:
 
 ```d, f, g = dgh.ub(X, Y, return_fg=True)```
 
 ## Contributing
 If you found a bug or want to suggest an enhancement, you can create a [GitHub Issue](https://docs.github.com/en/issues/tracking-your-work-with-issues/creating-an-issue). Alternatively, you can email vlad.oles (at) proton (dot) me.
 
 ## License
-dGH is released under the MIT license.
+dGH is released under the MIT license.
```

