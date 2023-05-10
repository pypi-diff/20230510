# Comparing `tmp/dufuz-0.1.1-py3-none-any.whl.zip` & `tmp/dufuz-0.1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,21 @@
-Zip file size: 12353 bytes, number of entries: 18
+Zip file size: 13342 bytes, number of entries: 19
 -rw-rw-rw-  2.0 fat      106 b- defN 23-May-03 15:34 dufuz/__init__.py
--rw-rw-rw-  2.0 fat      489 b- defN 23-May-03 15:41 dufuz/__main__.py
+-rw-rw-rw-  2.0 fat      675 b- defN 23-May-07 10:55 dufuz/__main__.py
 -rw-rw-rw-  2.0 fat      704 b- defN 23-Apr-28 07:27 dufuz/defuzzify.py
--rw-rw-rw-  2.0 fat     2298 b- defN 23-May-03 08:40 dufuz/dfn.py
+-rw-rw-rw-  2.0 fat     2394 b- defN 23-May-07 10:44 dufuz/dfn.py
 -rw-rw-rw-  2.0 fat      653 b- defN 23-Apr-29 09:10 dufuz/monitor.py
--rw-rw-rw-  2.0 fat      339 b- defN 23-Apr-28 07:11 dufuz/tnorm.py
+-rw-rw-rw-  2.0 fat      479 b- defN 23-May-07 01:19 dufuz/negation.py
+-rw-rw-rw-  2.0 fat      339 b- defN 23-May-07 01:12 dufuz/tnorm.py
 -rw-rw-rw-  2.0 fat      104 b- defN 23-May-02 11:51 dufuz/core/__init__.py
 -rw-rw-rw-  2.0 fat     1150 b- defN 23-May-02 12:15 dufuz/core/domain.py
--rw-rw-rw-  2.0 fat     7073 b- defN 23-May-03 08:09 dufuz/core/environment.py
--rw-rw-rw-  2.0 fat     3545 b- defN 23-May-03 18:22 dufuz/core/number.py
+-rw-rw-rw-  2.0 fat     8055 b- defN 23-May-07 10:52 dufuz/core/environment.py
+-rw-rw-rw-  2.0 fat     3751 b- defN 23-May-07 09:59 dufuz/core/number.py
 -rw-rw-rw-  2.0 fat       49 b- defN 23-May-02 21:48 dufuz/interpreter/__init__.py
--rw-rw-rw-  2.0 fat     9735 b- defN 23-May-03 22:50 dufuz/interpreter/interpret.py
--rw-rw-rw-  2.0 fat     1174 b- defN 23-May-03 22:45 dufuz/interpreter/lexer.py
--rw-rw-rw-  2.0 fat     5028 b- defN 23-May-03 22:45 dufuz/interpreter/parser.py
--rw-rw-rw-  2.0 fat     1764 b- defN 23-May-03 22:51 dufuz-0.1.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-03 22:51 dufuz-0.1.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        6 b- defN 23-May-03 22:51 dufuz-0.1.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1372 b- defN 23-May-03 22:51 dufuz-0.1.1.dist-info/RECORD
-18 files, 35681 bytes uncompressed, 10137 bytes compressed:  71.6%
+-rw-rw-rw-  2.0 fat    13313 b- defN 23-May-07 10:51 dufuz/interpreter/interpret.py
+-rw-rw-rw-  2.0 fat     1212 b- defN 23-May-06 08:07 dufuz/interpreter/lexer.py
+-rw-rw-rw-  2.0 fat     5265 b- defN 23-May-06 08:07 dufuz/interpreter/parser.py
+-rw-rw-rw-  2.0 fat      899 b- defN 23-May-09 20:21 dufuz-0.1.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-09 20:21 dufuz-0.1.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        6 b- defN 23-May-09 20:21 dufuz-0.1.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1445 b- defN 23-May-09 20:21 dufuz-0.1.2.dist-info/RECORD
+19 files, 40691 bytes uncompressed, 11016 bytes compressed:  72.9%
```

## zipnote {}

```diff
@@ -9,14 +9,17 @@
 
 Filename: dufuz/dfn.py
 Comment: 
 
 Filename: dufuz/monitor.py
 Comment: 
 
