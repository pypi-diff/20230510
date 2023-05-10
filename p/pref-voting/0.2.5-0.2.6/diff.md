# Comparing `tmp/pref_voting-0.2.5.tar.gz` & `tmp/pref_voting-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pref_voting-0.2.5.tar", max compression
+gzip compressed data, was "pref_voting-0.2.6.tar", max compression
```

## Comparing `pref_voting-0.2.5.tar` & `pref_voting-0.2.6.tar`

### file list

```diff
@@ -1,26 +1,27 @@
--rw-r--r--   0        0        0     1068 2022-07-08 15:47:57.000000 pref_voting-0.2.5/LICENSE
--rw-r--r--   0        0        0     2689 2023-05-10 10:43:09.900462 pref_voting-0.2.5/README.md
--rw-r--r--   0        0        0       22 2023-05-10 10:43:11.491032 pref_voting-0.2.5/pref_voting/__init__.py
--rw-r--r--   0        0        0     9684 2023-05-10 10:41:09.367527 pref_voting-0.2.5/pref_voting/analysis.py
--rw-r--r--   0        0        0      715 2023-04-27 22:56:23.847953 pref_voting-0.2.5/pref_voting/axiom.py
--rw-r--r--   0        0        0       43 2023-04-27 22:57:52.337540 pref_voting-0.2.5/pref_voting/axioms.py
--rw-r--r--   0        0        0    23064 2023-05-09 19:06:46.659038 pref_voting-0.2.5/pref_voting/c1_methods.py
--rw-r--r--   0        0        0     8564 2023-02-15 17:29:01.299008 pref_voting-0.2.5/pref_voting/combined_methods.py
--rw-r--r--   0        0        0    11511 2023-05-09 19:08:40.182737 pref_voting-0.2.5/pref_voting/dominance_axioms.py
--rw-r--r--   0        0        0    20644 2023-04-09 19:35:14.204698 pref_voting-0.2.5/pref_voting/generate_profiles.py
--rw-r--r--   0        0        0    10484 2023-01-11 11:10:14.000000 pref_voting-0.2.5/pref_voting/generate_weighted_majority_graphs.py
--rw-r--r--   0        0        0     1806 2022-08-08 19:08:16.000000 pref_voting-0.2.5/pref_voting/helper.py
--rw-r--r--   0        0        0    73235 2023-04-03 00:50:48.493987 pref_voting-0.2.5/pref_voting/iterative_methods.py
--rw-r--r--   0        0        0    20246 2022-07-12 12:12:35.000000 pref_voting-0.2.5/pref_voting/maj_graph_ex1.png
--rw-r--r--   0        0        0    57869 2022-12-27 22:07:30.000000 pref_voting-0.2.5/pref_voting/margin_based_methods.py
--rw-r--r--   0        0        0    25682 2023-04-03 23:28:48.128269 pref_voting-0.2.5/pref_voting/other_methods.py
--rw-r--r--   0        0        0     9527 2022-07-08 18:36:14.000000 pref_voting-0.2.5/pref_voting/pr_voting_methods.py
--rw-r--r--   0        0        0    26881 2023-04-27 22:28:39.276752 pref_voting-0.2.5/pref_voting/profiles.py
--rw-r--r--   0        0        0    34203 2023-04-27 22:31:21.483788 pref_voting-0.2.5/pref_voting/profiles_with_ties.py
--rw-r--r--   0        0        0    11064 2023-05-05 16:30:25.075183 pref_voting-0.2.5/pref_voting/scoring_methods.py
--rw-r--r--   0        0        0     5381 2023-02-15 15:31:23.315651 pref_voting-0.2.5/pref_voting/voting_method.py
--rw-r--r--   0        0        0      253 2022-07-31 21:02:46.000000 pref_voting-0.2.5/pref_voting/voting_methods.py
--rw-r--r--   0        0        0    48830 2023-01-09 01:33:03.000000 pref_voting-0.2.5/pref_voting/weighted_majority_graphs.py
--rw-r--r--   0        0        0      715 2023-05-10 10:43:08.457638 pref_voting-0.2.5/pyproject.toml
--rw-r--r--   0        0        0     3663 1970-01-01 00:00:00.000000 pref_voting-0.2.5/setup.py
--rw-r--r--   0        0        0     3783 1970-01-01 00:00:00.000000 pref_voting-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0     1068 2022-07-08 15:47:57.000000 pref_voting-0.2.6/LICENSE
+-rw-r--r--   0        0        0     2689 2023-05-10 11:16:25.003207 pref_voting-0.2.6/README.md
+-rw-r--r--   0        0        0       22 2023-05-10 11:16:23.256657 pref_voting-0.2.6/pref_voting/__init__.py
+-rw-r--r--   0        0        0     9684 2023-05-10 10:41:09.367527 pref_voting-0.2.6/pref_voting/analysis.py
+-rw-r--r--   0        0        0      715 2023-04-27 22:56:23.847953 pref_voting-0.2.6/pref_voting/axiom.py
+-rw-r--r--   0        0        0      360 2023-05-10 11:16:28.091090 pref_voting-0.2.6/pref_voting/axiom_helpers.py
+-rw-r--r--   0        0        0       43 2023-04-27 22:57:52.337540 pref_voting-0.2.6/pref_voting/axioms.py
+-rw-r--r--   0        0        0    23065 2023-05-10 11:22:02.837497 pref_voting-0.2.6/pref_voting/c1_methods.py
+-rw-r--r--   0        0        0     8564 2023-02-15 17:29:01.299008 pref_voting-0.2.6/pref_voting/combined_methods.py
+-rw-r--r--   0        0        0    11517 2023-05-10 11:16:27.288554 pref_voting-0.2.6/pref_voting/dominance_axioms.py
+-rw-r--r--   0        0        0    20643 2023-05-10 11:16:22.353419 pref_voting-0.2.6/pref_voting/generate_profiles.py
+-rw-r--r--   0        0        0    10484 2023-01-11 11:10:14.000000 pref_voting-0.2.6/pref_voting/generate_weighted_majority_graphs.py
+-rw-r--r--   0        0        0     1806 2022-08-08 19:08:16.000000 pref_voting-0.2.6/pref_voting/helper.py
+-rw-r--r--   0        0        0    73229 2023-05-10 11:16:21.455329 pref_voting-0.2.6/pref_voting/iterative_methods.py
+-rw-r--r--   0        0        0    20246 2022-07-12 12:12:35.000000 pref_voting-0.2.6/pref_voting/maj_graph_ex1.png
+-rw-r--r--   0        0        0    57868 2023-05-10 11:18:39.320393 pref_voting-0.2.6/pref_voting/margin_based_methods.py
+-rw-r--r--   0        0        0    25681 2023-05-10 11:20:32.560828 pref_voting-0.2.6/pref_voting/other_methods.py
+-rw-r--r--   0        0        0     9526 2023-05-10 11:24:57.793416 pref_voting-0.2.6/pref_voting/pr_voting_methods.py
+-rw-r--r--   0        0        0    26881 2023-04-27 22:28:39.276752 pref_voting-0.2.6/pref_voting/profiles.py
+-rw-r--r--   0        0        0    34203 2023-04-27 22:31:21.483788 pref_voting-0.2.6/pref_voting/profiles_with_ties.py
+-rw-r--r--   0        0        0    11064 2023-05-05 16:30:25.075183 pref_voting-0.2.6/pref_voting/scoring_methods.py
+-rw-r--r--   0        0        0     5381 2023-02-15 15:31:23.315651 pref_voting-0.2.6/pref_voting/voting_method.py
+-rw-r--r--   0        0        0      253 2022-07-31 21:02:46.000000 pref_voting-0.2.6/pref_voting/voting_methods.py
+-rw-r--r--   0        0        0    48834 2023-05-10 11:24:52.540248 pref_voting-0.2.6/pref_voting/weighted_majority_graphs.py
+-rw-r--r--   0        0        0      715 2023-05-10 11:25:08.655118 pref_voting-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0     3663 1970-01-01 00:00:00.000000 pref_voting-0.2.6/setup.py
+-rw-r--r--   0        0        0     3783 1970-01-01 00:00:00.000000 pref_voting-0.2.6/PKG-INFO
```

### Comparing `pref_voting-0.2.5/LICENSE` & `pref_voting-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pref_voting-0.2.5/README.md` & `pref_voting-0.2.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 - v0.1.23 (2022-12-27): Add instant_runoff_for_truncated_linear_orders and functions to truncate overvotes in a ProfileWithTies, add smith_irv_put, document analysis functions
 - v0.1.25 (2023-1-11): Add condorcet_irv, condorcet_irv_put; Update documentation; add axioms.py; add display and equality to Ranking class; fix enumerate ceots functions
 - v0.1.27 (2023-2-07): Add Borda for ProfileWithTies
 - v0.2 (2023-2-15): Add Benham, add anonymize to Profile method, comment out numba to make compatible with Python 3.11, add add_unranked_candidates to ProfileWithTies
 - v0.2.1 (2023-2-15): Bug fixes
 - v0.2.3 (2023-4-2): Add plurality_with_runoff_with_explanation
 - v0.2.4 (2023-4-9): Update generate_truncated_profile so that it implements the IC probability model.
