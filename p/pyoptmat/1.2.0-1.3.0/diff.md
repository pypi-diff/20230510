# Comparing `tmp/pyoptmat-1.2.0.tar.gz` & `tmp/pyoptmat-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyoptmat-1.2.0.tar", last modified: Thu Apr  6 02:13:07 2023, max compression
+gzip compressed data, was "pyoptmat-1.3.0.tar", last modified: Wed May 10 19:50:08 2023, max compression
```

## Comparing `pyoptmat-1.2.0.tar` & `pyoptmat-1.3.0.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 02:13:07.667960 pyoptmat-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-04-06 02:13:03.000000 pyoptmat-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-04-06 02:13:07.667960 pyoptmat-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-04-06 02:13:03.000000 pyoptmat-1.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 02:13:07.663960 pyoptmat-1.2.0/pyoptmat/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 02:13:03.000000 pyoptmat-1.2.0/pyoptmat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14123 2023-04-06 02:13:03.000000 pyoptmat-1.2.0/pyoptmat/chunktime.py
--rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-04-06 02:13:03.000000 pyoptmat-1.2.0/pyoptmat/damage.py
--rw-r--r--   0 runner    (1001) docker     (123)    18369 2023-04-06 02:13:03.000000 pyoptmat-1.2.0/pyoptmat/experiments.py
--rw-r--r--   0 runner    (1001) docker     (123)    46061 2023-04-06 02:13:03.000000 pyoptmat-1.2.0/pyoptmat/flowrules.py
--rw-r--r--   0 runner    (1001) docker     (123)    35630 2023-04-06 02:13:03.000000 pyoptmat-1.2.0/pyoptmat/hardening.py
--rw-r--r--   0 runner    (1001) docker     (123)    17426 2023-04-06 02:13:03.000000 pyoptmat-1.2.0/pyoptmat/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-04-06 02:13:03.000000 pyoptmat-1.2.0/pyoptmat/neuralode.py
--rw-r--r--   0 runner    (1001) docker     (123)    21387 2023-04-06 02:13:03.000000 pyoptmat-1.2.0/pyoptmat/ode.py
--rw-r--r--   0 runner    (1001) docker     (123)    19718 2023-04-06 02:13:03.000000 pyoptmat-1.2.0/pyoptmat/optimize.py
--rw-r--r--   0 runner    (1001) docker     (123)     7089 2023-04-06 02:13:03.000000 pyoptmat-1.2.0/pyoptmat/scaling.py
--rw-r--r--   0 runner    (1001) docker     (123)    12202 2023-04-06 02:13:03.000000 pyoptmat-1.2.0/pyoptmat/solvers.py
--rw-r--r--   0 runner    (1001) docker     (123)    18011 2023-04-06 02:13:03.000000 pyoptmat-1.2.0/pyoptmat/temperature.py
--rw-r--r--   0 runner    (1001) docker     (123)    14860 2023-04-06 02:13:03.000000 pyoptmat-1.2.0/pyoptmat/utility.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 02:13:07.663960 pyoptmat-1.2.0/pyoptmat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-04-06 02:13:07.000000 pyoptmat-1.2.0/pyoptmat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-04-06 02:13:07.000000 pyoptmat-1.2.0/pyoptmat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 02:13:07.000000 pyoptmat-1.2.0/pyoptmat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-06 02:13:07.000000 pyoptmat-1.2.0/pyoptmat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-06 02:13:07.000000 pyoptmat-1.2.0/pyoptmat.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 02:13:07.000000 pyoptmat-1.2.0/pyoptmat.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-06 02:13:07.667960 pyoptmat-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-04-06 02:13:03.000000 pyoptmat-1.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 02:13:07.667960 pyoptmat-1.2.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)    13085 2023-04-06 02:13:03.000000 pyoptmat-1.2.0/test/test_adjoint_gradients.py
--rw-r--r--   0 runner    (1001) docker     (123)    35434 2023-04-06 02:13:03.000000 pyoptmat-1.2.0/test/test_batch_gradient.py
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-04-06 02:13:03.000000 pyoptmat-1.2.0/test/test_chunktime.py
--rw-r--r--   0 runner    (1001) docker     (123)     4866 2023-04-06 02:13:03.000000 pyoptmat-1.2.0/test/test_damage.py
--rw-r--r--   0 runner    (1001) docker     (123)    20725 2023-04-06 02:13:03.000000 pyoptmat-1.2.0/test/test_flowrules.py
--rw-r--r--   0 runner    (1001) docker     (123)    18620 2023-04-06 02:13:03.000000 pyoptmat-1.2.0/test/test_hardening.py
--rw-r--r--   0 runner    (1001) docker     (123)    13211 2023-04-06 02:13:03.000000 pyoptmat-1.2.0/test/test_model_gradient.py
--rw-r--r--   0 runner    (1001) docker     (123)    16944 2023-04-06 02:13:03.000000 pyoptmat-1.2.0/test/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     9162 2023-04-06 02:13:03.000000 pyoptmat-1.2.0/test/test_ode.py
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-04-06 02:13:03.000000 pyoptmat-1.2.0/test/test_scaling.py
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-04-06 02:13:03.000000 pyoptmat-1.2.0/test/test_solvers.py
--rw-r--r--   0 runner    (1001) docker     (123)    16483 2023-04-06 02:13:03.000000 pyoptmat-1.2.0/test/test_temperature_scaling.py
--rw-r--r--   0 runner    (1001) docker     (123)     7769 2023-04-06 02:13:03.000000 pyoptmat-1.2.0/test/test_utility.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 19:50:08.541592 pyoptmat-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-05-10 19:50:04.000000 pyoptmat-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-05-10 19:50:08.541592 pyoptmat-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-05-10 19:50:04.000000 pyoptmat-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 19:50:08.541592 pyoptmat-1.3.0/pyoptmat/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 19:50:04.000000 pyoptmat-1.3.0/pyoptmat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21760 2023-05-10 19:50:04.000000 pyoptmat-1.3.0/pyoptmat/chunktime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-05-10 19:50:04.000000 pyoptmat-1.3.0/pyoptmat/damage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18369 2023-05-10 19:50:04.000000 pyoptmat-1.3.0/pyoptmat/experiments.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46061 2023-05-10 19:50:04.000000 pyoptmat-1.3.0/pyoptmat/flowrules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35630 2023-05-10 19:50:04.000000 pyoptmat-1.3.0/pyoptmat/hardening.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15812 2023-05-10 19:50:04.000000 pyoptmat-1.3.0/pyoptmat/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-10 19:50:04.000000 pyoptmat-1.3.0/pyoptmat/neuralode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24843 2023-05-10 19:50:04.000000 pyoptmat-1.3.0/pyoptmat/ode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19718 2023-05-10 19:50:04.000000 pyoptmat-1.3.0/pyoptmat/optimize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7089 2023-05-10 19:50:04.000000 pyoptmat-1.3.0/pyoptmat/scaling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12202 2023-05-10 19:50:04.000000 pyoptmat-1.3.0/pyoptmat/solvers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18011 2023-05-10 19:50:04.000000 pyoptmat-1.3.0/pyoptmat/temperature.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14860 2023-05-10 19:50:04.000000 pyoptmat-1.3.0/pyoptmat/utility.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 19:50:08.541592 pyoptmat-1.3.0/pyoptmat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-05-10 19:50:08.000000 pyoptmat-1.3.0/pyoptmat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-05-10 19:50:08.000000 pyoptmat-1.3.0/pyoptmat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 19:50:08.000000 pyoptmat-1.3.0/pyoptmat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-10 19:50:08.000000 pyoptmat-1.3.0/pyoptmat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-10 19:50:08.000000 pyoptmat-1.3.0/pyoptmat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 19:50:08.000000 pyoptmat-1.3.0/pyoptmat.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-10 19:50:08.541592 pyoptmat-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-05-10 19:50:04.000000 pyoptmat-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 19:50:08.541592 pyoptmat-1.3.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)    13085 2023-05-10 19:50:04.000000 pyoptmat-1.3.0/test/test_adjoint_gradients.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35434 2023-05-10 19:50:04.000000 pyoptmat-1.3.0/test/test_batch_gradient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-05-10 19:50:04.000000 pyoptmat-1.3.0/test/test_chunktime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4866 2023-05-10 19:50:04.000000 pyoptmat-1.3.0/test/test_damage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20725 2023-05-10 19:50:04.000000 pyoptmat-1.3.0/test/test_flowrules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18620 2023-05-10 19:50:04.000000 pyoptmat-1.3.0/test/test_hardening.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13211 2023-05-10 19:50:04.000000 pyoptmat-1.3.0/test/test_model_gradient.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16944 2023-05-10 19:50:04.000000 pyoptmat-1.3.0/test/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9162 2023-05-10 19:50:04.000000 pyoptmat-1.3.0/test/test_ode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-05-10 19:50:04.000000 pyoptmat-1.3.0/test/test_scaling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-05-10 19:50:04.000000 pyoptmat-1.3.0/test/test_solvers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16483 2023-05-10 19:50:04.000000 pyoptmat-1.3.0/test/test_temperature_scaling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7769 2023-05-10 19:50:04.000000 pyoptmat-1.3.0/test/test_utility.py
```

### Comparing `pyoptmat-1.2.0/LICENSE` & `pyoptmat-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyoptmat-1.2.0/PKG-INFO` & `pyoptmat-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyoptmat
-Version: 1.2.0
+Version: 1.3.0
 Summary: Statistical inference for material models
 Home-page: https://github.com/Argonne-National-Laboratory/pyoptmat
 Author: Argonne National Laboratory
 Author-email: messner@anl.gov
 License: UNKNOWN
 Keywords: materials inference modeling
 Platform: UNKNOWN