+Filename: dufuz/negation.py
+Comment: 
+
 Filename: dufuz/tnorm.py
 Comment: 
 
 Filename: dufuz/core/__init__.py
 Comment: 
 
 Filename: dufuz/core/domain.py
@@ -36,20 +39,20 @@
 
 Filename: dufuz/interpreter/lexer.py
 Comment: 
 
 Filename: dufuz/interpreter/parser.py
 Comment: 
 
-Filename: dufuz-0.1.1.dist-info/METADATA
+Filename: dufuz-0.1.2.dist-info/METADATA
 Comment: 
 
-Filename: dufuz-0.1.1.dist-info/WHEEL
+Filename: dufuz-0.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: dufuz-0.1.1.dist-info/top_level.txt
+Filename: dufuz-0.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: dufuz-0.1.1.dist-info/RECORD
+Filename: dufuz-0.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## dufuz/__main__.py

```diff
@@ -1,13 +1,16 @@
 from .interpreter import interpret
 import torch
-from . import DiscreteEnvironment, tnorm
+from . import DiscreteEnvironment, tnorm, negation
 import argparse
 
 
 parser = argparse.ArgumentParser(description='Run a dufuz file.')
 parser.add_argument("path", type=str)
 parser.add_argument("--tol", type=float, default=0.01)
 parser.add_argument("--device", type=str, default="cuda:0")
+parser.add_argument("--logic", type=str, default="lukasiewicz")
 args = parser.parse_args()
-env = DiscreteEnvironment(tnorm=tnorm.lukasiewicz, tol=args.tol, device=torch.device(args.device))
+env = DiscreteEnvironment(tnorm=getattr(tnorm, args.logic),
+                          memory_logic_not=getattr(negation, args.logic),
+                          tol=args.tol, device=torch.device(args.device))
 interpret(env, args.path)
```

## dufuz/dfn.py

```diff
@@ -1,22 +1,23 @@
 from dufuz.core import Environment, Domain, Number
-from dufuz.tnorm import lukasiewicz
+from dufuz import tnorm, negation
 import torch
 
 
 class DiscreteEnvironment(Environment):
     def __init__(self,
                  device='cuda',
-                 tnorm=lukasiewicz,
+                 tnorm=tnorm.lukasiewicz,
+                 memory_logic_not=negation.lukasiewicz,
                  tol=0.01,
                  breadth=1,
                  lower=None,
                  upper=None,
                  strategy="modulo"):
-        super().__init__(device=device, tnorm=tnorm)
+        super().__init__(device=device, tnorm=tnorm, memory_logic_not=memory_logic_not)
         self.tol = tol
         self.breadth = breadth
         self.lower = lower
         self.upper = upper
         self.strategy = strategy
 
     def number(self, value, form=None, breadth=None):
```

## dufuz/core/environment.py