-- v0.2.5 (2023-5-10): Add axiom class, dominance axioms, and axiom_violations_data.
+- v0.2.6 (2023-5-10): Add axiom class, dominance axioms, and axiom_violations_data.
 
 ## Questions?
 
 Feel free to [send me an email](https://pacuit.org/) if you have questions about the project.
 
 ## License
```

### Comparing `pref_voting-0.2.5/pref_voting/analysis.py` & `pref_voting-0.2.6/pref_voting/analysis.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.2.5/pref_voting/axiom.py` & `pref_voting-0.2.6/pref_voting/axiom.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.2.5/pref_voting/c1_methods.py` & `pref_voting-0.2.6/pref_voting/c1_methods.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,15 +107,15 @@
     c_scores = edata.copeland_scores(curr_cands = curr_cands)
     max_score = max(c_scores.values())
     return sorted([c for c in c_scores.keys() if c_scores[c] == max_score])
 
 
 @vm(name = "Llull")
 def llull(edata, curr_cands = None):
-    """The Llull score for a candidate :math:`c` is the number of candidates that :math:`c` is weakly majority preferred to.  This is equivalent to calucating the Copeland scores for a candidate :math:`c` with 1 point for each candidate that :math:`c` is majority preferred to, 1/2 point for each candidate that :math:`c` is tied with, and 0 points for each candidate that is majority preferred to :math:`c`.  The Llull winners are the candidates with the maximum Llull score in the profile restricted to ``curr_cands``. 
+    """The Llull score for a candidate :math:`c` is the number of candidates that :math:`c` is weakly majority preferred to.  This is equivalent to calculating the Copeland scores for a candidate :math:`c` with 1 point for each candidate that :math:`c` is majority preferred to, 1/2 point for each candidate that :math:`c` is tied with, and 0 points for each candidate that is majority preferred to :math:`c`.  The Llull winners are the candidates with the maximum Llull score in the profile restricted to ``curr_cands``. 
 
     Args:
         edata (Profile, ProfileWithTies, MajorityGraph, MarginGraph): Any election data that has a `copeland_scores` method. 
         curr_cands (List[int], optional): If set, then find the winners for the profile restricted to the candidates in ``curr_cands``
 
     Returns: 
         A sorted list of candidates
```

### Comparing `pref_voting-0.2.5/pref_voting/combined_methods.py` & `pref_voting-0.2.6/pref_voting/combined_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.2.5/pref_voting/dominance_axioms.py` & `pref_voting-0.2.6/pref_voting/dominance_axioms.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,17 +3,17 @@
     Author: Eric Pacuit (epacuit@umd.edu)
     Date: April 27, 2023
     
     Dominance axioms 
 """
 
 from pref_voting.axiom import Axiom
+from pref_voting.c1_methods import smith_set, schwartz_set
+from pref_voting.axiom_helpers import *
 
-def list_to_string(cands, cmap): 
-    return "{" + ', '.join([cmap[c] for c in cands]) + "}"
 
 def has_pareto_violation(edata, vm, verbose=False):
     """
     Returns True if some winner according to vm is Pareto dominated (there is a candidate that is unanimously preferred to the winner).
     
     Args:
         edata (Profile, ProfileWithTies): the election data.
```

### Comparing `pref_voting-0.2.5/pref_voting/generate_profiles.py` & `pref_voting-0.2.6/pref_voting/generate_profiles.py`

 * *Files 0% similar despite different names*

```diff
@@ -476,15 +476,15 @@
         for B in combinations(A, k):  # i.e., all nonempty subsets B
             for order in strict_weak_orders(set(A) - set(B)):
                 yield [B] + order
 
 
 def generate_truncated_profile(num_cands, num_voters, max_num_ranked=3,probmod="IC"):
     """Generate a :class:`ProfileWithTies` with ``num_cands`` candidates and ``num_voters``.  
-    `The ballots will be truncated linear orders of the candidates.
+    The ballots will be truncated linear orders of the candidates.
 
     Args:
         num_cands (int): The number of candidates to include in the profile. 
         num_voters (int): The number of voters to include in the profile.
         max_num_ranked (int, default=3): The maximum level to truncate the linear ranking. 
         probmod (str): optional (default "IC")
```

### Comparing `pref_voting-0.2.5/pref_voting/generate_weighted_majority_graphs.py` & `pref_voting-0.2.6/pref_voting/generate_weighted_majority_graphs.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.2.5/pref_voting/helper.py` & `pref_voting-0.2.6/pref_voting/helper.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.2.5/pref_voting/iterative_methods.py` & `pref_voting-0.2.6/pref_voting/iterative_methods.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,22 +39,22 @@
         Related functions:  :func:`pref_voting.iterative_methods.instant_runoff_tb`, :func:`pref_voting.iterative_methods.instant_runoff_put`, :func:`pref_voting.iterative_methods.instant_runoff_with_explanation`
    
     :Example: 
 
     .. exec_code:: 
 
         from pref_voting.profiles import Profile
-        from pref_voting.iterative_methods import instant_runoff, ranked_choice, alterantive_vote, hare
+        from pref_voting.iterative_methods import instant_runoff, ranked_choice, alternative_vote, hare
         
         prof = Profile([[2, 1, 0], [0, 2, 1], [1, 2, 0]], [1, 2, 2])
 
         prof.display()
         instant_runoff.display(prof)
         ranked_choice.display(prof)
-        alterantive_vote.display(prof)
+        alternative_vote.display(prof)
         hare.display(prof)
 
     """
 
     # need the total number of all candidates in a profile to check when all candidates have been removed   
     num_cands = profile.num_cands 
     
@@ -88,15 +88,15 @@
 
 # Create some aliases for instant runoff
 instant_runoff.set_name("Hare")
 hare = copy.deepcopy(instant_runoff)
 instant_runoff.set_name("Ranked Choice")
 ranked_choice = copy.deepcopy(instant_runoff)
 instant_runoff.set_name("Alternative Vote")
-alterantive_vote = copy.deepcopy(instant_runoff)
+alternative_vote = copy.deepcopy(instant_runoff)
 
 # reset the name Instant Runoff
 instant_runoff.set_name("Instant Runoff")
 
 @vm(name = "Instant Runoff TB")
 def instant_runoff_tb(profile, curr_cands = None, tie_breaker = None):
     """Instant Runoff (``instant_runoff``) with tie breaking:  If there is  more than one candidate with the fewest number of first-place votes, then remove the candidate with lowest in the tie_breaker ranking from the profile.
@@ -164,15 +164,15 @@
                        if not isin(cands_to_ignore,c) and _num_rank_first(rs, rcounts, cands_to_ignore, c) >= strict_maj_size]
      
     return sorted(winners)
 
 
 @vm(name = "Instant Runoff PUT")
 def instant_runoff_put(profile, curr_cands = None):
-    """Instant Runoff (:fun:`instant_runoff`) with parallel universe tie-breaking (PUT).  Apply the Instant Runoff method with a tie-breaker for each possible linear order over the candidates. 
+    """Instant Runoff (:func:`instant_runoff`) with parallel universe tie-breaking (PUT).  Apply the Instant Runoff method with a tie-breaker for each possible linear order over the candidates. 
     
     Args:
         profile (Profile): An anonymous profile of linear orders on a set of candidates
         curr_cands (List[int], optional): If set, then find the winners for the profile restricted to the candidates in ``curr_cands``
 
     Returns: 
         A sorted list of candidates
@@ -313,22 +313,21 @@
      
     return sorted(winners), elims_list
 
 
 @vm(name="Instant Runoff")
 def instant_runoff_for_truncated_linear_orders(profile, curr_cands = None, threshold = None, hide_warnings = False): 
     """
-    Intant Runoff for Truncated Linear Orders.  Iteratively remove the candidates with the fewest number 
-    of first place votes, until there is a candidate with more than the treshold number of first-place votes. 
-    If a threshold is not set, then it is stirclty more than half of the non-empty ballots. 
+    Instant Runoff for Truncated Linear Orders.  Iteratively remove the candidates with the fewest number of first place votes, until there is a candidate with more than the threshold number of first-place votes. 
+    If a threshold is not set, then it is strictly more than half of the non-empty ballots. 
     
     Args:
         profile (ProfileWithTies): An anonymous profile with no ties in the ballots (note that ProfileWithTies allows for truncated linear orders).
-        threshold (int, float, optional): The threshold needed to win the election.  If it is not set, then it is striclty more than half of the remaining ballots.
-        hide_warnings (bool, optional): Show or hide the warnings when more than one candidate is eleminated in a round.
+        threshold (int, float, optional): The threshold needed to win the election.  If it is not set, then it is strictly more than half of the remaining ballots.
+        hide_warnings (bool, optional): Show or hide the warnings when more than one candidate is eliminated in a round.
 
     Returns: 
         A sorted list of candidates
     
     .. note:: This is the simultaneous version of instant runoff, not the parallel-universe tiebreaking version. 
     It is intended to be run on profiles with large number of voters in which there is a very low probability 
     of a tie in the fewest number of first place votes.   A warning is displayed when more than one candidate is
@@ -512,15 +511,15 @@
             winners.append(c1)
             winners.append(c2)
     
     return sorted(list(set(winners))), list(all_runoff_pairs)
 
 @vm(name = "Coombs")
 def coombs(profile, curr_cands = None):
-    """If there is a majority winner then that candidate is the Coombs winner.     If there is no majority winner, then remove all candidates that are ranked last by the greatest number of voters.  Continue removing candidates with the most last-place votes until there is a candidate with a majority of first place votes.  
+    """If there is a majority winner then that candidate is the Coombs winner.   If there is no majority winner, then remove all candidates that are ranked last by the greatest number of voters.  Continue removing candidates with the most last-place votes until there is a candidate with a majority of first place votes.  
     
     .. important::
         If there is  more than one candidate with the largest number of last-place votes, then *all* such candidates are removed from the profile. 
     
     Args:
         profile (Profile): An anonymous profile of linear orders on a set of candidates
         curr_cands (List[int], optional): If set, then find the winners for the profile restricted to the candidates in ``curr_cands``
@@ -698,15 +697,15 @@
     
     rs, rcounts = profile.rankings_counts # get all the ranking data
     
     winners = [c for c in candidates 
                if _num_rank_first(rs, rcounts, np.empty(0), c) >= strict_maj_size]
 
     if len(winners) == 0:
-        # run Coombs with tie-breaker for each permulation of candidates
+        # run Coombs with tie-breaker for each permutation of candidates
         for tb in permutations(candidates):
             winners += coombs_tb(profile, curr_cands = curr_cands, tie_breaker = tb) 
 
     return sorted(list(set(winners)))
 
 def coombs_with_explanation(profile, curr_cands = None):
     """
@@ -984,15 +983,15 @@
         for tb in permutations(candidates):
             winners += baldwin_tb(profile, curr_cands = curr_cands, tie_breaker = tb) 
 
     return sorted(list(set(winners)))
 
 
 def baldwin_with_explanation(profile, curr_cands = None):
-    """Baldwin with an explanation. In addition to the winner(s), return the order in which the candidates are eliminated as a list of dictionaries specifying the Borda scores in the profile resctricted to the candidates that have not been eliminated.    
+    """Baldwin with an explanation. In addition to the winner(s), return the order in which the candidates are eliminated as a list of dictionaries specifying the Borda scores in the profile restricted to the candidates that have not been eliminated.    
 
     Args:
         profile (Profile): An anonymous profile of linear orders on a set of candidates
         curr_cands (List[int], optional): If set, then find the winners for the profile restricted to the candidates in ``curr_cands``
 
     Returns: 
         A sorted list of candidates
@@ -1133,15 +1132,15 @@
         else:
             updated_rankings = _find_updated_profile(rankings, cands_to_ignore, num_cands)
             
     return winners
 
 
 def strict_nanson_with_explanation(profile, curr_cands = None):
-    """Strict Nanson with an explanation. In addition to the winner(s), return the order in which the candidates are eliminated as a list of dictionaries specifying the Borda scores in the profile resctricted to the candidates that have not been eliminated and the average Borda score.    
+    """Strict Nanson with an explanation. In addition to the winner(s), return the order in which the candidates are eliminated as a list of dictionaries specifying the Borda scores in the profile restricted to the candidates that have not been eliminated and the average Borda score.    
     
     Args:
         profile (Profile): An anonymous profile of linear orders on a set of candidates
         curr_cands (List[int], optional): If set, then find the winners for the profile restricted to the candidates in ``curr_cands``
 
     Returns: 
         A sorted list of candidates
@@ -1288,15 +1287,15 @@
             updated_rankings = _find_updated_profile(rankings, cands_to_ignore, num_cands)
             
     return winners
 
 
 def weak_nanson_with_explanation(profile, curr_cands = None):
     """
-    Weak Nanson with an explanation. In addition to the winner(s), return the order in which the candidates are eliminated as a list of dictionaries specifying the Borda scores in the profile resctricted to the candidates that have not been eliminated and the average Borda score.    
+    Weak Nanson with an explanation. In addition to the winner(s), return the order in which the candidates are eliminated as a list of dictionaries specifying the Borda scores in the profile restricted to the candidates that have not been eliminated and the average Borda score.    
     
     Args:
         profile (Profile): An anonymous profile of linear orders on a set of candidates
         curr_cands (List[int], optional): If set, then find the winners for the profile restricted to the candidates in ``curr_cands``
 
     Returns: 
         A sorted list of candidates
@@ -1513,15 +1512,15 @@
         curr_cands (List[int], optional): If set, then find the winners for the profile restricted to the candidates in ``curr_cands``
 
     Returns: 
         A sorted list of candidates
 
     .. seealso::
 
-        Related functions:  :func:`pref_voting.iterative_methods.benahm_put`
+        Related functions:  :func:`pref_voting.iterative_methods.benham_put`
 
     """
 
     # need the total number of all candidates in a profile to check when all candidates have been removed   
     num_cands = profile.num_cands 
     
     candidates = profile.candidates if curr_cands is None else curr_cands
@@ -1601,15 +1600,15 @@
             if cw is not None: 
                 winners = [cw]
     return sorted(winners)
 
 
 @vm(name = "Benham PUT")
 def benham_put(profile, curr_cands = None):
-    """Benham (:fun:`benham`) with parallel universe tie-breaking (PUT).  Apply the Benham method with a tie-breaker for each possible linear order over the candidates. 
+    """Benham (:func:`benham`) with parallel universe tie-breaking (PUT).  Apply the Benham method with a tie-breaker for each possible linear order over the candidates. 
     
     Args:
         profile (Profile): An anonymous profile of linear orders on a set of candidates
         curr_cands (List[int], optional): If set, then find the winners for the profile restricted to the candidates in ``curr_cands``
 
     Returns: 
         A sorted list of candidates
```

### Comparing `pref_voting-0.2.5/pref_voting/maj_graph_ex1.png` & `pref_voting-0.2.6/pref_voting/maj_graph_ex1.png`

 * *Files identical despite different names*

### Comparing `pref_voting-0.2.5/pref_voting/margin_based_methods.py` & `pref_voting-0.2.6/pref_voting/margin_based_methods.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,15 +68,15 @@
 
 def minimax_scores(edata, curr_cands = None, score_method="margins"):
     """Return the minimax scores for each candidate, where the minimax score for :math:`c` is -1 * the maximum pairwise majority loss. 
 
     Args:
         edata (Profile, ProfileWithTies, MarginGraph): Any election data that has a `margin` method. 
         curr_cands (List[int], optional): If set, then find the winners for the profile restricted to the candidates in ``curr_cands``
-        score_method (str, optional): Options include "margins" (the default), "winning" assings to each candidate :math:`c` the maximum support of a candidate majority preferred to :math:`c`,  and "pairwise_opposition" assings to each candidate :math:`c` the maximum support of any candidate over :math:`c`.   These scores only lead to different results on non-linear profiles. 
+        score_method (str, optional): Options include "margins" (the default), "winning" assigns to each candidate :math:`c` the maximum support of a candidate majority preferred to :math:`c`,  and "pairwise_opposition" assigns to each candidate :math:`c` the maximum support of any candidate over :math:`c`.   These scores only lead to different results on non-linear profiles. 
 
     Returns: 
         A dictionary associating each candidate with its minimax score.
 
     .. seealso::
 
         :meth:`pref_voting.margin_based_methods.minimax`
@@ -1164,15 +1164,15 @@
     """
     
     return sorted(_simple_stable_voting(edata, curr_cands = curr_cands, mem_sv_winners = {}, strength_function = strength_function)[0])
 
 
 @vm(name = "Simple Stable Voting")
 def simple_stable_voting_faster(edata, curr_cands = None, strength_function = None): 
-    """Simple Stable Voting is Condorcet consistent.   It is faster to skip executing the recursive algorithm when there is a Condorcet winnerFirst check if there is a Condorcet winner.  If so, return the Condorcet winner, otherwise find the Simple Stable Voting winnner using _simple_stable_voting
+    """Simple Stable Voting is Condorcet consistent.   It is faster to skip executing the recursive algorithm when there is a Condorcet winnerFirst check if there is a Condorcet winner.  If so, return the Condorcet winner, otherwise find the Simple Stable Voting winner using _simple_stable_voting
 
     Args:
         edata (Profile, ProfileWithTies, MarginGraph): Any election data that has a `margin` method. 
         curr_cands (List[int], optional): If set, then find the winners for the profile restricted to the candidates in ``curr_cands``
         strength_function (function, optional): The strength function to be used to calculate the strength of a path.   The default is the margin method of ``edata``.   This only matters when the ballots are not linear orders. 
 
     Returns:
```

### Comparing `pref_voting-0.2.5/pref_voting/other_methods.py` & `pref_voting-0.2.6/pref_voting/other_methods.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 @vm(name = "Majority")
 def majority(profile, curr_cands = None):
     """The majority winner is the candidate with a strict majority  of first place votes.  Returns an empty list if there is no candidate with a strict majority of first place votes. Returns the majority winner in the ``profile`` restricted to ``curr_cands``.
 
     Args:
         profile (Profile): An anonymous profile of linear orders on a set of candidates
-        curr_cands (List[int], optional): If set, then find the winners for the profile restrcited to the candidates in ``curr_cands``
+        curr_cands (List[int], optional): If set, then find the winners for the profile restricted to the candidates in ``curr_cands``
 
     Returns: 
         A sorted list of candidates
 
     .. important:: 
         Formally, this is *not* a voting method since the function might return an empty list (when there is no candidate with a strict majority of first place votes).  Also, if there is a majority winner, then that winner is unique. 
 
@@ -196,15 +196,15 @@
     return sorted(list(set([p[0] for p in maximal_paths]))), maximal_paths
 
 ## Slater
 #
 
 def distance_to_margin_graph(edata, rel, exp = 1, curr_cands = None): 
     """
-    Calclulate the distance of ``rel`` (a relation) to the majority graph of ``edata``. 
+    Calculate the distance of ``rel`` (a relation) to the majority graph of ``edata``. 
     """
     candidates = edata.candidates if curr_cands is None else curr_cands
     
     penalty = 0
     for a,b in combinations(candidates, 2): 
         if edata.majority_prefers(a, b) and (b,a) in rel: 
             penalty += (edata.margin(a, b) ** exp)
@@ -227,15 +227,15 @@
         elif lin_order.index(b) < lin_order.index(a): 
             rel.append((b,a))     
     return rel
 
 
 def slater_rankings(edata, curr_cands = None): 
     """
-    A Slater ranking is a linear order :math:`R` of the candidates that minimises the number of edges in the majority graph we have to turn around before we obtain :math:`R`. 
+    A Slater ranking is a linear order :math:`R` of the candidates that minimizes the number of edges in the majority graph we have to turn around before we obtain :math:`R`. 
 
     Args:
         edata (Profile, ProfileWithTies, MarginGraph): Any election data that has a `margin` method. 
         curr_cands (List[int], optional): If set, then find the winners for the profile restricted to the candidates in ``curr_cands``
 
     Returns: 
         rankings: A list of Slater rankings.
@@ -270,15 +270,15 @@
         elif dist == min_dist: 
             rankings.append(lin_order)
     return rankings, min_dist
 
         
 @vm(name = "Slater")
 def slater(edata, curr_cands = None): 
-    """A Slater ranking is a linear order :math:`R` of the candidates that minimises the number of edges in the majority graph we have to turn around before we obtain :math:`R`.   A candidate is a Slater winner if the candidate is the top element of some Slater ranking.
+    """A Slater ranking is a linear order :math:`R` of the candidates that minimizes the number of edges in the majority graph we have to turn around before we obtain :math:`R`.   A candidate is a Slater winner if the candidate is the top element of some Slater ranking.
 
     Args:
         edata (Profile, ProfileWithTies, MarginGraph): Any election data that has a `margin` method. 
         curr_cands (List[int], optional): If set, then find the winners for the profile restricted to the candidates in ``curr_cands``
 
     Returns: 
         A sorted list of candidates
@@ -340,15 +340,15 @@
 
 def kemmeny_young_rankings(profile, curr_cands = None): 
     """
     A Kemmeny-Young ranking is a ranking that minimizes the sum of the Kendall tau distances to the voters' rankings.  
     
     Args:
         profile (Profile): An anonymous profile of linear orders on a set of candidates
-        curr_cands (List[int], optional): If set, then find the winners for the profile restrcited to the candidates in ``curr_cands``
+        curr_cands (List[int], optional): If set, then find the winners for the profile restricted to the candidates in ``curr_cands``
 
     Returns: 
         rankings: A list of Slater rankings.
         
         dist: The minimum distance of the Slater rankings.
 
 
@@ -381,15 +381,15 @@
 
 @vm(name = "Kemmeny-Young")
 def kemmeny_young(profile, curr_cands = None): 
     """A Kemmeny-Young ranking is a ranking that minimizes the sum of the Kendall tau distances to the voters' rankings.  The Kemmeny-Young winners are the candidates that are ranked first by some Kemmeny-Young ranking.
 
     Args:
         profile (Profile): An anonymous profile of linear orders on a set of candidates
-        curr_cands (List[int], optional): If set, then find the winners for the profile restrcited to the candidates in ``curr_cands``
+        curr_cands (List[int], optional): If set, then find the winners for the profile restricted to the candidates in ``curr_cands``
 
     Returns: 
         A sorted list of candidates
 
     :Example:
 
         .. exec_code::
@@ -426,15 +426,15 @@
 
 @vm(name = "Bucklin")
 def bucklin(profile, curr_cands = None): 
     """If a candidate has a strict majority of first-place votes, then that candidate is the winner. If no such candidate exists, then check the candidates that are ranked first or second.  If a candidate has a strict majority of first- or second-place voters, then that candidate is the winner. If no such winner is found move on to the 3rd, 4th, etc. place votes.  Return the candidates with the greatest overall score.  
     
     Args:
         profile (Profile): An anonymous profile of linear orders on a set of candidates
-        curr_cands (List[int], optional): If set, then find the winners for the profile restrcited to the candidates in ``curr_cands``
+        curr_cands (List[int], optional): If set, then find the winners for the profile restricted to the candidates in ``curr_cands``
 
     Returns: 
         A sorted list of candidates
 
     :Example: 
 
     .. exec_code:: 
@@ -474,15 +474,15 @@
 
 
 def bucklin_with_explanation(profile, curr_cands = None): 
     """Return the Bucklin winners and the score for each candidate. 
  
     Args:
         profile (Profile): An anonymous profile of linear orders on a set of candidates
-        curr_cands (List[int], optional): If set, then find the winners for the profile restrcited to the candidates in ``curr_cands``
+        curr_cands (List[int], optional): If set, then find the winners for the profile restricted to the candidates in ``curr_cands``
 
     Returns: 
 
         A sorted list of candidates
 
         A dictionary assigning the score for each candidate. 
 
@@ -530,15 +530,15 @@
 
 @vm(name = "Simplified Bucklin")
 def simplified_bucklin(profile, curr_cands = None): 
     """If a candidate has a strict majority of first-place votes, then that candidate is the winner. If no such candidate exists, then check the candidates that are ranked first or second.  If a candidate has a strict majority of first- or second-place voters, then that candidate is the winner. If no such winner is found move on to the 3rd, 4th, etc. place votes. 
 
     Args:
         profile (Profile): An anonymous profile of linear orders on a set of candidates
-        curr_cands (List[int], optional): If set, then find the winners for the profile restrcited to the candidates in ``curr_cands``
+        curr_cands (List[int], optional): If set, then find the winners for the profile restricted to the candidates in ``curr_cands``
 
     Returns: 
         A sorted list of candidates
 
     :Example: 
 
     .. exec_code:: 
@@ -577,15 +577,15 @@
     return sorted([c for c in candidates if cand_scores[c] >= strict_maj_size])
 
 def simplified_bucklin_with_explanation(profile, curr_cands = None): 
     """Return the Simplified Bucklin winners and the score for each candidate. 
  
     Args:
         profile (Profile): An anonymous profile of linear orders on a set of candidates
-        curr_cands (List[int], optional): If set, then find the winners for the profile restrcited to the candidates in ``curr_cands``
+        curr_cands (List[int], optional): If set, then find the winners for the profile restricted to the candidates in ``curr_cands``
 
     Returns: 
 
         A sorted list of candidates
 
         A dictionary assigning the score for each candidate. 
 
@@ -632,15 +632,15 @@
 
 @vm(name = "Weighted Bucklin")
 def weighted_bucklin(profile, curr_cands = None, strict_threshold = False, score = lambda num_cands, rank: (num_cands - rank)/ (num_cands - 1) if num_cands > 1 else 1): 
     """The Weighted Bucklin procedure, studied by D. Marc Kilgour, Jean-Charles Grégoire, and Angèle Foley. The k-th Weighted Bucklin score of a candidate c is the sum for j \leq k of the product of score(num_cands,j) and the number of voters who rank c in j-th place. Compute higher-order Weighted Bucklin scores until reaching a k such that some candidate's k-th Weighted Bucklin score is at least half the number of voters (or the strict majority size if strict_threshold = True). Then return the candidates with maximal k-th Weighted Bucklin score. Bucklin is the special case where strict_threshold = True and score = lambda num_cands, rank: 1.
     
     Args:
         profile (Profile): An anonymous profile of linear orders on a set of candidates
-        curr_cands (List[int], optional): If set, then find the winners for the profile restrcited to the candidates in ``curr_cands``
+        curr_cands (List[int], optional): If set, then find the winners for the profile restricted to the candidates in ``curr_cands``
         strict_threshold: If True, makes the threshold for the Bucklin procedure the strict majority size; otherwise threshold is half the number of voters, following Kilgour et al.
         score (function): A function that accepts two parameters ``num_cands`` (the number of candidates) and ``rank`` (a rank of a candidate) used to calculate the score of a candidate. The default ``score`` function is the normalized version of the classic Borda score vector.
 
     Returns: 
         A sorted list of candidates
 
     :Example:
```

### Comparing `pref_voting-0.2.5/pref_voting/pr_voting_methods.py` & `pref_voting-0.2.6/pref_voting/pr_voting_methods.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 '''
     File: pr_voting_methods.py
     Author: Eric Pacuit (epacuit@umd.edu)
     Date: April 5, 2021
     
     Implementations of probabilistic voting methods.   
-    Propbabilistic voting methods returns a lottery over the candidates of a profile, 
+    Probabilistic voting methods returns a lottery over the candidates of a profile, 
     where a lottery is represented as a dictionary assigning elements from [0,1]
     to  the candidates that sums to 1.  
 '''
 
 import numpy as np
 import os
 import uuid
```

### Comparing `pref_voting-0.2.5/pref_voting/profiles.py` & `pref_voting-0.2.6/pref_voting/profiles.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.2.5/pref_voting/profiles_with_ties.py` & `pref_voting-0.2.6/pref_voting/profiles_with_ties.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.2.5/pref_voting/scoring_methods.py` & `pref_voting-0.2.6/pref_voting/scoring_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.2.5/pref_voting/voting_method.py` & `pref_voting-0.2.6/pref_voting/voting_method.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.2.5/pref_voting/weighted_majority_graphs.py` & `pref_voting-0.2.6/pref_voting/weighted_majority_graphs.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 class MajorityGraph(object):
     """A majority graph is an asymmetric directed graph.  The nodes are the candidates and an edge from candidate :math:`c` to :math:`d` means that :math:`c` is majority preferred to :math:`d`.
 
     :param candidates: List of the candidates.  To be used as nodes in the majority graph.
     :type candidates: list[int] or  list[str]
     :param edges: List of the pairs of candidates describing the edges in the majority graph.   If :math:`(c,d)` is in the list of edges, then there is an edge from :math:`c` to :math:`d`.
     :type edges: list
-    :param cmap: Dictionary mapping candidates to candidate names (strings).  If not provied, each candidate name is mapped to itself.
+    :param cmap: Dictionary mapping candidates to candidate names (strings).  If not provided, each candidate name is mapped to itself.
     :type cmap: dict[int: str], optional
 
     :Example:
 
     The following code creates a majority graph in which 0 is majority preferred to 1, 1 is majority preferred to 2, and 2 is majority preferred to 0:
 
     .. code-block:: python
@@ -428,15 +428,15 @@
 class MarginGraph(MajorityGraph):
     """A margin graph is a weighted asymmetric directed graph.  The nodes are the candidates and an edge from candidate :math:`c` to :math:`d` with weight :math:`w` means that :math:`c` is majority preferred to :math:`d` by a **margin** of :math:`w`.
 
     :param candidates: List of the candidates.  To be used as nodes in the majority graph.
     :type candidates: list[int] or  list[str]
     :param w_edges: List of the pairs of candidates describing the edges in the majority graph.   If :math:`(c,d,w)` is in the list of edges, then there is an edge from :math:`c` to :math:`d` with weight :math:`w`.
     :type w_edges: list
-    :param cmap: Dictionary mapping candidates to candidate names (strings).  If not provied, each candidate name is mapped to itself.
+    :param cmap: Dictionary mapping candidates to candidate names (strings).  If not provided, each candidate name is mapped to itself.
     :type cmap: dict[int: str], optional
 
     :Example:
 
     The following code creates a margin graph in which 0 is majority preferred to 1 by a margin of 1, 1 is majority preferred to 2 by a margin of 3, and 2 is majority preferred to 0 by a margin of 5:
 
     .. code-block:: python
@@ -641,15 +641,15 @@
     ):
         """
         Display the margin graph with any edges that are  ``defeat`` edges highlighted in blue.
 
         Args:
             defeat (networkx.DiGraph): The defeat relation represented as a networkx object.
             curr_cands (List[int], optional): If set, then use the defeat relation for the profile restricted to the candidates in ``curr_cands``
-            show_undfeated (bool, optional): If true, color the undefeated candidates blue and the other candidates red.
+            show_undefeated (bool, optional): If true, color the undefeated candidates blue and the other candidates red.
             cmap (dict, optional): The cmap used to map candidates to candidate names
 
 
         """
 
         cmap = cmap if cmap is not None else self.cmap
         cmap_inverse = {cname: c for c, cname in cmap.items()}