```

### Comparing `pyoptmat-1.2.0/README.md` & `pyoptmat-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `pyoptmat-1.2.0/pyoptmat/chunktime.py` & `pyoptmat-1.3.0/pyoptmat/chunktime.py`

 * *Files 21% similar despite different names*

```diff
@@ -6,19 +6,22 @@
     These include:
         1. Sparse matrix classes for banded systems
         2. General sparse matrix classes
         3. Specialized solver routines working with banded systems
 """
 
 import warnings
+from math import prod, log2, floor
 
 import torch
-import torch.jit
+from torch.nn.functional import pad
 import numpy as np
 
+from pyoptmat.utility import mbmm
+
 
 def newton_raphson_chunk(fn, x0, solver, rtol=1e-6, atol=1e-10, miter=100):
     """
     Solve a nonlinear system with Newton's method with a tensor for a
     BackwardEuler type chunking operator context manager.
 
     Args:
@@ -116,63 +119,299 @@
     def shape(self):
         """
         Logical shape of the dense array
         """
         return (self.sbat, self.n, self.n)
 
 
-class BidiagonalThomasFactorization(BidiagonalOperator):
-    """
-    Manages the data needed to solve our bidiagonal system via Thomas
-    factorization
+class LUFactorization(BidiagonalOperator):
+    """A factorization that uses the LU decomposition of A
 
     Args:
         A (torch.tensor): tensor of shape (nblk,sbat,sblk,sblk) with the main diagonal
         B (torch.tensor): tensor of shape (nblk-1,sbat,sblk,sblk) with the off diagonal
     """
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
         self._setup_factorization()
 
+    def _setup_factorization(self):
+        """
+        Form the factorization...
+
+        Args:
+            diag (torch.tensor): diagonal blocks of shape (nblk, sbat, sblk, sblk)
+        """
+        self.lu, self.pivots, _ = torch.linalg.lu_factor_ex(self.A)
+
+
+def thomas_solve(lu, pivots, B, v):
+    """Simple function implementing a Thomas solve
+
+    Solves in place of v
+
+    Args:
+        lu (torch.tensor): factorized diagonal blocks, (nblk,sbat,sblk,sblk)
+        pivots (torch.tensor): pivots for factorization
+        B (torch.tensor): lower diagonal blocks (nblk-1,sbat,sblk,sblk)
+        v (torch.tensor): right hand side (nblk,sbat,sblk)
+    """
+    i = 0
+    v[i] = torch.linalg.lu_solve(lu[i], pivots[i], v[i])
+    for i in range(1, lu.shape[0]):
+        v[i] = torch.linalg.lu_solve(
+            lu[i], pivots[i], v[i] - torch.bmm(B[i - 1], v[i - 1].clone())
+        )
+
+    return v
+
+
+class BidiagonalThomasFactorization(LUFactorization):
+    """
+    Manages the data needed to solve our bidiagonal system via Thomas
+    factorization
+
+    Args:
+        A (torch.tensor): tensor of shape (nblk,sbat,sblk,sblk) with the main diagonal
+        B (torch.tensor): tensor of shape (nblk-1,sbat,sblk,sblk) with the off diagonal
+    """
+
     def forward(self, v):
         """
         Complete the backsolve for a given right hand side
 
         Args:
             v (torch.tensor): tensor of shape (sbat, sblk*nblk)
         """
-        y = torch.empty_like(v)
-        i = 0
-        s = self.sblk
-        y[:, i * s : (i + 1) * s] = torch.linalg.lu_solve(
-            self.lu[i], self.pivots[i], v[:, i * s : (i + 1) * s].unsqueeze(-1)
-        ).squeeze(-1)
-        # The .clone() here really makes no sense to me, but torch assures me it is necessary
-        for i in range(1, self.nblk):
-            y[:, i * s : (i + 1) * s] = torch.linalg.lu_solve(
-                self.lu[i],
-                self.pivots[i],
-                v[:, i * s : (i + 1) * s].unsqueeze(-1)
-                - torch.bmm(
-                    self.B[i - 1], y[:, (i - 1) * s : i * s].clone().unsqueeze(-1)
-                ),
-            ).squeeze(-1)
+        v = v.reshape((self.sbat, self.nblk, self.sblk)).transpose(0, 1).unsqueeze(-1)
+        v = thomas_solve(self.lu, self.pivots, self.B, v)
 
-        return y
+        return v.squeeze(-1).transpose(0, 1).flatten(start_dim=1)
 
-    def _setup_factorization(self):
+
+class BidiagonalPCRFactorization(LUFactorization):
+    """
+    Manages the data needed to solve our bidiagonal system via parallel cyclic reduction
+
+    Args:
+        A (torch.tensor): tensor of shape (nblk,sbat,sblk,sblk) with the main diagonal
+        B (torch.tensor): tensor of shape (nblk-1,sbat,sblk,sblk) with the off diagonal
+    """
+
+    def forward(self, v):
         """
-        Form the factorization...
+        Complete the backsolve for a given right hand side
 
         Args:
-            diag (torch.tensor): diagonal blocks of shape (nblk, sbat, sblk, sblk)
+            v (torch.tensor): tensor of shape (sbat, sblk*nblk)
         """
-        self.lu, self.pivots, _ = torch.linalg.lu_factor_ex(self.A)
+        # Reshape and add dimensions
+        # This puts the input into "blocked form"
+        # contiguous is necessary because my _cyclic_shift function assumes initially
+        # contiguous memory
+        v = (
+            v.reshape((self.sbat, self.nblk, self.sblk))
+            .transpose(0, 1)
+            .unsqueeze(-1)
+            .contiguous()
+        )
+
+        # We could do this in place if it wasn't for the pad
+        self.B = pad(self.B, (0, 0, 0, 0, 0, 0, 1, 0))
+
+        # Now figure out how many powers of 2 we need to complete our matrix
+        for s, e in zip(*self._pow2(self.nblk)):
+            self.B[s + 1 : e], v[s + 1 : e] = self._solve_block(
+                self.lu[s:e], self.pivots[s:e], self.B[s:e], v[s:e]
+            )
+
+        # To retain consistent sizes
+        self.B = self.B[1:]
+
+        return (
+            torch.linalg.lu_solve(self.lu, self.pivots, v)
+            .squeeze(-1)
+            .transpose(0, 1)
+            .flatten(start_dim=1)
+        )
+
+    def _solve_block(self, lu, pivots, B, v):
+        """Solve a subsection of the matrix via PCR
+
+        Args:
+            lu (torch.tensor): (ncurr,sbat,sblk,sblk)
+            pivots (torch.tensor): (ncurr,sbat,sblk)
+            B (torch.tensor): (ncurr,sbat,sblk,sblk)
+            v (torch.tensor): (ncurr,sbat,sblk,1)
+        """
+        # Number of iterations required to reduce this block
+        niter = lu.shape[0].bit_length() - 1
+
+        # Add the extra working dimension to the start of everything
+        lu = lu.unsqueeze(0)
+        pivots = pivots.unsqueeze(0)
+        B = B.unsqueeze(0)
+        v = v.unsqueeze(0)
+
+        # Actually start reduction!
+        for i in range(niter):
+            # Reduce RHS
+            v[:, 1:] -= mbmm(
+                B[:, 1:], torch.linalg.lu_solve(lu[:, :-1], pivots[:, :-1], v[:, :-1])
+            )
+
+            # Reduce off diagonal coefficients
+            B[:, 2:] = -mbmm(
+                B[:, 2:],
+                torch.linalg.lu_solve(lu[:, 1:-1], pivots[:, 1:-1], B[:, 1:-1]),
+            )
+
+            # Shuffle dimensions
+            v = self._cyclic_shift(v, i)
+            B = self._cyclic_shift(B, i)
+            lu = self._cyclic_shift(lu, i)
+            pivots = self._cyclic_shift(pivots, i)
+
+        return B.squeeze(1)[1:], v.squeeze(1)[1:]
+
+    @staticmethod
+    def _pow2(n):
+        """Calculate submatrix sizes
+
+        Args:
+            n (int): number of blocks
+
+        Returns:
+            two lists, one giving start block indices and the
+            second giving end block indices.
+
+        The first (start,end) pair is the largest power of 2 that fits in
+        n.  Subsequent pairs are the largest power of 2 that fit in the remainder
+        *with one overlap between the next increment and the previous*.
+        """
+
+        def sz(n):
+            return 2 ** floor(log2(n))
+
+        start = [0]
+        end = [sz(n)]
+        n -= end[-1]
+
+        while n > 0:
+            cz = sz(n + 1)
+            start.append(end[-1] - 1)
+            end.append(start[-1] + cz)
+            n -= cz - 1
+
+        return start, end
+
+    @staticmethod
+    def _cyclic_shift(A, n):
+        """Provide a view of the input with a cyclic shift applied
+
+        Args:
+            A (torch.tensor): input tensor
+            n (int): number of cyclic shifts
+        """
+        return A.as_strided(
+            (A.shape[0] * 2, A.shape[1] // 2) + A.shape[2:],
+            (prod(A.shape[2:]), 2 ** (n + 1) * prod(A.shape[2:])) + A.stride()[2:],
+        )
+
+
+class BidiagonalHybridFactorization(BidiagonalPCRFactorization):
+    """A factorization approach that switches from PCR to Thomas
+
+    Specifically, this class uses PCR until the PCR chunk size is
+    smaller than user provided minimum chunk size.  Then it switches
+    to Thomas.
+
+    Args:
+        A (torch.tensor): tensor of shape (nblk,sbat,sblk,sblk) with the main diagonal
+        B (torch.tensor): tensor of shape (nblk-1,sbat,sblk,sblk) with the off diagonal
+
+    Keyword Args:
+        min_size (int): minimum block size, default is zero
+    """
+
+    def __init__(self, *args, min_size=0, **kwargs):
+        super().__init__(*args, **kwargs)
+
+        # I use < below...
+        self.min_size = min_size + 1
+
+    def forward(self, v):
+        """
+        Complete the backsolve for a given right hand side
+
+        Args:
+            v (torch.tensor): tensor of shape (sbat, sblk*nblk)
+        """
+        # Reshape and add dimensions
+        # This puts the input into "blocked form"
+        # contiguous is necessary because my _cyclic_shift function assumes initially
+        # contiguous memory
+        v = (
+            v.reshape((self.sbat, self.nblk, self.sblk))
+            .transpose(0, 1)
+            .unsqueeze(-1)
+            .contiguous()
+        )
+
+        # We could do this in place if it wasn't for the pad
+        self.B = pad(self.B, (0, 0, 0, 0, 0, 0, 1, 0))
+
+        # Get the PCR blocks to actually use
+        start, end, last = self._pcr_blocks()
+
+        # Do PCR
+        for s, e in zip(start, end):
+            self.B[s + 1 : e], v[s + 1 : e] = self._solve_block(
+                self.lu[s:e], self.pivots[s:e], self.B[s:e], v[s:e]
+            )
+
+        # To retain consistent sizes
+        self.B = self.B[1:]
+
+        # We still need to solve the first block even if last is 0
+
+        # The actual LU solve for the solution
+        v[:last] = torch.linalg.lu_solve(self.lu[:last], self.pivots[:last], v[:last])
+
+        # Now take over for Thomas
+        for i in range(last, self.nblk):
+            v[i] = torch.linalg.lu_solve(
+                self.lu[i],
+                self.pivots[i],
+                v[i] - torch.bmm(self.B[i - 1], v[i - 1].clone()),
+            )
+
+        return v.squeeze(-1).transpose(0, 1).flatten(start_dim=1)
+
+    def _pcr_blocks(self):
+        """Figure out the PCR blocks we are actually going to use"""
+        # Figure out which blocks we're going to use
+        start, end = self._pow2(self.nblk)
+        # These are sorted...
+        blk_size = [e - s for e, s in zip(end, start)]
+        if blk_size[0] < self.min_size:
+            return [], [], 1
+
+        ilast = [i for i, j in enumerate(blk_size) if j < self.min_size]
+        if len(ilast) == 0:
+            ilast = len(start)
+        else:
+            ilast = ilast[0]
+
+        start = start[:ilast]
+        end = end[:ilast]
+
+        return start, end, end[-1]
 
 
 class BidiagonalForwardOperator(BidiagonalOperator):
     """
     A batched block banded matrix of the form:
 
     .. math::
@@ -197,14 +436,18 @@
     Args:
         A (torch.tensor): tensor of shape (nblk,sbat,sblk,sblk)
             storing the nblk diagonal blocks
         B (torch.tensor): tensor of shape (nblk-1,sbat,sblk,sblk)
             storing the nblk-1 off diagonal blocks
     """
 
+    def __init__(self, *args, inverse_operator=BidiagonalThomasFactorization, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.inverse_operator = inverse_operator
+
     def to_diag(self):
         """
         Convert to a SquareBatchedBlockDiagonalMatrix, for testing
         or legacy purposes
         """
         return SquareBatchedBlockDiagonalMatrix([self.A, self.B], [0, -1])
 
@@ -236,15 +479,15 @@
             .flatten(start_dim=1)
         )
 
     def inverse(self):
         """
         Return an inverse operator
         """
-        return BidiagonalThomasFactorization(self.A, self.B)
+        return self.inverse_operator(self.A, self.B)
 
 
 class ChunkTimeOperatorSolverContext:
     """
     Context manager for solving sparse chunked time systems
 
     Args:
```

