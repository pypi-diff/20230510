# Comparing `tmp/fstflowchat-0.0.6.tar.gz` & `tmp/fstflowchat-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fstflowchat-0.0.6.tar", last modified: Wed May 10 01:39:55 2023, max compression
+gzip compressed data, was "fstflowchat-0.0.7.tar", last modified: Wed May 10 02:46:06 2023, max compression
```

## Comparing `fstflowchat-0.0.6.tar` & `fstflowchat-0.0.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 kaze7539   (503) staff       (20)        0 2023-05-10 01:39:55.355319 fstflowchat-0.0.6/
--rw-r--r--   0 kaze7539   (503) staff       (20)     1071 2023-04-19 21:48:08.000000 fstflowchat-0.0.6/LICENSE
--rw-r--r--   0 kaze7539   (503) staff       (20)       28 2023-04-24 01:28:18.000000 fstflowchat-0.0.6/MANIFEST.in
--rw-r--r--   0 kaze7539   (503) staff       (20)     3321 2023-05-10 01:39:55.354382 fstflowchat-0.0.6/PKG-INFO
--rw-r--r--   0 kaze7539   (503) staff       (20)     2180 2023-05-08 16:46:47.000000 fstflowchat-0.0.6/README.md
--rw-r--r--   0 kaze7539   (503) staff       (20)       38 2023-05-10 01:39:55.355511 fstflowchat-0.0.6/setup.cfg
--rwxr-xr-x   0 kaze7539   (503) staff       (20)     8199 2023-05-10 01:39:38.000000 fstflowchat-0.0.6/setup.py
-drwxr-xr-x   0 kaze7539   (503) staff       (20)        0 2023-05-10 01:39:55.322375 fstflowchat-0.0.6/src/
-drwxr-xr-x   0 kaze7539   (503) staff       (20)        0 2023-05-10 01:39:55.342918 fstflowchat-0.0.6/src/fstflowchat/
--rw-r--r--   0 kaze7539   (503) staff       (20)     4384 2023-05-02 20:40:08.000000 fstflowchat-0.0.6/src/fstflowchat/__init__.py
--rw-r--r--   0 kaze7539   (503) staff       (20)     7200 2023-04-24 01:50:56.000000 fstflowchat-0.0.6/src/fstflowchat/example.py
--rw-r--r--   0 kaze7539   (503) staff       (20)      795 2023-04-23 23:37:09.000000 fstflowchat-0.0.6/src/fstflowchat/quiz.dot
-drwxr-xr-x   0 kaze7539   (503) staff       (20)        0 2023-05-10 01:39:55.353342 fstflowchat-0.0.6/src/fstflowchat.egg-info/
--rw-r--r--   0 kaze7539   (503) staff       (20)     3321 2023-05-10 01:39:55.000000 fstflowchat-0.0.6/src/fstflowchat.egg-info/PKG-INFO
--rw-r--r--   0 kaze7539   (503) staff       (20)      354 2023-05-10 01:39:55.000000 fstflowchat-0.0.6/src/fstflowchat.egg-info/SOURCES.txt
--rw-r--r--   0 kaze7539   (503) staff       (20)        1 2023-05-10 01:39:55.000000 fstflowchat-0.0.6/src/fstflowchat.egg-info/dependency_links.txt
--rw-r--r--   0 kaze7539   (503) staff       (20)       65 2023-05-10 01:39:55.000000 fstflowchat-0.0.6/src/fstflowchat.egg-info/entry_points.txt
--rw-r--r--   0 kaze7539   (503) staff       (20)       16 2023-05-10 01:39:55.000000 fstflowchat-0.0.6/src/fstflowchat.egg-info/requires.txt
--rw-r--r--   0 kaze7539   (503) staff       (20)       12 2023-05-10 01:39:55.000000 fstflowchat-0.0.6/src/fstflowchat.egg-info/top_level.txt
+drwxr-xr-x   0 kaze7539   (503) staff       (20)        0 2023-05-10 02:46:06.449325 fstflowchat-0.0.7/
+-rw-r--r--   0 kaze7539   (503) staff       (20)     1071 2023-04-19 21:48:08.000000 fstflowchat-0.0.7/LICENSE
+-rw-r--r--   0 kaze7539   (503) staff       (20)       28 2023-04-24 01:28:18.000000 fstflowchat-0.0.7/MANIFEST.in
+-rw-r--r--   0 kaze7539   (503) staff       (20)     3321 2023-05-10 02:46:06.448030 fstflowchat-0.0.7/PKG-INFO
+-rw-r--r--   0 kaze7539   (503) staff       (20)     2180 2023-05-08 16:46:47.000000 fstflowchat-0.0.7/README.md
+-rw-r--r--   0 kaze7539   (503) staff       (20)       38 2023-05-10 02:46:06.449530 fstflowchat-0.0.7/setup.cfg
+-rwxr-xr-x   0 kaze7539   (503) staff       (20)     8199 2023-05-10 02:45:38.000000 fstflowchat-0.0.7/setup.py
+drwxr-xr-x   0 kaze7539   (503) staff       (20)        0 2023-05-10 02:46:06.402384 fstflowchat-0.0.7/src/
+drwxr-xr-x   0 kaze7539   (503) staff       (20)        0 2023-05-10 02:46:06.434444 fstflowchat-0.0.7/src/fstflowchat/
+-rw-r--r--   0 kaze7539   (503) staff       (20)     4384 2023-05-02 20:40:08.000000 fstflowchat-0.0.7/src/fstflowchat/__init__.py
+-rw-r--r--   0 kaze7539   (503) staff       (20)     5949 2023-05-10 02:44:10.000000 fstflowchat-0.0.7/src/fstflowchat/example.py
+-rw-r--r--   0 kaze7539   (503) staff       (20)      795 2023-04-23 23:37:09.000000 fstflowchat-0.0.7/src/fstflowchat/quiz.dot
+drwxr-xr-x   0 kaze7539   (503) staff       (20)        0 2023-05-10 02:46:06.445747 fstflowchat-0.0.7/src/fstflowchat.egg-info/
+-rw-r--r--   0 kaze7539   (503) staff       (20)     3321 2023-05-10 02:46:06.000000 fstflowchat-0.0.7/src/fstflowchat.egg-info/PKG-INFO
+-rw-r--r--   0 kaze7539   (503) staff       (20)      354 2023-05-10 02:46:06.000000 fstflowchat-0.0.7/src/fstflowchat.egg-info/SOURCES.txt
+-rw-r--r--   0 kaze7539   (503) staff       (20)        1 2023-05-10 02:46:06.000000 fstflowchat-0.0.7/src/fstflowchat.egg-info/dependency_links.txt
+-rw-r--r--   0 kaze7539   (503) staff       (20)       65 2023-05-10 02:46:06.000000 fstflowchat-0.0.7/src/fstflowchat.egg-info/entry_points.txt
+-rw-r--r--   0 kaze7539   (503) staff       (20)       16 2023-05-10 02:46:06.000000 fstflowchat-0.0.7/src/fstflowchat.egg-info/requires.txt
+-rw-r--r--   0 kaze7539   (503) staff       (20)       12 2023-05-10 02:46:06.000000 fstflowchat-0.0.7/src/fstflowchat.egg-info/top_level.txt
```

### Comparing `fstflowchat-0.0.6/LICENSE` & `fstflowchat-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `fstflowchat-0.0.6/PKG-INFO` & `fstflowchat-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fstflowchat
-Version: 0.0.6
+Version: 0.0.7
 Summary: a small, pedagogical, fst-based dialog toolkit.
 Home-page: https://fstflowchat.readthedocs.io/en/latest/
 Author: Abe Kazemzadeh
 Project-URL: Bug Reports, https://github.com/abecode/fstflowchat/issues
 Project-URL: Funding, https://donate.pypi.org
 Project-URL: Say Thanks!, http://saythanks.io/to/example
 Project-URL: Source, https://github.com/abecode/fstflowchat/issues
```