```diff
@@ -12,18 +12,19 @@
     inv_sorted = (inverse+decimals).argsort()
     tot_counts = torch.cat((counts.new_zeros(1), counts.cumsum(dim=0)))[:-1]
     index = inv_sorted[tot_counts]
     return unique, index
 
 
 class Environment:
-    def __init__(self, device, tnorm=torch.minimum):
+    def __init__(self, device, tnorm, memory_logic_not):
         self.device = device
         self.monitors = list()
         self.tnorm = tnorm
+        self.memory_logic_not = memory_logic_not
 
     def discretize(self, values, elements):
         #mask = torch.logical_not(torch.isnan(values))
         #return torch.masked_select(values, mask), torch.masked_select(elements, mask)
         return values, elements
 
     def apply(self, method, a, b=None):
@@ -44,49 +45,56 @@
                               torch.reshape(b.domain.elements, shape=(-1, 1)))
         # squeeze
         values = torch.reshape(retvals, shape=[-1])
         elements = torch.reshape(elements, shape=[-1])
         # postprocess
         values, elements = self.discretize(values, elements)
         values, elements = self.reduce(values, elements)
-        # find non-zero positions and gather respective values (memberships) and elements (method outputs)
-        if elements.dtype != torch.bool:
-            positions = (values != 0)# > 1.E-12)
-            if positions.size() != values.size():
-                values = torch.masked_select(values, positions)
-                elements = torch.masked_select(elements, positions)
         for monitor in self.monitors:
             monitor.notify(elements.nelement(), None)
         return Number(values, Domain(elements, self))
 
     def reduce(self, values, elements):
         #values = torch.reshape(values, shape=[-1])
         #elements = torch.reshape(elements, shape=[-1])
         # keep only the largest values for each unique element (sort and then keep first occurences)
         sort_idx = torch.argsort(values, descending=True)
         values = values[sort_idx]
         elements = elements[sort_idx]
         elements, unique_idx = _unique(elements)
         values = values[unique_idx]
+
+        # find non-zero positions and gather respective values (memberships) and elements (method outputs)
+        if elements.dtype != torch.bool:
+            positions = (values != 0)# > 1.E-12)
+            if torch.is_same_size(values, elements) and positions.numel() > 0:
+                values = torch.masked_select(values, positions)
+                elements = torch.masked_select(elements, positions)
+
         return values, elements
 
     def point(self, value, membership=1):
         return Number([membership], Domain([value], self))
 
     def If(self, condition, a, b):
+        if a is None and b is None:
+            return None
         # self.combine(condition * a, self.Not(condition) * b) is viable only for logical clauses
         if not isinstance(condition, Number):
             condition = Number([1], Domain([condition], self))
-        if not isinstance(a, Number):
+        if a is not None and not isinstance(a, Number):
             a = Number([1], Domain([a], self))
-        if not isinstance(b, Number):
+        if b is not None and not isinstance(b, Number):
             b = Number([1], Domain([b], self))
         ret = None
         for branch, membership in condition.todict().items():
-            term = (a if branch == 1 else b)*Number([membership], Domain([1], self))
+            term = a if branch == 1 else b
+            if term is None:
+                continue
+            term = term*Number([membership], Domain([1], self))
             if ret is None:
                 ret = term
             else:
                 ret = self.combine(ret, term)
         return ret
 
     def le(self, a, b):
@@ -101,30 +109,40 @@
     def gt(self, a, b):
         return self.apply(operator.gt, a, b)#self.And(self.apply(operator.gt, a, b), self.Not(self.apply(operator.le, a, b)))
 
     def eq(self, a, b):
         return self.apply(operator.eq, a, b)#self.And(self.apply(operator.ge, a, b), self.apply(operator.le, a, b))
 
     def complement(self, a):
-        return Number(1-a.values, a.domain)
+        return Number(self.memory_logic_not(a.values), a.domain)
+
+    def transorm_membership(self, a, transformer):
+        return Number(transformer(a.values), a.domain)
+
+    def nullify(self, a):
+        return Number(torch.zeros(size=a.values.size(), device=a.values.device), a.domain)
 
     def Not(self, a):
         return self.apply(torch.logical_not, a)#Number(1-a.values, a.domain)
 
     def And(self, a, b):
-        return self.apply(operator.mul, a, b)
+        return self.apply(torch.logical_and, a, b)
 
     def Or(self, a, b):
         return self.combine(a, b)#self.apply(lambda x, y: x + y - x * y, a, b)
 
     def combine(self, number1, number2):
         if number1 is None:
             return number2
         if number2 is None:
             return number1
+        if not isinstance(number1, Number):
+            number1 = Number([1], Domain([number1], self))
+        if not isinstance(number2, Number):
+            number2 = Number([1], Domain([number2], self))
         values = torch.concat([number1.values, number2.values])
         elements = torch.concat([number1.domain.elements, number2.domain.elements])
         values, elements = self.reduce(values, elements)
         return Number(values, Domain(elements, self))
 
     def setlist(self, values, item, value):
         if not isinstance(value, Number):
@@ -132,29 +150,33 @@
         if not isinstance(item, Number):
             item = Number([1], Domain([item], self))
         else:
             item = self.apply(torch.round, item)
         for i, membership in item.todict().items():
             #if membership == 0:
             #    continue
+            if i != int(i):
+                continue
             i = int(i)
             if i < 0 or i >= len(values):
                 continue
-            membership = Number([membership], Domain([1], self))
+            membership = Number([membership, self.memory_logic_not(membership)], Domain([True, False], self))
             values[i] = self.If(membership, value, values[i])
 
     def getlist(self, values, item, default=None):
         if not isinstance(item, Number):
             item = Number([1], Domain([item], self))
         else:
             item = self.apply(torch.round, item)
         result = None
         for i, membership in item.todict().items():
-            #if membership == 0:
-            #    continue
+            if membership == 0:
+                continue  # TODO: this statement can lead to empty result
+            if i != int(i):
+                continue  # TODO: this statement can lead to empty result
             i = int(i)
             if i < 0 or i >= len(values):
                 continue
             membership = Number([membership], Domain([1], self))
             result = self.combine(self.apply(operator.mul, values[i], membership), result)
         if result is None:
             if default is None:
```