### Comparing `pyoptmat-1.2.0/pyoptmat/damage.py` & `pyoptmat-1.3.0/pyoptmat/damage.py`

 * *Files identical despite different names*

### Comparing `pyoptmat-1.2.0/pyoptmat/experiments.py` & `pyoptmat-1.3.0/pyoptmat/experiments.py`

 * *Files identical despite different names*

### Comparing `pyoptmat-1.2.0/pyoptmat/flowrules.py` & `pyoptmat-1.3.0/pyoptmat/flowrules.py`

 * *Files identical despite different names*

### Comparing `pyoptmat-1.2.0/pyoptmat/hardening.py` & `pyoptmat-1.3.0/pyoptmat/hardening.py`

 * *Files identical despite different names*

### Comparing `pyoptmat-1.2.0/pyoptmat/models.py` & `pyoptmat-1.3.0/pyoptmat/models.py`

 * *Files 10% similar despite different names*

```diff
@@ -157,51 +157,26 @@
     This class provides infrastructure for integrating constitutive models in
     either strain or stress control.
 
     Args:
       model:                        base strain-controlled model
       method (optional):            integrate method used to solve the equations, defaults
                                     to `"backward-euler"`
-      rtol (optional):              relative tolerance for implicit integration
-      atol (optional):              absolute tolerance for implicit integration
-      miter (optional):             maximum nonlinear iterations for implicit time integration
       d0 (optional):                intitial value of damage
       use_adjoint (optional):       if `True` use the adjoint approach to
-                                    calculate sensitivities, if `False` use
-                                    pytorch automatic differentiation
-      extra_params (optional):      additional, external parameter to include
-                                    in the adjoint calculation.  Used if not
-                                    all the parameters can be determined by
-                                    introspection
+      **kwargs:                     passed on to the odeint method
+
     """
 
-    def __init__(
-        self,
-        model,
-        *args,
-        method="backward-euler",
-        block_size=1,
-        rtol=1.0e-6,
-        atol=1.0e-4,
-        miter=100,
-        d0=0,
-        use_adjoint=True,
-        extra_params=None,
-        **kwargs
-    ):
-        super().__init__(*args, **kwargs)
+    def __init__(self, model, *args, d0=0, use_adjoint=True, **kwargs):
+        super().__init__(*args)
         self.model = model
-        self.method = method
-        self.block_size = block_size
-        self.rtol = rtol
-        self.atol = atol
-        self.miter = miter
         self.d0 = d0
         self.use_adjoint = use_adjoint
-        self.extra_params = extra_params
+        self.kwargs_for_integration = kwargs
 
         if self.use_adjoint:
             self.imethod = ode.odeint_adjoint
         else:
             self.imethod = ode.odeint
 
     def solve_both(self, times, temperatures, idata, control):
@@ -238,25 +213,15 @@
             self.model,
             rate_interpolator,
             base_interpolator,
             temperature_interpolator,
             control,
         )
 
-        return self.imethod(
-            bmodel,
-            init,
-            times,
-            block_size=self.block_size,
-            method=self.method,
-            rtol=self.rtol,
-            atol=self.atol,
-            miter=self.miter,
-            extra_params=self.extra_params,
-        )
+        return self.imethod(bmodel, init, times, **self.kwargs_for_integration)
 
     def solve_strain(self, times, strains, temperatures):
         """
         Basic model definition: take time and strain rate and return stress
 
         Args:
           times:          input times, shape (ntime)
@@ -288,25 +253,15 @@
         )
         init[:, -1] = self.d0
 
         emodel = StrainBasedModel(
             self.model, erate_interpolator, temperature_interpolator
         )
 
-        return self.imethod(
-            emodel,
-            init,
-            times,
-            block_size=self.block_size,
-            method=self.method,
-            rtol=self.rtol,
-            atol=self.atol,
-            miter=self.miter,
-            extra_params=self.extra_params,
-        )
+        return self.imethod(emodel, init, times, **self.kwargs_for_integration)
 
     def solve_stress(self, times, stresses, temperatures):
         """
         Inverse model definition: take time and stress rate and return strain
 
         Args:
           times:          input times, shape (ntime,)
@@ -344,25 +299,15 @@
         smodel = StressBasedModel(
             self.model,
             stress_rate_interpolator,
             stress_interpolator,
             temperature_interpolator,
         )
 
-        return self.imethod(
-            smodel,
-            init,
-            times,
-            block_size=self.block_size,
-            method=self.method,
-            rtol=self.rtol,
-            atol=self.atol,
-            miter=self.miter,
-            extra_params=self.extra_params,
-        )
+        return self.imethod(smodel, init, times, **self.kwargs_for_integration)
 
     def forward(self, t, y):
         """
         Evaluate both strain and stress control and paste into the right
         locations.
 
         Args:
```

