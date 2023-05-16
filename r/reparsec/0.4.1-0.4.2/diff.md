# Comparing `tmp/reparsec-0.4.1.tar.gz` & `tmp/reparsec-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reparsec-0.4.1.tar", max compression
+gzip compressed data, was "reparsec-0.4.2.tar", max compression
```

## Comparing `reparsec-0.4.1.tar` & `reparsec-0.4.2.tar`

### file list

```diff
@@ -1,28 +1,27 @@
--rw-r--r--   0        0        0     1071 2022-04-24 16:58:06.952758 reparsec-0.4.1/LICENSE
--rw-r--r--   0        0        0     1080 2022-08-16 19:34:10.881457 reparsec-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     2226 2022-08-12 18:29:17.047285 reparsec-0.4.1/README.md
--rw-r--r--   0        0        0      958 2022-08-16 19:34:10.881457 reparsec-0.4.1/src/reparsec/__init__.py
--rw-r--r--   0        0        0        0 2022-04-24 16:58:06.968384 reparsec-0.4.1/src/reparsec/core/__init__.py
--rw-r--r--   0        0        0      526 2022-08-16 19:20:10.139151 reparsec-0.4.1/src/reparsec/core/chain.py
--rw-r--r--   0        0        0    16631 2022-08-16 19:20:10.140150 reparsec-0.4.1/src/reparsec/core/combinators.py
--rw-r--r--   0        0        0     3061 2022-08-16 19:20:10.142150 reparsec-0.4.1/src/reparsec/core/layout.py
--rw-r--r--   0        0        0     1213 2022-08-16 19:20:10.143165 reparsec-0.4.1/src/reparsec/core/parser.py
--rw-r--r--   0        0        0     1895 2022-08-16 19:20:10.144152 reparsec-0.4.1/src/reparsec/core/primitive.py
--rw-r--r--   0        0        0     2792 2022-08-16 19:20:10.144152 reparsec-0.4.1/src/reparsec/core/recovery.py
--rw-r--r--   0        0        0     2166 2022-08-16 19:20:10.147159 reparsec-0.4.1/src/reparsec/core/repair.py
--rw-r--r--   0        0        0     2355 2022-08-13 07:53:50.029617 reparsec-0.4.1/src/reparsec/core/repair.py.orig
--rw-r--r--   0        0        0     4683 2022-08-16 19:20:10.149161 reparsec-0.4.1/src/reparsec/core/result.py
--rw-r--r--   0        0        0     4068 2022-08-16 19:20:10.152152 reparsec-0.4.1/src/reparsec/core/scannerless.py
--rw-r--r--   0        0        0     4560 2022-08-16 19:20:10.154131 reparsec-0.4.1/src/reparsec/core/sequence.py
--rw-r--r--   0        0        0      846 2022-08-07 20:53:38.616870 reparsec-0.4.1/src/reparsec/core/stream.py
--rw-r--r--   0        0        0      970 2022-08-16 19:20:10.155140 reparsec-0.4.1/src/reparsec/core/types.py
--rw-r--r--   0        0        0     1294 2022-08-16 19:20:10.156120 reparsec-0.4.1/src/reparsec/layout.py
--rw-r--r--   0        0        0     4965 2022-08-16 19:20:10.158139 reparsec-0.4.1/src/reparsec/lexer.py
--rw-r--r--   0        0        0    27053 2022-08-16 19:20:10.160133 reparsec-0.4.1/src/reparsec/parser.py
--rw-r--r--   0        0        0     1323 2022-08-16 19:20:10.165139 reparsec-0.4.1/src/reparsec/primitive.py
--rw-r--r--   0        0        0        0 2022-04-24 16:58:06.984009 reparsec-0.4.1/src/reparsec/py.typed
--rw-r--r--   0        0        0     2213 2022-08-16 19:20:10.168121 reparsec-0.4.1/src/reparsec/scannerless.py
--rw-r--r--   0        0        0     1816 2022-08-16 19:20:10.170133 reparsec-0.4.1/src/reparsec/sequence.py
--rw-r--r--   0        0        0     5191 2022-08-16 19:20:10.172130 reparsec-0.4.1/src/reparsec/types.py
--rw-r--r--   0        0        0     3159 2022-08-16 19:35:21.566810 reparsec-0.4.1/setup.py
--rw-r--r--   0        0        0     3157 2022-08-16 19:35:21.566810 reparsec-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1071 2022-04-24 16:58:06.952758 reparsec-0.4.2/LICENSE
+-rw-r--r--   0        0        0     1127 2022-08-28 16:15:24.720910 reparsec-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     2978 2022-08-28 16:15:24.718906 reparsec-0.4.2/README.md
+-rw-r--r--   0        0        0      958 2022-08-28 16:15:24.721938 reparsec-0.4.2/src/reparsec/__init__.py
+-rw-r--r--   0        0        0        0 2022-04-24 16:58:06.968384 reparsec-0.4.2/src/reparsec/core/__init__.py
+-rw-r--r--   0        0        0      526 2022-08-16 19:20:10.139151 reparsec-0.4.2/src/reparsec/core/chain.py
+-rw-r--r--   0        0        0    16366 2022-08-28 16:15:24.723523 reparsec-0.4.2/src/reparsec/core/combinators.py
+-rw-r--r--   0        0        0     3061 2022-08-16 19:20:10.142150 reparsec-0.4.2/src/reparsec/core/layout.py
+-rw-r--r--   0        0        0     1213 2022-08-16 19:20:10.143165 reparsec-0.4.2/src/reparsec/core/parser.py
+-rw-r--r--   0        0        0     1895 2022-08-16 19:20:10.144152 reparsec-0.4.2/src/reparsec/core/primitive.py
+-rw-r--r--   0        0        0     2762 2022-08-28 16:15:24.724618 reparsec-0.4.2/src/reparsec/core/recovery.py
+-rw-r--r--   0        0        0     2208 2022-08-28 16:15:24.725371 reparsec-0.4.2/src/reparsec/core/repair.py
+-rw-r--r--   0        0        0     4683 2022-08-28 16:15:24.726383 reparsec-0.4.2/src/reparsec/core/result.py
+-rw-r--r--   0        0        0     4068 2022-08-28 11:41:33.862842 reparsec-0.4.2/src/reparsec/core/scannerless.py
+-rw-r--r--   0        0        0     4560 2022-08-28 11:41:33.865837 reparsec-0.4.2/src/reparsec/core/sequence.py
+-rw-r--r--   0        0        0      846 2022-08-07 20:53:38.616870 reparsec-0.4.2/src/reparsec/core/stream.py
+-rw-r--r--   0        0        0      970 2022-08-16 19:20:10.155140 reparsec-0.4.2/src/reparsec/core/types.py
+-rw-r--r--   0        0        0     1294 2022-08-16 19:20:10.156120 reparsec-0.4.2/src/reparsec/layout.py
+-rw-r--r--   0        0        0     4965 2022-08-16 19:20:10.158139 reparsec-0.4.2/src/reparsec/lexer.py
+-rw-r--r--   0        0        0    28219 2022-08-28 16:15:24.727383 reparsec-0.4.2/src/reparsec/parser.py
+-rw-r--r--   0        0        0     1323 2022-08-16 19:20:10.165139 reparsec-0.4.2/src/reparsec/primitive.py
+-rw-r--r--   0        0        0        0 2022-04-24 16:58:06.984009 reparsec-0.4.2/src/reparsec/py.typed
+-rw-r--r--   0        0        0     2213 2022-08-16 19:20:10.168121 reparsec-0.4.2/src/reparsec/scannerless.py
+-rw-r--r--   0        0        0     1816 2022-08-16 19:20:10.170133 reparsec-0.4.2/src/reparsec/sequence.py
+-rw-r--r--   0        0        0     4009 2022-08-28 16:15:24.728384 reparsec-0.4.2/src/reparsec/types.py
+-rw-r--r--   0        0        0     3933 2022-08-28 16:15:39.373148 reparsec-0.4.2/setup.py
+-rw-r--r--   0        0        0     3960 2022-08-28 16:15:39.373148 reparsec-0.4.2/PKG-INFO
```

### Comparing `reparsec-0.4.1/LICENSE` & `reparsec-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `reparsec-0.4.1/pyproject.toml` & `reparsec-0.4.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "reparsec"
-version = "0.4.1"
+version = "0.4.2"
 description = "Parser"
 authors = ["ethframe <ethframe@gmail.com>"]
 license = "MIT License"
 readme = "README.md"
 repository = "https://github.com/ethframe/reparsec"
 documentation = "https://reparsec.readthedocs.io/"
 classifiers = [
@@ -12,14 +12,15 @@
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.6",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Typing :: Typed",
 ]
 packages = [
     { include = "reparsec", from = "src" },
 ]
 
 [tool.poetry.dependencies]
```