## dufuz/core/number.py

```diff
@@ -21,27 +21,33 @@
         if div is None:
             div = self.values.max()
         return Number(self.values / div, self.domain)
 
     def center(self, threshold=1):
         return torch.masked_select(self.domain.elements, (self.values > threshold-1.E-12)).cpu().numpy()
 
-    def plot(self, plt=None, hold=False):
+    def plot(self, plt=None, hold=False, marker='.', **kwargs):
         if plt is None:
             from matplotlib import pyplot as plt
-        plt.scatter(self.domain.elements.cpu().numpy(), self.values.cpu().numpy(), marker='.')
+        plt.scatter(self.domain.elements.cpu().numpy(), self.values.cpu().numpy(), marker=marker, **kwargs)
         if not hold:
             plt.show()
 
+    def complement(self):
+        return self.domain.env.complement(self)
+
     def todict(self, threshold=0):
-        return dict({k: v for k,v in zip(self.domain.elements.cpu().numpy(), self.values.cpu().numpy()) if v > threshold})
+        return dict({k: v for k, v in zip(self.domain.elements.cpu().numpy(), self.values.cpu().numpy()) if v > threshold})
 
     def choose(self, a, b):
         return self.env.If(self, a, b)
 
+    def is_crisp(self):
+        return torch.sum(self.values) == torch.max(self.values)
+
     def __str__(self):
         return str(self.todict(-1))
 
     def __and__(self, other):
         return self.env.And(self, other)
 
     def __or__(self, other):
```

## dufuz/interpreter/interpret.py