### Comparing `pyoptmat-1.2.0/pyoptmat/neuralode.py` & `pyoptmat-1.3.0/pyoptmat/neuralode.py`

 * *Files identical despite different names*

### Comparing `pyoptmat-1.2.0/pyoptmat/ode.py` & `pyoptmat-1.3.0/pyoptmat/ode.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# pylint: disable=too-many-arguments
+
 """
     Module defining the key objects and functions to integrate ODEs
     and provide the sensitivity of the results with respect to the
     model parameters either through backpropogation AD or the adjoint method.
 
     The key functions are :py:func:`pyoptmat.odeint` and
     :py:func:`pyoptmat.odeint_adjoint`.  These functions both
@@ -41,25 +43,30 @@
 
 
 class BackwardEulerScheme:
     """
     Integration with the backward Euler method
     """
 
-    def form_operators(self, dy, yd, yJ, dt):
+    def form_operators(
+        self, dy, yd, yJ, dt, solver=chunktime.BidiagonalThomasFactorization
+    ):
         """
         Form the residual and sparse Jacobian of the batched system
 
         Args:
             dy (torch.tensor): (ntime+1, nbatch, nsize) tensor with the increments in y
             yd (torch.tensor): (ntime, nbatch, nsize) tensor giving the ODE rate
             yJ (torch.tensor): (ntime, nbatch, nsize, nsize) tensor giving the derivative
                 of the ODE
             dt (torch.tensor): (ntime, nbatch) tensor giving the time step
 
