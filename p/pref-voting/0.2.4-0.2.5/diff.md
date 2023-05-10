# Comparing `tmp/pref_voting-0.2.4.tar.gz` & `tmp/pref_voting-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pref_voting-0.2.4.tar", max compression
+gzip compressed data, was "pref_voting-0.2.5.tar", max compression
```

## Comparing `pref_voting-0.2.4.tar` & `pref_voting-0.2.5.tar`

### file list

```diff
@@ -1,24 +1,26 @@
--rw-r--r--   0        0        0     1068 2022-07-08 15:47:57.000000 pref_voting-0.2.4/LICENSE
--rw-r--r--   0        0        0     2605 2023-04-09 19:41:59.470121 pref_voting-0.2.4/README.md
--rw-r--r--   0        0        0       22 2023-04-09 19:41:57.461372 pref_voting-0.2.4/pref_voting/__init__.py
--rw-r--r--   0        0        0     6950 2023-01-11 11:10:50.000000 pref_voting-0.2.4/pref_voting/analysis.py
--rw-r--r--   0        0        0      617 2023-03-19 17:14:54.163308 pref_voting-0.2.4/pref_voting/axioms.py
--rw-r--r--   0        0        0    23041 2023-01-11 11:10:14.000000 pref_voting-0.2.4/pref_voting/c1_methods.py
--rw-r--r--   0        0        0     8564 2023-02-15 17:29:01.299008 pref_voting-0.2.4/pref_voting/combined_methods.py
--rw-r--r--   0        0        0    20644 2023-04-09 19:35:14.204698 pref_voting-0.2.4/pref_voting/generate_profiles.py
--rw-r--r--   0        0        0    10484 2023-01-11 11:10:14.000000 pref_voting-0.2.4/pref_voting/generate_weighted_majority_graphs.py
--rw-r--r--   0        0        0     1806 2022-08-08 19:08:16.000000 pref_voting-0.2.4/pref_voting/helper.py
--rw-r--r--   0        0        0    73235 2023-04-03 00:50:48.493987 pref_voting-0.2.4/pref_voting/iterative_methods.py
--rw-r--r--   0        0        0    20246 2022-07-12 12:12:35.000000 pref_voting-0.2.4/pref_voting/maj_graph_ex1.png
--rw-r--r--   0        0        0    57869 2022-12-27 22:07:30.000000 pref_voting-0.2.4/pref_voting/margin_based_methods.py
--rw-r--r--   0        0        0    25682 2023-04-03 23:28:48.128269 pref_voting-0.2.4/pref_voting/other_methods.py
--rw-r--r--   0        0        0     9527 2022-07-08 18:36:14.000000 pref_voting-0.2.4/pref_voting/pr_voting_methods.py
--rw-r--r--   0        0        0    26712 2023-02-15 16:01:48.269224 pref_voting-0.2.4/pref_voting/profiles.py
--rw-r--r--   0        0        0    34045 2023-03-19 16:14:32.871530 pref_voting-0.2.4/pref_voting/profiles_with_ties.py
--rw-r--r--   0        0        0    11064 2023-03-12 17:38:09.515720 pref_voting-0.2.4/pref_voting/scoring_methods.py
--rw-r--r--   0        0        0     5381 2023-02-15 15:31:23.315651 pref_voting-0.2.4/pref_voting/voting_method.py
--rw-r--r--   0        0        0      253 2022-07-31 21:02:46.000000 pref_voting-0.2.4/pref_voting/voting_methods.py
--rw-r--r--   0        0        0    48830 2023-01-09 01:33:03.000000 pref_voting-0.2.4/pref_voting/weighted_majority_graphs.py
--rw-r--r--   0        0        0      715 2023-04-09 19:40:36.986854 pref_voting-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     3578 1970-01-01 00:00:00.000000 pref_voting-0.2.4/setup.py
--rw-r--r--   0        0        0     3699 1970-01-01 00:00:00.000000 pref_voting-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1068 2022-07-08 15:47:57.000000 pref_voting-0.2.5/LICENSE
+-rw-r--r--   0        0        0     2689 2023-05-10 10:43:09.900462 pref_voting-0.2.5/README.md
+-rw-r--r--   0        0        0       22 2023-05-10 10:43:11.491032 pref_voting-0.2.5/pref_voting/__init__.py
+-rw-r--r--   0        0        0     9684 2023-05-10 10:41:09.367527 pref_voting-0.2.5/pref_voting/analysis.py
+-rw-r--r--   0        0        0      715 2023-04-27 22:56:23.847953 pref_voting-0.2.5/pref_voting/axiom.py
+-rw-r--r--   0        0        0       43 2023-04-27 22:57:52.337540 pref_voting-0.2.5/pref_voting/axioms.py
+-rw-r--r--   0        0        0    23064 2023-05-09 19:06:46.659038 pref_voting-0.2.5/pref_voting/c1_methods.py
+-rw-r--r--   0        0        0     8564 2023-02-15 17:29:01.299008 pref_voting-0.2.5/pref_voting/combined_methods.py
+-rw-r--r--   0        0        0    11511 2023-05-09 19:08:40.182737 pref_voting-0.2.5/pref_voting/dominance_axioms.py
+-rw-r--r--   0        0        0    20644 2023-04-09 19:35:14.204698 pref_voting-0.2.5/pref_voting/generate_profiles.py
+-rw-r--r--   0        0        0    10484 2023-01-11 11:10:14.000000 pref_voting-0.2.5/pref_voting/generate_weighted_majority_graphs.py
+-rw-r--r--   0        0        0     1806 2022-08-08 19:08:16.000000 pref_voting-0.2.5/pref_voting/helper.py
+-rw-r--r--   0        0        0    73235 2023-04-03 00:50:48.493987 pref_voting-0.2.5/pref_voting/iterative_methods.py
+-rw-r--r--   0        0        0    20246 2022-07-12 12:12:35.000000 pref_voting-0.2.5/pref_voting/maj_graph_ex1.png
+-rw-r--r--   0        0        0    57869 2022-12-27 22:07:30.000000 pref_voting-0.2.5/pref_voting/margin_based_methods.py
+-rw-r--r--   0        0        0    25682 2023-04-03 23:28:48.128269 pref_voting-0.2.5/pref_voting/other_methods.py
+-rw-r--r--   0        0        0     9527 2022-07-08 18:36:14.000000 pref_voting-0.2.5/pref_voting/pr_voting_methods.py
+-rw-r--r--   0        0        0    26881 2023-04-27 22:28:39.276752 pref_voting-0.2.5/pref_voting/profiles.py
+-rw-r--r--   0        0        0    34203 2023-04-27 22:31:21.483788 pref_voting-0.2.5/pref_voting/profiles_with_ties.py
+-rw-r--r--   0        0        0    11064 2023-05-05 16:30:25.075183 pref_voting-0.2.5/pref_voting/scoring_methods.py
+-rw-r--r--   0        0        0     5381 2023-02-15 15:31:23.315651 pref_voting-0.2.5/pref_voting/voting_method.py
+-rw-r--r--   0        0        0      253 2022-07-31 21:02:46.000000 pref_voting-0.2.5/pref_voting/voting_methods.py
+-rw-r--r--   0        0        0    48830 2023-01-09 01:33:03.000000 pref_voting-0.2.5/pref_voting/weighted_majority_graphs.py
+-rw-r--r--   0        0        0      715 2023-05-10 10:43:08.457638 pref_voting-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0     3663 1970-01-01 00:00:00.000000 pref_voting-0.2.5/setup.py
+-rw-r--r--   0        0        0     3783 1970-01-01 00:00:00.000000 pref_voting-0.2.5/PKG-INFO
```

### Comparing `pref_voting-0.2.4/LICENSE` & `pref_voting-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pref_voting-0.2.4/README.md` & `pref_voting-0.2.5/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -53,15 +53,16 @@
 - v0.1.14 (2022-12-19): Add plurality_scores to ProfileWithTies; add generate ceots function; bug fixes 
 - v0.1.23 (2022-12-27): Add instant_runoff_for_truncated_linear_orders and functions to truncate overvotes in a ProfileWithTies, add smith_irv_put, document analysis functions
 - v0.1.25 (2023-1-11): Add condorcet_irv, condorcet_irv_put; Update documentation; add axioms.py; add display and equality to Ranking class; fix enumerate ceots functions
 - v0.1.27 (2023-2-07): Add Borda for ProfileWithTies
 - v0.2 (2023-2-15): Add Benham, add anonymize to Profile method, comment out numba to make compatible with Python 3.11, add add_unranked_candidates to ProfileWithTies
 - v0.2.1 (2023-2-15): Bug fixes
 - v0.2.3 (2023-4-2): Add plurality_with_runoff_with_explanation
