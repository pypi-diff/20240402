# Comparing `tmp/orderedsets-2024.1-py3-none-any.whl.zip` & `tmp/orderedsets-2024.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 6928 bytes, number of entries: 7
--rw-r--r--  2.0 unx    13664 b- defN 24-Mar-04 20:27 orderedsets/__init__.py
+Zip file size: 7040 bytes, number of entries: 7
+-rw-r--r--  2.0 unx    13646 b- defN 24-Apr-02 21:07 orderedsets/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 24-Jan-25 23:07 orderedsets/py.typed
--rw-r--r--  2.0 unx     1097 b- defN 24-Mar-04 21:31 orderedsets-2024.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     4414 b- defN 24-Mar-04 21:31 orderedsets-2024.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Mar-04 21:31 orderedsets-2024.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 24-Mar-04 21:31 orderedsets-2024.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      566 b- defN 24-Mar-04 21:31 orderedsets-2024.1.dist-info/RECORD
-7 files, 19845 bytes uncompressed, 5920 bytes compressed:  70.2%
+-rw-r--r--  2.0 unx     1097 b- defN 24-Apr-02 21:49 orderedsets-2024.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     4584 b- defN 24-Apr-02 21:49 orderedsets-2024.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-02 21:49 orderedsets-2024.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 24-Apr-02 21:49 orderedsets-2024.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      566 b- defN 24-Apr-02 21:49 orderedsets-2024.2.dist-info/RECORD
+7 files, 19997 bytes uncompressed, 6032 bytes compressed:  69.8%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: orderedsets/__init__.py
 Comment: 
 
 Filename: orderedsets/py.typed
 Comment: 
 
-Filename: orderedsets-2024.1.dist-info/LICENSE
+Filename: orderedsets-2024.2.dist-info/LICENSE
 Comment: 
 
-Filename: orderedsets-2024.1.dist-info/METADATA
+Filename: orderedsets-2024.2.dist-info/METADATA
 Comment: 
 
-Filename: orderedsets-2024.1.dist-info/WHEEL
+Filename: orderedsets-2024.2.dist-info/WHEEL
 Comment: 
 
-Filename: orderedsets-2024.1.dist-info/top_level.txt
+Filename: orderedsets-2024.2.dist-info/top_level.txt
 Comment: 
 
-Filename: orderedsets-2024.1.dist-info/RECORD
+Filename: orderedsets-2024.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## orderedsets/__init__.py