+        Keyword Args:
+            solver (chunktime.BidiagonalOperator): inverse method
+
         Returns:
             R (torch.tensor): residual tensor of shape
                 (nbatch, ntime * nsize)
             J (tensor.tensor): sparse Jacobian tensor of logical
                 size (nbatch, ntime*nsize, ntime*nsize)
         """
         # Basic shape info
@@ -77,15 +84,15 @@
         )
 
         # Form the overall jacobian
         # This has I-J blocks on the main block diagonal and -I on the -1 block diagonal
         I = torch.eye(prob_size, device=dt.device).expand(ntime, batch_size, -1, -1)
 
         return R, chunktime.BidiagonalForwardOperator(
-            I - yJ[1:] * dt.unsqueeze(-1).unsqueeze(-1), -I[1:]
+            I - yJ[1:] * dt.unsqueeze(-1).unsqueeze(-1), -I[1:], inverse_operator=solver
         )
 
     def update_adjoint(self, dt, J, a_prev, grads):
         """
         Update the adjoint for a block of time
 
         Args:
@@ -141,25 +148,30 @@
 
 
 class ForwardEulerScheme:
     """
     Integration with the forward Euler method
     """
 
-    def form_operators(self, dy, yd, yJ, dt):
+    def form_operators(
+        self, dy, yd, yJ, dt, solver=chunktime.BidiagonalThomasFactorization
+    ):
         """
         Form the residual and sparse Jacobian of the batched system
 
         Args:
             dy (torch.tensor): (ntime+1, nbatch, nsize) tensor with the increments in y
             yd (torch.tensor): (ntime, nbatch, nsize) tensor giving the ODE rate
             yJ (torch.tensor): (ntime, nbatch, nsize, nsize) tensor giving the derivative
                 of the ODE
             dt (torch.tensor): (ntime, nbatch) tensor giving the time step
 
+        Keyword Args:
+            solver (chunktime.BidiagonalOperator): inverse method
+
         Returns:
             R (torch.tensor): residual tensor of shape
                 (nbatch, ntime * nsize)
             J (tensor.tensor): sparse Jacobian tensor of logical size
                 (nbatch, ntime*nsize, ntime*nsize)
         """
         # Basic shape info