```diff
@@ -1,9 +1,32 @@
 from dufuz.interpreter.lexer import DufuzLexer
 from dufuz.interpreter.parser import DufuzParser
+from dufuz.core import Number, Domain
+import operator
+import torch
+
+
+class Range:
+    def __init__(self, env):
+        self.env = env
+
+    def __call__(self, a, b=None, inc=None):
+        if b is None:
+            a, b = 0, a
+        if inc is None:
+            inc = 1
+        x = a if isinstance(a, Number) else Number([1], Domain([a], self.env.spawner))
+        while True:
+            next_x = x+inc
+            comparison = self.env.spawner.apply(operator.lt, next_x, b)  # treat crisp arithmetics as fuzzy too
+            if comparison.todict().get(True, 0) <= 0:
+                break
+            toyield = self.env.spawner.If(comparison, x, None)
+            yield toyield
+            x = next_x
 
 
 class Variable:
     def __init__(self, executor, name):
         self.executor = executor
         self.name = name
 
@@ -50,15 +73,17 @@
 
 class Executor:
     def __init__(self, spawner):
         self.spawner = spawner
         self.env = {"print": print,
                     "int": int,
                     "float": float,
-                    "range": range,
+                    "range": Range(self),
+                    "list": list,
+                    "map": map,
                     "len": len,
                     "str": str,
                     "zip": zip,
                     "True": True,
                     "False": False}
         self.asvar = False
         self.asname = False
@@ -105,15 +130,16 @@
             self.asvar = False
         return ret
 
     def notop(self, value):
         return self.spawner.Not(value)
 
     def list(self, iterator):
-        assert isinstance(iterator, Iter)
+        if not isinstance(iterator, Iter):
+            return [iterator]
         return iterator.list
 
     def next(self, element, next):
         if not isinstance(next, Iter):
             next = Iter([next])
         if not isinstance(element, Iter):
             element = Iter([element])
@@ -123,15 +149,15 @@
         if self.asvar:
             return Element(self, values, element)
         if isinstance(values, tuple):
             return values[element]
         return self.spawner.getlist(values, element)
 
     def number(self, number):
-        return number
+        return number#self.spawner.number(number, breadth=0)
 
     def scope(self, result):
         return result
 
     def fuzzy(self, number, breadth):
         return self.spawner.number(number, breadth=breadth)
 
@@ -173,14 +199,17 @@
 
     def orop(self, x, y):
         return x | y
 
     def sub(self, x, y):
         return x - y
 
+    def neg(self, x):
+        return -x
+
     def div(self, x, y):
         return x / y
 
     def le(self, x, y):
         return x <= y
 
     def ge(self, x, y):
@@ -205,21 +234,22 @@
     def importmember(self, module, name, alias):
         import importlib
         module = importlib.import_module(module)
         self.env[alias] = getattr(module, name)
 
 
 class Func:
-    def __init__(self, path, executor, parser, lexer, lines, args):
+    def __init__(self, path, executor, parser, lexer, lines, args, ret_env=False):
         self.path = path
         self.executor = executor
         self.lines = lines
         self.parser = parser
         self.lexer = lexer
         self.args = args
+        self.ret_env = ret_env
 
     def __call__(self, *args, **kwargs):
         prev_env = self.executor.env
         self.executor.env = {k: v for k, v in self.executor.env.items()}
         loops = list()
         parser = self.parser
         lexer = self.lexer
@@ -254,15 +284,14 @@
                 i += 1
                 continue
             tree = parser.parse(lexer.tokenize(stripped_line))
             #print(list(lexer.tokenize(stripped_line)))
             if not tree:
                 print(line)
                 raise Exception("Invalid expression at file\""+self.path+"\", line "+str(i))
-            #print(tree)
             if tree[0] == "def":
                 func_name = tree[1]
                 func_lines = list()
                 func_args = executor.run(tree[2], asvar=True).list if isinstance(tree[2], tuple) and tree[2][0] == "next" else [executor.run(tree[2], asvar=True)]
                 func_args = [arg.name for arg in func_args]
                 i += 1
                 while i < len(lines):
@@ -273,18 +302,66 @@
                     if depth <= block:
                         break
                     func_lines.append(lines[i])
                     i += 1
                 func_lines.append("")
                 executor.env[func_name] = Func(func_name, executor, parser, lexer, func_lines, func_args)
                 i -= 1
+            elif tree[0] == "while":
+                while_condition = tree[1]
+                while_lines = list()
+                i += 1
+                while i < len(lines):
+                    if not lines[i].strip():
+                        i += 1
+                        continue
+                    depth = len(lines[i])-len(lines[i].lstrip())
+                    if depth <= block:
+                        break
+                    while_lines.append(lines[i])
+                    i += 1
+                while_lines.append("")
+                loop = Func(str(while_condition), executor, parser, lexer, while_lines, [], ret_env=True)
+                appended_env = dict()#{k: v for k, v in self.executor.env.items()}
+                prev_cond = Number([1], Domain([True], self.executor.spawner))
+                while True:
+                    condition = self.executor.run(while_condition)
+                    if not isinstance(condition, Number):
+                        condition = Number([1], Domain([condition], self.executor.spawner))
+                    is_true = prev_cond.todict().get(True, 0)
+                    residual = Number([is_true, self.executor.spawner.memory_logic_not(is_true)], Domain([True, False], self.executor.spawner))
+                    prev_cond = self.executor.spawner.And(condition, residual)
+                    #print(residual, condition, prev_cond)
+                    condition = prev_cond
+                    for k, v in self.executor.env.items():
+                        if isinstance(v, Number) or isinstance(appended_env.get(k, None), Number):
+                            v = condition.choose(None, v)
+                            if k in appended_env:
+                                appended_env[k] = self.executor.spawner.combine(v, appended_env[k])
+                            else:
+                                appended_env[k] = v
+                        else:
+                            appended_env[k] = v
+                    if condition.todict().get(True, 0) == 0:
+                        break
+                    self.executor.env = loop()
+                i -= 1
+                for k, v in appended_env.items():
+                    self.executor.env[k] = v
             elif tree[0] == "return":
                 ret = executor.run(tree[1])
                 self.executor.env = prev_env
                 return ret
+            elif tree[0] == "break":
+                self.executor.env = prev_env
+                internal_env = self.executor.env
+                self.executor.env = prev_env
+                if self.ret_env:
+                    return internal_env
+                return
             elif tree[0] == "for":
                 loops.append(("for", i+1, block, executor.run(tree[1], asvar=True), iter(executor.run(tree[2]))))
                 try:
                     element = next(loops[-1][4])
                     var = loops[-1][3]
                     if isinstance(var, Iter):
                         for var, element in zip(var.list, element):
@@ -292,15 +369,18 @@
                     else:
                         var.assign(element)
                 except StopIteration:
                     loops.pop()
             else:
                 executor.run(tree)
             i += 1
+        internal_env = self.executor.env
         self.executor.env = prev_env
+        if self.ret_env:
+            return internal_env
         return None
 
 
 def interpret(environment, path):
     lexer = DufuzLexer()
     parser = DufuzParser()
     executor = Executor(environment)
```