@@ -852,17 +852,17 @@
 
 
 class SupportGraph(MajorityGraph):
     """A support graph is a weighted asymmetric directed graph.  The nodes are the candidates and an edge from candidate :math:`c` to :math:`d` with weight :math:`w` means that the **support** of  :math:`c` over :math:`d` is :math:`w`.
 
     :param candidates: List of the candidates.  To be used as nodes in the majority graph.
     :type candidates: list[int] or  list[str]
-    :param w_edges: List representing the edges in the majority graph with supports. If :math:`(c,d,(n,m))` is in the list of edges, then there is an edge from :math:`c` to :math:`d`, the suppoer for :math:`c` over :math:`d` is :math:`n`, and the support for :math:`d` over :math:`c` is :math:`m`. 
+    :param w_edges: List representing the edges in the majority graph with supports. If :math:`(c,d,(n,m))` is in the list of edges, then there is an edge from :math:`c` to :math:`d`, the support for :math:`c` over :math:`d` is :math:`n`, and the support for :math:`d` over :math:`c` is :math:`m`. 
     :type w_edges: list
-    :param cmap: Dictionary mapping candidates to candidate names (strings).  If not provied, each candidate name is mapped to itself.
+    :param cmap: Dictionary mapping candidates to candidate names (strings).  If not provided, each candidate name is mapped to itself.
     :type cmap: dict[int: str], optional
 
     :Example:
 
     The following code creates a support graph in which:
 
     - 0 is majority preferred to 1, the number of voters who rank 0 over 1 is 4, and the number of voters who rank 1 over 0 is 3;
@@ -1041,15 +1041,15 @@
                 for c2 in profile.candidates
             ],
             cmap=cmap,
         )
 
 
 ###
-# funcitons to display graphs in tikz
+# functions to display graphs in tikz
 ##
 def three_cand_tikz_str(g, cmap=None):
     """Returns the TikZ code to display the graph ``g`` based on 3 candidates (may be a MajorityGraph, MarginGraph or a SupportGraph)."""
 
     a = g.candidates[0]
     b = g.candidates[1]
     c = g.candidates[2]
```

### Comparing `pref_voting-0.2.5/pyproject.toml` & `pref_voting-0.2.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=42",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [tool.poetry]
 name = "pref_voting"
-version = "0.2.5"
+version = "0.2.6"
 description = "pref_voting is a Python packaging that contains tools to reason about election profiles and margin graphs, and implementations of a variety of preferential voting methods."
 authors = ["Eric Pacuit <epacuit@umd.edu>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/voting-tools/pref_voting"
 repository = "https://github.com/voting-tools/pref_voting"
```

### Comparing `pref_voting-0.2.5/setup.py` & `pref_voting-0.2.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,17 +12,17 @@
  'networkx>=3.0,<4.0',
  'random2>=1.0.1,<2.0.0',
  'scipy>=1.0.0,<2.0.0',
  'tabulate>=0.9.0,<0.10.0']
 
 setup_kwargs = {
     'name': 'pref-voting',
-    'version': '0.2.5',
+    'version': '0.2.6',
     'description': 'pref_voting is a Python packaging that contains tools to reason about election profiles and margin graphs, and implementations of a variety of preferential voting methods.',
-    'long_description': 'pref_voting\n==========\n\n## Installation\n\nWith pip package manager:\n\n```bash\npip install pref_voting\n```\n## Documentation\n\nOnline documentation is available at [https://pref_voting.readthedocs.io](https://pref_voting.readthedocs.io).\n\n## Profiles and Voting Methods\n\nA profile (of linear orders over the candidates) is created by initializing a Profile class object.  This needs a list of rankings (each ranking is a tuple of numbers), the number of candidates, and a list giving the number of each ranking in the profile:\n\n```python\nfrom pref_voting.profiles import Profile\n\nrankings = [(0, 1, 2, 3), (2, 3, 1, 0), (3, 1, 2, 0), (1, 2, 0, 3), (1, 3, 2, 0)]\nrcounts = [5, 3, 2, 4, 3]\n\nprof = Profile(rankings, rcounts=rcounts)\n```\n\nThe function generate_profile is used to generate a profile for a given number of candidates and voters:  \n```python\nfrom pref_voting.generate_profiles import generate_profile\n\n# generate a profile using the Impartial Culture probability model\nprof = generate_profile(3, 4) # prof is a Profile object\n\n# generate a profile using the Impartial Anonymous Culture probability model\nprof = generate_profile(3, 4, probmod = "IAC") # prof is a Profile object \n```\n\n```python\nfrom pref_voting.profiles import Profile\nfrom pref_voting.voting_methods import *\n\nprof = Profile(rankings, num_cands, rcounts=rcounts)\nprint(f"{split_cycle.name} winners:  {split_cycle(prof)}")\nsplit_cycle.display(prof)\n\n```\n\n## Versions\n\n- v0.1.10 (2022-08-09): **Initial release** \n- v0.1.13 (2022-11-05): Minor updates and bug fixes \n- v0.1.14 (2022-12-19): Add plurality_scores to ProfileWithTies; add generate ceots function; bug fixes \n- v0.1.23 (2022-12-27): Add instant_runoff_for_truncated_linear_orders and functions to truncate overvotes in a ProfileWithTies, add smith_irv_put, document analysis functions\n- v0.1.25 (2023-1-11): Add condorcet_irv, condorcet_irv_put; Update documentation; add axioms.py; add display and equality to Ranking class; fix enumerate ceots functions\n- v0.1.27 (2023-2-07): Add Borda for ProfileWithTies\n- v0.2 (2023-2-15): Add Benham, add anonymize to Profile method, comment out numba to make compatible with Python 3.11, add add_unranked_candidates to ProfileWithTies\n- v0.2.1 (2023-2-15): Bug fixes\n- v0.2.3 (2023-4-2): Add plurality_with_runoff_with_explanation\n- v0.2.4 (2023-4-9): Update generate_truncated_profile so that it implements the IC probability model.\n- v0.2.5 (2023-5-10): Add axiom class, dominance axioms, and axiom_violations_data.\n\n## Questions?\n\nFeel free to [send me an email](https://pacuit.org/) if you have questions about the project.\n\n## License\n\n[MIT](https://github.com/jontingvold/pyrankvote/blob/master/LICENSE.txt)\n',
+    'long_description': 'pref_voting\n==========\n\n## Installation\n\nWith pip package manager:\n\n```bash\npip install pref_voting\n```\n## Documentation\n\nOnline documentation is available at [https://pref_voting.readthedocs.io](https://pref_voting.readthedocs.io).\n\n## Profiles and Voting Methods\n\nA profile (of linear orders over the candidates) is created by initializing a Profile class object.  This needs a list of rankings (each ranking is a tuple of numbers), the number of candidates, and a list giving the number of each ranking in the profile:\n\n```python\nfrom pref_voting.profiles import Profile\n\nrankings = [(0, 1, 2, 3), (2, 3, 1, 0), (3, 1, 2, 0), (1, 2, 0, 3), (1, 3, 2, 0)]\nrcounts = [5, 3, 2, 4, 3]\n\nprof = Profile(rankings, rcounts=rcounts)\n```\n\nThe function generate_profile is used to generate a profile for a given number of candidates and voters:  \n```python\nfrom pref_voting.generate_profiles import generate_profile\n\n# generate a profile using the Impartial Culture probability model\nprof = generate_profile(3, 4) # prof is a Profile object\n\n# generate a profile using the Impartial Anonymous Culture probability model\nprof = generate_profile(3, 4, probmod = "IAC") # prof is a Profile object \n```\n\n```python\nfrom pref_voting.profiles import Profile\nfrom pref_voting.voting_methods import *\n\nprof = Profile(rankings, num_cands, rcounts=rcounts)\nprint(f"{split_cycle.name} winners:  {split_cycle(prof)}")\nsplit_cycle.display(prof)\n\n```\n\n## Versions\n\n- v0.1.10 (2022-08-09): **Initial release** \n- v0.1.13 (2022-11-05): Minor updates and bug fixes \n- v0.1.14 (2022-12-19): Add plurality_scores to ProfileWithTies; add generate ceots function; bug fixes \n- v0.1.23 (2022-12-27): Add instant_runoff_for_truncated_linear_orders and functions to truncate overvotes in a ProfileWithTies, add smith_irv_put, document analysis functions\n- v0.1.25 (2023-1-11): Add condorcet_irv, condorcet_irv_put; Update documentation; add axioms.py; add display and equality to Ranking class; fix enumerate ceots functions\n- v0.1.27 (2023-2-07): Add Borda for ProfileWithTies\n- v0.2 (2023-2-15): Add Benham, add anonymize to Profile method, comment out numba to make compatible with Python 3.11, add add_unranked_candidates to ProfileWithTies\n- v0.2.1 (2023-2-15): Bug fixes\n- v0.2.3 (2023-4-2): Add plurality_with_runoff_with_explanation\n- v0.2.4 (2023-4-9): Update generate_truncated_profile so that it implements the IC probability model.\n- v0.2.6 (2023-5-10): Add axiom class, dominance axioms, and axiom_violations_data.\n\n## Questions?\n\nFeel free to [send me an email](https://pacuit.org/) if you have questions about the project.\n\n## License\n\n[MIT](https://github.com/jontingvold/pyrankvote/blob/master/LICENSE.txt)\n',
     'author': 'Eric Pacuit',
     'author_email': 'epacuit@umd.edu',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/voting-tools/pref_voting',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `pref_voting-0.2.5/PKG-INFO` & `pref_voting-0.2.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pref-voting
-Version: 0.2.5
+Version: 0.2.6
 Summary: pref_voting is a Python packaging that contains tools to reason about election profiles and margin graphs, and implementations of a variety of preferential voting methods.
 Home-page: https://github.com/voting-tools/pref_voting
 License: MIT
 Author: Eric Pacuit
 Author-email: epacuit@umd.edu
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -79,15 +79,15 @@
 - v0.1.23 (2022-12-27): Add instant_runoff_for_truncated_linear_orders and functions to truncate overvotes in a ProfileWithTies, add smith_irv_put, document analysis functions
 - v0.1.25 (2023-1-11): Add condorcet_irv, condorcet_irv_put; Update documentation; add axioms.py; add display and equality to Ranking class; fix enumerate ceots functions
 - v0.1.27 (2023-2-07): Add Borda for ProfileWithTies
 - v0.2 (2023-2-15): Add Benham, add anonymize to Profile method, comment out numba to make compatible with Python 3.11, add add_unranked_candidates to ProfileWithTies
 - v0.2.1 (2023-2-15): Bug fixes
 - v0.2.3 (2023-4-2): Add plurality_with_runoff_with_explanation
 - v0.2.4 (2023-4-9): Update generate_truncated_profile so that it implements the IC probability model.
-- v0.2.5 (2023-5-10): Add axiom class, dominance axioms, and axiom_violations_data.
+- v0.2.6 (2023-5-10): Add axiom class, dominance axioms, and axiom_violations_data.
 
 ## Questions?
 
 Feel free to [send me an email](https://pacuit.org/) if you have questions about the project.
 
 ## License
```