@@ -177,15 +189,17 @@
         )
 
         # Form the overall jacobian
         # This has I on the diagonal and -I - J*dt on the off diagonal
         I = torch.eye(prob_size, device=dt.device).expand(ntime, batch_size, -1, -1)
 
         return R, chunktime.BidiagonalForwardOperator(
-            I, -I[1:] - yJ[1:-1] * dt[1:].unsqueeze(-1).unsqueeze(-1)
+            I,
+            -I[1:] - yJ[1:-1] * dt[1:].unsqueeze(-1).unsqueeze(-1),
+            inverse_operator=solver,
         )
 
     def update_adjoint(self, dt, J, a_prev, grads):
         """
         Update the adjoint for a block of time
 
         Args:
@@ -243,30 +257,35 @@
     Keyword Args:
         scheme (TimeIntegrationScheme):  time integration scheme, default is
             backward euler
         block_size (int): target block size
         rtol (float): relative tolerance for Newton's method
         atol (float): absolute tolerance for Newton's method
         miter (int): maximum number of Newton iterations
-        sparse_linear_solver (str): method to solve batched sparse Ax = b, options
+        linear_solve_method (str): method to solve batched sparse Ax = b, options
             are currently "direct" or "dense"
+        direct_solve_method (str): method to use for the direct solver, options are
+            currently "thomas", "pcr", or "hybrid"
+        direct_solve_min_size (int): minimum PCR block size for the hybrid approach
         adjoint_params: parameters to track for the adjoint backward pass
         guess_type (string): strategy for initial guess, options are "zero" and "previous"
     """
 
     def __init__(
         self,
         func,
         y0,
         scheme=BackwardEulerScheme(),
         block_size=1,
         rtol=1.0e-6,
         atol=1.0e-4,
         miter=100,
         linear_solve_method="direct",
+        direct_solve_method="thomas",
+        direct_solve_min_size=0,
         adjoint_params=None,
         guess_type="zero",
         **kwargs,
     ):
         # Store basic info about the system
         self.func = func
         self.y0 = y0