### Comparing `fstflowchat-0.0.6/README.md` & `fstflowchat-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `fstflowchat-0.0.6/setup.py` & `fstflowchat-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/guides/single-sourcing-package-version/
-    version="0.0.6",  # Required
+    version="0.0.7",  # Required
     
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description="a small, pedagogical, fst-based dialog toolkit.",  # Optional
     
     # This is an optional longer description of your project that represents
```

### Comparing `fstflowchat-0.0.6/src/fstflowchat/__init__.py` & `fstflowchat-0.0.7/src/fstflowchat/__init__.py`

 * *Files identical despite different names*

### Comparing `fstflowchat-0.0.6/src/fstflowchat/example.py` & `fstflowchat-0.0.7/src/fstflowchat/example.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,32 +1,15 @@
+#!/usr/bin/env python3
+
+from typing import Callable
 import random
-import sys
-import pygraphviz as pgv
-import pathlib
+import fstflowchat as ffc
 
 
 
-def get_graph_functions(g: pgv.agraph.AGraph):
-    """gets a list of the names of the functions referred to in the
-    graph's edges
-    """
-    fnames_out = []
-    for e in g.edges_iter():
-        print(e, e.attr['label'])
-        fnames = e.attr['label'].split(':')
-        print(fnames)
-        fnames_out.extend(fnames)
-    return fnames_out
-
-def is_implemented(fname: str) -> bool:
-    """ checks to see if there is a function named fname"""
-    if fname in globals() and callable(globals()[fname]):
-        return True
-    return False
-
 def intercept_decorator(condition):
     def decorator(f):
         def inner(input_):
             return condition(input_) and f(input_)
         return inner
     return decorator
 