```diff
@@ -72,52 +72,52 @@
         """Return a string representation of this set."""
         if len(self) == 0:
             return "OrderedSet()"
         return "OrderedSet({" + ", ".join([repr(k) for k in self._dict]) + "})"
 
     def add(self, element: T) -> None:
         """Add *element* to this set."""
-        self._dict = {**self._dict, **{element: None}}
+        self._dict[element] = None
 
     def clear(self) -> None:
         """Remove all elements from this set."""
         self._dict.clear()
 
     def copy(self) -> OrderedSet[T]:
         """Return a shallow copy of this set."""
         return OrderedSet(self._dict.copy())
 
     def difference(self, *others: Iterable[T]) -> OrderedSet[T]:
         """Return all elements that are in this set but not in *others*."""
         if not others:
             return OrderedSet(self._dict)
         other_elems = set.union(*map(set, others))
-        items = {item: None for item in self if item not in other_elems}
+        items = [item for item in self._dict if item not in other_elems]
         return OrderedSet(items)
 
     def difference_update(self, *others: Iterable[T]) -> None:
         """Update this set to remove all items that are in *others*."""
         for other in others:
             for e in other:
                 self.discard(e)
 
     def discard(self, element: T) -> None:
-        """Remove *element* from this set, if it is present."""
+        """Remove *element* from this set if it is present."""
+        # try/except and self._dict.pop(element, None) seem to be slower than this,
+        # independent of whether 'element' is present or not.
         if element in self._dict:
             del self._dict[element]
 
     def intersection(self, *others: Iterable[T]) -> OrderedSet[T]:
-        """Return the intersection of this set and *others*."""
+        """Return a new set with elements common to this set and all *others*."""
         if not others:
             return OrderedSet(self._dict)
 
-        result_elements = []
-        for element in self._dict.keys():
-            if all(element in other for other in others):
-                result_elements.append(element)
+        oth = set(self).intersection(*others)
+        result_elements = [element for element in self._dict if element in oth]
 
         return OrderedSet(result_elements)
 
     def intersection_update(self, *others: Iterable[T]) -> None:
         """Update this set to be the intersection of itself and *others*."""
         if not others:
             return
@@ -138,18 +138,15 @@
 
     def issuperset(self, s: Iterable[T]) -> bool:
         """Return whether this set is a superset of *s*."""
         return set(self).issuperset(set(s))
 
     def pop(self) -> T:
         """Remove and return the most recently added element from this set."""
-        items = list(self._dict)
-        result = items.pop()
-        self._dict = dict.fromkeys(items)
-        return result
+        return self._dict.popitem()[0]
 
     def remove(self, element: T) -> None:
         """Remove *element* from this set, raising :exc:`KeyError` if not present."""
         del self._dict[element]
 
     def symmetric_difference(self, s: Iterable[T]) -> OrderedSet[T]:
         """Return the symmetric difference of this set and *s*."""
@@ -158,15 +155,15 @@
                           + [e for e in s if e not in self._dict]))
 
     def symmetric_difference_update(self, s: Iterable[T]) -> None:
         """Update this set to be the symmetric difference of itself and *s*."""
         self._dict = self.symmetric_difference(s)._dict
 
     def union(self, *others: Iterable[T]) -> OrderedSet[T]:
-        """Return the union of this set and *others*."""
+        """Return a new set with elements from this set and *others*."""
         return OrderedSet(list(self._dict)
                           + [e for other in others for e in other])
 
     def update(self, *others: Iterable[T]) -> None:
         """Update this set to be the union of itself and *others*."""
         self._dict = self.union(*others)._dict
 
@@ -265,15 +262,15 @@
         # change across Python invocations (e.g. due to hash randomization of
         # strings stored in the FrozenOrderedSet), so make sure it is not saved
         # here.
         return (self.__class__, (self._dict,))
 
     def __hash__(self) -> int:
         """Return a hash of this set."""
-        if self._my_hash:
+        if self._my_hash is not None:
             return self._my_hash
 
         self._my_hash = hash(frozenset(self))
         return self._my_hash
 
     def __eq__(self, other: object) -> bool:
         """Return whether this set is equal to *other*."""
@@ -304,26 +301,24 @@
         return FrozenOrderedSet(self._dict)
 
     def difference(self, *others: Iterable[T]) -> FrozenOrderedSet[T]:
         """Return the difference of this set and *others*."""
         if not others:
             return FrozenOrderedSet(self._dict)
         other_elems = set.union(*map(set, others))
-        items = {item: None for item in self if item not in other_elems}
+        items = [item for item in self._dict if item not in other_elems]
         return FrozenOrderedSet(items)
 
     def intersection(self, *others: Iterable[T]) -> FrozenOrderedSet[T]:
         """Return the intersection of this set and *others*."""
         if not others:
             return FrozenOrderedSet(self._dict)
 
-        result_elements = []
-        for element in self._dict.keys():
-            if all(element in other for other in others):
-                result_elements.append(element)
+        oth = set(self).intersection(*others)
+        result_elements = [element for element in self._dict if element in oth]
 
         return FrozenOrderedSet(result_elements)
 
     def symmetric_difference(self, s: Iterable[T]) -> FrozenOrderedSet[T]:
         """Return the symmetric difference of this set and *s*."""
         return FrozenOrderedSet(
             dict.fromkeys([e for e in self._dict if e not in s]
```

## Comparing `orderedsets-2024.1.dist-info/LICENSE` & `orderedsets-2024.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `orderedsets-2024.1.dist-info/METADATA` & `orderedsets-2024.2.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orderedsets
-Version: 2024.1
+Version: 2024.2
 Summary: An implementation of mutable and immutable ordered sets.
 Author-email: Matthias Diener <matthias.diener@gmail.com>, Andreas Kloeckner <inform@tiker.net>
 License: MIT License
         
         Copyright (c) 2023 University of Illinois Board of Trustees
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -43,15 +43,17 @@
 
 # orderedsets
 
 An implementation of mutable and immutable ordered sets as thin wrappers around
 Python's `dict` class.
 These classes are meant as drop-in replacements for Python's builtin `set` and
 `frozenset` classes. Care has been taken to provide the same functionality as the Python classes,
-without API additions or removals, to allow easy switching between set implementations.
+without API additions or removals, to allow easy switching between set implementations. These classes are often
+[faster than other ordered set implementations](https://matthiasdiener.github.io/orderedsets/speed.html)
+(but slower than Python's builtin sets).
 
 In contrast to Python's builtin `set` and `frozenset` classes, the order of
 items is kept (generally, insertion order), such that iterating over items in
 the set as well as mutating operations are deterministic.
 
 This package has no external dependencies.
```