@@ -288,14 +307,28 @@
         self.adjoint_params = adjoint_params
 
         # Setup the linear solver context
         self.linear_solve_context = chunktime.ChunkTimeOperatorSolverContext(
             linear_solve_method, **kwargs
         )
 
+        # Setup the direct solver type
+        if direct_solve_method == "thomas":
+            self.direct_solver = chunktime.BidiagonalThomasFactorization
+        elif direct_solve_method == "pcr":
+            self.direct_solver = chunktime.BidiagonalPCRFactorization
+        elif direct_solve_method == "hybrid":
+            self.direct_solver = lambda A, B: chunktime.BidiagonalHybridFactorization(
+                A, B, min_size=direct_solve_min_size
+            )
+        else:
+            raise ValueError(
+                f"Unknown batched bidiagonal solver method {direct_solve_method}!"
+            )
+
         # Initial guess for integration
         self.guess_type = guess_type
 
         # Cached solutions
         self.t = None
         self.result = None
 
@@ -440,15 +473,15 @@
             # Calculate the time steps
             times = torch.vstack((t_start.unsqueeze(0), t))
             dt = times.diff(dim=0)
 
             # Batch update the rate and jacobian
             yd, yJ = func(times, y)
 
-            return self.scheme.form_operators(dy, yd, yJ, dt)
+            return self.scheme.form_operators(dy, yd, yJ, dt, solver=self.direct_solver)
 
         dy = chunktime.newton_raphson_chunk(
             RJ,
             y_guess,
             self.linear_solve_context,
             rtol=self.rtol,
             atol=self.atol,
@@ -480,26 +513,39 @@
     Input variables and initial condition have shape :code:`(nbatch, nvar)`
 
     Input times have shape :code:`(ntime, nbatch)`
 
     Output history has shape :code:`(ntime, nbatch, nvar)`
 
     Args:
-      func (function):      returns tensor defining the derivative y_dot and,
-                            optionally, the jacobian as a second return value
-      y0 (torch.tensor):    initial conditions
-      times (torch.tensor): time locations to provide solutions at
+        func (function):        returns tensor defining the derivative y_dot and,
+                                optionally, the jacobian as a second return value
+        y0 (torch.tensor):      initial conditions
+        times (torch.tensor):   time locations to provide solutions at
 
     Keyword Args:
-      method (string):                      integration method, currently `"backward-euler"` or
+        method (string):                    integration method, currently `"backward-euler"` or
                                             `"forward-euler"`
-      extra-params (list of parameters):    not used here, just maintains compatibility with
-                                            the adjoint interface
-      kwargs:                               keyword arguments passed on to specific
-                                            solver methods
+        extra_params (list of parameters):  additional parameters that need to be included
+                                            in the backward pass that are not determinable
+                                            via introsection of :code:`func`
+        scheme (TimeIntegrationScheme):     time integration scheme, default is
+                                            `BackwardEulerScheme`
+        block_size (int):                   target block size
+        rtol (float):                       relative tolerance for Newton's method
+        atol (float):                       absolute tolerance for Newton's method
+        miter (int):                        maximum number of Newton iterations
+        linear_solve_method (str):          method to solve batched sparse Ax = b, options
+                                            are currently "direct" or "dense"
+        direct_solve_method (str):          method to use for the direct solver, options are
+                                            currently "thomas", "pcr", or "hybrid"
+        direct_solve_min_size (int):        minimum PCR block size for the hybrid approach
+        adjoint_params:                     parameters to track for the adjoint backward pass
+        guess_type (string):                strategy for initial guess, options are "zero"
+                                            and "previous"
     """
     solver = FixedGridBlockSolver(func, y0, scheme=int_methods[method], **kwargs)
 
     return solver.integrate(times)
 
 
 class IntegrateWithAdjoint(torch.autograd.Function):
@@ -551,27 +597,39 @@
     Input variables and initial condition have shape :code:`(nbatch, nvar)`
 
     Input times have shape :code:`(ntime, nbatch)`
 
     Output history has shape :code:`(ntime, nbatch, nvar)`
 
     Args:
-      func (function):      returns tensor defining the derivative y_dot and,
-                            optionally, the jacobian as a second return value
-      y0 (torch.tensor):    initial conditions
-      times (torch.tensor): time locations to provide solutions at
+        func (function):        returns tensor defining the derivative y_dot and,
+                                optionally, the jacobian as a second return value
+        y0 (torch.tensor):      initial conditions
+        times (torch.tensor):   time locations to provide solutions at
 
     Keyword Args:
-      method (string):                      integration method, currently `"backward-euler"` or
+        method (string):                    integration method, currently `"backward-euler"` or
                                             `"forward-euler"`
-      extra-params (list of parameters):    additional parameters that need to be included
+        extra_params (list of parameters):  additional parameters that need to be included
                                             in the backward pass that are not determinable
                                             via introsection of :code:`func`
-      kwargs:                               keyword arguments passed on to specific
-                                            solver methods
+        scheme (TimeIntegrationScheme):     time integration scheme, default is
+                                            `BackwardEulerScheme`
+        block_size (int):                   target block size
+        rtol (float):                       relative tolerance for Newton's method
+        atol (float):                       absolute tolerance for Newton's method
+        miter (int):                        maximum number of Newton iterations
+        linear_solve_method (str):          method to solve batched sparse Ax = b, options
+                                            are currently "direct" or "dense"
+        direct_solve_method (str):          method to use for the direct solver, options are
+                                            currently "thomas", "pcr", or "hybrid"
+        direct_solve_min_size (int):        minimum PCR block size for the hybrid approach
+        adjoint_params:                     parameters to track for the adjoint backward pass
+        guess_type (string):                strategy for initial guess, options are "zero"
+                                            and "previous"
     """
     # Grab parameters for backward
     if extra_params is None:
         extra_params = []
     adjoint_params = tuple(p for p in func.parameters()) + tuple(extra_params)
 
     solver = FixedGridBlockSolver(
```

### Comparing `pyoptmat-1.2.0/pyoptmat/optimize.py` & `pyoptmat-1.3.0/pyoptmat/optimize.py`

 * *Files identical despite different names*

### Comparing `pyoptmat-1.2.0/pyoptmat/scaling.py` & `pyoptmat-1.3.0/pyoptmat/scaling.py`

 * *Files identical despite different names*

### Comparing `pyoptmat-1.2.0/pyoptmat/solvers.py` & `pyoptmat-1.3.0/pyoptmat/solvers.py`

 * *Files identical despite different names*

### Comparing `pyoptmat-1.2.0/pyoptmat/temperature.py` & `pyoptmat-1.3.0/pyoptmat/temperature.py`

 * *Files identical despite different names*

### Comparing `pyoptmat-1.2.0/pyoptmat/utility.py` & `pyoptmat-1.3.0/pyoptmat/utility.py`

 * *Files identical despite different names*

### Comparing `pyoptmat-1.2.0/pyoptmat.egg-info/PKG-INFO` & `pyoptmat-1.3.0/pyoptmat.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyoptmat
-Version: 1.2.0
+Version: 1.3.0
 Summary: Statistical inference for material models
 Home-page: https://github.com/Argonne-National-Laboratory/pyoptmat
 Author: Argonne National Laboratory
 Author-email: messner@anl.gov
 License: UNKNOWN
 Keywords: materials inference modeling
 Platform: UNKNOWN
```

### Comparing `pyoptmat-1.2.0/pyoptmat.egg-info/SOURCES.txt` & `pyoptmat-1.3.0/pyoptmat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyoptmat-1.2.0/setup.py` & `pyoptmat-1.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 with open(os.path.join(this_directory, 'README.md'), encoding = 'utf-8') as f:
   long_description = f.read()
 
 setup (
     # Name of the project
     name = 'pyoptmat',
     # Version
-    version = '1.2.0',
+    version = '1.3.0',
     # One line-description
     description = "Statistical inference for material models",
     # README
     long_description = long_description,
     long_description_content_type = 'text/markdown',
     # Project webpage
     url='https://github.com/Argonne-National-Laboratory/pyoptmat',
```

### Comparing `pyoptmat-1.2.0/test/test_adjoint_gradients.py` & `pyoptmat-1.3.0/test/test_adjoint_gradients.py`

 * *Files identical despite different names*

### Comparing `pyoptmat-1.2.0/test/test_batch_gradient.py` & `pyoptmat-1.3.0/test/test_batch_gradient.py`

 * *Files identical despite different names*

### Comparing `pyoptmat-1.2.0/test/test_damage.py` & `pyoptmat-1.3.0/test/test_damage.py`

 * *Files identical despite different names*

### Comparing `pyoptmat-1.2.0/test/test_flowrules.py` & `pyoptmat-1.3.0/test/test_flowrules.py`

 * *Files identical despite different names*

### Comparing `pyoptmat-1.2.0/test/test_hardening.py` & `pyoptmat-1.3.0/test/test_hardening.py`

 * *Files identical despite different names*

### Comparing `pyoptmat-1.2.0/test/test_model_gradient.py` & `pyoptmat-1.3.0/test/test_model_gradient.py`

 * *Files identical despite different names*

### Comparing `pyoptmat-1.2.0/test/test_models.py` & `pyoptmat-1.3.0/test/test_models.py`

 * *Files identical despite different names*

### Comparing `pyoptmat-1.2.0/test/test_ode.py` & `pyoptmat-1.3.0/test/test_ode.py`

 * *Files identical despite different names*

### Comparing `pyoptmat-1.2.0/test/test_scaling.py` & `pyoptmat-1.3.0/test/test_scaling.py`

 * *Files identical despite different names*

### Comparing `pyoptmat-1.2.0/test/test_solvers.py` & `pyoptmat-1.3.0/test/test_solvers.py`

 * *Files identical despite different names*

### Comparing `pyoptmat-1.2.0/test/test_temperature_scaling.py` & `pyoptmat-1.3.0/test/test_temperature_scaling.py`

 * *Files identical despite different names*

### Comparing `pyoptmat-1.2.0/test/test_utility.py` & `pyoptmat-1.3.0/test/test_utility.py`

 * *Files identical despite different names*