### Comparing `reparsec-0.4.1/src/reparsec/__init__.py` & `reparsec-0.4.2/src/reparsec/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,8 +21,8 @@
 
     "Delay", "Parser", "Tuple2", "Tuple3", "Tuple4", "Tuple5", "Tuple6",
     "Tuple7", "Tuple8", "TupleParser", "alt", "attempt", "between", "bind",
     "chainl1", "chainr1", "fmap", "label", "many", "maybe", "recover",
     "recover_with", "recover_with_fn", "sep_by", "seq", "seql", "seqr"
 )
 
-__version__ = "0.4.1"
+__version__ = "0.4.2"
```

### Comparing `reparsec-0.4.1/src/reparsec/core/chain.py` & `reparsec-0.4.2/src/reparsec/core/chain.py`

 * *Files identical despite different names*

### Comparing `reparsec-0.4.1/src/reparsec/core/combinators.py` & `reparsec-0.4.2/src/reparsec/core/combinators.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Callable, Iterable, List, Optional, Tuple, TypeVar, Union
 
 from .chain import Append
 from .parser import ParseFastFn, ParseFn, ParseFns, ParseObj
 from .recovery import MergeFn, continue_parse, join_repairs
-from .repair import Insert, OpItem, Repair
+from .repair import make_user_insert
 from .result import Error, Ok, Recovered, Result, SimpleResult
 from .types import Ctx
 
 S = TypeVar("S")
 A = TypeVar("A")
 B = TypeVar("B")
 C = TypeVar("C")
@@ -449,27 +449,26 @@
 
     def recover(
             stream: S, pos: int, ctx: Ctx[S], ins: int,
             rem: Optional[int]) -> Result[A, S]:
         r = parse_fn(stream, pos, ctx, ins, rem)
         if type(r) is Recovered:
             for p in r.repairs:
-                if p.skip is None:
-                    p.auto = False
+                if p.prio is None:
+                    p.prio = 0
         return r
 
     return recover
 
 
 def recover(parse_fns: ParseFns[S, A]) -> ParseFns[S, A]:
     return ParseFns(_recover_fast(parse_fns), _recover(parse_fns))
 
 