@@ -60,53 +43,56 @@
 
 def ru_ready_msg(input_: str) -> str:
     return "if you're ready, say \"yes\" or \"ready\""
 
 def ask_question(input_:str) -> str:
     question_to_ask = questions.pop(0)
     previous_questions.append(question_to_ask)
-    return question_to_ask
+    return question_to_ask.text()
 
 def quiz_done_or_user_exit(input_: str) -> bool:
     if quiz_done(input_):
         return True
     if user_exit(input_):
         return True
     return False
 
 def not_quiz_done_or_user_exit(input_: str) -> bool:
     return not quiz_done_or_user_exit(input_)
 
 @intercept_decorator(not_quiz_done_or_user_exit)
 def correct_answ(input_:str) -> bool:
     global correct_count
-    if score_answer(previous_questions[-1], input_) == "correct":
+    ##if score_answer(previous_questions[-1], input_) == "correct":
+    if previous_questions[-1].score_answer(input_) == "correct":
         correct_count += 1
         return True
     return False
 
 @intercept_decorator(not_quiz_done_or_user_exit)
 def wrong_answ(input_:str) -> bool:
-    if score_answer(previous_questions[-1], input_) == "wrong":
+    global incorrect_count
+    if previous_questions[-1].score_answer(input_) == "incorrect":
+        incorrect_count += 1
         return True
     return False
 
 @intercept_decorator(not_quiz_done_or_user_exit)
 def partially_correct(input_: str) -> bool:
     global partial_count
-    if score_answer(previous_questions[-1], input_) == "partial":
+    if previous_questions[-1].score_answer(input_) == "partial":
         partial_count += 1
         return True
     return False
 
 def feedback_then_next_question(input_: str) -> str:
     return "eh, that was a so-so answer. \n" + ask_question(input_)
 
 def feedback_drilldown_then_next_question(input_: str) -> str:
-    return "nope, pay more attention to lectures and reading\n"
+    return "wrong, pay more attention to lectures and reading\n" + ask_question(input_)
 
 def quiz_done(input_: str) -> bool:
     if len(questions) == 0:
         return True
     return False
 
 def user_exit(input_: str) -> bool:
@@ -114,137 +100,122 @@
         return True
     if "quit" in input_.lower():
         return True
     if "this sucks" in input_.lower():
         return True
     return False
 
-def score_answer(question, answer):
-    """ right now this is not implemented, just returns a random value"""
-    res =  "correct"
-    res = random.choice(["correct", "incorrect", "partial"])
-    if len(questions) == 2:
-        res = "correct"
-    if len(questions) == 1:
-        res = "partial"
-    if len(questions) == 0:
-        res = "incorrect"
-    print(f"question: {question}; answer: {answer}; result: {res}")
-    return res
 
 def give_results(input_: str) -> str:
-    return f"You got {correct_count} right, and {partial_count} partially correct"
+    return f"You got {correct_count} right, {incorrect_count} wrong, and {partial_count} partially correct"
 
 def user_asks_q(input_: str) -> bool:
     if input_.endswith("?"):
         return True
     return False
 
 def answer_question(input_: str) -> str:
     return "I'm sorry, I don't know how to answer that.  Let's just say bye and finish this."
 
 def grade_last_and_give_results(input_: str) -> bool:
     """this is is for the last question in the list, only for when we
     transition from ask_questions to after_test
 
     """
-    global correct_count, partial_count
-    res = score_answer(previous_questions[-1], input_)
+    output_ = ""
+    global correct_count, partial_count, incorrect_count
+    res = previous_questions[-1].score_answer(input_)
     if res == "correct":
         correct_count += 1
     if res == "partial":
         partial_count += 1
+        output_ = "eh, that was a so-so answer. \n"
+    if res == "incorrect":
+        incorrect_count += 1
+        output_ = "wrong, pay more attention to lectures and reading\n"
 
-    return give_results(input_)
+    return output_ + give_results(input_)
 
 def not_user_asks_q(input_: str) -> bool:
     return not user_asks_q(input_)
 
 def goodbye(input_: str) -> str:
     return "goodbye, thanks for testing the dialog system!"
 