-- v0.2.4 (2023-4-9): Update generate_truncated_profile so that it implements and IC probability model.
+- v0.2.4 (2023-4-9): Update generate_truncated_profile so that it implements the IC probability model.
+- v0.2.5 (2023-5-10): Add axiom class, dominance axioms, and axiom_violations_data.
 
 ## Questions?
 
 Feel free to [send me an email](https://pacuit.org/) if you have questions about the project.
 
 ## License
```

### Comparing `pref_voting-0.2.4/pref_voting/analysis.py` & `pref_voting-0.2.5/pref_voting/analysis.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
     File: analysis.py
     Author: Eric Pacuit (epacuit@umd.edu)
     Date: August 9, 2022
-    
+    Updated: May 9, 2023
+
     Functions to analyze voting methods
 """
 
 from pref_voting.generate_profiles import generate_profile
 from pref_voting.profiles import Profile
 from tqdm.notebook import tqdm
 from functools import partial
@@ -80,15 +81,15 @@
 
     return {
         "has_cw": cw is not None,
         "cw_winner": {vm.name: cw is not None and [cw] == vm(prof) for vm in vms},
     }
 
 
-def find_condorcet_efficiency(
+def condorcet_efficiency_data(
     vms,
     numbers_of_candidates=[3, 4, 5],
     numbers_of_voters=[4, 10, 20, 50, 100, 500, 1000],
     probmods=["IC"],
     num_trials=10000,
     use_parallel=True,
     num_cpus=12,
@@ -111,62 +112,138 @@
         pool = Pool(num_cpus)
 
     data_for_df = {
         "vm": list(),
         "num_cands": list(),
         "num_voters": list(),
         "probmod": list(),
+        "num_trials": list(),
         "percent_condorcet_winners": list(),
         "condorcet_efficiency": list(),
     }
     for probmod in probmods:
         for num_cands in numbers_of_candidates:
             for num_voters in numbers_of_voters:
 
-                print(f"{num_cands} candidates, {num_voters}, {num_voters + 1} voters")
-                get_data0 = partial(
+                print(f"{num_cands} candidates, {num_voters} voters")
+                get_data = partial(
                     record_condorcet_efficiency_data,
                     vms,
                     num_cands,
                     num_voters,
                     probmod,
                 )
 
-                get_data1 = partial(
-                    record_condorcet_efficiency_data,
-                    vms,
-                    num_cands,
-                    num_voters + 1,
-                    probmod,
-                )
-
                 if use_parallel:
-                    data0 = pool.map(get_data0, range(num_trials))
-                    data1 = pool.map(get_data1, range(num_trials))
+                    data = pool.map(get_data, range(num_trials))
                 else:
-                    data0 = list(map(get_data0, range(num_trials)))
-                    data1 = list(map(get_data1, range(num_trials)))
+                    data = list(map(get_data, range(num_trials)))
 
-                data = data0 + data1
                 num_cw = 0
                 num_choose_cw = {vm.name: 0 for vm in vms}
                 for d in data:
                     if d["has_cw"]:
                         num_cw += 1
                         for vm in vms:
                             num_choose_cw[vm.name] += int(d["cw_winner"][vm.name])
 
-                num_profiles = 2 * num_trials
                 for vm in vms:
                     data_for_df["vm"].append(vm.name)
                     data_for_df["num_cands"].append(num_cands)
-                    data_for_df["num_voters"].append((num_voters, num_voters + 1))
+                    data_for_df["num_voters"].append(num_voters)
                     data_for_df["probmod"].append(probmod)
+                    data_for_df["num_trials"].append(num_trials)
                     data_for_df["percent_condorcet_winners"].append(
-                        num_cw / num_profiles
+                        num_cw / num_trials
                     )
                     data_for_df["condorcet_efficiency"].append(
                         num_choose_cw[vm.name] / num_cw
                     )
 
     return pd.DataFrame(data_for_df)
 
+# helper function for axiom_violations_data
+def record_axiom_violation_data(
+    axioms, 
+    vms, 
+    num_cands, 
+    num_voters, 
+    probmod, 
+    verbose, 
+    t
+    ):
+
+    prof = generate_profile(num_cands, num_voters, probmod=probmod)
+    
+    return {ax.name: {vm.name: ax.has_violation(prof, vm, verbose=verbose) for vm in vms} for ax in axioms}
+
+def axiom_violations_data(
+    axioms,
+    vms,
+    numbers_of_candidates=[3, 4, 5],
+    numbers_of_voters=[4, 5, 10, 11,  20, 21, 50, 51,  100, 101,  500, 501,  1000, 1001],
+    probmods=["IC"],
+    num_trials=10000,
+    verbose=False,
+    use_parallel=True,
+    num_cpus=12,
+):
+    """
+    Returns a Pandas DataFrame with the Condorcet efficiency of a list of voting methods.
+
+    Args:
+        vms (list(functions)): A list of voting methods,
+        numbers_of_candidates (list(int), default = [3, 4, 5]): The numbers of candidates to check.
+        numbers_of_voters (list(int), default = [5, 25, 50, 100]): The numbers of voters to check.
+        probmod (str, default="IC"): The probability model to be passed to the ``generate_profile`` method
+        num_trials (int, default=10000): The number of profiles to check for different winning sets.
+        use_parallel (bool, default=True): If True, then use parallel processing.
+        num_cpus (int, default=12): The number of (virtual) cpus to use if using parallel processing.
+
+    """
+
+    if use_parallel:
+        pool = Pool(num_cpus)
+
+    data_for_df = {
+        "axiom": list(),
+        "vm": list(),
+        "num_cands": list(),
+        "num_voters": list(),
+        "probmod": list(),
+        "num_trials": list(),
+        "num_violations": list(),
+    }
+    for probmod in probmods:
+        print(f"{probmod} probability model")
+        for num_cands in tqdm(numbers_of_candidates, leave=False):
+            for num_voters in tqdm(numbers_of_voters, leave=False):
+                #print(f"{num_cands} candidates, {num_voters} voters")
+                _verbose = verbose if not use_parallel else False
+                get_data = partial(
+                    record_axiom_violation_data,
+                    axioms,
+                    vms,
+                    num_cands,
+                    num_voters,
+                    probmod,
+                    _verbose
+                )
+
+                if use_parallel:
+                    data = pool.map(get_data, range(num_trials))
+                else:
+                    data = list(map(get_data, range(num_trials)))
+
+                for ax in axioms: 
+                    for vm in vms: 
+                        data_for_df["axiom"].append(ax.name)
+                        data_for_df["vm"].append(vm.name)
+                        data_for_df["num_cands"].append(num_cands)
+                        data_for_df["num_voters"].append(num_voters)
+                        data_for_df["probmod"].append(probmod)
+                        data_for_df["num_trials"].append(num_trials)
+                        data_for_df["num_violations"].append(sum([d[ax.name][vm.name] for d in data]))
+    print("Done.")
+    return pd.DataFrame(data_for_df)
+
+
```

### Comparing `pref_voting-0.2.4/pref_voting/c1_methods.py` & `pref_voting-0.2.5/pref_voting/c1_methods.py`

 * *Files 2% similar despite different names*

```diff
@@ -556,16 +556,15 @@
     defeat.add_nodes_from(candidates)
     defeat.add_edges_from([(a, b) for a in candidates for b in candidates if a != b and a in smith_set and b not in smith_set])
     return defeat
 
 
 @vm(name = "GOCHA")
 def gocha(edata, curr_cands = None):
-    """The GOCHA set (also known as the Schwartz set) is the smallest set of candidates with the property
-    that every candidate inside the set is not majority preferred by every candidate outside the set.
+    """The GOCHA set (also known as the Schwartz set) is the set of all candidates x such that if y can reach x in the transitive closer of the majority relation, then x can reach y in the transitive closer of the majority relation.
       
     Args:
         edata (Profile, ProfileWithTies, MajorityGraph, MarginGraph): Any election data that has a `majority_prefers` method. 
         curr_cands (List[int], optional): If set, then find the winners for the profile restricted to the candidates in ``curr_cands``
 
     Returns: 
         A sorted list of candidates
@@ -578,23 +577,21 @@
 
     :Example: 
           
     .. plot::  margin_graphs_examples/mg_ex_top_cycle_gocha.py
         :context: reset  
         :include-source: True
 
-
     .. code-block:: 
 
         from pref_voting.c1_methods import top_cycle, gocha, schwartz_set
 
         gocha.display(prof)
         schwartz_set.display(prof)
 
-
     .. exec_code:: 
         :hide_code:
 
         from pref_voting.profiles import Profile
         from pref_voting.c1_methods import gocha, schwartz_set
         
         prof = Profile([[1, 2, 0, 3], [1, 3, 0, 2], [3, 1, 0, 2], [0, 3, 1, 2]], [1, 1, 1, 1])
```

### Comparing `pref_voting-0.2.4/pref_voting/combined_methods.py` & `pref_voting-0.2.5/pref_voting/combined_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.2.4/pref_voting/generate_profiles.py` & `pref_voting-0.2.5/pref_voting/generate_profiles.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.2.4/pref_voting/generate_weighted_majority_graphs.py` & `pref_voting-0.2.5/pref_voting/generate_weighted_majority_graphs.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.2.4/pref_voting/helper.py` & `pref_voting-0.2.5/pref_voting/helper.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.2.4/pref_voting/iterative_methods.py` & `pref_voting-0.2.5/pref_voting/iterative_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.2.4/pref_voting/maj_graph_ex1.png` & `pref_voting-0.2.5/pref_voting/maj_graph_ex1.png`

 * *Files identical despite different names*

### Comparing `pref_voting-0.2.4/pref_voting/margin_based_methods.py` & `pref_voting-0.2.5/pref_voting/margin_based_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.2.4/pref_voting/other_methods.py` & `pref_voting-0.2.5/pref_voting/other_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.2.4/pref_voting/pr_voting_methods.py` & `pref_voting-0.2.5/pref_voting/pr_voting_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.2.4/pref_voting/profiles.py` & `pref_voting-0.2.5/pref_voting/profiles.py`

 * *Files 2% similar despite different names*

```diff
@@ -149,15 +149,15 @@
 class Profile(object):
     """An anonymous profile of linear rankings of :math:`n` candidates.  It is assumed that the candidates are named :math:`0, 1, \ldots, n-1` and a ranking of the candidates is a list of candidate names.  For instance, the list ``[0, 2, 1]`` represents the ranking in which :math:`0` is ranked above :math:`2`, :math:`2` is ranked above :math:`1`, and :math:`0` is ranked above :math:`1`.   
 
     :param rankings: List of rankings in the profile, where a ranking is a list of candidates.
     :type rankings: list[list[int]]
     :param rcounts: List of the number of voters associated with each ranking.  Should be the same length as rankings.   If not provided, it is assumed that 1 voters submitted each element of ``rankings``.   
     :type rcounts: list[int], optional
-    :param cmap: Dictionary mapping candidates (integers) to candidate names (strings).  If not provied, each candidate name is mapped to itself. 
+    :param cmap: Dictionary mapping candidates (integers) to candidate names (strings).  If not provided, each candidate name is mapped to itself. 
     :type cmap: dict[int: str], optional
 
     :Example:
     
     The following code creates a profile in which 
     2 voters submitted the ranking ``[0, 1, 2]``, 3 voters submitted the ranking ``[1, 2, 0]``, and 1 voter submitted the ranking ``[2, 0, 1]``: 
 
@@ -181,15 +181,15 @@
         
         # for number of each ranking
         self._rcounts = np.array([1]*len(rankings)) if rcounts is None else np.array(rcounts) 
         
         # for each voter, the rankings of each candidate
         self._ranks = np.array([[_r.index(c) + 1 for c in self.candidates] for  _r in rankings])
         
-        # 2d array where the c,d entery is the support of c over d
+        # 2d array where the c,d entry is the support of c over d
         self._tally = np.array([[_support(self._ranks, self._rcounts, c1, c2) 
                                  for c2 in self.candidates] for c1 in self.candidates ])
         
         # mapping candidates to candidate names
         self.cmap = cmap if cmap is not None else {c:str(c) for c in self.candidates}
                 
         # total number of voters
@@ -239,15 +239,14 @@
         :param c1: the first candidate
         :type c1: int
         :param c2: the second candidate
         :type c2: int
         :rtype: int
 
         """
-
         return _margin(self._tally, c1, c2)
         
     def majority_prefers(self, c1, c2): 
         """Returns true if more voters rank :math:`c1` over :math:`c2` than :math:`c2` over :math:`c1`; otherwise false. 
         
         :param c1: the first candidate
         :type c1: int
@@ -320,20 +319,20 @@
         """Returns the list of candidates that are majority preferred to ``cand`` in the profile restricted to the candidates in ``curr_cands``. 
         """        
         candidates = self.candidates if curr_cands is None else curr_cands
         
         return [c for c in candidates if self.majority_prefers(c, cand)]
 
     def dominates(self, cand, curr_cands = None): 
-        """Returns the list of candidates that ``cand`` is majority preferred to in the majority graph restricted to ``curr_cands``.
+        """Returns the list of candidates that ``cand`` is majority preferred to in the profiles restricted to ``curr_cands``.
         """
         candidates = self.candidates if curr_cands is None else curr_cands
         
         return [c for c in candidates if self.majority_prefers(cand, c)]
-
+    
     def copeland_scores(self, curr_cands = None, scores = (1,0,-1)):
         """The Copeland scores in the profile restricted to the candidates in ``curr_cands``. 
 
         The **Copeland score** for candidate :math:`c` is calculated as follows:  :math:`c` receives ``scores[0]`` points for every candidate that  :math:`c` is majority preferred to, ``scores[1]`` points for every candidate that is tied with :math:`c`, and ``scores[2]`` points for every candidate that is majority preferred to :math:`c`. The default ``scores`` is ``(1, 0, -1)``. 
         
 
         :param curr_cands: restrict attention to candidates in this list. Defaults to all candidates in the profile if not provided. 
@@ -618,14 +617,18 @@
             rcounts.append(rc)
             rankings.append(r)
 
         cmap = {int(c_cname.split(":")[0]): str(c_cname.split(":")[1]) for c_cname in cmap_data}
 
         return cls(rankings, num_cands, rcounts, cmap)
     
+    def description(self): 
+        rs, cs = self.rankings_counts
+        return f"Profile({[list(r) for r in rs]}, rcounts={[int(c) for c in cs]}, cmap={self.cmap})"
+    
     def __str__(self): 
         # print the profile as a table
         
         return tabulate([[self.cmap[c] for c in cs] for cs in self._rankings.transpose()], self._rcounts, tablefmt="pretty")    
 
 def simple_lift(ranking, c):
     """
```

### Comparing `pref_voting-0.2.4/pref_voting/profiles_with_ties.py` & `pref_voting-0.2.5/pref_voting/profiles_with_ties.py`

 * *Files 0% similar despite different names*

```diff
@@ -834,14 +834,17 @@
                 rs[str(r)] += c
             else: 
                 rs[str(r)] = c
                 
         for r,c in rs.items(): 
             print(f"{r} {c}")
 
+    def description(self): 
+        return f"ProfileWithTies({[r.rmap for r in self.rankings]}, rcounts={[int(c) for c in self.rcounts]}, cmap={self.cmap})"
+
     def display(self, cmap=None, style="pretty", curr_cands=None):
         """Display a profile (restricted to ``curr_cands``) as an ascii table (using tabulate).
 
         :param cmap: the candidate map (overrides the cmap associated with this profile)
         :type cmap: dict[int,str], optional
         :param style: the candidate map to use (overrides the cmap associated with this profile)
         :type style: str ---  "pretty" or "fancy_grid" (or any other style option for tabulate)
```

### Comparing `pref_voting-0.2.4/pref_voting/scoring_methods.py` & `pref_voting-0.2.5/pref_voting/scoring_methods.py`

 * *Files 0% similar despite different names*

```diff
@@ -93,15 +93,15 @@
     
     max_borda_score = max(borda_scores.values())
     
     return sorted([c for c in curr_cands if borda_scores[c] == max_borda_score])
 
 @vm(name = "Anti-Plurality")
 def anti_plurality(profile, curr_cands = None):
-    """The **Anti-Plurlity score** of a candidate $c$ is the number of voters that rank $c$ in last place.  The Anti-Plurality winnners are the candidates with the smallest Anit-Plurality score in the ``profile`` restricted to ``curr_cands``. 
+    """The **Anti-Plurality score** of a candidate $c$ is the number of voters that rank $c$ in last place.  The Anti-Plurality winners are the candidates with the smallest Anti-Plurality score in the ``profile`` restricted to ``curr_cands``. 
 
     Args:
         profile (Profile): An anonymous profile of linear orders on a set of candidates
         curr_cands (List[int], optional): If set, then find the winners for the profile restricted to the candidates in ``curr_cands``
 
     Returns: 
         A sorted list of candidates
```

### Comparing `pref_voting-0.2.4/pref_voting/voting_method.py` & `pref_voting-0.2.5/pref_voting/voting_method.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.2.4/pref_voting/weighted_majority_graphs.py` & `pref_voting-0.2.5/pref_voting/weighted_majority_graphs.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.2.4/pyproject.toml` & `pref_voting-0.2.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=42",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [tool.poetry]
 name = "pref_voting"
-version = "0.2.4"
+version = "0.2.5"
 description = "pref_voting is a Python packaging that contains tools to reason about election profiles and margin graphs, and implementations of a variety of preferential voting methods."
 authors = ["Eric Pacuit <epacuit@umd.edu>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/voting-tools/pref_voting"
 repository = "https://github.com/voting-tools/pref_voting"
```

### Comparing `pref_voting-0.2.4/setup.py` & `pref_voting-0.2.5/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,17 +12,17 @@
  'networkx>=3.0,<4.0',
  'random2>=1.0.1,<2.0.0',
  'scipy>=1.0.0,<2.0.0',
  'tabulate>=0.9.0,<0.10.0']
 
 setup_kwargs = {
     'name': 'pref-voting',
-    'version': '0.2.4',
+    'version': '0.2.5',
     'description': 'pref_voting is a Python packaging that contains tools to reason about election profiles and margin graphs, and implementations of a variety of preferential voting methods.',
-    'long_description': 'pref_voting\n==========\n\n## Installation\n\nWith pip package manager:\n\n```bash\npip install pref_voting\n```\n## Documentation\n\nOnline documentation is available at [https://pref_voting.readthedocs.io](https://pref_voting.readthedocs.io).\n\n## Profiles and Voting Methods\n\nA profile (of linear orders over the candidates) is created by initializing a Profile class object.  This needs a list of rankings (each ranking is a tuple of numbers), the number of candidates, and a list giving the number of each ranking in the profile:\n\n```python\nfrom pref_voting.profiles import Profile\n\nrankings = [(0, 1, 2, 3), (2, 3, 1, 0), (3, 1, 2, 0), (1, 2, 0, 3), (1, 3, 2, 0)]\nrcounts = [5, 3, 2, 4, 3]\n\nprof = Profile(rankings, rcounts=rcounts)\n```\n\nThe function generate_profile is used to generate a profile for a given number of candidates and voters:  \n```python\nfrom pref_voting.generate_profiles import generate_profile\n\n# generate a profile using the Impartial Culture probability model\nprof = generate_profile(3, 4) # prof is a Profile object\n\n# generate a profile using the Impartial Anonymous Culture probability model\nprof = generate_profile(3, 4, probmod = "IAC") # prof is a Profile object \n```\n\n```python\nfrom pref_voting.profiles import Profile\nfrom pref_voting.voting_methods import *\n\nprof = Profile(rankings, num_cands, rcounts=rcounts)\nprint(f"{split_cycle.name} winners:  {split_cycle(prof)}")\nsplit_cycle.display(prof)\n\n```\n\n## Versions\n\n- v0.1.10 (2022-08-09): **Initial release** \n- v0.1.13 (2022-11-05): Minor updates and bug fixes \n- v0.1.14 (2022-12-19): Add plurality_scores to ProfileWithTies; add generate ceots function; bug fixes \n- v0.1.23 (2022-12-27): Add instant_runoff_for_truncated_linear_orders and functions to truncate overvotes in a ProfileWithTies, add smith_irv_put, document analysis functions\n- v0.1.25 (2023-1-11): Add condorcet_irv, condorcet_irv_put; Update documentation; add axioms.py; add display and equality to Ranking class; fix enumerate ceots functions\n- v0.1.27 (2023-2-07): Add Borda for ProfileWithTies\n- v0.2 (2023-2-15): Add Benham, add anonymize to Profile method, comment out numba to make compatible with Python 3.11, add add_unranked_candidates to ProfileWithTies\n- v0.2.1 (2023-2-15): Bug fixes\n- v0.2.3 (2023-4-2): Add plurality_with_runoff_with_explanation\n- v0.2.4 (2023-4-9): Update generate_truncated_profile so that it implements and IC probability model.\n\n## Questions?\n\nFeel free to [send me an email](https://pacuit.org/) if you have questions about the project.\n\n## License\n\n[MIT](https://github.com/jontingvold/pyrankvote/blob/master/LICENSE.txt)\n',
+    'long_description': 'pref_voting\n==========\n\n## Installation\n\nWith pip package manager:\n\n```bash\npip install pref_voting\n```\n## Documentation\n\nOnline documentation is available at [https://pref_voting.readthedocs.io](https://pref_voting.readthedocs.io).\n\n## Profiles and Voting Methods\n\nA profile (of linear orders over the candidates) is created by initializing a Profile class object.  This needs a list of rankings (each ranking is a tuple of numbers), the number of candidates, and a list giving the number of each ranking in the profile:\n\n```python\nfrom pref_voting.profiles import Profile\n\nrankings = [(0, 1, 2, 3), (2, 3, 1, 0), (3, 1, 2, 0), (1, 2, 0, 3), (1, 3, 2, 0)]\nrcounts = [5, 3, 2, 4, 3]\n\nprof = Profile(rankings, rcounts=rcounts)\n```\n\nThe function generate_profile is used to generate a profile for a given number of candidates and voters:  \n```python\nfrom pref_voting.generate_profiles import generate_profile\n\n# generate a profile using the Impartial Culture probability model\nprof = generate_profile(3, 4) # prof is a Profile object\n\n# generate a profile using the Impartial Anonymous Culture probability model\nprof = generate_profile(3, 4, probmod = "IAC") # prof is a Profile object \n```\n\n```python\nfrom pref_voting.profiles import Profile\nfrom pref_voting.voting_methods import *\n\nprof = Profile(rankings, num_cands, rcounts=rcounts)\nprint(f"{split_cycle.name} winners:  {split_cycle(prof)}")\nsplit_cycle.display(prof)\n\n```\n\n## Versions\n\n- v0.1.10 (2022-08-09): **Initial release** \n- v0.1.13 (2022-11-05): Minor updates and bug fixes \n- v0.1.14 (2022-12-19): Add plurality_scores to ProfileWithTies; add generate ceots function; bug fixes \n- v0.1.23 (2022-12-27): Add instant_runoff_for_truncated_linear_orders and functions to truncate overvotes in a ProfileWithTies, add smith_irv_put, document analysis functions\n- v0.1.25 (2023-1-11): Add condorcet_irv, condorcet_irv_put; Update documentation; add axioms.py; add display and equality to Ranking class; fix enumerate ceots functions\n- v0.1.27 (2023-2-07): Add Borda for ProfileWithTies\n- v0.2 (2023-2-15): Add Benham, add anonymize to Profile method, comment out numba to make compatible with Python 3.11, add add_unranked_candidates to ProfileWithTies\n- v0.2.1 (2023-2-15): Bug fixes\n- v0.2.3 (2023-4-2): Add plurality_with_runoff_with_explanation\n- v0.2.4 (2023-4-9): Update generate_truncated_profile so that it implements the IC probability model.\n- v0.2.5 (2023-5-10): Add axiom class, dominance axioms, and axiom_violations_data.\n\n## Questions?\n\nFeel free to [send me an email](https://pacuit.org/) if you have questions about the project.\n\n## License\n\n[MIT](https://github.com/jontingvold/pyrankvote/blob/master/LICENSE.txt)\n',
     'author': 'Eric Pacuit',
     'author_email': 'epacuit@umd.edu',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/voting-tools/pref_voting',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `pref_voting-0.2.4/PKG-INFO` & `pref_voting-0.2.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pref-voting
-Version: 0.2.4
+Version: 0.2.5
 Summary: pref_voting is a Python packaging that contains tools to reason about election profiles and margin graphs, and implementations of a variety of preferential voting methods.
 Home-page: https://github.com/voting-tools/pref_voting
 License: MIT
 Author: Eric Pacuit
 Author-email: epacuit@umd.edu
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -78,15 +78,16 @@
 - v0.1.14 (2022-12-19): Add plurality_scores to ProfileWithTies; add generate ceots function; bug fixes 
 - v0.1.23 (2022-12-27): Add instant_runoff_for_truncated_linear_orders and functions to truncate overvotes in a ProfileWithTies, add smith_irv_put, document analysis functions
 - v0.1.25 (2023-1-11): Add condorcet_irv, condorcet_irv_put; Update documentation; add axioms.py; add display and equality to Ranking class; fix enumerate ceots functions
 - v0.1.27 (2023-2-07): Add Borda for ProfileWithTies
 - v0.2 (2023-2-15): Add Benham, add anonymize to Profile method, comment out numba to make compatible with Python 3.11, add add_unranked_candidates to ProfileWithTies
 - v0.2.1 (2023-2-15): Bug fixes
 - v0.2.3 (2023-4-2): Add plurality_with_runoff_with_explanation
-- v0.2.4 (2023-4-9): Update generate_truncated_profile so that it implements and IC probability model.
+- v0.2.4 (2023-4-9): Update generate_truncated_profile so that it implements the IC probability model.
+- v0.2.5 (2023-5-10): Add axiom class, dominance axioms, and axiom_violations_data.
 
 ## Questions?
 
 Feel free to [send me an email](https://pacuit.org/) if you have questions about the project.
 
 ## License
```