## dufuz/interpreter/lexer.py

```diff
@@ -1,29 +1,30 @@
 from sly import Lexer
 
 
 class DufuzLexer(Lexer):
     tokens = {NAME, NUMBER, STRING, NOT, AND, OR, IF, WHILE, ELSE, FOR, IN, IMPORT, FROM, AS, DEF, RETURN, NEQ,
-              LE, GE, LT, GT, EQ, ASSIGN, DOT}
+              LE, GE, LT, GT, EQ, ASSIGN, DOT, BREAK}
 
     ignore = '\t '
     literals = {'+', '-', '/', '*', '(', ')', '[', ']', '?', ':', ','}
 
     ELSE = r"else"
     DEF = r"def "
-    NOT = r"not"
-    AND = r"and"
-    OR = r"or"
-    IF = r"if"
-    WHILE = r"while"
-    FOR = r"for"
-    IN = r"in"
-    IMPORT = r"import"
+    NOT = r"not "
+    AND = r"and "
+    OR = r"or "
+    IF = r"if "
+    WHILE = r"while "
+    FOR = r"for "
+    IN = r"in "
+    IMPORT = r"import "
     RETURN = r"return"
-    FROM = r"from"
+    FROM = r"from "
+    BREAK = r"break"
     AS = r"as"
     DOT = r"\."
     NEQ = r"\!\="
     GE = r"\>\="
     LE = r"\<\="
     EQ = r"\=\="
     GT = r"\>"
```

## dufuz/interpreter/parser.py

```diff
@@ -36,14 +36,18 @@
     def statement(self, p):
         return "importmember", p.namespace, p.NAME, p.NAME
 
     @_('FROM namespace IMPORT NAME AS NAME')
     def statement(self, p):
         return "importmember", p.namespace, p.NAME0, p.NAME1
 
+    @_('BREAK')
+    def statement(self, p):
+        return "break"
+
     @_('NAME DOT namespace')
     def namespace(self, p):
         return p.NAME + "." + p.namespace
 
     @_('NAME')
     def namespace(self, p):
         return p.NAME
@@ -52,14 +56,18 @@
     def statement(self, p):
         return "assign", p.assignee, p.expr
 
     @_('FOR names IN expr ":"')
     def statement(self, p):
         return "for", p.names, p.expr
 
+    @_('WHILE expr ":"')
+    def statement(self, p):
+        return "while", p.expr
+
     @_('NAME')
     def names(self, p):
         return "assignee", p.NAME
 
     @_('names "," names')
     def names(self, p):
         return "next", p.names0, p.names1
@@ -140,14 +148,18 @@
     def expr(self, p):
         return "add", p.expr0, p.expr1
 
     @_('expr "-" expr')
     def expr(self, p):
         return "sub", p.expr0, p.expr1
 
+    @_('"-" expr')
+    def expr(self, p):
+        return "neg", p.expr
+
     @_('expr "*" expr')
     def expr(self, p):
         return "mul", p.expr0, p.expr1
 
     @_('expr "/" expr')
     def expr(self, p):
         return "div", p.expr0, p.expr1
```