-class FST():
-    def __init__(self, graph, start, end):
-        self.graph = graph
-        self.start = self.currentstate = start
-        self.end = end
-        self.is_running = True
-
-    def __call__(self, input_: str) -> str:
-        print(f"*******currentstate {self.currentstate}")
-        neighbor_edges = self.graph.out_edges(self.currentstate)
-        print("neighbor_edges")
-        valid_edges = []
-        output_fns = []
-        for e in neighbor_edges:
-            print(e)
-            test_fn, out_fn = e.attr['label'].split(":")
-            print("\t", test_fn, out_fn)
-            if globals()[test_fn](input_):
-                valid_edges.append(e)
-                output_fns.append(out_fn)
-        print("there are " + str(len(valid_edges)) + " valid next states",
-              file=sys.stderr)
-        print("\t", valid_edges,
-              file=sys.stderr)
-
-        
-        if len(valid_edges) == 0:
-            print("no valid transitions", file=sys.stderr)
-            exit(-1)
-        
-        # we will pick the first True test function
-        self.currentstate = valid_edges[0][1]
-        print(f"*******currentstate {self.currentstate}")
-        return globals()[output_fns[0]](input_)
-        
 # set up the quiz questions
 questions = ["Do you know what a database is?",
              "Is SELECT in DML or DDL?",
              "Briefly describe sixth normal form (6NF)."]
 previous_questions = []
 
 # set up the correct answer counts
 correct_count = 0
 partial_count = 0
-                              
-def main():
-    # read graph
-    try:
-        here = pathlib.Path(__file__).parent.resolve()
-        graph = pgv.AGraph((here / "quiz.dot"))
-    except IndexError:
-        print("need to give the name of a dot file graph as input",
-              file=sys.stderr)
-        exit(-1)
-        
-    # check if the graph is fully implemented
-    fully_implemented = True
-    for fname in get_graph_functions(graph):
-        if not is_implemented(fname):
-            print(f"there is no function named {fname}", file=sys.stderr)
-            fully_implemented = False
-            exit(-1)
+incorrect_count = 0
+
+class QuizQuestion():
+    def __init__(self, question: str, score_fn: Callable[[str], str]):
+        self._question = question
+        self._score_fn = score_fn
+    def score_answer(self, answer) -> str:
+        return self._score_fn(answer)
+    def text(self):
+        return self._question
+    
+# set up the quiz questions
+q1 = "Do you know what a database is?"
+def is_affirmative(input_: str) -> bool:
+  """ this is oversimplified, just a demo"""
+  if "yes" in input_.lower():
+    return True
+  return False
+
+def grade_q1(ans: str) -> str:
+    if is_affirmative(ans):
+        return "correct"
+    return "incorrect"
+q2 = "Is SELECT in DML or DDL?"
+def grade_q2(ans: str) -> str:
+    if "DDL" in ans:
+        return "incorrect"
+    if "DML" in ans:
+        return "correct"
+    else:
+        return "partial"
+q3 = "Briefly describe sixth normal form (6NF)."
+def grade_q3(ans: str) -> str:
+    return "partial"
+
+questions = [QuizQuestion(q1, grade_q1),
+             QuizQuestion(q2, grade_q2),
+             QuizQuestion(q3, grade_q3)]
+previous_questions = []
 
 
+    
+            
+def main():
+    graph = ffc.Graph("quiz.dot")
 
+    # check to make sure the graph's functions have been implemented
+    if not graph.check_implementation(env=globals()):
+        graph.check_implementation(verbose=True, env=globals())
 
             
     # run the dialog graph
-    agent = FST(graph, "start", "goodbye")
-    agent_output = agent("") # prime the agent because it needs input to start
-    user_input = input(agent_output + "\n")
-    while(agent.is_running):
-        agent_output = agent(user_input)
-        user_input = input(agent_output + "\n")
-        
+    agent = ffc.FST(graph, "start", "goodbye", globals())
+    agent.run()
     
-            
+
 if __name__ == "__main__":
     main()
+        
+    
+    
+
```

### Comparing `fstflowchat-0.0.6/src/fstflowchat/quiz.dot` & `fstflowchat-0.0.7/src/fstflowchat/quiz.dot`

 * *Files identical despite different names*

### Comparing `fstflowchat-0.0.6/src/fstflowchat.egg-info/PKG-INFO` & `fstflowchat-0.0.7/src/fstflowchat.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fstflowchat
-Version: 0.0.6
+Version: 0.0.7
 Summary: a small, pedagogical, fst-based dialog toolkit.
 Home-page: https://fstflowchat.readthedocs.io/en/latest/
 Author: Abe Kazemzadeh
 Project-URL: Bug Reports, https://github.com/abecode/fstflowchat/issues
 Project-URL: Funding, https://donate.pypi.org
 Project-URL: Say Thanks!, http://saythanks.io/to/example
 Project-URL: Source, https://github.com/abecode/fstflowchat/issues
```