-def _recover_with_fast(
-        parse_fns: ParseFns[S, A], x: A, vs: str) -> ParseFastFn[S, A]:
+def _recover_with_fast(parse_fns: ParseFns[S, A]) -> ParseFastFn[S, A]:
     return parse_fns.fast_fn
 
 
 def _recover_with(
         parse_fns: ParseFns[S, A], x: A, vs: str) -> ParseFn[S, A]:
     parse_fn = parse_fns.fn
 
@@ -479,33 +478,30 @@
         if rem is None:
             return parse_fn(stream, pos, ctx, ins, None)
         r = parse_fn(stream, pos, ctx, ins, rem)
         if type(r) is Ok or r.consumed:
             return r
         if rem:
             loc = ctx.get_loc(stream, pos)
-            rep = Repair(
-                None, False, rem - 1, [OpItem(Insert(vs), loc, r.expected)],
-                x, pos, ctx, (), True
-            )
+            rep = make_user_insert(rem, x, pos, ctx, loc, vs, r.expected)
             if type(r) is Error:
                 return Recovered([rep], None, loc)
-            return Recovered([rep, *r.repairs], r.min_skip, loc, r.expected)
+            return Recovered([rep, *r.repairs], r.min_prio, loc, r.expected)
         return r
 
     return recover_with
 
 
 def recover_with(
         parse_fns: ParseFns[S, A], x: A,
         label: Optional[str] = None) -> ParseFns[S, A]:
     vs = repr(x) if label is None else label
 
     return ParseFns(
-        _recover_with_fast(parse_fns, x, vs),
+        _recover_with_fast(parse_fns),
         _recover_with(parse_fns, x, vs)
     )
 
 
 def _recover_with_fn_fast(parse_fns: ParseFns[S, A]) -> ParseFastFn[S, A]:
     return parse_fns.fast_fn
 
@@ -522,26 +518,21 @@
             return parse_fn(stream, pos, ctx, ins, None)
         r = parse_fn(stream, pos, ctx, ins, rem)
         if type(r) is Ok or r.consumed:
             return r
         if rem:
             x = fn(stream, pos)
             loc = ctx.get_loc(stream, pos)