## Comparing `dufuz-0.1.1.dist-info/RECORD` & `dufuz-0.1.2.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 dufuz/__init__.py,sha256=qzOmaC1-_4aR1uexA7AUrGjVYKkwTeHmcmuBHq5JRvI,106
-dufuz/__main__.py,sha256=9YfPArh8Ud4FcseRCLNyqF5SuRjZsSvnqZOe5_HCsjQ,489
+dufuz/__main__.py,sha256=u5SBSurw5Umxu-NoOpkfwoF2MoK7Tnrcq97jzG-byzA,675
 dufuz/defuzzify.py,sha256=1QUztb6NRRXHe_5Ilv3m3-Ds4_E9X3wO6nAOE5KeuRk,704
-dufuz/dfn.py,sha256=_iHuiW41O5E4yunbVsCBTlb6Kekc9mFTTTUBdmm1KX8,2298
+dufuz/dfn.py,sha256=vOQZIue5GNv9uFqJ87lZvIXouVmkkSNDaU32wFewgYw,2394
 dufuz/monitor.py,sha256=PpTckJVU1MdqZMBmOzIKYSJByNtFmzo30Hj30rmHWkA,653
+dufuz/negation.py,sha256=X5vBTYmz1l3dqFRFwWrbJl3vQqZjcuCDJjUvjLz6EPU,479
 dufuz/tnorm.py,sha256=1P2mKnsdFfeo6hM5cXpg1CN5G9wokzdVsKcPa56FJk0,339
 dufuz/core/__init__.py,sha256=d5UUP4Ul9gVsEjDy3ukyWPYEy-1lfHRyxbH_MbSq9gU,104
 dufuz/core/domain.py,sha256=31OmdzQ036neaUtpRZ7Sfa2GSbcGZABi1DacpCN1KHA,1150
-dufuz/core/environment.py,sha256=KOTcUkkSGIOON8bUWMldjjHoqLBp7LoljBbbI21dhsM,7073
-dufuz/core/number.py,sha256=92PojWnplnNeWrFZvhrpIn1bb_cax-6KT00tgOuLACo,3545
+dufuz/core/environment.py,sha256=FJ3u0Tzz51rZz7c5Df2pX-wydB9MJmPnt8GWPIjAc_Q,8055
+dufuz/core/number.py,sha256=9R_LK70aXWxW-lTK_CXJVxQjBATcSa8aTe6solK_oxQ,3751
 dufuz/interpreter/__init__.py,sha256=A8zHBTrxIcsDCogfkoHKBez9fNMvQurRCW2LsIqoZZ8,49
-dufuz/interpreter/interpret.py,sha256=-VSNrHCj1HkFnBC0-KpZeMxgqt-Rp8EreneYOPrfSd4,9735
-dufuz/interpreter/lexer.py,sha256=6zds46LTAI-1D4j3TA8ofeky69p1jsVNG1IQoUYHH80,1174
-dufuz/interpreter/parser.py,sha256=c-aFupWPhpXU0i4S6IY1A7wIGOrgssLxzqXTqSzQ1dE,5028
-dufuz-0.1.1.dist-info/METADATA,sha256=0gwt17MEXbs1T4CBVsZGnLWUHf5dA9hSv37ELJVBJKc,1764
-dufuz-0.1.1.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-dufuz-0.1.1.dist-info/top_level.txt,sha256=uOCyq9ewMXY6duF8r0nDnXUzV3tAbqwAyt1x2L0EAHY,6
-dufuz-0.1.1.dist-info/RECORD,,
+dufuz/interpreter/interpret.py,sha256=dQvN5qE0gJ4qRgtcgrJmIW5c4094DO2ATjZT-R8DplU,13313
+dufuz/interpreter/lexer.py,sha256=8Aql3cV0DZ7J_K_PBBWTQRVRHStJuZUgWb3KVkrMsSs,1212
+dufuz/interpreter/parser.py,sha256=DbklD5QVd1OiyUD-M_FD1CHu6bHPvaAMx8O1YkDRdjE,5265
+dufuz-0.1.2.dist-info/METADATA,sha256=BJ9j32eJLzeDDGpTSv15g4cp0nnJgWh6Q0Ont07Vzh4,899
+dufuz-0.1.2.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+dufuz-0.1.2.dist-info/top_level.txt,sha256=uOCyq9ewMXY6duF8r0nDnXUzV3tAbqwAyt1x2L0EAHY,6
+dufuz-0.1.2.dist-info/RECORD,,
```