-            rep = Repair(
-                None, False, rem - 1, [
-                    OpItem(
-                        Insert(repr(x) if label is None else label),
-                        loc, r.expected
-                    )
-                ],
-                x, pos, ctx, (), True
+            rep = make_user_insert(
+                rem, x, pos, ctx, loc, repr(x) if label is None else label,
+                r.expected
             )
             if type(r) is Error:
                 return Recovered([rep], None, loc)
-            return Recovered([rep, *r.repairs], r.min_skip, loc, r.expected)
+            return Recovered([rep, *r.repairs], r.min_prio, loc, r.expected)
         return r
 
     return recover_with_fn
 
 
 def recover_with_fn(
         parse_fns: ParseFns[S, A], fn: Callable[[S, int], A],
```

### Comparing `reparsec-0.4.1/src/reparsec/core/layout.py` & `reparsec-0.4.2/src/reparsec/core/layout.py`

 * *Files identical despite different names*

### Comparing `reparsec-0.4.1/src/reparsec/core/parser.py` & `reparsec-0.4.2/src/reparsec/core/parser.py`

 * *Files identical despite different names*

### Comparing `reparsec-0.4.1/src/reparsec/core/primitive.py` & `reparsec-0.4.2/src/reparsec/core/primitive.py`

 * *Files identical despite different names*

### Comparing `reparsec-0.4.1/src/reparsec/core/recovery.py` & `reparsec-0.4.2/src/reparsec/core/recovery.py`

 * *Files 14% similar despite different names*

```diff
@@ -21,54 +21,53 @@
 
     reps: List[Repair[C, S]] = []
     for r in ra.repairs:
         rb = parse(r.value, r.pos, r.ctx, r.ins)
         if type(rb) is Ok:
             reps.append(
                 Repair(
-                    r.skip, r.auto, r.ins if r.pos == rb.pos else ins,
-                    r.ops, merge(r.value, rb.value), rb.pos, rb.ctx,
+                    r.cost, r.prio, r.ins if r.pos == rb.pos else ins, r.ops,
+                    merge(r.value, rb.value), rb.pos, rb.ctx,
                     _append_expected(r, rb.expected, rb.consumed),
                     r.consumed or rb.consumed
                 )
             )
         elif type(rb) is Recovered:
             for rr in rb.repairs:
                 reps.append(
                     Repair(
-                        r.skip, r.auto, rr.ins, _join_ops(r, rr),
+                        r.cost + rr.cost, r.prio, rr.ins, _join_ops(r, rr),
                         merge(r.value, rr.value), rr.pos, rr.ctx,
                         _append_expected(r, rr.expected, rr.consumed),
                         r.consumed or rr.consumed
                     )
                 )
 
-    return Recovered(reps, ra.min_skip, ra.loc, ra.expected, ra.consumed)
+    return Recovered(reps, ra.min_prio, ra.loc, ra.expected, ra.consumed)
 
 
 def join_repairs(
         ra: Recovered[A, S], rb: Recovered[B, S]) -> Recovered[Union[A, B], S]:
     reps: List[Repair[Union[A, B], S]] = list(ra.repairs)
-    min_skip = ra.min_skip
-    if min_skip is not None:
+    min_prio = ra.min_prio
+    if min_prio is not None:
         reps.extend(
-            r for r in rb.repairs
-            if not r.auto or r.skip is not None and r.skip < min_skip
+            r for r in rb.repairs if r.prio is not None and r.prio < min_prio
         )
-        if rb.min_skip is not None and rb.min_skip < min_skip:
-            min_skip = rb.min_skip
+        if rb.min_prio is not None and rb.min_prio < min_prio:
+            min_prio = rb.min_prio
     else:
-        reps.extend(r for r in rb.repairs if not r.auto or r.skip is not None)
-        min_skip = rb.min_skip
+        reps.extend(r for r in rb.repairs if r.prio is not None)
+        min_prio = rb.min_prio
     if ra.consumed:
-        return Recovered(reps, min_skip, ra.loc, ra.expected, True)
+        return Recovered(reps, min_prio, ra.loc, ra.expected, True)
     if rb.consumed:
-        return Recovered(reps, min_skip, rb.loc, rb.expected, True)
+        return Recovered(reps, min_prio, rb.loc, rb.expected, True)
     return Recovered(
-        reps, min_skip, ra.loc, Append(ra.expected, rb.expected),
+        reps, min_prio, ra.loc, Append(ra.expected, rb.expected),
         ra.consumed or rb.consumed
     )
 
 
 def _join_ops(rep: Repair[A, S], repb: Repair[B, S]) -> List[OpItem]:
     ops = [OpItem(i.op, i.loc, i.expected, i.consumed) for i in rep.ops]
     ops_prepend_expected(repb.ops, rep.expected, rep.consumed)
```

### Comparing `reparsec-0.4.1/src/reparsec/core/repair.py` & `reparsec-0.4.2/src/reparsec/core/repair.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from dataclasses import dataclass
-from typing import Generic, Iterable, List, Optional, Tuple, TypeVar, Union
+from typing import Generic, Iterable, List, Optional, TypeVar, Union
 
 from typing_extensions import final
 
 from .chain import Append
 from .types import Ctx, Loc
 
 A = TypeVar("A")
@@ -12,53 +12,44 @@
 
 
 @dataclass
 @final
 class Skip:
     count: int
 
-    def cost(self) -> int:
-        return self.count
-
 
 @dataclass
 @final
 class Insert:
     label: str
 
-    def cost(self) -> int:
-        return 1
-
 
 RepairOp = Union[Skip, Insert]
 
 
 @dataclass
 class OpItem:
     op: RepairOp
     loc: Loc
     expected: Iterable[str] = ()
     consumed: bool = False
 
 
 @dataclass
 class Repair(Generic[A_co, S]):
-    skip: Optional[int]
-    auto: bool
+    cost: int
+    prio: Optional[int]
     ins: int
     ops: List[OpItem]
     value: A_co
     pos: int
     ctx: Ctx[S]
     expected: Iterable[str] = ()
     consumed: bool = False
 
-    def cost(self) -> Tuple[int, int, int]:
-        return sum(op.op.cost() for op in self.ops), -self.pos, int(self.auto)
-
 
 def ops_set_expected(ops: List[OpItem], expected: Iterable[str]) -> None:
     for op in ops:
         if not op.consumed:
             op.expected = expected
 
 
@@ -70,27 +61,36 @@
             op.consumed |= consumed
 
 
 def make_insert(
         rem: int, value: A, pos: int, ctx: Ctx[S], loc: Loc, label: str,
         expected: Iterable[str] = ()) -> Repair[A, S]:
     return Repair(
-        None, True, rem - 1, [OpItem(Insert(label), loc, expected)], value,
+        1, None, rem - 1, [OpItem(Insert(label), loc, expected)], value,
         pos, ctx, (), True
     )
 
 
+def make_user_insert(
+        rem: int, value: A, pos: int, ctx: Ctx[S], loc: Loc, label: str,
+        expected: Iterable[str] = ()) -> Repair[A, S]:
+    return Repair(
+        1, 0, rem - 1, [OpItem(Insert(label), loc, expected)], value, pos, ctx,
+        (), True
+    )
+
+
 def make_skip(
         ins: int, value: A, pos: int, ctx: Ctx[S], loc: Loc, skip: int,
         expected: Iterable[str] = ()) -> Repair[A, S]:
     return Repair(
-        skip, True, ins, [OpItem(Skip(skip), loc, expected)], value, pos, ctx,
+        skip, False, ins, [OpItem(Skip(skip), loc, expected)], value, pos, ctx,
         (), True
     )
 
 
 def make_pending_skip(
         ins: int, value: A, pos: int, ctx: Ctx[S], loc: Loc, skip: int,
         expected: Iterable[str] = ()) -> Repair[A, S]:
     return Repair(
-        skip, True, ins, [OpItem(Skip(skip), loc, expected)], value, pos, ctx
+        skip, False, ins, [OpItem(Skip(skip), loc, expected)], value, pos, ctx
     )
```

### Comparing `reparsec-0.4.1/src/reparsec/core/result.py` & `reparsec-0.4.2/src/reparsec/core/result.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,43 +85,43 @@
             self.expected = Append(expected, self.expected)
             self.consumed |= consumed
         return self
 
 
 @final
 class Recovered(Generic[A_co, S]):
-    __slots__ = "repairs", "min_skip", "loc", "expected", "consumed"
+    __slots__ = "repairs", "min_prio", "loc", "expected", "consumed"
 
     def __init__(
-            self, repairs: List[Repair[A_co, S]], min_skip: Optional[int],
+            self, repairs: List[Repair[A_co, S]], min_prio: Optional[int],
             loc: Loc, expected: Iterable[str] = (), consumed: bool = False):
         self.repairs = repairs
-        self.min_skip = min_skip
+        self.min_prio = min_prio
         self.loc = loc
         self.expected = expected
         self.consumed = consumed
 
     def __repr__(self) -> str:
         return (
-            "Recovered(repairs={!r}, min_skip={!r}, loc={!r}, expected={!r},"
+            "Recovered(repairs={!r}, min_prio={!r}, loc={!r}, expected={!r},"
             " consumed={!r})"
         ).format(
-            self.repairs, self.min_skip, self.loc, self.expected, self.consumed
+            self.repairs, self.min_prio, self.loc, self.expected, self.consumed
         )
 
     def fmap(self, fn: Callable[[A_co], B]) -> "Recovered[B, S]":
         return Recovered(
             [
                 Repair(
-                    r.skip, r.auto, r.ins, r.ops, fn(r.value), r.pos, r.ctx,
+                    r.cost, r.prio, r.ins, r.ops, fn(r.value), r.pos, r.ctx,
                     r.expected, r.consumed
                 )
                 for r in self.repairs
             ],
-            self.min_skip, self.loc, self.expected, self.consumed
+            self.min_prio, self.loc, self.expected, self.consumed
         )
 
     def set_ctx(self, ctx: Ctx[S]) -> "Recovered[A_co, S]":
         for r in self.repairs:
             r.ctx = ctx
         return self
```

### Comparing `reparsec-0.4.1/src/reparsec/core/scannerless.py` & `reparsec-0.4.2/src/reparsec/core/scannerless.py`

 * *Files identical despite different names*

### Comparing `reparsec-0.4.1/src/reparsec/core/sequence.py` & `reparsec-0.4.2/src/reparsec/core/sequence.py`

 * *Files identical despite different names*

### Comparing `reparsec-0.4.1/src/reparsec/core/stream.py` & `reparsec-0.4.2/src/reparsec/core/stream.py`

 * *Files identical despite different names*

### Comparing `reparsec-0.4.1/src/reparsec/core/types.py` & `reparsec-0.4.2/src/reparsec/core/types.py`

 * *Files identical despite different names*

### Comparing `reparsec-0.4.1/src/reparsec/layout.py` & `reparsec-0.4.2/src/reparsec/layout.py`

 * *Files identical despite different names*

### Comparing `reparsec-0.4.1/src/reparsec/lexer.py` & `reparsec-0.4.2/src/reparsec/lexer.py`

 * *Files identical despite different names*

### Comparing `reparsec-0.4.1/src/reparsec/parser.py` & `reparsec-0.4.2/src/reparsec/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,26 +3,61 @@
 """
 
 from typing import Callable, List, Optional, Tuple, TypeVar, Union
 
 from .core import combinators
 from .core.parser import ParseFns, ParseObj
 from .core.result import Result, SimpleResult
-from .core.types import Ctx
-from .types import ParserParseObj
+from .core.types import Ctx, Loc
+from .types import ParseResult, ResultWrapper
 
 S = TypeVar("S")
 S_contra = TypeVar("S_contra", contravariant=True)
 A = TypeVar("A")
 A_co = TypeVar("A_co", covariant=True)
 B = TypeVar("B")
 C = TypeVar("C")
 
 
-class Parser(ParserParseObj[S_contra, A_co]):
+def _get_loc(loc: Loc, stream: S, pos: int) -> Loc:
+    return Loc(pos, 0, 0)
+
+
+def _fmt_loc(loc: Loc) -> str:
+    return repr(loc.pos)
+
+
+class Parser(ParseObj[S_contra, A_co]):
+    def parse(
+            self, stream: S_contra, recover: bool = False, *,
+            max_insertions: int = 5,
+            get_loc: Callable[[Loc, S_contra, int], Loc] = _get_loc,
+            fmt_loc: Callable[[Loc], str] = _fmt_loc
+    ) -> ParseResult[A_co, S_contra]:
+        """
+        Parses input.
+
+        :param stream: Input to parse
+        :param recover: Flag to enable error recovery
+        :param max_insertions: Maximal number of token insertions in a row
+            during error recovery
+        :param get_loc: Function that constructs new ``Loc`` from a previous
+            ``Loc``, a stream, and position in the stream
+        :param fmt_loc: Function that converts ``Loc`` to string
+        """
+
+        ctx = Ctx(0, Loc(0, 0, 0), get_loc)
+        if recover:
+            result = self.parse_fn(
+                stream, 0, ctx, max_insertions, max_insertions
+            )
+        else:
+            result = self.parse_fast_fn(stream, 0, ctx)
+        return ResultWrapper(result, fmt_loc)
+
     def fmap(self, fn: Callable[[A_co], B]) -> "TupleParser[S_contra, B]":
         """
         Transforms the result of the parser by applying ``fn`` to it.
 
         >>> from reparsec.sequence import satisfy
 
         >>> satisfy(str.isdigit).fmap(lambda x: int(x) + 1).parse("0").unwrap()
```

### Comparing `reparsec-0.4.1/src/reparsec/primitive.py` & `reparsec-0.4.2/src/reparsec/primitive.py`

 * *Files identical despite different names*

### Comparing `reparsec-0.4.1/src/reparsec/scannerless.py` & `reparsec-0.4.2/src/reparsec/scannerless.py`

 * *Files identical despite different names*

### Comparing `reparsec-0.4.1/src/reparsec/sequence.py` & `reparsec-0.4.2/src/reparsec/sequence.py`

 * *Files identical despite different names*

### Comparing `reparsec-0.4.1/src/reparsec/types.py` & `reparsec-0.4.2/src/reparsec/types.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,18 +2,17 @@
 Core parser API.
 """
 
 from abc import abstractmethod
 from dataclasses import dataclass
 from typing import Callable, Generic, List, Optional, TypeVar
 
-from .core.parser import ParseObj
 from .core.repair import RepairOp, Skip
 from .core.result import Error, Ok, Result
-from .core.types import Ctx, Loc
+from .core.types import Loc
 
 S = TypeVar("S")
 S_contra = TypeVar("S_contra", contravariant=True)
 A_co = TypeVar("A_co", covariant=True)
 B = TypeVar("B")
 
 
@@ -95,58 +94,21 @@
         :exc:`ParseError`.
 
         :param recover: Flag to enable error recovery
         :raise: :exc:`ParseError`
         """
 
 
-def _get_loc(loc: Loc, stream: S, pos: int) -> Loc:
-    return Loc(pos, 0, 0)
-
-
-def _fmt_loc(loc: Loc) -> str:
-    return repr(loc.pos)
-
-
-class ParserParseObj(ParseObj[S_contra, A_co]):
-    def parse(
-            self, stream: S_contra, recover: bool = False, *,
-            max_insertions: int = 5,
-            get_loc: Callable[[Loc, S_contra, int], Loc] = _get_loc,
-            fmt_loc: Callable[[Loc], str] = _fmt_loc
-    ) -> ParseResult[A_co, S_contra]:
-        """
-        Parses input.
-
-        :param stream: Input to parse
-        :param recover: Flag to enable error recovery
-        :param max_insertions: Maximal number of token insertions in a row
-            during error recovery
-        :param get_loc: Function that constructs new ``Loc`` from a previous
-            ``Loc``, a stream, and position in the stream
-        :param fmt_loc: Function that converts ``Loc`` to string
-        """
-
-        ctx = Ctx(0, Loc(0, 0, 0), get_loc)
-        if recover:
-            result = self.parse_fn(
-                stream, 0, ctx, max_insertions, max_insertions
-            )
-        else:
-            result = self.parse_fast_fn(stream, 0, ctx)
-        return _ParseResult(result, fmt_loc)
-
-
-class _ParseResult(ParseResult[A_co, S]):
+class ResultWrapper(ParseResult[A_co, S]):
     def __init__(self, result: Result[A_co, S], fmt_loc: Callable[[Loc], str]):
         self._result = result
         self._fmt_loc = fmt_loc
 
     def fmap(self, fn: Callable[[A_co], B]) -> ParseResult[B, S]:
-        return _ParseResult(self._result.fmap(fn), self._fmt_loc)
+        return ResultWrapper(self._result.fmap(fn), self._fmt_loc)
 
     def unwrap(self, recover: bool = False) -> A_co:
         if type(self._result) is Ok:
             return self._result.value
 
         if type(self._result) is Error:
             raise ParseError([
@@ -161,15 +123,18 @@
             raise ParseError([
                 ErrorItem(
                     self._result.loc,
                     self._fmt_loc(self._result.loc),
                     list(self._result.expected)
                 )
             ])
-        repair = min(self._result.repairs, key=lambda r: r.cost())
+        repair = min(
+            self._result.repairs,
+            key=lambda r: (r.cost, -r.pos, r.prio is None)
+        )
         if recover:
             return repair.value
         errors = [
             ErrorItem(
                 item.loc, self._fmt_loc(item.loc), list(item.expected), item.op
             )
             for item in repair.ops
```

### Comparing `reparsec-0.4.1/setup.py` & `reparsec-0.4.2/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,17 +14,17 @@
 ['typing-extensions>=4.1,<5.0']
 
 extras_require = \
 {':python_version >= "3.6" and python_version < "3.7"': ['dataclasses>=0.8,<0.9']}
 
 setup_kwargs = {
     'name': 'reparsec',
-    'version': '0.4.1',
+    'version': '0.4.2',
     'description': 'Parser',
-    'long_description': '[![Build status](https://github.com/ethframe/reparsec/workflows/Tests/badge.svg?branch=master)](https://github.com/ethframe/reparsec/actions?query=workflow%3ATests+branch%3Amaster+event%3Apush)\n[![codecov.io](https://codecov.io/gh/ethframe/reparsec/branch/master/graph/badge.svg)](https://codecov.io/gh/ethframe/reparsec)\n[![Documentation status](https://readthedocs.org/projects/reparsec/badge/?version=latest)](https://reparsec.readthedocs.io/en/latest/?badge=latest)\n[![PyPI version](https://img.shields.io/pypi/v/reparsec)](https://pypi.org/project/reparsec)\n\n# reparsec\n\nSmall parsec-like parser combinators library with semi-automatic error recovery.\n\n## Installation\n\n```\npip install reparsec\n```\n\n## Usage\n\n* [Tutorial](https://reparsec.readthedocs.io/en/latest/pages/tutorial.html)\n* [Documentation](https://reparsec.readthedocs.io/en/latest/index.html)\n\nSimple arithmetic expression parser and calculator:\n\n```python\nfrom typing import Callable\n\nfrom reparsec import Delay\nfrom reparsec.scannerless import literal, regexp\nfrom reparsec.sequence import eof\n\n\ndef op_action(op: str) -> Callable[[int, int], int]:\n    return {\n        "+": lambda a, b: a + b,\n        "-": lambda a, b: a - b,\n        "*": lambda a, b: a * b,\n    }[op]\n\n\nspaces = regexp(r"\\s*")\nnumber = regexp(r"\\d+").fmap(int) << spaces\nmul_op = regexp(r"[*]").fmap(op_action) << spaces\nadd_op = regexp(r"[-+]").fmap(op_action) << spaces\nl_paren = literal("(") << spaces\nr_paren = literal(")") << spaces\n\nexpr = Delay[str, int]()\nvalue = number | expr.between(l_paren, r_paren)\nexpr.define(value.chainl1(mul_op).chainl1(add_op))\n\nparser = expr << eof()\n\nprint(parser.parse("1 + 2 * (3 + 4)").unwrap())\n```\n\nOutput:\n\n```\n15\n```\n\nOut-of-the-box error recovery:\n\n```python\nresult = parser.parse("1 + 2 * * (3 + 4 5)", recover=True)\n\ntry:\n    result.unwrap()\nexcept ParseError as e:\n    print(e)\n\nprint(result.unwrap(recover=True))\n```\n\nOutput:\n\n```\nat 8: expected \'(\' (skipped 2 tokens), at 17: expected \')\' (skipped 1 token)\n15\n```\n\nMore examples:\n  * [JSON parser](https://github.com/ethframe/reparsec/blob/master/tests/parsers/json.py)\n  * [Scannerless JSON parser](https://github.com/ethframe/reparsec/blob/master/tests/parsers/json_scannerless.py)\n',
+    'long_description': '[![Build status](https://github.com/ethframe/reparsec/workflows/Tests/badge.svg?branch=master)](https://github.com/ethframe/reparsec/actions?query=workflow%3ATests+branch%3Amaster+event%3Apush)\n[![codecov.io](https://codecov.io/gh/ethframe/reparsec/branch/master/graph/badge.svg)](https://codecov.io/gh/ethframe/reparsec)\n[![Documentation status](https://readthedocs.org/projects/reparsec/badge/?version=latest)](https://reparsec.readthedocs.io/en/latest/?badge=latest)\n[![PyPI version](https://img.shields.io/pypi/v/reparsec)](https://pypi.org/project/reparsec)\n\n# reparsec\n\nSmall parsec-like parser combinators library with semi-automatic error recovery.\n\n## Installation\n\n```\npip install reparsec\n```\n\n## Usage\n\n* [Tutorial](https://reparsec.readthedocs.io/en/latest/pages/tutorial.html)\n* [Documentation](https://reparsec.readthedocs.io/en/latest/index.html)\n\n## Example\n\nWith `reparsec`, simple arithmetic expression parser and evaluator could be written like this:\n\n```python\nfrom typing import Callable\n\nfrom reparsec import Delay\nfrom reparsec.scannerless import literal, parse, regexp\nfrom reparsec.sequence import eof\n\n\ndef op_action(op: str) -> Callable[[int, int], int]:\n    return {\n        "+": lambda a, b: a + b,\n        "-": lambda a, b: a - b,\n        "*": lambda a, b: a * b,\n    }[op]\n\n\nspaces = regexp(r"\\s*")\nnumber = regexp(r"\\d+").fmap(int) << spaces\nmul_op = regexp(r"[*]").fmap(op_action) << spaces\nadd_op = regexp(r"[-+]").fmap(op_action) << spaces\nl_paren = literal("(") << spaces\nr_paren = literal(")") << spaces\n\nexpr = Delay[str, int]()\nexpr.define(\n    (\n        number |\n        expr.between(l_paren, r_paren)\n    )\n    .chainl1(mul_op)\n    .chainl1(add_op)\n)\n\nparser = expr << eof()\n```\n\nThis parser can:\n\n* evaluate an expression:\n  ```python\n  >>> parser.parse("1 + 2 * (3 + 4)").unwrap()\n  15\n  ```\n* report first syntax error:\n  ```python\n  >>> parser.parse("1 + 2 * * (3 + 4 5)").unwrap()\n  Traceback (most recent call last):\n    ...\n  reparsec.types.ParseError: at 8: expected \'(\'\n  ```\n* attempt to recover and report multiple syntax errors:\n  ```python\n  >>> parser.parse("1 + 2 * * (3 + 4 5)", recover=True).unwrap()\n  Traceback (most recent call last):\n    ...\n  reparsec.types.ParseError: at 8: expected \'(\' (skipped 2 tokens), at 17: expected \')\' (skipped 1 token)\n  ```\n* automatically repair input and return some result:\n  ```python\n  >>> parser.parse("1 + 2 * * (3 + 4 5)", recover=True).unwrap(recover=True)\n  15\n  ```\n* track line and column numbers:\n  ```python\n  >>> parse(parser, """1 +\n  ... 2 * * (\n  ... 3 + 4 5)""", recover=True).unwrap()\n  Traceback (most recent call last):\n    ...\n  reparsec.types.ParseError: at 2:5: expected \'(\' (skipped 2 tokens), at 3:7: expected \')\' (skipped 1 token)\n  ```\n\nMore examples:\n  * [JSON parser](https://github.com/ethframe/reparsec/blob/master/tests/parsers/json.py)\n  * [Scannerless JSON parser](https://github.com/ethframe/reparsec/blob/master/tests/parsers/json_scannerless.py)\n',
     'author': 'ethframe',
     'author_email': 'ethframe@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/ethframe/reparsec',
     'package_dir': package_dir,
     'packages': packages,
```

### Comparing `reparsec-0.4.1/PKG-INFO` & `reparsec-0.4.2/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,31 +1,7 @@
-Metadata-Version: 2.1
-Name: reparsec
-Version: 0.4.1
-Summary: Parser
-Home-page: https://github.com/ethframe/reparsec
-License: MIT
-Author: ethframe
-Author-email: ethframe@gmail.com
-Requires-Python: >=3.6,<4.0
-Classifier: Development Status :: 4 - Beta
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Typing :: Typed
-Requires-Dist: dataclasses (>=0.8,<0.9); python_version >= "3.6" and python_version < "3.7"
-Requires-Dist: typing-extensions (>=4.1,<5.0)
-Project-URL: Documentation, https://reparsec.readthedocs.io/
-Project-URL: Repository, https://github.com/ethframe/reparsec
-Description-Content-Type: text/markdown
-
 [![Build status](https://github.com/ethframe/reparsec/workflows/Tests/badge.svg?branch=master)](https://github.com/ethframe/reparsec/actions?query=workflow%3ATests+branch%3Amaster+event%3Apush)
 [![codecov.io](https://codecov.io/gh/ethframe/reparsec/branch/master/graph/badge.svg)](https://codecov.io/gh/ethframe/reparsec)
 [![Documentation status](https://readthedocs.org/projects/reparsec/badge/?version=latest)](https://reparsec.readthedocs.io/en/latest/?badge=latest)
 [![PyPI version](https://img.shields.io/pypi/v/reparsec)](https://pypi.org/project/reparsec)
 
 # reparsec
 
@@ -38,21 +14,23 @@
 ```
 
 ## Usage
 
 * [Tutorial](https://reparsec.readthedocs.io/en/latest/pages/tutorial.html)
 * [Documentation](https://reparsec.readthedocs.io/en/latest/index.html)
 
-Simple arithmetic expression parser and calculator:
+## Example
+
+With `reparsec`, simple arithmetic expression parser and evaluator could be written like this:
 
 ```python
 from typing import Callable
 
 from reparsec import Delay
-from reparsec.scannerless import literal, regexp
+from reparsec.scannerless import literal, parse, regexp
 from reparsec.sequence import eof
 
 
 def op_action(op: str) -> Callable[[int, int], int]:
     return {
         "+": lambda a, b: a + b,
         "-": lambda a, b: a - b,
@@ -64,45 +42,58 @@
 number = regexp(r"\d+").fmap(int) << spaces
 mul_op = regexp(r"[*]").fmap(op_action) << spaces
 add_op = regexp(r"[-+]").fmap(op_action) << spaces
 l_paren = literal("(") << spaces
 r_paren = literal(")") << spaces
 
 expr = Delay[str, int]()
-value = number | expr.between(l_paren, r_paren)
-expr.define(value.chainl1(mul_op).chainl1(add_op))
+expr.define(
+    (
+        number |
+        expr.between(l_paren, r_paren)
+    )
+    .chainl1(mul_op)
+    .chainl1(add_op)
+)
 
 parser = expr << eof()
-
-print(parser.parse("1 + 2 * (3 + 4)").unwrap())
-```
-
-Output:
-
-```
-15
-```
-
-Out-of-the-box error recovery:
-
-```python
-result = parser.parse("1 + 2 * * (3 + 4 5)", recover=True)
-
-try:
-    result.unwrap()
-except ParseError as e:
-    print(e)
-
-print(result.unwrap(recover=True))
 ```
 
-Output:
+This parser can:
 
-```
-at 8: expected '(' (skipped 2 tokens), at 17: expected ')' (skipped 1 token)
-15
-```
+* evaluate an expression:
+  ```python
+  >>> parser.parse("1 + 2 * (3 + 4)").unwrap()
+  15
+  ```
+* report first syntax error:
+  ```python
+  >>> parser.parse("1 + 2 * * (3 + 4 5)").unwrap()
+  Traceback (most recent call last):
+    ...
+  reparsec.types.ParseError: at 8: expected '('
+  ```
+* attempt to recover and report multiple syntax errors:
+  ```python
+  >>> parser.parse("1 + 2 * * (3 + 4 5)", recover=True).unwrap()
+  Traceback (most recent call last):
+    ...
+  reparsec.types.ParseError: at 8: expected '(' (skipped 2 tokens), at 17: expected ')' (skipped 1 token)
+  ```
+* automatically repair input and return some result:
+  ```python
+  >>> parser.parse("1 + 2 * * (3 + 4 5)", recover=True).unwrap(recover=True)
+  15
+  ```
+* track line and column numbers:
+  ```python
+  >>> parse(parser, """1 +
+  ... 2 * * (
+  ... 3 + 4 5)""", recover=True).unwrap()
+  Traceback (most recent call last):
+    ...
+  reparsec.types.ParseError: at 2:5: expected '(' (skipped 2 tokens), at 3:7: expected ')' (skipped 1 token)
+  ```
 
 More examples:
   * [JSON parser](https://github.com/ethframe/reparsec/blob/master/tests/parsers/json.py)
   * [Scannerless JSON parser](https://github.com/ethframe/reparsec/blob/master/tests/parsers/json_scannerless.py)
-
```

