# Comparing `tmp/qldpc-0.0.8.tar.gz` & `tmp/qldpc-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qldpc-0.0.8.tar", max compression
+gzip compressed data, was "qldpc-0.0.9.tar", max compression
```

## Comparing `qldpc-0.0.8.tar` & `qldpc-0.0.9.tar`

### file list

```diff
@@ -1,18 +1,19 @@
--rw-r--r--   0        0        0    11358 2024-01-06 01:03:13.384764 qldpc-0.0.8/LICENSE
--rw-r--r--   0        0        0     3978 2024-03-15 14:26:44.914324 qldpc-0.0.8/README.md
--rw-r--r--   0        0        0     4370 2024-03-19 21:40:37.707911 qldpc-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      219 2024-03-19 15:42:26.348531 qldpc-0.0.8/qldpc/__init__.py
--rw-r--r--   0        0        0    34387 2024-03-19 21:31:13.171390 qldpc-0.0.8/qldpc/abstract.py
--rw-r--r--   0        0        0     7223 2024-03-19 15:42:26.348531 qldpc-0.0.8/qldpc/abstract_test.py
--rw-r--r--   0        0        0    66995 2024-03-19 21:39:28.310631 qldpc-0.0.8/qldpc/codes.py
--rw-r--r--   0        0        0    17602 2024-03-19 21:31:13.172390 qldpc-0.0.8/qldpc/codes_test.py
--rw-r--r--   0        0        0     6387 2024-03-19 15:42:26.348531 qldpc-0.0.8/qldpc/decoder.py
--rw-r--r--   0        0        0     2259 2024-03-19 15:42:26.348531 qldpc-0.0.8/qldpc/decoder_test.py
--rw-r--r--   0        0        0     2035 2024-03-19 17:34:21.199468 qldpc-0.0.8/qldpc/named_codes.py
--rw-r--r--   0        0        0     2482 2024-03-19 17:44:30.377978 qldpc-0.0.8/qldpc/named_codes_test.py
--rw-r--r--   0        0        0    11443 2024-03-19 15:42:26.348531 qldpc-0.0.8/qldpc/objects.py
--rw-r--r--   0        0        0     5053 2024-03-19 15:42:26.348531 qldpc-0.0.8/qldpc/objects_test.py
--rw-r--r--   0        0        0        0 2023-12-28 20:08:33.445385 qldpc-0.0.8/qldpc/py.typed
--rw-r--r--   0        0        0     7487 2024-03-19 16:58:45.273188 qldpc-0.0.8/qldpc/small_groups.py
--rw-r--r--   0        0        0     8391 2024-03-19 17:44:30.377978 qldpc-0.0.8/qldpc/small_groups_test.py
--rw-r--r--   0        0        0     5475 1970-01-01 00:00:00.000000 qldpc-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0    11358 2024-01-06 01:03:13.384764 qldpc-0.0.9/LICENSE
+-rw-r--r--   0        0        0     4755 2024-03-28 02:09:55.432602 qldpc-0.0.9/README.md
+-rw-r--r--   0        0        0     4198 2024-03-28 13:33:02.369161 qldpc-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      219 2024-03-19 22:37:40.195418 qldpc-0.0.9/qldpc/__init__.py
+-rw-r--r--   0        0        0    34557 2024-03-28 02:09:55.433601 qldpc-0.0.9/qldpc/abstract.py
+-rw-r--r--   0        0        0     7680 2024-03-28 02:09:55.433601 qldpc-0.0.9/qldpc/abstract_test.py
+-rw-r--r--   0        0        0    90976 2024-03-28 03:18:02.474171 qldpc-0.0.9/qldpc/codes.py
+-rw-r--r--   0        0        0    22219 2024-03-28 02:09:55.433601 qldpc-0.0.9/qldpc/codes_test.py
+-rw-r--r--   0        0        0     6541 2024-03-24 21:39:24.069554 qldpc-0.0.9/qldpc/decoder.py
+-rw-r--r--   0        0        0     2265 2024-03-24 21:39:24.069554 qldpc-0.0.9/qldpc/decoder_test.py
+-rw-r--r--   0        0        0     2036 2024-03-28 02:09:42.426462 qldpc-0.0.9/qldpc/named_codes.py
+-rw-r--r--   0        0        0     2482 2024-03-24 21:39:24.069554 qldpc-0.0.9/qldpc/named_codes_test.py
+-rw-r--r--   0        0        0     8403 2024-03-28 02:09:42.426462 qldpc-0.0.9/qldpc/named_groups.py
+-rw-r--r--   0        0        0     9914 2024-03-28 02:09:42.426462 qldpc-0.0.9/qldpc/named_groups_test.py
+-rw-r--r--   0        0        0    18535 2024-03-28 02:09:55.433601 qldpc-0.0.9/qldpc/objects.py
+-rw-r--r--   0        0        0     5547 2024-03-28 02:09:55.434602 qldpc-0.0.9/qldpc/objects_test.py
+-rw-r--r--   0        0        0        0 2023-12-28 20:08:33.445385 qldpc-0.0.9/qldpc/py.typed
+-rw-r--r--   0        0        0      550 2024-03-28 13:26:51.181313 qldpc-0.0.9/qldpc/test.py
+-rw-r--r--   0        0        0     6208 1970-01-01 00:00:00.000000 qldpc-0.0.9/PKG-INFO
```

### Comparing `qldpc-0.0.8/LICENSE` & `qldpc-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `qldpc-0.0.8/README.md` & `qldpc-0.0.9/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # qLDPC
 
-This package contains tools for constructing and analyzing [quantum low density partity check (qLDPC) codes](https://errorcorrectionzoo.org/c/qldpc).
+This package contains tools for constructing and analyzing [quantum low density parity check (qLDPC) codes](https://errorcorrectionzoo.org/c/qldpc).
 
 ## 📦 Installation
 
 This package requires Python>=3.10, and can be installed from PyPI with
 ```
 pip install qldpc
 ```
@@ -14,26 +14,31 @@
 pip install -e qLDPC
 ```
 You can also `pip install -e 'qLDPC[dev]'` to additionally install some development tools.
 
 ## 🚀 Features
 
 Notable features include:
-- `abstract.py`: module for basic abstract algebra (groups, algebras, and representations thereof).
 - `ClassicalCode`: class for representing classical linear error-correcting codes over finite fields.
+  - Various pre-defined classical code families.
+  - Communication with the [GAP/GUAVA](https://www.gap-system.org/Packages/guava.html) package for [even more codes](https://docs.gap-system.org/pkg/guava/doc/chap5.html).
 - `QuditCode`: general class for constructing [Galois-qudit codes](https://errorcorrectionzoo.org/c/galois_into_galois).
 - `CSSCode`: general class for constructing [quantum CSS codes](https://errorcorrectionzoo.org/c/css) out of two mutually compatible `ClassicalCode`s.
   - `CSSCode.get_logical_ops`: method to construct a complete basis of nontrivial logical operators for a `CSSCode`.
-  - `CSSCode.get_distance`: method to compute the code distance (i.e., the minimum weight of a nontrivial logical operator) of a `CSSCode`.  Includes options for computing the exact code distance by brute force, as well as estimate (or upper bound) with the method of [arXiv:2308.07915](https://arxiv.org/abs/2308.07915).
+  - `CSSCode.get_distance`: method to compute the code distance (i.e., the minimum weight of a nontrivial logical operator) of a `CSSCode`.  Includes options for computing the exact code distance by brute force, as well as an estimate (or upper bound) with the method of [arXiv:2308.07915](https://arxiv.org/abs/2308.07915).
   - Includes options for applying local Hadamard transformations, which is useful for tailoring a `CSSCode` to biased noise (see [arXiv:2202.01702](https://arxiv.org/abs/2202.01702)).  Options to apply more general Clifford code deformations are pending.
 - `GBCode`: class for constructing [generalized bicycle codes](https://errorcorrectionzoo.org/c/generalized_bicycle), as described in [arXiv:1904.02703](https://arxiv.org/abs/1904.02703).
 - `QCCode`: class for constructing the [quasi-cyclic codes](https://errorcorrectionzoo.org/c/quantum_quasi_cyclic) in [arXiv:2308.07915](https://arxiv.org/abs/2308.07915).
 - `HGPCode`: class for constructing [hypergraph product codes](https://errorcorrectionzoo.org/c/hypergraph_product) out of two `ClassicalCode`s.
 - `LPCode`: class for constructing [lifted product codes](https://errorcorrectionzoo.org/c/lifted_product) out of two protographs (i.e., matrices whose entries are elements of a group algebra).  See [arXiv:2012.04068](https://arxiv.org/abs/2012.04068) and [arXiv:2202.01702](https://arxiv.org/abs/2202.01702).
 - `QTCode`: class for constructing [quantum Tanner codes](https://errorcorrectionzoo.org/c/quantum_tanner) out of (a) two symmetric subsets `A` and `B` of a group `G`, and (b) two `ClassicalCode`s with block lengths `|A|` and `|B|`.  See [arXiv:2202.13641](https://arxiv.org/abs/2202.13641) and [arXiv:2206.07571](https://arxiv.org/abs/2206.07571).
+- `abstract.py`: module for basic abstract algebra (groups, algebras, and representations thereof).
+  - Various pre-defined groups (mostly borrowed from [SymPy](https://docs.sympy.org/latest/modules/combinatorics/named_groups.html)).
+  - Communication with the [GAP](https://www.gap-system.org/) computer algebra system and [GroupNames.org](https://people.maths.bris.ac.uk/~matyd/GroupNames/) for constructing [even more groups](https://docs.gap-system.org/doc/ref/chap50.html).
+- `objects.py`: module for constructing and helper objects such as Cayley complexes and chain complexes, which are instrumental for the construction of various quantum codes.
 
 ## 🤔 Questions and issues
 
 If this project gains interest and traction, I'll add a documentation webpage and material to help users get started quickly.  I am also planning to write a paper that presents and explains this project.  In the meantime, you can explore the documentation and explanations in the source code.  `qldpc/codes_test.py` contains some examples of using the classes and methods described above.
 
 If you have any questions, feedback, or requests, please [open an issue on GitHub](https://github.com/Infleqtion/qLDPC/issues/new) or email me at [michael.perlin@infleqtion.com](mailto:michael.perlin@infleqtion.com)!
```

### Comparing `qldpc-0.0.8/pyproject.toml` & `qldpc-0.0.9/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "qLDPC"
-version = "0.0.8"
-description = "Tools for constructing and analyzing quantum low density partity check (qLDPC) codes."
+version = "0.0.9"
+description = "Tools for constructing and analyzing quantum low density parity check (qLDPC) codes."
 license = "Apache-2.0"
 authors = ["Michael A. Perlin <mika.perlin@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/Infleqtion/qLDPC"
 keywords = [
   "quantum computing",
   "quantum error correction",
@@ -35,18 +35,14 @@
 ldpc = ">=0.1.0"
 networkx = ">=2.6.2"
 numpy = ">=1.22.0"
 platformdirs = ">=4.0.0"
 pymatching = ">=2.1.0"
 sympy = ">=1.12"
 
-# TODO: remove once https://github.com/python/typeshed/issues/11254 is resolved
-# more context: https://github.com/Infleqtion/qLDPC/pull/10
-types-protobuf = "<=4.24.0.4"
-
 checks-superstaq = { version = ">=0.5.0", optional = true }
 
 [tool.poetry.extras]
 dev = ["checks-superstaq"]
 
 # Check script configuration:
```

### Comparing `qldpc-0.0.8/qldpc/abstract.py` & `qldpc-0.0.9/qldpc/abstract.py`

 * *Files 3% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 
 import galois
 import numpy as np
 import numpy.typing as npt
 import sympy.combinatorics as comb
 import sympy.core
 
-from qldpc import small_groups
+from qldpc import named_groups
 
 DEFAULT_FIELD_ORDER = 2
 
 
 ################################################################################
 # groups and group members
 
@@ -189,14 +189,15 @@
         return self._group
 
     @property
     def field(self) -> type[galois.FieldArray]:
         """Base field of this group."""
         return self._field
 
+    @property
     def order(self) -> int:
         """Number of members in this group."""
         return self._group.order()
 
     @property
     def generators(self) -> Sequence[GroupMember]:
         """Generators of this group."""
@@ -230,15 +231,15 @@
     @functools.cached_property
     def table(self) -> npt.NDArray[np.int_]:
         """Multiplication (Cayley) table for this group."""
         members = {member: idx for idx, member in enumerate(self.generate())}
         return np.array(
             [members[aa * bb] for aa in self.generate() for bb in self.generate()],
             dtype=int,
-        ).reshape((self.order(),) * 2)
+        ).reshape(self.order, self.order)
 
     @classmethod
     def from_table(
         cls,
         table: npt.NDArray[np.int_] | Sequence[Sequence[int]],
         field: int | None = None,
         integer_lift: IntegerLift | None = None,
@@ -339,18 +340,18 @@
         """Construct a random symmetric subset of a given size.
 
         Note: this is not a uniformaly random subset, only a "sufficiently random" one.
 
         WARNING: not all groups have symmetric subsets of arbitrary size.  If called with a poor
         choice of group and subset size, this method may never terminate.
         """
-        if not 0 < size <= self.order():
+        if not 0 < size <= self.order:
             raise ValueError(
                 "A random symmetric subset of this group must have a size between 1 and"
-                f" {self.order()} (provided: {size})"
+                f" {self.order} (provided: {size})"
             )
         if seed is not None:
             sympy.core.random.seed(seed)
 
         singles = set()  # group members equal to their own inverse
         doubles = set()  # pairs of group members and their inverses
         while True:  # sounds dangerous, but bear with me
@@ -377,14 +378,22 @@
                 for _ in range(num_extra // 2):
                     member = doubles.pop()
                     doubles.remove(~member)
                 if num_extra % 2:
                     singles.pop()
                 return singles | doubles
 
+    @classmethod
+    def from_name(cls, name: str) -> Group:
+        """Named group in the GAP computer algebra system."""
+        standardized_name = name.strip().replace(" ", "")  # remove whitespace
+        generators = named_groups.get_generators(standardized_name)
+        group = comb.PermutationGroup(*[GroupMember(gen) for gen in generators])
+        return Group(group)
+
 
 ################################################################################
 # elements of a group algebra
 
 
 class Element:
     """An element of a group algebra over a finite field F_q.
@@ -411,60 +420,72 @@
             and all(self._vec[member] == other._vec[member] for member in self._vec)
             and all(self._vec[member] == other._vec[member] for member in other._vec)
         )
 
     def __iter__(self) -> Iterator[tuple[GroupMember, galois.FieldArray]]:
         yield from self._vec.items()
 
-    def __add__(self, other: GroupMember | Element) -> Element:
-        new_element = self.copy()
+    def __add__(self, other: int | GroupMember | Element) -> Element:
+        if isinstance(other, int):
+            return self + other * self.one()
 
         if isinstance(other, GroupMember):
+            new_element = self.copy()
             new_element._vec[other] += self.field(1)
             return new_element
 
-        # isinstance(other, Element)
-        for member, val in other:
-            new_element._vec[member] += val
-        return new_element
+        if isinstance(other, Element):
+            new_element = self.copy()
+            for member, val in other:
+                new_element._vec[member] += val
+            return new_element
+
+        return NotImplemented  # pragma: no cover
 
-    def __sub__(self, other: GroupMember | Element) -> Element:
+    def __sub__(self, other: Element | GroupMember | int) -> Element:
         return self + (-1) * other
 
     def __radd__(self, other: GroupMember) -> Element:
         return self + other
 
     def __mul__(self, other: int | GroupMember | Element) -> Element:
-        new_element = self.zero()
-
         if isinstance(other, int):
             # multiply coefficients by 'other'
+            new_element = self.zero()
             for member, val in self:
                 new_element._vec[member] = val * other
             return new_element
 
         if isinstance(other, GroupMember):
             # multiply group members by 'other'
+            new_element = self.zero()
             for member, val in self:
                 new_element._vec[member * other] = val
+            return new_element
 
-        # collect and multiply pairs of terms from 'self' and 'other'
-        for (aa, x_a), (bb, y_b) in itertools.product(self, other):
-            new_element._vec[aa * bb] += x_a * y_b
-        return new_element
+        if isinstance(other, Element):
+            # collect and multiply pairs of terms from 'self' and 'other'
+            new_element = self.zero()
+            for (aa, x_a), (bb, y_b) in itertools.product(self, other):
+                new_element._vec[aa * bb] += x_a * y_b
+            return new_element
+
+        return NotImplemented  # pragma: no cover
 
     def __rmul__(self, other: int | GroupMember) -> Element:
         if isinstance(other, int):
             return self * other
 
-        # multiply group members by "other"
-        new_element = self.zero()
-        for member, val in self:
-            new_element._vec[other * member] = val
-        return new_element
+        if isinstance(other, GroupMember):
+            new_element = self.zero()
+            for member, val in self:
+                new_element._vec[other * member] = val
+            return new_element
+
+        return NotImplemented  # pragma: no cover
 
     def __neg__(self) -> Element:
         return self * (-1)
 
     def __pow__(self, power: int) -> Element:
         return functools.reduce(Element.__mul__, [self] * power, self.one())
 
@@ -514,83 +535,79 @@
         return new_element
 
 
 ################################################################################
 # protographs: Element-valued matrices
 
 
-ObjectMatrix = npt.NDArray[np.object_] | Sequence[Sequence[object]]
-
-
-class Protograph:
-    """Matrix with Element entries."""
-
-    _matrix: npt.NDArray[np.object_]
-
-    def __init__(self, matrix: Protograph | ObjectMatrix) -> None:
-        if isinstance(matrix, Protograph):
-            self._matrix = matrix.matrix
-        else:
-            self._matrix = np.array(matrix, ndmin=2)
-
-    def __eq__(self, other: object) -> bool:
-        return isinstance(other, Protograph) and np.array_equal(self._matrix, other._matrix)
+class Protograph(npt.NDArray[np.object_]):
+    """Array whose entries are members of a group algebra over a finite field."""
 
-    def __rmul__(self, val: int) -> Protograph:
-        return Protograph(self._matrix * val)
+    _group: Group
 
-    def __mul__(self, val: int) -> Protograph:
-        return val * self
+    def __new__(
+        cls, array: npt.NDArray[np.object_] | Sequence[Sequence[object]], group: Group | None = None
+    ) -> Protograph:
+        protograph = np.asarray(array).view(cls)
 
-    @property
-    def matrix(self) -> npt.NDArray[np.object_]:
-        """Element-valued numpy matrix of this protograph."""
-        return self._matrix
+        # identify the base group for this protograph
+        for value in protograph.ravel():
+            if not isinstance(value, Element):
+                raise ValueError(
+                    "Requirement failed: all entries of a protograph must be Element-valued"
+                )
+            else:
+                if not (group is None or group == value.group):
+                    raise ValueError("Inconsistent base groups provided for protograph")
+                group = value.group
+
+        if group is None:
+            raise ValueError("Cannot determine underlying group for a protograh")
+        protograph._group = group
 
-    @property
-    def shape(self) -> tuple[int, ...]:
-        """Dimensions (shape) of this protograph."""
-        return self._matrix.shape
+        return protograph
 
     @property
     def group(self) -> Group:
-        """Group associated with this protograph."""
-        return self._matrix[0, 0].group
+        """Base group of this protograph."""
+        return self._group
 
     @property
     def field(self) -> type[galois.FieldArray]:
         """Base field of this protograph."""
         return self.group.field
 
     def lift(self) -> galois.FieldArray:
         """Block matrix obtained by lifting each entry of the protograph."""
-        vals = [val.lift() for val in self.matrix.ravel()]
+        vals = [val.lift() for val in self.ravel()]
         tensor = np.transpose(np.reshape(vals, self.shape + vals[0].shape), [0, 2, 1, 3])
         rows = tensor.shape[0] * tensor.shape[1]
         cols = tensor.shape[2] * tensor.shape[3]
-        return tensor.reshape(rows, cols)  # type:ignore[return-value]
+        return self.field(tensor.reshape(rows, cols))
 
     @property
     def T(self) -> Protograph:
-        """Transpose of this protograph, which also transposes every matrix entry."""
-        entries = [entry.T for entry in self._matrix.ravel()]
-        return Protograph(np.array(entries).reshape(self._matrix.shape).T)
+        """Transpose of this protograph, which also transposes every array entry."""
+        vals = [val.T for val in self.ravel()]
+        return Protograph(np.array(vals, dtype=object).reshape(self.shape).T)
 
     @classmethod
-    def build(cls, group: Group, matrix: ObjectMatrix, *, field: int = 2) -> Protograph:
+    def build(
+        cls, group: Group, array: npt.NDArray[np.object_] | Sequence[Sequence[object]]
+    ) -> Protograph:
         """Construct a protograph.
 
-        The constructed protograph is built from (i) a group, and (ii) a matrix populated by group
+        The constructed protograph is built from (i) a group, and (ii) an array populated by group
         members or zero/"falsy" entries.  The protograph is obtained by elevating the group memebers
         to elements of the group algebra (over the prime number field).  Zero/"falsy" entries of the
         matrix are interpreted as zeros of the group algebra.
         """
-        matrix = np.array(matrix)
-        vals = [Element(group, member) if member else Element(group) for member in matrix.ravel()]
-        return Protograph(np.array(vals, dtype=object).reshape(matrix.shape))
+        array = np.array(array, dtype=object)
+        vals = [Element(group, member) if member else Element(group) for member in array.ravel()]
+        return Protograph(np.array(vals, dtype=object).reshape(array.shape))
 
 
 ################################################################################
 # "simple" named groups
 
 
 class TrivialGroup(Group):
@@ -633,14 +650,31 @@
     basis vector <i| as <i| L(g^p) = < i + p mod R |.
     """
 
     def __init__(self, order: int) -> None:
         super().__init__(comb.named_groups.CyclicGroup(order))
 
 
+class AbelianGroup(Group):
+    """Direct product of cyclic groups of the specified orders.
+
+    By default, an AbelianGroup member of the form ∏_i g_i^{a_i}, where {g_i} are the generators of
+    the group, gets lifted to a direct sum ⨁_i L(g_i)^{a_i}.  If an AbelianGroup is initalized with
+    product_lift=True, the group members get lifted to a Kronecker product ⨂_i L(g_i)^{a_i}.
+    """
+
+    def __init__(self, *orders: int, product_lift: bool = False) -> None:
+        if product_lift:
+            groups = [CyclicGroup(order) for order in orders]
+            group = Group.product(*groups)
+            super().__init__(group)
+        else:
+            super().__init__(comb.named_groups.AbelianGroup(*orders))
+
+
 class DihedralGroup(Group):
     """Dihedral group of a specified order."""
 
     def __init__(self, order: int) -> None:
         super().__init__(comb.named_groups.DihedralGroup(order))
 
 
@@ -654,64 +688,14 @@
 class SymmetricGroup(Group):
     """Symmetric group of a specified order."""
 
     def __init__(self, order: int) -> None:
         super().__init__(comb.named_groups.SymmetricGroup(order))
 
 
-class DicyclicGroup(Group):
-    """Dicyclic group of order <= 20.
-
-    Generating matrices taken from: https://people.maths.bris.ac.uk/~matyd/GroupNames/dicyclic.html
-
-    Additional references:
-    - https://en.wikipedia.org/wiki/Dicyclic_group
-    - https://groupprops.subwiki.org/wiki/Dicyclic_group
-    """
-
-    def __init__(self, order: int) -> None:  # noqa: max-complexity
-        if not (order > 0 and order % 4 == 0):
-            raise ValueError(
-                "Dicyclic groups only supported for orders that are positive multiples of 4"
-                + f" (provided: {order})"
-            )
-        if not order <= 20:
-            raise ValueError(
-                f"Dicyclic groups only supported for orders up to 20 (provided: {order})"
-            )
-
-        if order == 4:
-            gen_a = comb.Permutation(0, 2)(1, 3)
-            gen_b = comb.Permutation(0, 3, 2, 1)
-
-        elif order == 8:
-            gen_a = comb.Permutation(1, 2, 3, 4)(5, 6, 7, 8)
-            gen_b = comb.Permutation(1, 7, 3, 5)(2, 6, 4, 8)
-
-        elif order == 12:
-            # Special case with more compact representation:
-            # https://math.stackexchange.com/a/2837920
-            gen_a = comb.Permutation(1, 2, 3)(4, 6)(5, 7)
-            gen_b = comb.Permutation(2, 3)(4, 5, 6, 7)
-
-        elif order == 16:
-            gen_a = comb.Permutation(1, 2, 3, 4, 5, 6, 7, 8)(9, 10, 11, 12, 13, 14, 15, 16)
-            gen_b = comb.Permutation(1, 9, 5, 13)(2, 16, 6, 12)(3, 15, 7, 11)(4, 14, 8, 10)
-
-        elif order == 20:
-            gen_a = comb.Permutation(1, 2, 3, 4, 5, 6, 7, 8, 9, 10)(
-                11, 12, 13, 14, 15, 16, 17, 18, 19, 20
-            )
-            gen_b = comb.Permutation(1, 14, 6, 19)(2, 13, 7, 18)(3, 12, 8, 17)(4, 11, 9, 16)(
-                5, 20, 10, 15
-            )
-
-        super().__init__(comb.PermutationGroup(gen_a, gen_b))
-
-
 class QuaternionGroup(Group):
     """Quaternion group: 1, i, j, k, -1, -i, -j, -k."""
 
     def __init__(self) -> None:
         table = [
             [0, 1, 2, 3, 4, 5, 6, 7],
             [1, 4, 3, 6, 5, 0, 7, 2],
@@ -741,14 +725,40 @@
                 blocks = [[zero, -imag], [-imag, zero]]
             return sign * np.block(blocks).T % 3
 
         group = Group.from_table(table, integer_lift=lift)
         super().__init__(group._group, field=3, lift=group._lift)
 
 
+class SmallGroup(Group):
+    """Group indexed by the GAP computer algebra system."""
+
+    def __init__(self, order: int, index: int) -> None:
+        num_groups = SmallGroup.number(order)
+        if not 1 <= index <= num_groups:
+            raise ValueError(
+                f"Index for SmallGroup of order {order} must be between 1 and {num_groups}"
+                + f" (provided: {index})"
+            )
+
+        name = f"SmallGroup({order},{index})"
+        super().__init__(Group.from_name(name))
+
+    @classmethod
+    def number(cls, order: int) -> int:
+        """The number of groups of a given order."""
+        return named_groups.get_small_group_number(order)
+
+    @classmethod
+    def generator(cls, order: int) -> Iterator[SmallGroup]:
+        """Iterator over all groups of a given order."""
+        for ii in range(SmallGroup.number(order)):
+            yield SmallGroup(order, ii + 1)
+
+
 ################################################################################
 # special linear (SL) and projective special linear (PSL) groups
 
 
 class SpecialLinearGroup(Group):
     """Special linear group (SL): square matrices with determinant 1."""
 
@@ -874,20 +884,7 @@
             # to quotient SL(d,q) by -I, force the first non-zero entry to be <= q/2
             if vec[(vec != 0).argmax()] <= type(mat).order // 2:
                 yield mat
 
 
 SL = SpecialLinearGroup
 PSL = ProjectiveSpecialLinearGroup
-
-
-################################################################################
-# groups indexed by the GAP computer algebra system
-
-
-class SmallGroup(Group):
-    """Groups indexed by the GAP computer algebra system."""
-
-    def __init__(self, order: int, index: int) -> None:
-        generators = small_groups.get_generators(order, index)
-        group = comb.PermutationGroup(*[GroupMember(gen) for gen in generators])
-        super().__init__(group)
```

### Comparing `qldpc-0.0.8/qldpc/abstract_test.py` & `qldpc-0.0.9/qldpc/abstract_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -55,14 +55,16 @@
     assert group == abstract.Group.from_generating_mats()
 
 
 def test_lift() -> None:
     """Lift named group elements."""
     assert_valid_lift(abstract.TrivialGroup())
     assert_valid_lift(abstract.CyclicGroup(3))
+    assert_valid_lift(abstract.AbelianGroup(2, 3))
+    assert_valid_lift(abstract.AbelianGroup(2, 3, product_lift=True))
     assert_valid_lift(abstract.DihedralGroup(3))
     assert_valid_lift(abstract.AlternatingGroup(3))
     assert_valid_lift(abstract.SymmetricGroup(3))
     assert_valid_lift(abstract.QuaternionGroup())
 
 
 def assert_valid_lift(group: abstract.Group) -> None:
@@ -101,42 +103,49 @@
 
 def test_algebra() -> None:
     """Construct elements of a group algebra."""
     group = abstract.TrivialGroup(field=3)
     zero = abstract.Element(group)
     one = abstract.Element(group).one()
     assert zero.group == group
-    assert one + one + one == group.identity + 2 * one == -one + one == one - one == zero
+    assert one + 2 == group.identity + 2 * one == -one + 1 == one - 1 == zero
     assert group.identity * one == one * group.identity == one**2 == one
     assert np.array_equal(zero.lift(), np.array(0, ndmin=2))
     assert np.array_equal(one.lift(), np.array(1, ndmin=2))
 
 
 def test_protograph() -> None:
     """Construct and lift a protograph."""
     matrix = np.random.randint(2, size=(3, 3))
     protograph = abstract.TrivialGroup.to_protograph(matrix)
     assert protograph.group == abstract.TrivialGroup()
-    assert 1 * protograph == protograph * 1 == protograph
-    assert protograph == abstract.Protograph(protograph)
-    assert np.array_equal(protograph.lift(), matrix)
     assert protograph.field == abstract.TrivialGroup().field
+    assert np.array_equal(protograph.lift(), matrix)
+
+    # fail to construct a valid protograph
+    with pytest.raises(ValueError, match="must be Element-valued"):
+        abstract.Protograph([[0]])
+    with pytest.raises(ValueError, match="Inconsistent base groups"):
+        groups = [abstract.TrivialGroup(), abstract.CyclicGroup(1)]
+        abstract.Protograph([[abstract.Element(group) for group in groups]])
+    with pytest.raises(ValueError, match="Cannot determine underlying group"):
+        abstract.Protograph([])
 
 
 def test_transpose() -> None:
     """Transpose various objects."""
     group = abstract.CyclicGroup(4)
     for member in group.generate():
         element = abstract.Element(group, member)
         assert element.T.T == element
 
     x0, x1, x2, x3 = group.generate()
     matrix = [[x0, 0, x1], [x2, 0, x3]]
     protograph = abstract.Protograph.build(group, matrix)
-    assert protograph.T.T == protograph
+    assert np.array_equal(protograph.T.T, protograph)
 
 
 def test_random_symmetric_subset() -> None:
     """Cover Group.random_symmetric_subset."""
     group = abstract.CyclicGroup(2) * abstract.CyclicGroup(3)
     for seed in [0, 1]:
         subset = group.random_symmetric_subset(size=2, seed=seed)
@@ -145,58 +154,55 @@
     subset = group.random_symmetric_subset(size=1, exclude_identity=False, seed=0)
     assert subset == {group.identity}
 
     with pytest.raises(ValueError, match="must have a size between"):
         group.random_symmetric_subset(size=0)
 
 
-def test_dicyclic_group() -> None:
-    """Dicyclic group."""
-    for order in range(4, 21, 4):
-        group = abstract.DicyclicGroup(order)
-        gen_a, gen_b = group.generators
-        assert gen_a ** (order // 2) == gen_b**4 == group.identity
-
-    with pytest.raises(ValueError, match="positive multiples of 4"):
-        abstract.DicyclicGroup(2)
-
-    with pytest.raises(ValueError, match="orders up to 20"):
-        abstract.DicyclicGroup(24)
-
-
 def test_SL(field: int = 3) -> None:
     """Special linear group."""
     for linear_rep in [False, True]:
         group = abstract.SL(2, field=field, linear_rep=linear_rep)
         gens = group.generators
         mats = group.get_generator_mats()
         assert np.array_equal(group.lift(gens[0]), mats[0])
         assert np.array_equal(group.lift(gens[1]), mats[1].view(np.ndarray))
 
-    assert len(list(abstract.SL.iter_mats(2, 2))) == abstract.SL(2, 2).order()
+    assert len(list(abstract.SL.iter_mats(2, 2))) == abstract.SL(2, 2).order
 
     # cover representation with different generators
     assert len(abstract.SL(2, 5).generators) == 2
 
 
 def test_PSL(field: int = 3) -> None:
     """Projective special linear group."""
     group = abstract.PSL(2, 2)
     assert group.generators == abstract.SL(2, 2).generators
     assert group.dimension == 2
 
-    assert len(list(abstract.PSL.iter_mats(2, 2))) == abstract.PSL(2, 2).order()
-    assert abstract.PSL(2, 3).order() == 24
+    assert len(list(abstract.PSL.iter_mats(2, 2))) == abstract.PSL(2, 2).order
+    assert abstract.PSL(2, 3).order == 24
 
     with pytest.raises(ValueError, match="not yet supported"):
         abstract.PSL(3, 3)
 
 
-def test_small_groups() -> None:
+def test_small_group() -> None:
     """Groups indexed by the GAP computer algebra system."""
     order, index = 2, 1
     desired_group = abstract.CyclicGroup(order)
-    generators = [tuple(gen.array_form) for gen in desired_group.generators]
 
-    with unittest.mock.patch("qldpc.small_groups.get_generators", return_value=generators):
-        group = abstract.SmallGroup(order, index)
-        assert group.generators == desired_group.generators
+    # invalid group index
+    with (
+        pytest.raises(ValueError, match="Index for SmallGroup"),
+        unittest.mock.patch("qldpc.named_groups.get_small_group_number", return_value=index),
+    ):
+        abstract.SmallGroup(order, 0)
+
+    # everything works as expected
+    generators = [tuple(gen.array_form) for gen in desired_group.generators]
+    with (
+        unittest.mock.patch("qldpc.abstract.SmallGroup.number", return_value=index),
+        unittest.mock.patch("qldpc.named_groups.get_generators", return_value=generators),
+    ):
+        assert abstract.SmallGroup(order, index).generators == desired_group.generators
+        assert list(abstract.SmallGroup.generator(order)) == [desired_group]
```

### Comparing `qldpc-0.0.8/qldpc/codes.py` & `qldpc-0.0.9/qldpc/codes.py`

 * *Files 18% similar despite different names*

```diff
@@ -17,26 +17,36 @@
 
 from __future__ import annotations
 
 import abc
 import functools
 import itertools
 import random
-from collections.abc import Collection, Hashable, Iterable, Sequence
+from collections.abc import Callable, Collection, Iterable, Sequence
 from typing import Literal
 
 import galois
 import ldpc.mod2
 import networkx as nx
 import numpy as np
 import numpy.typing as npt
+import sympy
+import sympy.combinatorics as comb
 
 import qldpc
 from qldpc import abstract, named_codes
-from qldpc.objects import CayleyComplex, Node, Pauli, QuditOperator
+from qldpc.objects import (
+    PAULIS_XZ,
+    CayleyComplex,
+    ChainComplex,
+    Node,
+    Pauli,
+    PauliXZ,
+    QuditOperator,
+)
 
 DEFAULT_FIELD_ORDER = 2
 
 
 def get_random_nontrivial_vec(field: type[galois.FieldArray], size: int) -> galois.FieldArray:
     """Get a random nontrivial vector of a given size."""
     while not (vec := field.Random(size)).any():
@@ -106,29 +116,41 @@
         """Convert a Tanner graph into a parity check matrix."""
 
 
 ################################################################################
 # classical codes
 
 
+# TODO:
+# - add code concatenation
 class ClassicalCode(AbstractCode):
     """Classical linear error-correcting code over a finite field F_q.
 
     A classical binary code C = {x} is a set of vectors x (with entries in F_q) called code words.
     We consider only linear codes, for which any linear combination of code words is also code word.
 
     Operationally, we define a classical code by a parity check matrix H with dimensions
     (num_checks, num_bits).  Each row of H represents a linear constraint (a "check") that code
     words must satisfy.  A vector x is a code word iff H @ x = 0.
     """
 
     _matrix: galois.FieldArray
+    _exact_distance: int | None = None
 
-    def __contains__(self, word: npt.NDArray[np.int_] | Sequence[int]) -> bool:
-        return not np.any(self.matrix @ self.field(word))
+    def __contains__(
+        self, words: npt.NDArray[np.int_] | Sequence[int] | Sequence[Sequence[int]] | ClassicalCode
+    ) -> bool:
+        """Does this code contain the given word(s)?
+
+        If passed a ClassicalCode for "words", interpret it to mean "all words in the given code",
+        which are spanned by the code's generator matrix.
+        """
+        if isinstance(words, ClassicalCode):
+            words = words.generator
+        return not np.any(self.matrix @ self.field(words).T)
 
     @classmethod
     def matrix_to_graph(cls, matrix: npt.NDArray[np.int_] | Sequence[Sequence[int]]) -> nx.DiGraph:
         """Convert a parity check matrix H into a Tanner graph.
 
         The Tanner graph is a bipartite graph with (num_checks, num_bits) vertices, respectively
         identified with the checks and bits of the code.  The check vertex c and the bit vertex b
@@ -144,25 +166,42 @@
         return graph
 
     @classmethod
     def graph_to_matrix(cls, graph: nx.DiGraph) -> galois.FieldArray:
         """Convert a Tanner graph into a parity check matrix."""
         num_bits = sum(1 for node in graph.nodes() if node.is_data)
         num_checks = len(graph.nodes()) - num_bits
-        field = graph.order if hasattr(graph, "order") else DEFAULT_FIELD_ORDER
+        field = getattr(graph, "order", DEFAULT_FIELD_ORDER)
         matrix = galois.GF(field).Zeros((num_checks, num_bits))
         for node_c, node_b, data in graph.edges(data=True):
             matrix[node_c.index, node_b.index] = data.get("val", 1)
         return matrix
 
     @functools.cached_property
     def generator(self) -> galois.FieldArray:
         """Generator of this code: a matrix whose rows for a basis for code words."""
         return self.matrix.null_space()
 
+    def __eq__(self, other: object) -> bool:
+        """Equality test between two classical code instances."""
+        return (
+            isinstance(other, ClassicalCode)
+            and self.field is other.field
+            and np.array_equal(self.matrix, other.matrix)
+        )
+
+    @classmethod
+    def equiv(cls, code_a: ClassicalCode, code_b: ClassicalCode) -> bool:
+        """Test equivalence between two classical codes.
+
+        Two classical codes are equivalent if they have the same code words.  Equivalently, codes
+        C_a and C_b are equivalent if they contain each other, C_a ⊆ C_b and C_b ⊆ C_a.
+        """
+        return code_a.field is code_b.field and code_a in code_b and code_b in code_a
+
     def words(self) -> galois.FieldArray:
         """Code words of this code."""
         vectors = itertools.product(self.field.elements, repeat=self.generator.shape[0])
         return self.field(list(vectors)) @ self.generator
 
     def get_random_word(self) -> galois.FieldArray:
         """Random code word: a sum all generators with random field coefficients."""
@@ -178,21 +217,21 @@
         return ClassicalCode(self.generator)
 
     def __invert__(self) -> ClassicalCode:
         return self.dual()
 
     @classmethod
     def tensor_product(cls, code_a: ClassicalCode, code_b: ClassicalCode) -> ClassicalCode:
-        """Tensor product C_a ⊗ C_b of two codes C_a and C_b.
+        """Tensor product C_a ⨂ C_b of two codes C_a and C_b.
 
         Let G_a and G_b respectively denote the generators C_a and C_b.
-        Definition: C_a ⊗ C_b is the code whose generators are G_a ⊗ G_b.
+        Definition: C_a ⨂ C_b is the code whose generators are G_a ⨂ G_b.
 
-        Observation: G_a ⊗ G_b is the check matrix of ~(C_a ⊗ C_b).
-        We therefore construct ~(C_a ⊗ C_b) and return its dual ~~(C_a ⊗ C_b) = C_a ⊗ C_b.
+        Observation: G_a ⨂ G_b is the check matrix of ~(C_a ⨂ C_b).
+        We therefore construct ~(C_a ⨂ C_b) and return its dual ~~(C_a ⨂ C_b) = C_a ⨂ C_b.
         """
         if code_a.field is not code_b.field:
             raise ValueError("Cannot take tensor product of codes over different fields")
         gen_a: npt.NDArray[np.int_] = code_a.generator
         gen_b: npt.NDArray[np.int_] = code_b.generator
         return ~ClassicalCode(np.kron(gen_a, gen_b))
 
@@ -244,17 +283,24 @@
     ) -> int:
         """Compute the minimal weight of a nontrivial code word by brute force.
 
         If passed a vector, compute the minimal Hamming distance between the vector and a code word.
         """
         if vector is not None:
             words = self.words() - self.field(vector)[np.newaxis, :]
-        else:
-            words = self.words()[1:]
-        return np.min(np.count_nonzero(words.view(np.ndarray), axis=1))
+            return np.min(np.count_nonzero(words.view(np.ndarray), axis=1))
+
+        # if we know the exact code distance, return it
+        if self._exact_distance is not None:
+            return self._exact_distance
+
+        # we do not know the exact distance, so compute it
+        words = self.words()[1:]
+        self._exact_distance = np.min(np.count_nonzero(words.view(np.ndarray), axis=1))
+        return self._exact_distance
 
     def get_distance_bound(
         self,
         num_trials: int = 1,
         *,
         vector: Sequence[int] | npt.NDArray[np.int_] | None = None,
         **decoder_args: object,
@@ -354,22 +400,52 @@
 
         while has_zero_row_or_column(matrix := code_field.Random((checks, bits))):
             pass
 
         return ClassicalCode(matrix)
 
     @classmethod
+    def from_generator(
+        self, generator: npt.NDArray[np.int_] | Sequence[Sequence[int]], field: int | None = None
+    ) -> ClassicalCode:
+        """Construct a ClassicalCode from a generator matrix."""
+        return ~ClassicalCode(generator, field)
+
+    @classmethod
     def from_name(cls, name: str) -> ClassicalCode:
         """Named code in the GAP computer algebra system."""
         standardized_name = name.strip().replace(" ", "")  # remove whitespace
         matrix, field = named_codes.get_code(standardized_name)
         return ClassicalCode(matrix, field)
 
-    # TODO(?): maybe add modification options
-    # https://users.math.msu.edu/users/halljo/classes/codenotes/mod.pdf
+    def puncture(self, *bits: int) -> ClassicalCode:
+        """Delete the specified bits from a code.
+
+        To delete bits from the code, we remove the corresponding columns from its generator matrix.
+        """
+        assert all(0 <= bit < self.num_bits for bit in bits)
+        bits_to_keep = [bit for bit in range(self.num_bits) if bit not in bits]
+        generator = [word[bits_to_keep] for word in self.generator]
+        return ClassicalCode.from_generator(generator, self.field.order)
+
+    def shorten(self, *bits: int) -> ClassicalCode:
+        """Shorten a code to the words that are zero on the specified bits, and delete those bits.
+
+        To shorten a code on a given bit, we:
+        - move the bit to the first position,
+        - row-reduce the generator matrix into the form [ identity_matrix, other_stuff ], and
+        - delete the first row and column from the generator matrix.
+        """
+        assert all(0 <= bit < self.num_bits for bit in bits)
+        generator = self.generator
+        for bit in sorted(bits, reverse=True):
+            generator = np.roll(generator, -bit, axis=1)  # type:ignore[assignment]
+            generator = generator.row_reduce()[1:, 1:]
+            generator = np.roll(generator, bit, axis=1)  # type:ignore[assignment]
+        return ClassicalCode.from_generator(generator)
 
 
 class RepetitionCode(ClassicalCode):
     """Classical repetition code."""
 
     def __init__(self, bits: int, field: int | None = None) -> None:
         self._field = galois.GF(field or DEFAULT_FIELD_ORDER)
@@ -391,14 +467,15 @@
 
 
 class HammingCode(ClassicalCode):
     """Classical Hamming code."""
 
     def __init__(self, rank: int, field: int | None = None) -> None:
         """Construct a Hamming code of a given rank."""
+        self._exact_distance = 3
         self._field = galois.GF(field or DEFAULT_FIELD_ORDER)
         if self.field.order == 2:
             # parity check matrix: columns = all nonzero bitstrings
             bitstrings = list(itertools.product([0, 1], repeat=rank))
             self._matrix = self.field(bitstrings[1:]).T
 
         else:
@@ -446,14 +523,15 @@
     References:
     - https://errorcorrectionzoo.org/c/reed_muller
     - https://feog.github.io/10-coding.pdf
     """
 
     def __init__(self, order: int, size: int, field: int | None = None) -> None:
         self._assert_valid_params(order, size)
+        self._exact_distance = 2 ** (size - order)
         self._order = order
         self._size = size
 
         generator = ReedMullerCode.get_generator(order, size)
         self._matrix = ClassicalCode(generator, field).generator
         self._field = galois.GF(field or DEFAULT_FIELD_ORDER)
 
@@ -476,44 +554,22 @@
     def _assert_valid_params(self, order: int, size: int) -> None:
         if not (size >= 0 and 0 <= order <= size):
             raise ValueError(
                 "Reed-Muller code R(r,m) must have m >= 0 and 0 <= r <= m\n"
                 + f"Provided: (r,m) = ({order},{size})"
             )
 
-    def get_distance_exact(
-        self, *, vector: Sequence[int] | npt.NDArray[np.int_] | None = None
-    ) -> int:
-        """Minimal weight of a nontrivial code word.
-
-        If passed a vector, compute (by brute force) the minimal Hamming distance between the vector
-        and a code word.
-        """
-        if vector is None:
-            return 2 ** (self._size - self._order)
-        return super().get_distance_exact(vector=vector)
-
-    def get_one_distance_bound(
-        self, *, vector: Sequence[int] | npt.NDArray[np.int_] | None = None, **decoder_args: object
-    ) -> int:
-        """Return a single upper bound on code distance.
-
-        If passed a vector, compute (by decoding) the minimal Hamming distance between the vector
-        and a code word.
-        """
-        if vector is None:
-            return self.get_distance_exact()
-        return super().get_one_distance_bound(vector=vector, **decoder_args)
-
 
 ################################################################################
 # quantum codes
 
 
 # TODO:
+# - add code concatenation
+# - investigate weight reduction: https://arxiv.org/abs/2402.05228
 # - add is_CSS method to figure out whether this is a CSS Code
 #   - see https://quantumcomputing.stackexchange.com/questions/15432/
 #   - also compute and store sub-codes, if CSS
 #   - also add QuditCode.to_CSS() -> CSSCode
 class QuditCode(AbstractCode):
     """Quantum stabilizer code for Galois qudits, with dimension q = p^m for prime p and integer m.
 
@@ -529,14 +585,16 @@
     Warning: here j, r, s, etc. not integers, but elements of the Galois field GF(q), which has
     different rules for addition and multiplication when q is not a prime number.
 
     Helpful lecture by Gottesman: https://www.youtube.com/watch?v=JWg4zrNAF-g
     """
 
     _matrix: galois.FieldArray
+    _exact_distance_x: int | None = None
+    _exact_distance_z: int | None = None
 
     @property
     def num_checks(self) -> int:
         """Number of parity checks (stabilizers) in this code."""
         return self.matrix.shape[0]
 
     @property
@@ -601,16 +659,16 @@
     def get_stabilizers(self) -> list[str]:
         """Stabilizers (checks) of this code, represented by strings."""
         matrix = self.matrix.reshape(self.num_checks, 2, self.num_qudits)
         stabilizers = []
         for check in range(self.num_checks):
             ops = []
             for qudit in range(self.num_qudits):
-                val_x = matrix[check, Pauli.X.index, qudit]
-                val_z = matrix[check, Pauli.Z.index, qudit]
+                val_x = matrix[check, Pauli.X, qudit]
+                val_z = matrix[check, Pauli.Z, qudit]
                 vals_xz = (val_x, val_z)
                 if self.field.order == 2:
                     ops.append(str(Pauli(vals_xz)))
                 else:
                     ops.append(str(QuditOperator(vals_xz)))
             stabilizers.append(" ".join(ops))
         return stabilizers
@@ -667,14 +725,16 @@
 
     code_x: ClassicalCode  # X-type parity checks, measuring Z-type errors
     code_z: ClassicalCode  # Z-type parity checks, measuring X-type errors
 
     _conjugate: slice | Sequence[int]
     _codes_equal: bool
     _logical_ops: galois.FieldArray | None = None
+    _exact_distance_x: int | None = None
+    _exact_distance_z: int | None = None
 
     def __init__(
         self,
         code_x: ClassicalCode | npt.NDArray[np.int_] | Sequence[Sequence[int]],
         code_z: ClassicalCode | npt.NDArray[np.int_] | Sequence[Sequence[int]],
         field: int | None = None,
         *,
@@ -690,44 +750,69 @@
         if field is None and self.code_x.field is not self.code_z.field:
             raise ValueError("The sub-codes provided for this CSSCode are over different fields")
         self._field = self.code_x.field
 
         if not skip_validation and not self.is_valid:
             raise ValueError("The sub-codes provided for this CSSCode are incompatible")
 
-        self._conjugate = conjugate or ()
+        self._conjugated_qubits = conjugate or ()
         self._codes_equal = self.code_x == self.code_z
 
     @functools.cached_property
     def is_valid(self) -> bool:
         """Is this a valid CSS code?"""
         return self.code_x.num_bits == self.code_z.num_bits and not np.any(
-            self.code_x.matrix @ self.code_z.matrix.T
+            self.matrix_x @ self.matrix_z.T
         )
 
     @functools.cached_property
     def matrix(self) -> galois.FieldArray:
         """Overall parity check matrix."""
         matrix = np.block(
             [
-                [self.code_z.matrix, np.zeros_like(self.code_z.matrix)],
-                [np.zeros_like(self.code_x.matrix), self.code_x.matrix],
+                [self.matrix_z, np.zeros_like(self.matrix_z)],
+                [np.zeros_like(self.matrix_x), self.matrix_x],
             ]
         )
-        return self.field(self.conjugate(matrix, self._conjugate))
+        return self.field(self.conjugate(matrix, self.conjugated_qubits))
+
+    @property
+    def matrix_x(self) -> galois.FieldArray:
+        """X-type parity checks."""
+        return self.code_x.matrix
+
+    @property
+    def matrix_z(self) -> galois.FieldArray:
+        """Z-type parity checks."""
+        return self.code_z.matrix
+
+    @property
+    def conjugated_qubits(self) -> slice | Sequence[int]:
+        """Which qubits are conjugated?"""
+        return self._conjugated_qubits
+
+    @property
+    def num_checks_x(self) -> int:
+        """Number of X-type parity checks in this code."""
+        return self.matrix_x.shape[0]
+
+    @property
+    def num_checks_z(self) -> int:
+        """Number of X-type parity checks in this code."""
+        return self.matrix_z.shape[0]
 
     @property
     def num_checks(self) -> int:
         """Number of parity checks in this code."""
-        return self.code_x.matrix.shape[0] + self.code_z.matrix.shape[0]
+        return self.num_checks_x + self.num_checks_z
 
     @property
     def num_qudits(self) -> int:
         """Number of data qudits in this code."""
-        return self.code_x.matrix.shape[1]
+        return self.matrix_x.shape[1]
 
     @property
     def dimension(self) -> int:
         """Number of logical qudits encoded by this code."""
         return self.code_x.dimension + self.code_z.dimension - self.num_qudits
 
     def get_code_params(
@@ -744,15 +829,15 @@
         Keyword arguments are passed to the calculation of code distance.
         """
         distance = self.get_distance(pauli=None, bound=bound, vector=None, **decoder_args)
         return self.num_qudits, self.dimension, distance, self.get_weight()
 
     def get_distance(
         self,
-        pauli: Literal[Pauli.X, Pauli.Z] | None = None,
+        pauli: PauliXZ | None = None,
         *,
         bound: int | bool | None = None,
         vector: Sequence[int] | npt.NDArray[np.int_] | None = None,
         **decoder_args: object,
     ) -> int:
         """Compute (or upper bound) the minimal weight of a nontrivial logical operator.
 
@@ -767,46 +852,57 @@
         `CSSCode.get_one_distance_bound`.
         """
         if bound is None:
             return self.get_distance_exact(pauli, vector=vector)
         return self.get_distance_bound(pauli, num_trials=int(bound), vector=vector, **decoder_args)
 
     def get_distance_exact(
-        self,
-        pauli: Literal[Pauli.X, Pauli.Z] | None,
-        *,
-        vector: Sequence[int] | npt.NDArray[np.int_] | None = None,
+        self, pauli: PauliXZ | None, *, vector: Sequence[int] | npt.NDArray[np.int_] | None = None
     ) -> int:
         """Compute the minimal weight of a nontrivial code word by brute force.
 
         If provided a vector, compute the minimum Hamming distance between this vector and a
         (possibly trivial) X-type or Z-type logical operator, as applicable.
         """
-        assert pauli in [None, Pauli.X, Pauli.Z]
+        assert pauli is None or pauli in PAULIS_XZ
         if pauli is None:
             return min(
                 self.get_distance_exact(Pauli.X, vector=vector),
                 self.get_distance_exact(Pauli.Z, vector=vector),
             )
 
-        code_x = self.code_x if pauli == Pauli.X else self.code_z
-        code_z = self.code_z if pauli == Pauli.X else self.code_x
-
         if vector is not None:
+            code_z = self.code_z if pauli == Pauli.X else self.code_x
             ops_x = code_z.words()
             vector = self.field(vector)
             return min(np.count_nonzero(word - vector) for word in ops_x)
 
+        # if we know the exact code distance, return it
+        if pauli == Pauli.X and self._exact_distance_x is not None:
+            return self._exact_distance_x
+        if pauli == Pauli.Z and self._exact_distance_z is not None:
+            return self._exact_distance_z
+
+        # we do not know the exact distance, so compute it
+        code_x = self.code_x if pauli == Pauli.X else self.code_z
+        code_z = self.code_z if pauli == Pauli.X else self.code_x
         dual_code_x = ~code_x
         nontrivial_ops_x = (word for word in code_z.words() if word not in dual_code_x)
-        return min(np.count_nonzero(word) for word in nontrivial_ops_x)
+        distance = min(np.count_nonzero(word) for word in nontrivial_ops_x)
+
+        # save the exact distance and return
+        if pauli == Pauli.X:
+            self._exact_distance_x = distance
+        if pauli == Pauli.Z:
+            self._exact_distance_z = distance
+        return distance
 
     def get_distance_bound(
         self,
-        pauli: Literal[Pauli.X, Pauli.Z] | None = None,
+        pauli: PauliXZ | None = None,
         num_trials: int = 1,
         *,
         vector: Sequence[int] | npt.NDArray[np.int_] | None = None,
         **decoder_args: object,
     ) -> int:
         """Compute an upper bound on code distance by minimizing many individual upper bounds.
 
@@ -820,15 +916,15 @@
             self.get_one_distance_bound(pauli, vector=vector, **decoder_args)
             for _ in range(num_trials)
         )
         return min(distance_bounds, default=self.num_qudits)
 
     def get_one_distance_bound(
         self,
-        pauli: Literal[Pauli.X, Pauli.Z] | None = None,
+        pauli: PauliXZ | None = None,
         *,
         vector: Sequence[int] | npt.NDArray[np.int_] | None = None,
         **decoder_args: object,
     ) -> int:
         """Compute a single upper bound on code distance.
 
         If provided a vector, compute the minimum Hamming distance between this vector and a
@@ -859,16 +955,16 @@
 
         We solve the above decoding problem with a decoder in `decode`.  If the decoder fails to
         find a solution, try again with a new random operator Z(w_z).  If the decoder succeeds in
         finding a solution w_x, this solution corresponds to a logical X-type operator X(w_x) -- and
         presumably one of low Hamming weight, since decoders try to find low-weight solutions.
         Return the Hamming weight |w_x|.
         """
-        assert pauli in [None, Pauli.X, Pauli.Z]
-        pauli = pauli or random.choice([Pauli.X, Pauli.Z])
+        assert pauli is None or pauli in PAULIS_XZ
+        pauli = pauli or random.choice(PAULIS_XZ)
 
         # define code_z and pauli_z as if we are computing X-distance
         code_z = self.code_z if pauli == Pauli.X else self.code_x
         pauli_z: Literal[Pauli.Z, Pauli.X] = Pauli.Z if pauli == Pauli.X else Pauli.X
 
         if vector is not None:
             # find the distance of the given vector from a logical X-type operator
@@ -898,29 +994,38 @@
             # check whether decoding was successful
             actual_syndrome = effective_check_matrix @ candidate_logical_op % self.field.order
             logical_op_found = np.array_equal(actual_syndrome, effective_syndrome)
 
         # return the Hamming weight of the logical operator
         return int(np.count_nonzero(candidate_logical_op))
 
-    def get_logical_ops(self) -> galois.FieldArray:
+    def get_logical_ops(self, pauli: PauliXZ | None = None) -> galois.FieldArray:
         """Complete basis of nontrivial X-type and Z-type logical operators for this code.
 
         Logical operators are represented by a three-dimensional array `logical_ops` with dimensions
         (2, k, n), where k and n are respectively the numbers of logical and physical qudits in this
         code.  The bitstring `logical_ops[0, 4, :]`, for example, indicates the support (i.e., the
         physical qudits addressed nontrivially) by the logical Pauli-X operator on logical qudit 4.
 
+        If passed a pauli operator (Pauli.X or Pauli.Z), return the two-dimensional array of logical
+        operators of the specified type.
+
         In the case of qudits with dimension > 2, the "Pauli-X" and "Pauli-Z" operators constructed
         by this method are the unit shift and phase operators that generate all logical X-type and
         Z-type qudit operators.
 
         Logical operators are constructed using the method described in Section 4.1 of Gottesman's
         thesis (arXiv:9705052), slightly modified and generalized for qudits.
         """
+        assert pauli is None or pauli in PAULIS_XZ
+
+        # if requested, retrieve logical operators of one type only
+        if pauli is not None:
+            return self.get_logical_ops()[pauli]
+
         # memoize manually because other methods may modify the logical operators computed here
         if self._logical_ops is not None:
             return self._logical_ops
 
         num_qudits = self.num_qudits
         dimension = self.dimension
         identity = self.field.Identity(dimension)
@@ -947,16 +1052,16 @@
                 pivots = np.concatenate([[pivots[0]], pivots[1:][pivots[1:] != 0]])
 
             # identify remaining columns and return
             other = [qq for qq in range(matrix.shape[1]) if qq not in pivots]
             return matrix_RRE, pivots, other
 
         # identify check matrices for X/Z-type errors, and the current qudit locations
-        checks_x: npt.NDArray[np.int_] = self.code_z.matrix
-        checks_z: npt.NDArray[np.int_] = self.code_x.matrix
+        checks_x: npt.NDArray[np.int_] = self.matrix_z
+        checks_z: npt.NDArray[np.int_] = self.matrix_x
         qudit_locs = np.arange(num_qudits, dtype=int)
 
         # row reduce the check matrix for X-type errors and move its pivots to the back
         checks_x, pivot_x, other_x = row_reduce(checks_x)
         checks_x = np.hstack([checks_x[:, other_x], checks_x[:, pivot_x]])
         checks_z = np.hstack([checks_z[:, other_x], checks_z[:, pivot_x]])
         qudit_locs = np.hstack([qudit_locs[other_x], qudit_locs[pivot_x]])
@@ -990,15 +1095,15 @@
         logicals_x = logicals_x[:, permutation]
         logicals_z = logicals_z[:, permutation]
 
         self._logical_ops = self.field(np.stack([logicals_x, logicals_z]))
         return self._logical_ops
 
     def get_random_logical_op(
-        self, pauli: Literal[Pauli.X, Pauli.Z], *, ensure_nontrivial: bool = False
+        self, pauli: PauliXZ, *, ensure_nontrivial: bool = False
     ) -> galois.FieldArray:
         """Return a random logical operator of a given type.
 
         A random logical operator may be trivial, which is to say that it may be equal to the
         identity modulo stabilizers.  If `ensure_nontrivial is True`, ensure that the logical
         operator we return is nontrivial.
         """
@@ -1006,34 +1111,34 @@
         if not ensure_nontrivial:
             return (self.code_z if pauli == Pauli.X else self.code_x).get_random_word()
 
         # generate random logical ops until we find ones with a nontrivial commutation relation
         noncommuting_ops_found = False
         while not noncommuting_ops_found:
             op_a = self.get_random_logical_op(pauli, ensure_nontrivial=False)
-            op_b = self.get_random_logical_op(pauli, ensure_nontrivial=False)
+            op_b = self.get_random_logical_op(
+                ~pauli, ensure_nontrivial=False  # type:ignore[arg-type]
+            )
             noncommuting_ops_found = bool(np.any(op_a @ op_b))
 
         return op_a
 
-    def reduce_logical_op(
-        self, pauli: Literal[Pauli.X, Pauli.Z], logical_index: int, **decoder_args: object
-    ) -> None:
+    def reduce_logical_op(self, pauli: PauliXZ, logical_index: int, **decoder_args: object) -> None:
         """Reduce the weight of a logical operator.
 
         A minimal-weight logical operator is found by enforcing that it has a trivial syndrome, and
         that it commutes with all logical operators except its dual.  This is essentially the same
         method as that used in CSSCode.get_one_distance_bound.
         """
         assert pauli == Pauli.X or pauli == Pauli.Z
         assert 0 <= logical_index < self.dimension
 
         # effective check matrix = syndromes and other logical operators
         code = self.code_z if pauli == Pauli.X else self.code_x
-        all_dual_ops = self.get_logical_ops()[(~pauli).index]
+        all_dual_ops = self.get_logical_ops(~pauli)  # type:ignore[arg-type]
         effective_check_matrix = np.vstack([code.matrix, all_dual_ops]).view(np.ndarray)
         dual_op_index = code.num_checks + logical_index
 
         # enforce that the new logical operator commutes with everything except its dual
         effective_syndrome = np.zeros((code.num_checks + self.dimension), dtype=int)
         effective_syndrome[dual_op_index] = 1
         _fix_decoder_args_for_nonbinary_fields(decoder_args, self.field, bound_index=dual_op_index)
@@ -1043,21 +1148,19 @@
             candidate_logical_op = qldpc.decoder.decode(
                 effective_check_matrix, effective_syndrome, **decoder_args
             )
             actual_syndrome = effective_check_matrix @ candidate_logical_op % self.field.order
             logical_op_found = np.array_equal(actual_syndrome, effective_syndrome)
 
         assert self._logical_ops is not None
-        self._logical_ops[pauli.index, logical_index] = candidate_logical_op
+        self._logical_ops[pauli, logical_index] = candidate_logical_op
 
-    def reduce_logical_ops(
-        self, pauli: Literal[Pauli.X, Pauli.Z] | None = None, **decoder_args: object
-    ) -> None:
+    def reduce_logical_ops(self, pauli: PauliXZ | None = None, **decoder_args: object) -> None:
         """Reduce the weight of all logical operators."""
-        assert pauli in [None, Pauli.X, Pauli.Z]
+        assert pauli is None or pauli in PAULIS_XZ
         if pauli is None:
             self.reduce_logical_ops(Pauli.X, **decoder_args)
             self.reduce_logical_ops(Pauli.Z, **decoder_args)
         else:
             for logical_index in range(self.dimension):
                 self.reduce_logical_op(pauli, logical_index, **decoder_args)
 
@@ -1083,25 +1186,22 @@
             decoder_args["lower_bound_row"] = bound_index
 
 
 ################################################################################
 # bicycle and quasi-cyclic codes
 
 
-# TODO: add special/simpler cases of code distance calculations and bounds, if and where available
-
-
 class GBCode(CSSCode):
     """Generalized bicycle (GB) code.
 
-    A GBCode code is built out of two square matrices A and B, which are combined as
-    - matrix_x = [A, B.T], and
-    - matrix_z = [B, A.T],
-    to form the parity check matrices of a CSSCode.  As long as A and B.T commute, the parity check
-    matrices matrix_x and matrix_z satisfy the requirements of a CSSCode by construction.
+    A GBCode code is built out of two matrices A and B, which are combined as
+    - matrix_x = [A, B], and
+    - matrix_z = [B.T, -A.T],
+    to form the parity check matrices of a CSSCode.  If A and B commute, the parity check matrices
+    matrix_x and matrix_z satisfy the requirements of a CSSCode.
 
     References:
     - https://arxiv.org/abs/2012.04068
     """
 
     def __init__(
         self,
@@ -1110,78 +1210,306 @@
         field: int | None = None,
         *,
         conjugate: slice | Sequence[int] = (),
     ) -> None:
         """Construct a generalized bicycle code."""
         if matrix_b is None:
             matrix_b = matrix_a  # pragma: no cover
-        matrix_a = np.array(matrix_a)
-        matrix_b = np.array(matrix_b)
-        if not np.array_equal(matrix_a @ matrix_b.T, matrix_b.T @ matrix_a):
+
+        code_field = galois.GF(field or DEFAULT_FIELD_ORDER)
+        matrix_a = code_field(matrix_a)
+        matrix_b = code_field(matrix_b)
+        if not np.array_equal(matrix_a @ matrix_b, matrix_b @ matrix_a):
             raise ValueError("The matrices provided for this GBCode are incompatible")
-        matrix_x = np.block([matrix_a, matrix_b.T])
-        matrix_z = np.block([matrix_b, matrix_a.T])
+
+        matrix_x = np.block([matrix_a, matrix_b])
+        matrix_z = np.block([matrix_b.T, -matrix_a.T])
         CSSCode.__init__(self, matrix_x, matrix_z, field, conjugate=conjugate, skip_validation=True)
 
 
-class QCCode(GBCode):
-    """Quasi-cyclic (QC) code.
+QuasiCyclicPlaquetteMap = Callable[[int, int, int | PauliXZ], tuple[int, int]]
 
-    Inspired by arXiv:2308.07915.
 
-    A quasi-cyclic code is a CSS code with subcode parity check matrices
-    - matrix_x = [A, B.T], and
-    - matrix_z = [B, A.T],
-    where A and B are block matrices identified with elements of a multivariate polynomial ring.
-    Specifically, we can expand (say) A = sum_{i,j} A_{ij} x_i^j, where A_{ij} are coefficients
-    and each x_i is the generator of a cyclic group of order R_i.
+class QCCode(GBCode):
+    """Quasi-cyclic (QC) codes from arXiv:2308.07915.
 
-    We (tentatively) restrict the coefficients A_{ij} to be in {0, 1}.
+    A quasi-cyclic code is a CSS code with subcode parity check matrices
+    - matrix_x = [A, B], and
+    - matrix_z = [B.T, -A.T],
+    where A = A_{ij} x^i y^j and B = B_{ij} x^i y^j are bivariate polynomials.  Here:
+    - A_{ij} and B_{ij} are scalar coefficients (over some finite field),
+    - x generates a group of order R_x, and
+    - y generates a group of order R_y.
 
     A quasi-cyclic code is defined by...
-    [1] sequence (R_0, R_1, ...) of cyclic group orders (one per variable, x_i), and
-    [2] a list of nonzero terms in A and B, with the term x_i^j identified by the tuple (i, j).
-    The polynomial A = x + y^3 + z^2, for example, is identified by [(0, 1), (1, 3), (2, 2)].
+    [1] two cyclic group orders, and
+    [2] two sympy polynomials in two variables.
+    By default, group orders are associated in lexicographic order with free variables of the
+    polynomials.  Group orders can also be assigned to variables explicitly with a dictionary.
     """
 
     def __init__(
         self,
-        dims: Sequence[int],
-        terms_a: Collection[tuple[Hashable, int]],
-        terms_b: Collection[tuple[Hashable, int]] | None = None,
+        orders: tuple[int, int] | dict[sympy.Symbol, int],
+        poly_a: sympy.Basic,
+        poly_b: sympy.Basic | None = None,
         field: int | None = None,
         *,
-        conjugate: slice | Sequence[int] = (),
+        conjugate: bool = False,
     ) -> None:
         """Construct a quasi-cyclic code."""
-        if field and field != 2:
-            raise ValueError("Non-boolean (field > 2) quasi-cyclic codes are not supported")
-
-        if terms_b is None:
-            terms_b = terms_a  # pragma: no cover
+        if poly_b is None:
+            poly_b = poly_a  # pragma: no cover
+        self.poly_a = sympy.Poly(poly_a)
+        self.poly_b = sympy.Poly(poly_b)
 
         # identify the symbols used to denote cyclic group generators
-        symbols = tuple({symbol for symbol, _ in list(terms_a) + list(terms_b)})
-        if len(symbols) != len(dims):
-            raise ValueError(
-                f"Number of cyclic group orders, {dims}, does not match the number of generator"
-                f" symbols, {symbols}"
+        symbols = poly_a.free_symbols | poly_b.free_symbols
+        if len(symbols) < len(orders) or (
+            isinstance(orders, dict) and any(symbol not in orders for symbol in symbols)
+        ):
+            raise ValueError(f"Could not match symbols {symbols} to group orders {orders}")
+
+        # identify cyclic group orders with symbols in the polynomials
+        if not isinstance(orders, dict):
+            orders_dict = {}
+            for symbol, order in zip(symbols, orders):
+                assert isinstance(symbol, sympy.Symbol), f"Invalid symbol: {symbol}"
+                orders_dict[symbol] = order
+            orders = orders_dict
+        self.symbols = tuple(orders.keys())
+        self.orders = tuple(orders.values())
+
+        # identify the group generator associated with each symbol
+        self.group = abstract.AbelianGroup(*orders.values(), product_lift=True)
+        self.gens = self.group.generators
+        self.symbol_gens = dict(zip(self.symbols, self.gens))
+
+        # hadamard-transform qubits in the "R" sector
+        num_qudits = self.group.order * 2
+        qudits_to_conjugate: slice | Sequence[int] = (
+            slice(num_qudits // 2, num_qudits + 1) if conjugate else ()
+        )
+
+        # build defining matrices of a generalized bicycle code
+        matrix_a = self.eval(self.poly_a).lift().view(np.ndarray)
+        matrix_b = self.eval(self.poly_b).lift().view(np.ndarray)
+        GBCode.__init__(self, matrix_a, matrix_b, field, conjugate=qudits_to_conjugate)
+
+    def eval(
+        self,
+        expr: sympy.Integer | sympy.Symbol | sympy.Pow | sympy.Mul | sympy.Poly,
+    ) -> abstract.Element:
+        """Convert a sympy expression into an element of a group algebra."""
+        # evaluate simple cases
+        if isinstance(expr, sympy.Integer):
+            return int(expr) * abstract.Element(self.group, self.to_group_member(expr))
+        if isinstance(expr, (sympy.Symbol, sympy.Pow)):
+            return abstract.Element(self.group, self.to_group_member(expr))
+
+        # evaluate a product or polynomial
+        element = abstract.Element(self.group)
+        for term in expr.as_expr().args:
+            element += functools.reduce(
+                abstract.Element.__mul__,
+                [self.eval(factor) for factor in term.as_ordered_factors()],
             )
+        return element
 
-        # identify the base cyclic groups, their product, and the generators
-        groups = [abstract.CyclicGroup(dim) for dim in dims]
-        group = abstract.Group.product(*groups)
-        generators = group.generators
+    def to_group_member(
+        self, expr: sympy.Integer | sympy.Symbol | sympy.Pow | sympy.Mul
+    ) -> abstract.GroupMember:
+        """Convert a sympy expression into an associated member of this code's base group."""
+        if isinstance(expr, sympy.Integer):
+            return self.group.identity
+        if isinstance(expr, sympy.Symbol):
+            return self.symbol_gens[expr]
+        if isinstance(expr, sympy.Pow):
+            base, exp = expr.as_base_exp()
+            return self.symbol_gens[base] ** exp
+        if isinstance(expr, sympy.Mul):
+            output = self.group.identity
+            for factor in expr.args:
+                if not isinstance(factor, sympy.Integer):
+                    base, exp = factor.as_base_exp()
+                    output *= self.symbol_gens[base] ** exp
+            return output
+        return NotImplemented  # pragma: no cover
+
+    def get_exponents(
+        self, expr: sympy.Integer | sympy.Symbol | sympy.Pow | sympy.Mul
+    ) -> tuple[int, int]:
+        """Get the exponents of a term, for example converting x**2 y**4 into (2, 4)."""
+        exponents = {}
+        if isinstance(expr, sympy.Symbol):
+            exponents[expr] = 1
+        elif isinstance(expr, sympy.Pow):
+            base, exp = expr.as_base_exp()
+            exponents[base] = exp
+        elif isinstance(expr, sympy.Mul):
+            for factor in expr.args:
+                base, exp = factor.as_base_exp()
+                exponents[base] = exp
+        return exponents.get(self.symbols[0], 0), exponents.get(self.symbols[1], 0)
+
+    @functools.cache
+    def get_toric_mappings(self) -> Sequence[tuple[QuasiCyclicPlaquetteMap, tuple[int, int]]]:
+        """Get plaquette mappings that arrange qubits in a toric layout.
+
+        Each plaquette looks like:
+            L X
+            Z R
+        where L and R are data qubits, and X and Z are checks.  In a toric layout, plaquettes are
+        arranged in a grid, and each check addresses all of its neighboring data qubits, as well as
+        a few far-away qubits.
+        """
+        if not nx.is_weakly_connected(self.graph):
+            # a connected tanner graph is a baseline requirement for a toric mapping to exist
+            return []
+
+        # identify individual terms in the polynomials
+        terms_a = self.poly_a.as_expr().args
+        terms_b = self.poly_b.as_expr().args
+
+        # find combinations of terms that enable a toric layout
+        toric_params = []
+        for (a_1, a_2), (b_1, b_2) in itertools.product(
+            itertools.combinations(terms_a, 2), itertools.combinations(terms_b, 2)
+        ):
+            gen_a = self.to_group_member(a_1 * a_2 ** (-1))
+            gen_b = self.to_group_member(b_1 * b_2 ** (-1))
+            if (
+                gen_a.order() * gen_b.order() == self.group.order
+                and comb.PermutationGroup(gen_a, gen_b).order() == self.group.order
+            ):
+                toric_params.append((a_1, a_2, b_1, b_2))
+
+        # identify torus shapes and qubit-to-plaquette mappings
+        layout_data = []
+        for a_1, a_2, b_1, b_2 in toric_params:
+            shift_a = a_1 * a_2 ** (-1)
+            shift_b = b_1 * b_2 ** (-1)
+            """
+            For generators of the form
+                g = x^p y^q  <-- shift_a,
+                h = x^u y^v  <-- shift_b,
+            build a grid_map (dictionary) that maps (i, j) --> (a, b), where
+                x^i y^j = g^a h^b.
+            Equivalently, we want
+                i = a p + b u  mod order(x),
+                j = b q + b v  mod order(y).
+            """
+            gen_g = self.to_group_member(shift_a)
+            gen_h = self.to_group_member(shift_b)
+            pp, qq = self.get_exponents(shift_a)
+            uu, vv = self.get_exponents(shift_b)
+            torus_shape: tuple[int, int] = (gen_g.order(), gen_h.order())
+            grid_map = {
+                (
+                    (aa * pp + bb * uu) % self.orders[0],
+                    (aa * qq + bb * vv) % self.orders[1],
+                ): (aa, bb)
+                for aa, bb in np.ndindex(torus_shape)
+            }
+            # figure out how to shift qubits in each sector:
+            # (0 <--> L) or (1 <--> R) for data qubits, and X or Z for check qubits
+            sector_shifts = {
+                0: (0, 0),  # "L" data qubits
+                1: self.get_exponents(a_2 ** (-1) * b_1),  # "R" data qubits
+                Pauli.X: self.get_exponents(a_2 ** (-1)),  # "X" check qubits
+                Pauli.Z: self.get_exponents(b_1),  # "Z" check qubits
+            }
+
+            plaquette_map = functools.partial(
+                self.full_plaquette_map,
+                grid_map=grid_map,
+                sector_shifts=sector_shifts,
+                torus_shape=torus_shape,
+            )
+            layout_data.append((plaquette_map, torus_shape))
 
-        # build defining matrices of a generalized bicycle code
-        members_a = [generators[symbols.index(ss)] ** pp for ss, pp in terms_a]
-        members_b = [generators[symbols.index(ss)] ** pp for ss, pp in terms_b]
-        matrix_a = abstract.Element(group, *members_a).lift()
-        matrix_b = abstract.Element(group, *members_b).lift()
-        GBCode.__init__(self, matrix_a, matrix_b, field, conjugate=conjugate)
+        return layout_data
+
+    def full_plaquette_map(
+        self,
+        ii: int,
+        jj: int,
+        qubit_sector: int | PauliXZ,
+        grid_map: dict[tuple[int, int], tuple[int, int]],
+        sector_shifts: dict[int | PauliXZ, tuple[int, int]],
+        torus_shape: tuple[int, int],
+    ) -> tuple[int, int]:
+        """Map from "original" plaquette coordinates to "shifted" plaquette coordinates."""
+        s_i = (ii - sector_shifts[qubit_sector][0]) % self.orders[0]
+        s_j = (jj - sector_shifts[qubit_sector][1]) % self.orders[1]
+        s_a, s_b = grid_map[s_i, s_j]
+        return s_a % torus_shape[0], s_b % torus_shape[1]
+
+    def get_toric_checks(
+        self, plaquette_map: QuasiCyclicPlaquetteMap, torus_shape: tuple[int, int]
+    ) -> tuple[npt.NDArray[np.int_], npt.NDArray[np.int_]]:
+        """Build X-type and Z-type parity check matrices for a toric layout."""
+
+        # loop over each of X-type and Z-type parity checks
+        for pauli in PAULIS_XZ:
+            matrix = self.matrix_x if pauli == Pauli.X else self.matrix_z
+            old_checks = matrix.reshape(*self.orders, 2, *self.orders)
+            new_checks = self.field.Zeros((*torus_shape, 2, *torus_shape))
+
+            # loop over every check
+            for c_i, c_j in np.ndindex(*self.orders):
+                c_a, c_b = plaquette_map(c_i, c_j, pauli)
+
+                # loop over every qubit
+                for sector, d_i, d_j in zip(*np.where(old_checks[c_i, c_j])):
+                    d_a, d_b = plaquette_map(d_i, d_j, sector)
+                    new_checks[c_a, c_b, sector, d_a, d_b] = old_checks[c_i, c_j, sector, d_i, d_j]
+
+            # save the shifted checks to an X/Z parity check matrix as appropriate
+            if pauli == Pauli.X:
+                matrix_x = new_checks.reshape(self.matrix_x.shape)
+            else:
+                assert pauli == Pauli.Z
+                matrix_z = new_checks.reshape(self.matrix_z.shape)
+
+        return matrix_x, matrix_z
+
+    def get_check_shifts(
+        self, plaquette_map: QuasiCyclicPlaquetteMap, torus_shape: tuple[int, int]
+    ) -> tuple[set[tuple[int, int]], set[tuple[int, int]]]:
+        """Get the relative positions of data qubits addressed by X-type and Z-type check qubits."""
+        # identify the parity check matrices
+        matrix_x, matrix_z = self.get_toric_checks(plaquette_map, torus_shape)
+
+        def get_loc(aa: int, bb: int, corner: int | PauliXZ) -> tuple[int, int]:
+            """Get the location of a qubit on the torus."""
+            return 2 * aa + int(corner in [1, Pauli.X]), 2 * bb + int(corner in [1, Pauli.Z])
+
+        # relative coordinates, organized by stabilizer type
+        shifts: dict[PauliXZ, set[tuple[int, int]]] = {}
+
+        paulis_xz: list[PauliXZ] = [Pauli.X, Pauli.Z]
+        for pauli in paulis_xz:
+            shifts[pauli] = set()
+            matrix = matrix_x if pauli == Pauli.X else matrix_z
+
+            # identify the location and support of one check qubit
+            c_a, c_b = get_loc(0, 0, pauli)
+            check = matrix[0].reshape(2, *torus_shape)
+
+            # identify the relative position of all data qubits addressed by this check
+            for sector, aa, bb in zip(*np.where(check)):
+                d_a, d_b = get_loc(aa, bb, sector)  # position of this data qubit
+                shift_a = (d_a - c_a) % (2 * torus_shape[0])
+                shift_b = (d_b - c_b) % (2 * torus_shape[1])
+                shift_a = shift_a if shift_a <= torus_shape[0] else shift_a - 2 * torus_shape[0]
+                shift_b = shift_b if shift_b <= torus_shape[1] else shift_b - 2 * torus_shape[1]
+                shifts[pauli].add((shift_a, shift_b))
+
+        return shifts[Pauli.X], shifts[Pauli.Z]
 
 
 ################################################################################
 # hypergraph and lifted product codes
 
 
 class HGPCode(CSSCode):
@@ -1247,19 +1575,23 @@
         *,
         conjugate: bool = False,
     ) -> None:
         """Hypergraph product of two classical codes, as in arXiv:2202.01702.
 
         The parity check matrices of the hypergraph product code are:
 
-        matrix_x = [H1 ⊗ In2, -Im1 ⊗ H2.T]
-        matrix_z = [In1 ⊗ H2,  H1.T ⊗ Im2]
+        matrix_x = [ H1 ⨂ In2, Im1 ⨂ H2.T]
+        matrix_z = [-In1 ⨂ H2, H1.T ⨂ Im2]
 
         Here (H1, H2) == (matrix_a, matrix_b), and I[m/n][1/2] are identity matrices,
         with (m1, n1) = H1.shape and (m2, n2) = H2.shape.
+
+        A minus sign in one sector of matrix_x or matrix_z is necessary to satisfy CSS code
+        requirements with nonbinary fields.  The placement of this sign is chosen for consistency
+        with the tensor product of chain complexes.
         """
         if code_b is None:
             code_b = code_a
         code_a = ClassicalCode(code_a, field)
         code_b = ClassicalCode(code_b, field)
         field = code_a.field.order
 
@@ -1277,26 +1609,28 @@
 
         CSSCode.__init__(
             self, matrix_x, matrix_z, field, conjugate=qudits_to_conjugate, skip_validation=True
         )
 
     @classmethod
     def get_matrix_product(
-        cls, matrix_a: npt.NDArray[np.int_], matrix_b: npt.NDArray[np.int_]
+        cls,
+        matrix_a: npt.NDArray[np.int_ | np.object_],
+        matrix_b: npt.NDArray[np.int_ | np.object_],
     ) -> nx.DiGraph:
         """Hypergraph product of two parity check matrices."""
         # construct the nontrivial blocks of the final parity check matrices
         mat_H1_In2 = np.kron(matrix_a, np.eye(matrix_b.shape[1], dtype=int))
         mat_In1_H2 = np.kron(np.eye(matrix_a.shape[1], dtype=int), matrix_b)
         mat_H1_Im2_T = np.kron(matrix_a.T, np.eye(matrix_b.shape[0], dtype=int))
         mat_Im1_H2_T = np.kron(np.eye(matrix_a.shape[0], dtype=int), matrix_b.T)
 
         # construct the X-sector and Z-sector parity check matrices
-        matrix_x = np.block([mat_H1_In2, -mat_Im1_H2_T])
-        matrix_z = np.block([mat_In1_H2, mat_H1_Im2_T])
+        matrix_x = np.block([mat_H1_In2, mat_Im1_H2_T])
+        matrix_z = np.block([-mat_In1_H2, mat_H1_Im2_T])
         return matrix_x, matrix_z
 
     @classmethod
     def get_graph_product(
         cls, graph_a: nx.DiGraph, graph_b: nx.DiGraph, *, conjugate: bool = False
     ) -> nx.DiGraph:
         """Hypergraph product of two Tanner graphs."""
@@ -1318,22 +1652,21 @@
 
             # by default, this edge is Z-type iff the check qudit is in the (0, 1) sector
             op = QuditOperator((0, data.get("val", 1)))
             if node_check[0].is_data:
                 # make this a X-type operator
                 op = ~op
 
-            # special treatment of qudits in the (1, 1) sector
-            if not node_qudit[0].is_data:
-                # account for the minus sign in the X-type subcode
-                if not node_check[0].is_data:
-                    op = -op
-                # flip X <--> Z operators for the conjugated code
-                if conjugate:
-                    op = ~op
+            # for a conjugated code, flip X <--> Z operators in the (1, 1) sector
+            if conjugate and not node_qudit[0].is_data:
+                op = ~op
+
+            # account for the minus sign in the (0, 0) sector of the Z-type subcode
+            if node_qudit[0].is_data and node_check[0].is_data:
+                op = -op
 
             graph[node_check][node_qudit][QuditOperator] = op
 
         # relabel nodes, from (node_a, node_b) --> node_combined
         node_map = HGPCode.get_product_node_map(graph_a.nodes, graph_b.nodes)
         graph = nx.relabel_nodes(graph, node_map)
 
@@ -1369,102 +1702,66 @@
 
 
 class LPCode(CSSCode):
     """Lifted product (LP) code.
 
     A lifted product code is essentially the same as a hypergraph product code, except that the
     parity check matrices are "protographs", or matrices whose entries are members of a group
-    algebra over the field Z_2 ~ {0,1}.  Each of these entries can be "lifted" to a representation
-    as orthogonal matrices over a finite field, in which case the protograph is interpreted as a
-    block matrix; this is called "lifting" the protograph.
+    algebra over a finite field F_q.  Each of these entries can be "lifted" to a representation as
+    orthogonal matrices over F_q, in which case the protograph is interpreted as a block matrix;
+    this is called "lifting" the protograph.
 
     Notes:
     - A lifted product code with protographs of size 1×1 is a generalized bicycle code.
     - A lifted product code with protographs whose entries get lifted to 1×1 matrices is a
         hypergraph product code of the lifted protographs.
 
     References:
     - https://errorcorrectionzoo.org/c/lifted_product
     - https://arxiv.org/abs/2202.01702
     - https://arxiv.org/abs/2012.04068
     """
 
     def __init__(
         self,
-        protograph_a: abstract.Protograph | npt.NDArray[np.object_] | Sequence[Sequence[object]],
-        protograph_b: (
-            abstract.Protograph | npt.NDArray[np.object_] | Sequence[Sequence[object]] | None
-        ) = None,
+        protograph_a: npt.NDArray[np.object_] | Sequence[Sequence[object]],
+        protograph_b: npt.NDArray[np.object_] | Sequence[Sequence[object]] | None = None,
         *,
         conjugate: bool = False,
     ) -> None:
         """Lifted product of two protographs, as in arXiv:2012.04068."""
         if protograph_b is None:
             protograph_b = protograph_a
         protograph_a = abstract.Protograph(protograph_a)
         protograph_b = abstract.Protograph(protograph_b)
         field = protograph_a.field.order
 
         # identify X-sector and Z-sector parity checks
-        matrix_x, matrix_z = LPCode.get_matrix_product(protograph_a, protograph_b)
+        matrix_x, matrix_z = HGPCode.get_matrix_product(protograph_a, protograph_b)
+        matrix_x = abstract.Protograph(matrix_x).lift()
+        matrix_z = abstract.Protograph(matrix_z).lift()
 
         # identify the number of qudits in each sector
         self.sector_size = protograph_a.group.lift_dim * np.outer(
             protograph_a.shape[::-1],
             protograph_b.shape[::-1],
         )
 
         # identify which qudits to conjugate (Hadamard-transform)
         qudits_to_conjugate = slice(self.sector_size[0, 0], None) if conjugate else None
 
         CSSCode.__init__(
             self, matrix_x, matrix_z, field, conjugate=qudits_to_conjugate, skip_validation=True
         )
 
-    @classmethod
-    def get_matrix_product(
-        cls, protograph_a: abstract.Protograph, protograph_b: abstract.Protograph
-    ) -> nx.DiGraph:
-        """Matrix-based hypergraph product similar to that in HGPCode, but with protographs.
-
-        There is one crucial subtlety when computing the hypergraph product of protographs.  When
-        taking the transpose of a protograph, P --> P.T, we also need to transpose the individual
-        (algebra-valued) entries of the protograph.  That is,
-
-        P = ⌈ a, b ⌉  ==>  P.T = ⌈ a.T, c.T ⌉
-            ⌊ c, d ⌋             ⌊ b.T, d.T ⌋.
-
-        If we simply take the hypergraph product of two protograph matrices directly, numpy will not
-        know to take the transpose of matrix entries when taking the transpose of a matrix.  For
-        this reason, we need to take the transpose of a protograph "manually" when using it for the
-        hypergraph product.
-        """
-        # identify sub-matrices and their transposes
-        matrix_a = protograph_a.matrix
-        matrix_b = protograph_b.matrix
-        matrix_a_T = protograph_a.T.matrix
-        matrix_b_T = protograph_b.T.matrix
-
-        # construct the nontrivial blocks of the final parity check matrices
-        mat_H1_In2 = np.kron(matrix_a, np.eye(matrix_b.shape[1], dtype=int))
-        mat_In1_H2 = np.kron(np.eye(matrix_a.shape[1], dtype=int), matrix_b)
-        mat_H1_Im2_T = np.kron(matrix_a_T, np.eye(matrix_b.shape[0], dtype=int))
-        mat_Im1_H2_T = np.kron(np.eye(matrix_a.shape[0], dtype=int), matrix_b_T)
-
-        # construct the X-sector and Z-sector parity check matrices
-        matrix_x = abstract.Protograph(np.block([mat_H1_In2, -mat_Im1_H2_T])).lift()
-        matrix_z = abstract.Protograph(np.block([mat_In1_H2, mat_H1_Im2_T])).lift()
-        return matrix_x, matrix_z
-
 
 ################################################################################
 # classical and quantum Tanner codes
 
 
-# TODO: add TannerCode construction based on undirected graphs
 class TannerCode(ClassicalCode):
     """Classical Tanner code, as described in DOI:10.1109/TIT.1981.1056404.
 
     A Tanner code T(G,C) is constructed from:
     [1] A bipartite "half-regular" graph G.  That is, a graph...
         ... with two sets of nodes, V and W.
         ... in which all nodes in V have degree n.
@@ -1476,24 +1773,30 @@
     The Tanner code T(G,C) is defined on |W| bits.  A |W|-bit string x is a code word of T(G,C) iff,
     for every node v in V, the bits of x incident to v are a code word of C.
 
     This construction requires an ordering the edges E(v) adjacent to each vertex v.  This class
     sorts E(v) by the value of the "sort" attribute attached to each edge.  If there is no "sort"
     attribute, its value is treated as corresponding neighbor of v.
 
+    Tanner codes can similarly be defined on regular (undirected) graphs G' = (V',E') by placing
+    checks on V' and bits on E'.
+
     Notes:
     - If the subcode C has m checks, its parity matrix has shape (m,n).
     - The code T(G,C) has |W| bits and |V|m checks.
     """
 
     subgraph: nx.DiGraph
     subcode: ClassicalCode
 
-    def __init__(self, subgraph: nx.DiGraph, subcode: ClassicalCode) -> None:
+    def __init__(self, subgraph: nx.Graph, subcode: ClassicalCode) -> None:
         """Construct a classical Tanner code."""
+        if not isinstance(subgraph, nx.DiGraph):
+            subgraph = TannerCode.as_directed_subgraph(subgraph)
+
         self.subgraph = subgraph
         self.subcode = subcode
         sources = [node for node in subgraph if subgraph.in_degree(node) == 0]
         sinks = [node for node in subgraph if subgraph.out_degree(node) == 0]
         sink_indices = {sink: idx for idx, sink in enumerate(sorted(sinks))}
 
         num_bits = len(sinks)
@@ -1508,27 +1811,43 @@
     def _get_sorted_neighbors(self, node: object) -> Sequence[object]:
         """Sorted neighbors of the given node."""
         return sorted(
             self.subgraph.neighbors(node),
             key=lambda neighbor: self.subgraph[node][neighbor].get("sort", neighbor),
         )
 
-
+    @classmethod
+    def as_directed_subgraph(self, subgraph: nx.Graph) -> nx.DiGraph:
+        """Convert an undirected graph for a Tanner code into a directed graph for the same code."""
+        directed_subgraph = nx.DiGraph()
+        for node_a, node_b, edge_data in subgraph.edges(data=True):
+            edge = frozenset([node_a, node_b])
+            directed_subgraph.add_edge(node_a, edge)
+            directed_subgraph.add_edge(node_b, edge)
+            if (sort_data := edge_data.pop("sort", None)) is not None:
+                directed_subgraph[node_a][edge]["sort"] = sort_data[node_a]
+                directed_subgraph[node_b][edge]["sort"] = sort_data[node_b]
+        return directed_subgraph
+
+
+# TODO: investigate construction in
+# https://github.com/errorcorrectionzoo/eczoo_data/files/9210173/rotated.pdf
+# see also Section 7 of https://arxiv.org/abs/2206.07571
 class QTCode(CSSCode):
-    """Quantum Tanner code: a CSS code for qudits defined on the faces of a Cayley complex
+    """Quantum Tanner code: a CSS code for qudits defined on the faces of a Cayley complex.
 
     Altogether, a quantum Tanner code is defined by:
     - two symmetric (self-inverse) subsets A and B of a group G, and
     - two classical codes C_A and C_B, respectively with block lengths |A| and |B|.
 
     The X-type parity checks of a quantum Tanner code are the checks of a classical Tanner code
-    whose generating graph is the subgraph_0 of the Cayley complex (A,B).  The subcode of this
-    classical Tanner code is ~(C_A ⊗ C_B), where ~C is the dual code to C.
+    whose generating graph is the subgraph_x of the Cayley complex (A,B).  The subcode of this
+    classical Tanner code is ~(C_A ⨂ C_B), where ~C is the dual code to C.
 
-    The Z-type parity checks are similarly defined with subgraph_1 and subcode ~(~C_A ⊗ ~C_B).
+    The Z-type parity checks are similarly defined with subgraph_z and subcode ~(~C_A ⨂ ~C_B).
 
     Notes:
     - "Good" quantum Tanner code: projective special linear group and random classical codes.
 
     References:
     - https://errorcorrectionzoo.org/c/quantum_tanner
     - https://arxiv.org/abs/2206.07571
@@ -1556,16 +1875,302 @@
         if field is None and code_a.field is not code_b.field:
             raise ValueError("The sub-codes provided for this QTCode are over different fields")
 
         self.complex = CayleyComplex(subset_a, subset_b, bipartite=bipartite)
         assert code_a.num_bits == len(self.complex.subset_a)
         assert code_b.num_bits == len(self.complex.subset_b)
 
-        subgraph_x, subgraph_z = self.complex.subgraphs()
+        subgraph_x, subgraph_z = QTCode.get_subgraphs(self.complex)
         subcode_x = ~ClassicalCode.tensor_product(code_a, code_b)
         subcode_z = ~ClassicalCode.tensor_product(~code_a, ~code_b)
         code_x = TannerCode(subgraph_x, subcode_x)
         code_z = TannerCode(subgraph_z, subcode_z)
         CSSCode.__init__(self, code_x, code_z, field, conjugate=conjugate, skip_validation=True)
 
+    @classmethod
+    def get_subgraphs(cls, cayplex: CayleyComplex) -> tuple[nx.DiGraph, nx.DiGraph]:
+        """Build the subgraphs of the inner (classical) Tanner codes for a quantum Tanner code.
+
+        These subgraphs are defined using the faces of a Cayley complex.  Each face looks like:
+
+         g ―――――――――― gb
+
+         |  f(g,a,b)  |
+
+        ag ――――――――― agb
+
+        where f(g,a,b) = {g, ab, gb, agb}.  Specifically, the (directed) subgraphs are:
+        - subgraph_x with edges ( g, f(g,a,b)), and
+        - subgraph_z with edges (ag, f(g,a,b)).
+        Classical Tanner codes on these subgraphs are used as to construct quantum Tanner code.
+
+        As a matter of practice, defining classical Tanner codes on subgraph_x and subgraph_z
+        requires choosing an ordering on the edges incident to every source node of these graphs.
+        If the group G is equipped with a total order, a natural ordering of edges incident to every
+        source node is induced by assigning the label (a, b) to edge (g, f(g,a,b)).  Consistency
+        then requires that edge (ag, f(g,a,b)) has label (a^-1, b), as verified by defining g' = ag
+        and checking that f(g,a,b) = f(g',a^-1,b).
+        """
+        subgraph_x = nx.DiGraph()
+        subgraph_z = nx.DiGraph()
+        nodes_x, _ = nx.bipartite.sets(cayplex.graph)
+        for gg, aa, bb in itertools.product(nodes_x, cayplex.subset_a, cayplex.subset_b):
+            aa_gg, gg_bb, aa_gg_bb = aa * gg, gg * bb, aa * gg * bb
+            face = frozenset([gg, aa_gg, gg_bb, aa_gg_bb])
+            subgraph_x.add_edge(gg, face, sort=(aa, bb))
+            subgraph_z.add_edge(aa_gg, face, sort=(~aa, bb))
+        return subgraph_x, subgraph_z
+
+
+################################################################################
+# common quantum codes
+
+
+class SurfaceCode(CSSCode):
+    """The one and only!
+
+    Actually, there are two variants: "ordinary" and "rotated" surface codes.
+    The rotated code is more qubit-efficient.
+
+    If constructed with conjugate=True, every other qubit is Hadamard-transformed in a checkerboard
+    pattern.  The rotated surface code with conjugate=True is the XZZX code in arXiv:2009.07851.
+    """
+
+    def __init__(
+        self,
+        rows: int,
+        cols: int | None = None,
+        rotated: bool = True,
+        field: int | None = None,
+        *,
+        conjugate: bool = False,
+    ) -> None:
+        if cols is None:
+            cols = rows
+
+        # save known distances
+        self._exact_distance_x = cols
+        self._exact_distance_z = rows
+
+        # which qubits should be Hadamard-transformed?
+        qudits_to_conjugate: slice | Sequence[int] | None
+
+        if rotated:
+            # rotated surface code
+            matrix_x, matrix_z = SurfaceCode.get_rotated_checks(rows, cols)
+
+            if conjugate:
+                # Hadamard-transform qubits in a checkerboard pattern
+                qudits_to_conjugate = [
+                    idx for idx, (row, col) in enumerate(np.ndindex(rows, cols)) if (row + col) % 2
+                ]
+
+            else:
+                qudits_to_conjugate = None
+
+        else:
+            # "original" surface code
+            code_a = RepetitionCode(rows, field)
+            code_b = RepetitionCode(cols, field)
+            code_ab = HGPCode(code_a, code_b, field, conjugate=conjugate)
+            matrix_x = code_ab.matrix_x
+            matrix_z = code_ab.matrix_z
+            qudits_to_conjugate = code_ab.conjugated_qubits
+
+        CSSCode.__init__(
+            self,
+            matrix_x,
+            matrix_z,
+            field=field,
+            conjugate=qudits_to_conjugate,
+            skip_validation=True,
+        )
+
+    @classmethod
+    def get_rotated_checks(
+        cls, rows: int, cols: int
+    ) -> tuple[npt.NDArray[np.int_], npt.NDArray[np.int_]]:
+        """Build X-sector and Z-sector parity check matrices.
+
+        Example 5x5 rotated surface code layout:
+
+             ―――     ―――
+            | ⋅ |   | ⋅ |
+            ○―――○―――○―――○―――○―――
+            | × | ⋅ | × | ⋅ | × |
+         ―――○―――○―――○―――○―――○―――
+        | × | ⋅ | × | ⋅ | × |
+         ―――○―――○―――○―――○―――○―――
+            | × | ⋅ | × | ⋅ | × |
+         ―――○―――○―――○―――○―――○―――
+        | × | ⋅ | × | ⋅ | × |
+         ―――○―――○―――○―――○―――○
+                | ⋅ |   | ⋅ |
+                 ―――     ―――
+
+        Here:
+        - Circles (○) denote data qubits (of which there are 5×5 = 25 total).
+        - Tiles with a cross (×) denote X-type parity checks (12 total).
+        - Tiles with a dot (⋅) denote Z-type parity checks (12 total).
+
+        Reference: https://errorcorrectionzoo.org/c/rotated_surface
+        """
+
+        def get_check(
+            row_indices: Sequence[int], col_indices: Sequence[int]
+        ) -> npt.NDArray[np.int_]:
+            """Check on the qubits with the given indices, dropping any that are out of bounds."""
+            check = np.zeros((rows, cols), dtype=int)
+            for row, col in zip(row_indices, col_indices):
+                if 0 <= row < rows and 0 <= col < cols:
+                    check[row, col] = 1
+            return check.ravel()
+
+        checks_x = []
+        checks_z = []
+        for row in range(-1, rows):
+            for col in range(-1, cols):
+                row_indices = [row, row + 1, row, row + 1]
+                col_indices = [col, col, col + 1, col + 1]
+                check = get_check(row_indices, col_indices)
+
+                # exclude exterior corner tiles that only touch one data qubit
+                if np.count_nonzero(check) == 1:
+                    continue
+
+                if row % 2 == col % 2:
+                    if 0 <= row < rows - 1:
+                        # no X-type parity checks on the top/bottom boundaries
+                        checks_x.append(check)
+                elif 0 <= col < cols - 1:
+                    # no Z-type parity checks on the left/right boundaries
+                    checks_z.append(check)
 
-# TODO: add ordinary + rotated SurfaceCode and ToricCode
+        return np.array(checks_x), np.array(checks_z)
+
+
+class ToricCode(CSSCode):
+    """Surface code with periodic bounary conditions, encoding two logical qudits.
+
+    Reference: https://errorcorrectionzoo.org/c/surface
+    """
+
+    def __init__(
+        self,
+        rows: int,
+        cols: int | None = None,
+        rotated: bool = True,
+        field: int | None = None,
+        *,
+        conjugate: bool = False,
+    ) -> None:
+        if cols is None:
+            cols = rows
+
+        # save known distances
+        self._exact_distance_x = self._exact_distance_z = min(rows, cols)
+
+        # which qubits should be Hadamard-transformed?
+        qudits_to_conjugate: slice | Sequence[int] | None
+
+        if rotated:
+            # rotated toric code
+            if not (rows % 2 == cols % 2 == 0 and rows >= 4 and cols >= 4):
+                raise ValueError(
+                    "The rotated toric code must have even side lengths of at least four, not"
+                    + f" ({rows},{cols})"
+                )
+            matrix_x, matrix_z = ToricCode.get_rotated_checks(rows, cols)
+
+            if conjugate:
+                # Hadamard-transform qubits in a checkerboard pattern
+                qudits_to_conjugate = [
+                    idx for idx, (row, col) in enumerate(np.ndindex(rows, cols)) if (row + col) % 2
+                ]
+
+            else:
+                qudits_to_conjugate = None
+
+        else:
+            # "original" toric code
+            code_a = RingCode(rows, field)
+            code_b = RingCode(cols, field)
+            code_ab = HGPCode(code_a, code_b, field, conjugate=conjugate)
+            matrix_x = code_ab.matrix_x
+            matrix_z = code_ab.matrix_z
+            qudits_to_conjugate = code_ab.conjugated_qubits
+
+        CSSCode.__init__(
+            self,
+            matrix_x,
+            matrix_z,
+            field=field,
+            conjugate=qudits_to_conjugate,
+            skip_validation=True,
+        )
+
+    @classmethod
+    def get_rotated_checks(
+        cls, rows: int, cols: int
+    ) -> tuple[npt.NDArray[np.int_], npt.NDArray[np.int_]]:
+        """Build X-sector and Z-sector parity check matrices.
+
+        Same as in SurfaceCode.get_rotated_checks, but with periodic boundary conditions.
+        """
+
+        def get_check(
+            row_indices: Sequence[int], col_indices: Sequence[int]
+        ) -> npt.NDArray[np.int_]:
+            """Check on the qubits with the given indices, with periodic boundary conditions."""
+            check = np.zeros((rows, cols), dtype=int)
+            for row, col in zip(row_indices, col_indices):
+                check[row % rows, col % cols] = 1
+            return check.ravel()
+
+        checks_x = []
+        checks_z = []
+        for row in range(rows):
+            for col in range(cols):
+                row_indices = [row, row + 1, row, row + 1]
+                col_indices = [col, col, col + 1, col + 1]
+                check = get_check(row_indices, col_indices)
+                if row % 2 == col % 2:
+                    checks_x.append(check)
+                else:
+                    checks_z.append(check)
+
+        return np.array(checks_x), np.array(checks_z)
+
+
+class GeneralizedSurfaceCode(CSSCode):
+    """Surface or toric code defined on a multi-dimensional hypercubic lattice.
+
+    Reference: https://errorcorrectionzoo.org/c/higher_dimensional_surface
+    """
+
+    def __init__(
+        self,
+        size: int,
+        dim: int,
+        periodic: bool = False,
+        field: int | None = None,
+        *,
+        conjugate: slice | Sequence[int] | None = (),
+    ) -> None:
+        if dim < 2:
+            raise ValueError(
+                f"The dimension of a generalized surface code should be >= 2 (provided: {dim})"
+            )
+
+        base_code = RingCode(size, field) if periodic else RepetitionCode(size, field)
+
+        # build a chain complex one link at a time
+        chain = ChainComplex(base_code.matrix)
+        link = ChainComplex(base_code.matrix.T)
+        for _ in range(dim - 1):
+            chain = ChainComplex.tensor_product(chain, link)
+
+            # to reduce computational overhead, remove chain links that we don't care about
+            chain = ChainComplex(*chain.ops[:2])
+
+        matrix_x, matrix_z = chain.op(1), chain.op(2).T
+        CSSCode.__init__(self, matrix_x, matrix_z, field, conjugate=conjugate, skip_validation=True)
```

### Comparing `qldpc-0.0.8/qldpc/codes_test.py` & `qldpc-0.0.9/qldpc/codes_test.py`

 * *Files 16% similar despite different names*

```diff
@@ -18,24 +18,24 @@
 import itertools
 import unittest.mock
 
 import networkx as nx
 import numpy as np
 import pytest
 
-from qldpc import abstract, codes
+from qldpc import abstract, codes, objects
 
 
 def get_random_qudit_code(qudits: int, checks: int, field: int = 2) -> codes.QuditCode:
     """Construct a random (but probably trivial or invalid) QuditCode."""
     return codes.QuditCode(codes.ClassicalCode.random(2 * qudits, checks, field).matrix)
 
 
 def test_classical_codes() -> None:
-    """Construction of a few classical codes."""
+    """Classical code constructions."""
     assert codes.ClassicalCode.random(5, 3).num_bits == 5
     assert codes.HammingCode(3).get_distance() == 3
 
     num_bits = 2
     for code in [
         codes.RepetitionCode(num_bits, field=3),
         codes.RingCode(num_bits, field=3),
@@ -43,60 +43,61 @@
         assert code.num_bits == num_bits
         assert code.dimension == 1
         assert code.get_distance() == num_bits
         assert code.get_distance(bound=10) == num_bits
         assert code.get_weight() == 2
         assert code.get_random_word() in code
 
-    # test that rank of repetition and Hamming codes is independent of the field
+    # that rank of repetition and Hamming codes is independent of the field
     assert codes.RepetitionCode(3, 2).rank == codes.RepetitionCode(3, 3).rank
     assert codes.HammingCode(3, 2).rank == codes.HammingCode(3, 3).rank
 
-    # test invalid classical code construction
+    # invalid classical code construction
     with pytest.raises(ValueError, match="inconsistent"):
         codes.ClassicalCode(codes.ClassicalCode.random(2, 2, field=2), field=3)
 
+    # construct a code from its generator matrix
+    code = codes.ClassicalCode.random(5, 3)
+    assert codes.ClassicalCode.equiv(code, codes.ClassicalCode.from_generator(code.generator))
+
+    # puncture a code
+    assert codes.ClassicalCode.from_generator(code.generator[:, 1:]) == code.puncture(0)
+
+    # shortening a repetition code yields a trivial code
+    num_bits = 3
+    code = codes.RepetitionCode(num_bits)
+    words = [[0] * (num_bits - 1)]
+    assert np.array_equal(code.shorten(0).words(), words)
+
 
 def test_special_codes() -> None:
     """Reed-Solomon, BCH, and Reed-Muller codes."""
     assert codes.ReedSolomonCode(3, 2).dimension == 2
 
     bits, dimension = 7, 4
     assert codes.BCHCode(bits, dimension).dimension == dimension
     with pytest.raises(ValueError, match=r"2\^m - 1 bits"):
         codes.BCHCode(bits - 1, dimension)
 
     order, size = 1, 3
     code = codes.ReedMullerCode(order, size)
     assert code.dimension == codes.ClassicalCode(code.matrix).dimension
-    assert (
-        code.get_distance_exact()
-        == code.get_distance_bound()
-        == codes.ClassicalCode.get_distance_exact(code)
-    )
-    assert (
-        code.get_distance_exact(vector=[0] * code.num_bits)
-        == code.get_distance_bound(vector=[0] * code.num_bits)
-        == 0
-    )
-    dual_code = codes.ReedMullerCode(size - order - 1, size)
-    assert np.array_equal((~code).matrix, dual_code.matrix)
+    assert ~code == codes.ReedMullerCode(size - order - 1, size)
 
     with pytest.raises(ValueError, match="0 <= r <= m"):
         codes.ReedMullerCode(-1, 0)
 
 
 def test_named_codes(order: int = 2) -> None:
     """Named codes from the GAP computer algebra system."""
     code = codes.RepetitionCode(order)
     checks = [list(row) for row in code.matrix.view(np.ndarray)]
 
     with unittest.mock.patch("qldpc.named_codes.get_code", return_value=(checks, None)):
-        named_code = codes.ClassicalCode.from_name(f"RepetitionCode({order})")
-        assert np.array_equal(named_code.matrix, code.matrix)
+        assert codes.ClassicalCode.from_name(f"RepetitionCode({order})") == code
 
 
 def test_dual_code(bits: int = 5, checks: int = 3, field: int = 3) -> None:
     """Dual code construction."""
     code = codes.ClassicalCode.random(bits, checks, field)
     assert all(word_a @ word_b == 0 for word_a in code.words() for word_b in (~code).words())
 
@@ -172,16 +173,16 @@
     code.get_random_logical_op(codes.Pauli.X, ensure_nontrivial=False)
     code.get_random_logical_op(codes.Pauli.X, ensure_nontrivial=True)
 
     # test that logical operators are dual to each other and have trivial syndromes
     logicals = code.get_logical_ops()
     logicals_x, logicals_z = logicals[0], logicals[1]
     assert np.array_equal(logicals_x @ logicals_z.T, np.eye(code.dimension, dtype=int))
-    assert not np.any(code.code_z.matrix @ logicals_x.T)
-    assert not np.any(code.code_x.matrix @ logicals_z.T)
+    assert not np.any(code.matrix_z @ logicals_x.T)
+    assert not np.any(code.matrix_x @ logicals_z.T)
 
     # minimizing logical operator weight only supported for prime number fields
     code = codes.HGPCode(codes.ClassicalCode.random(4, 2, field=4))
     with pytest.raises(ValueError, match="prime number fields"):
         code.reduce_logical_op(codes.Pauli.X, 0)
 
 
@@ -206,29 +207,44 @@
     assert np.array_equal(code_a.matrix, code_b.matrix)
     assert stabilizers == code_b.get_stabilizers()
 
     with pytest.raises(ValueError, match="different lengths"):
         codes.QuditCode.from_stabilizers(["I", "I I"], field)
 
 
+def test_quantum_distance(field: int = 2) -> None:
+    """Distance calculations for qudit codes."""
+    code = codes.HGPCode(codes.RepetitionCode(2, field=field))
+    assert code.get_distance() == 2
+
+    # assert that the identity is a logical operator
+    assert 0 == code.get_distance(codes.Pauli.X, vector=[0] * code.num_qudits)
+    assert 0 == code.get_distance(codes.Pauli.X, vector=[0] * code.num_qudits, bound=True)
+
+
 @pytest.mark.parametrize("field", [2, 3])
 def test_graph_product(
     field: int,
     bits_checks_a: tuple[int, int] = (5, 3),
     bits_checks_b: tuple[int, int] = (3, 2),
     conjugate: bool = True,
 ) -> None:
-    """Equivalency of matrix-based and graph-based hypergraph products."""
+    """Equivalency of matrix-based, graph-based, and chain-based hypergraph products."""
     code_a = codes.ClassicalCode.random(*bits_checks_a, field=field)
     code_b = codes.ClassicalCode.random(*bits_checks_b, field=field)
 
     code = codes.HGPCode(code_a, code_b, conjugate=conjugate)
     graph = codes.HGPCode.get_graph_product(code_a.graph, code_b.graph, conjugate=conjugate)
-    assert np.array_equal(code.matrix, codes.QuditCode.graph_to_matrix(graph))
+    chain = objects.ChainComplex.tensor_product(code_a.matrix, code_b.matrix.T)
+    matrix_x, matrix_z = chain.op(1), chain.op(2).T
+
     assert nx.utils.graphs_equal(code.graph, graph)
+    assert np.array_equal(code.matrix, codes.QuditCode.graph_to_matrix(graph))
+    assert np.array_equal(code.matrix_x, matrix_x)
+    assert np.array_equal(code.matrix_z, matrix_z)
 
 
 def test_trivial_lift(
     bits_checks_a: tuple[int, int] = (4, 3),
     bits_checks_b: tuple[int, int] = (3, 2),
     field: int = 3,
 ) -> None:
@@ -298,47 +314,70 @@
     shift = abstract.Element(group, group.generators[0])
     element_a = unit - shift**width
     element_b = unit - shift
     code = codes.LPCode([[element_a]], [[element_b]], conjugate=True)
     assert np.array_equal(np.block(matrix), code.matrix)
 
 
-def test_cyclic_codes() -> None:
-    """Quasi-cyclic codes from arXiv:2308.07915."""
-    dims: tuple[int, ...]
+def test_cyclic_codes(field: int = 3) -> None:
+    """Quasi-cyclic codes from arXiv:2308.07915 and arXiv:2311.16980."""
+    from sympy.abc import x, y
 
+    # first code in Table 3 of arXiv:2308.07915
     dims = (6, 6)
-    terms_a = [("x", 3), ("y", 1), ("y", 2)]
-    terms_b = [("y", 3), ("x", 1), ("x", 2)]
-    code = codes.QCCode(dims, terms_a, terms_b, field=2)
+    poly_a = x**3 + y + y**2
+    poly_b = y**3 + x + x**2
+    code = codes.QCCode(dims, poly_a, poly_b, field=2)
     assert code.num_qudits == 72
     assert code.dimension == 12
     assert code.get_weight() == 6
 
-    dims = (15, 3)
-    terms_a = [("x", 9), ("y", 1), ("y", 2)]
-    terms_b = [("x", 0), ("x", 2), ("x", 7)]
-    code = codes.QCCode(dims, terms_a, terms_b, field=2)
-    assert code.num_qudits == 90
-    assert code.dimension == 8
+    # last code in Table II of arXiv:2311.16980
+    dims_dict = {x: 12, y: 4}
+    poly_a = 1 + y + x * y + x**9
+    poly_b = 1 + x**2 + x**7 + x**9 * y**2
+    code = codes.QCCode(dims_dict, poly_a, poly_b, field=2)
+    assert code.num_qudits == 96
+    assert code.dimension == 10
+    assert code.get_weight() == 8
+
+    # [[144, 12, 12]] code in Table 3 and Figure 2 of arXiv:2308.07915
+    dims = (12, 6)
+    poly_a = x**3 + y + y**2
+    poly_b = y**3 + x + x**2
+    code = codes.QCCode(dims, poly_a, poly_b, field=2)
+    assert code.num_qudits == 144
+    assert code.dimension == 12
     assert code.get_weight() == 6
 
-    with pytest.raises(ValueError, match="does not match"):
-        codes.QCCode((2, 3, 4), terms_a, terms_b, field=2)
+    # check that every check qubit addresses its neighboring data qubits
+    unit_shifts = {(0, 1), (1, 0), (0, -1), (-1, 0)}
+    for plaquette_map, torus_shape in code.get_toric_mappings():
+        shifts_x, shifts_z = code.get_check_shifts(plaquette_map, torus_shape)
+        assert unit_shifts.issubset(shifts_x)
+        assert unit_shifts.issubset(shifts_z)
 
-    with pytest.raises(ValueError, match="not supported"):
-        codes.QCCode(dims, terms_a, terms_b, field=3)
+    # check a case with no toric mappings
+    dims = (6, 6)
+    poly_a = 1 + y + y**2
+    poly_b = y**3 + x**2 + x**4
+    code = codes.QCCode(dims, poly_a, poly_b, field=2)
+    assert not code.get_toric_mappings()
+
+    # fail to match cyclic group orders to free variables
+    with pytest.raises(ValueError, match="Could not match"):
+        codes.QCCode({}, poly_a, poly_b, field=2)
 
 
 def test_GB_code_error() -> None:
     """Raise error when trying to construct incompatible generalized bicycle codes."""
-    matrix_a = [[1, 0], [0, -1]]
+    matrix_a = [[1, 0], [0, 2]]
     matrix_b = [[0, 1], [1, 0]]
     with pytest.raises(ValueError, match="incompatible"):
-        codes.GBCode(matrix_a, matrix_b)
+        codes.GBCode(matrix_a, matrix_b, field=3)
 
 
 def test_lifted_product_codes() -> None:
     """Lifted product codes in Eq. (5) of arXiv:2308.08648."""
     for lift_dim, matrix in [
         (16, [[0, 0, 0, 0, 0], [0, 2, 4, 7, 11], [0, 3, 10, 14, 15]]),
         (21, [[0, 0, 0, 0, 0], [0, 4, 5, 7, 17], [0, 14, 18, 12, 11]]),
@@ -349,82 +388,159 @@
         protograph = abstract.Protograph(proto_matrix)
         code = codes.LPCode(protograph)
         rate = code.dimension / code.num_qudits
         assert rate >= 2 / 17
 
 
 def test_tanner_code() -> None:
-    """Classical Tanner code construction.
-
-    In order to construct a random Tanner code, we need to construct a random regular directed
-    bipartite graph.  To this end, we first construct a random regular graph G = (V,E), and then
-    build a directed bipartite graph G' with vertex sets (V,E).  The edges in G' have the form
-    (v, {v,w}), where v is in V and {v,w} is in E.
-    """
-    subcode = codes.ClassicalCode.random(10, 5)
-    graph = nx.random_regular_graph(subcode.num_bits, subcode.num_bits * 2 + 2)
-    subgraph = nx.DiGraph()
-    for edge in graph.edges:
-        subgraph.add_edge(edge[0], edge)
-        subgraph.add_edge(edge[1], edge)
-    num_sources = sum(1 for node in subgraph if subgraph.in_degree(node) == 0)
-    num_sinks = subgraph.number_of_nodes() - num_sources
+    """Classical Tanner codes on random regular graphs."""
+    subcode = codes.ClassicalCode.random(5, 3)
+    subgraph = nx.random_regular_graph(subcode.num_bits, subcode.num_bits * 2 + 2)
+
+    tag = "sort_label"
+    for node_a, node_b in subgraph.edges:
+        subgraph[node_a][node_b]["sort"] = {node_a: tag, node_b: tag}
 
-    # build a classical Tanner code and check that it has the right number of checks/bits
     code = codes.TannerCode(subgraph, subcode)
-    assert code.num_bits == num_sinks
-    assert code.num_checks == num_sources * code.subcode.num_checks
-
-
-def test_surface_HGP_codes(distance: int = 2, field: int = 3) -> None:
-    """The surface and toric codes as hypergraph product codes."""
-    bit_code: codes.ClassicalCode
-
-    # surface code
-    bit_code = codes.RepetitionCode(distance, field=field)
-    code = codes.HGPCode(bit_code)
-    assert code.num_qudits == distance**2 + (distance - 1) ** 2
-    assert code.dimension == 1
-    assert code.get_distance(bound=10) == distance
+    assert code.num_bits == subgraph.number_of_edges()
+    assert code.num_checks == subgraph.number_of_nodes() * code.subcode.num_checks
+    assert all(code.subgraph.get_edge_data(*edge)["sort"] == tag for edge in code.subgraph.edges)
+
+
+def test_quantum_tanner() -> None:
+    """Quantum Tanner code."""
+    # build the subgraphs of a quantum Tanner code
+    group = abstract.CyclicGroup(12)
+    subset_a = group.random_symmetric_subset(4)
+    subset_b = group.random_symmetric_subset(4)
+    cayplex = objects.CayleyComplex(subset_a, subset_b)
+    subgraph_x, subgraph_z = codes.QTCode.get_subgraphs(cayplex)
+
+    # assert that subgraphs have the right number of nodes, edges, and node degrees
+    size_g = cayplex.group.order
+    size_a = len(cayplex.subset_a)
+    size_b = len(cayplex.subset_b)
+    num_faces = len(cayplex.faces)
+    for graph in [subgraph_x, subgraph_z]:
+        assert graph.number_of_nodes() == num_faces + size_g / 2
+        assert graph.number_of_edges() == num_faces * 2
+        sources = [node for node in graph.nodes if graph.in_degree(node) == 0]
+        assert {graph.out_degree(node) for node in sources} == {size_a * size_b}
 
-    # toric code
-    bit_code = codes.RingCode(distance, field=field)
-    code = codes.HGPCode(bit_code)
-    assert code.num_qudits == 2 * distance**2
-    assert code.dimension == 2
-    assert code.get_distance(bound=10) == distance
-
-    # check logical operators have the correct weight when reduced
-    code.reduce_logical_ops()
-    logical_ops = code.get_logical_ops().reshape((2 * code.dimension, -1))
-    assert all(np.count_nonzero(op) == distance for op in logical_ops)
-
-    # check that the identity operator is a logical operator
-    assert 0 == code.get_distance(codes.Pauli.X, vector=[0] * code.num_qudits)
-    assert 0 == code.get_distance(codes.Pauli.X, vector=[0] * code.num_qudits, bound=True)
+    # raise error if constructing QTCode with codes over different fields
+    subcode_a = codes.RepetitionCode(2, field=2)
+    subcode_b = codes.RepetitionCode(2, field=3)
+    with pytest.raises(ValueError, match="different fields"):
+        codes.QTCode([], [], subcode_a, subcode_b)
 
 
 def test_toric_tanner_code(size: int = 4) -> None:
     """Rotated toric code as a quantum Tanner code."""
-    assert size % 2 == 0, "Rotated toric QTCode construction only works for even side lengths"
-
     group = abstract.Group.product(abstract.CyclicGroup(size), repeat=2)
     shift_x, shift_y = group.generators
     subset_a = [shift_x, ~shift_x]
     subset_b = [shift_y, ~shift_y]
     subcode_a = codes.RepetitionCode(2, field=2)
     code = codes.QTCode(subset_a, subset_b, subcode_a, bipartite=False)
+    assert code.get_code_params() == (size**2, 2, size, 4)
 
-    # verify rotated toric code parameters
-    assert code.get_code_params(bound=10) == (size**2, 2, size, 4)
 
-    # raise error if constructing QTCode with codes over different fields
-    subcode_b = codes.RepetitionCode(2, field=subcode_a.field.order**2)
-    with pytest.raises(ValueError, match="different fields"):
-        code = codes.QTCode(subset_a, subset_b, subcode_a, subcode_b)
+def test_surface_codes(rows: int = 3, cols: int = 2, field: int = 3) -> None:
+    """Ordinary and rotated surface codes."""
 
+    # "ordinary"/original surface code
+    code = codes.SurfaceCode(rows, cols, rotated=False, field=field)
+    assert code.dimension == 1
+    assert code.num_qudits == rows * cols + (rows - 1) * (cols - 1)
+    assert code.get_distance(codes.Pauli.X, bound=10) == cols
+    assert code.get_distance(codes.Pauli.Z, bound=10) == rows
 
-@pytest.mark.parametrize("field", [3, 4])
-def test_qudit_distance(field: int) -> None:
-    """Distance calculations for qudits."""
-    code = codes.HGPCode(codes.RepetitionCode(2, field=field))
-    assert code.get_distance() == 2
+    # rotated surface code
+    code = codes.SurfaceCode(rows, cols, rotated=True, field=field)
+    assert code.dimension == 1
+    assert code.num_qudits == rows * cols
+    assert (
+        code.get_distance(codes.Pauli.X)
+        == codes.CSSCode.get_distance_exact(code, codes.Pauli.X)
+        == cols
+    )
+    assert (
+        code.get_distance(codes.Pauli.Z)
+        == codes.CSSCode.get_distance_exact(code, codes.Pauli.Z)
+        == rows
+    )
+
+    # test that the rotated surface code with conjugate=True is an XZZX code
+    code = codes.SurfaceCode(max(rows, cols), rotated=True, field=2, conjugate=True)
+    for row in code.matrix:
+        row_x, row_z = row[: code.num_qudits], row[-code.num_qudits :]
+        assert np.count_nonzero(row_x) == np.count_nonzero(row_z)
+
+
+def test_toric_codes(field: int = 3) -> None:
+    """Ordinary and rotated toric codes."""
+
+    # "ordinary"/original toric code
+    rows, cols = 5, 2
+    code = codes.ToricCode(rows, cols, rotated=False, field=field)
+    assert code.dimension == 2
+    assert code.num_qudits == 2 * rows * cols
+
+    # check minimal logical operator weights
+    code.reduce_logical_ops(with_ILP=True)
+    assert (
+        {rows, cols}
+        == {sum(op) for op in code.get_logical_ops(codes.Pauli.X).view(np.ndarray)}
+        == {sum(op) for op in code.get_logical_ops(codes.Pauli.Z).view(np.ndarray)}
+    )
+
+    # rotated toric code
+    distance = 4
+    code = codes.ToricCode(distance, rotated=True, field=field)
+    assert code.dimension == 2
+    assert code.num_qudits == distance**2
+    assert codes.CSSCode.get_distance(code) == distance
+
+    # rotated toric XZZX code
+    rows, cols = 6, 4
+    code = codes.ToricCode(rows, cols, rotated=True, field=field, conjugate=True)
+    for row in code.matrix:
+        row_x, row_z = row[: code.num_qudits], row[-code.num_qudits :]
+        assert np.count_nonzero(row_x) == np.count_nonzero(row_z)
+
+    # rotated toric code must have even side lengths
+    with pytest.raises(ValueError, match="must have even side lengths"):
+        codes.ToricCode(3, rotated=True)
+
+
+def test_generalized_surface_codes(size: int = 3, field: int = 2) -> None:
+    """Multi-dimensional surface and toric codes."""
+
+    # recover ordinary surface code in 2D
+    assert np.array_equal(
+        codes.GeneralizedSurfaceCode(size, dim=2, periodic=False, field=field).matrix,
+        codes.SurfaceCode(size, rotated=False, field=field).matrix,
+    )
+
+    # recover ordinary toric code in 2D
+    assert np.array_equal(
+        codes.GeneralizedSurfaceCode(size, dim=2, periodic=True, field=field).matrix,
+        codes.ToricCode(size, rotated=False, field=field).matrix,
+    )
+
+    for dim in [3, 4]:
+        # surface code
+        code = codes.GeneralizedSurfaceCode(size, dim, periodic=False, field=field)
+        assert code.dimension == 1
+        assert code.num_qudits == size**dim + (dim - 1) * size ** (dim - 2) * (size - 1) ** 2
+        assert code.get_distance(codes.Pauli.Z, bound=10) == size
+        assert code.get_distance(codes.Pauli.X, bound=10) == size ** (dim - 1)
+
+        # toric code
+        code = codes.GeneralizedSurfaceCode(size, dim, periodic=True, field=field)
+        assert code.dimension == dim
+        assert code.num_qudits == dim * size**dim
+        assert code.get_distance(codes.Pauli.Z, bound=10) == size
+        assert code.get_distance(codes.Pauli.X, bound=10) == size ** (dim - 1)
+
+    with pytest.raises(ValueError, match=">= 2"):
+        codes.GeneralizedSurfaceCode(size, dim=1)
```

### Comparing `qldpc-0.0.8/qldpc/decoder.py` & `qldpc-0.0.9/qldpc/decoder.py`

 * *Files 8% similar despite different names*

```diff
@@ -162,8 +162,12 @@
     """
     if callable(custom_decoder := decoder_args.pop("decoder", None)):
         return custom_decoder(matrix, syndrome, **decoder_args)
 
     if decoder_args.pop("with_ILP", False):
         return decode_with_ILP(matrix, syndrome, **decoder_args)
 
+    if decoder_args.pop("with_MWPM", False):
+        return decode_with_MWPM(matrix, syndrome, **decoder_args)
+
+    decoder_args.pop("with_BP_OSD", None)
     return decode_with_BP_OSD(matrix, syndrome, **decoder_args)
```

### Comparing `qldpc-0.0.8/qldpc/decoder_test.py` & `qldpc-0.0.9/qldpc/decoder_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 def test_decoding() -> None:
     """Decode a simple problem."""
     matrix = np.eye(3, 2, dtype=int)
     syndrome = np.array([1, 1, 0])
     error = np.array([1, 1], dtype=int)
     assert np.allclose(error, decoder.decode(matrix, syndrome, with_ILP=False))
     assert np.allclose(error, decoder.decode(matrix, syndrome, with_ILP=True))
-    assert np.allclose(error, decoder.decode_with_MWPM(matrix, syndrome))
+    assert np.allclose(error, decoder.decode(matrix, syndrome, with_MWPM=True))
 
     # decode over trinary field
     modulus = 3
     answer = -error % modulus
     result = decoder.decode(-matrix, syndrome, with_ILP=True, modulus=modulus, lower_bound_row=-1)
     assert np.allclose(answer, result)
```

### Comparing `qldpc-0.0.8/qldpc/named_codes.py` & `qldpc-0.0.9/qldpc/named_codes.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,38 +14,38 @@
    See the License for the specific language governing permissions and
    limitations under the License.
 """
 
 import ast
 import re
 
-from qldpc.small_groups import gap_is_installed, get_gap_result, use_disk_cache
+from qldpc.named_groups import gap_is_installed, get_gap_result, use_disk_cache
 
 
 @use_disk_cache("qldpc_codes")
-def get_code(name: str) -> tuple[list[list[int]], int | None]:
+def get_code(code: str) -> tuple[list[list[int]], int | None]:
     """Retrieve a group from GAP."""
 
     # run GAP commands
     if not gap_is_installed():
         raise ValueError("GAP 4 is not installed")
     commands = [
         'LoadPackage("guava");',
-        f"code := {name};",
+        f"code := {code};",
         "mat := CheckMat(code);",
         r'Print(LeftActingDomain(code), "\n");',
         r'for vec in mat do Print(List(vec, x -> Int(x)), "\n"); od;',
     ]
-    result = get_gap_result(commands)
+    result = get_gap_result(*commands)
 
     if "guava package is not available" in result.stdout:
         raise ValueError("GAP package GUAVA not available")
 
     if not result.stdout.strip():
-        raise ValueError(f"Code not recognized by the GAP package GUAVA: {name}")
+        raise ValueError(f"Code not recognized by the GAP package GUAVA: {code}")
 
     # identify base field and retrieve parity checks
     field: int | None = None
     checks = []
     for line in result.stdout.splitlines():
         if not line.strip():
             continue
```

### Comparing `qldpc-0.0.8/qldpc/named_codes_test.py` & `qldpc-0.0.9/qldpc/named_codes_test.py`

 * *Files identical despite different names*

### Comparing `qldpc-0.0.8/qldpc/objects_test.py` & `qldpc-0.0.9/qldpc/objects_test.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,14 +11,15 @@
    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
 """
 
+import galois
 import numpy as np
 import pytest
 
 from qldpc import abstract, objects
 
 
 def test_pauli() -> None:
@@ -101,22 +102,35 @@
         subset_a = [shift_x * shift_y, ~(shift_x * shift_y)]
         subset_b = [shift_x * shift_y**2, ~(shift_x * shift_y**2)]
         cayplex = objects.CayleyComplex(subset_a, subset_b, bipartite=bipartite)
         assert_valid_complex(cayplex)
 
 
 def assert_valid_complex(cayplex: objects.CayleyComplex) -> None:
-    """Run various sanity checks on a Cayley complex."""
-    # assert that the complex has the right number of vertices, edges, and faces
-    size_g = cayplex.group.order()
+    """Assert that a Cayley complex has the correct number of vertices, edges, and faces."""
+    size_g = cayplex.group.order
     size_a = len(cayplex.subset_a)
     size_b = len(cayplex.subset_b)
     assert cayplex.graph.number_of_nodes() == size_g
     assert cayplex.graph.number_of_edges() == size_g * (size_a + size_b) // 2
     assert len(cayplex.faces) == size_g * size_a * size_b // 4
 
-    # check that the subgraphs have the correct number of nodes, edges, and node degrees
-    for graph in cayplex.subgraphs():
-        assert graph.number_of_nodes() == len(cayplex.faces) + size_g / 2
-        assert graph.number_of_edges() == len(cayplex.faces) * 2
-        sources = [node for node in graph.nodes if graph.in_degree(node) == 0]
-        assert {graph.out_degree(node) for node in sources} == {size_a * size_b}
+
+def test_chain_complex(field: int = 3) -> None:
+    """Chain complex construction and errors."""
+
+    # tensor product of one-complexes
+    mat = np.random.randint(field, size=(2, 3))
+    two_chain = objects.ChainComplex.tensor_product(mat, mat, field)
+    assert not np.any(two_chain.op(0))
+    assert not np.any(two_chain.op(two_chain.num_links + 1))
+
+    # tensor product of a two-complex and its dual
+    objects.ChainComplex.tensor_product(two_chain, two_chain.T, field)
+
+    # invalid chain complex constructions
+    with pytest.raises(ValueError, match="Inconsistent base fields"):
+        objects.ChainComplex(galois.GF(field)(mat), field=field**2)
+    with pytest.raises(ValueError, match="boundary operators .* must compose to zero"):
+        objects.ChainComplex(mat, mat, field=field)
+    with pytest.raises(ValueError, match="different fields"):
+        objects.ChainComplex.tensor_product(galois.GF(field)(mat), galois.GF(field**2)(mat))
```

### Comparing `qldpc-0.0.8/qldpc/small_groups.py` & `qldpc-0.0.9/qldpc/named_groups.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Module for loading groups indexed by the GAP computer algebra system
+"""Module for loading groups from the GAP computer algebra system
 
    Copyright 2023 The qLDPC Authors and Infleqtion Inc.
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
@@ -15,71 +15,85 @@
    limitations under the License.
 """
 
 import functools
 import os
 import re
 import subprocess
-import tempfile
 import urllib.error
 import urllib.request
-from collections.abc import Callable, Hashable
+from collections.abc import Callable, Hashable, Sequence
 from typing import Any
 
 import diskcache
 import platformdirs
 
 GENERATORS_LIST = list[list[tuple[int, ...]]]
 GROUPNAMES_URL = "https://people.maths.bris.ac.uk/~matyd/GroupNames/"
 
 
+def maybe_get_webpage(order: int) -> str | None:
+    """Try to retrieve the webpage listing all groups up to a given order."""
+    try:
+        url = GROUPNAMES_URL + ("index500.html" if order > 60 else "")
+        page = urllib.request.urlopen(url)
+        return page.read().decode("utf-8")
+    except (urllib.error.URLError, urllib.error.HTTPError):
+        # we cannot access the webapage
+        return None
+
+
 def get_group_url(order: int, index: int) -> str | None:
     """Retrieve the webpage of an indexed GAP group on GroupNames.org."""
 
-    try:
-        # load index
-        extra = "index500.html" if order > 60 else ""
-        index_url = GROUPNAMES_URL + extra
-        index_page = urllib.request.urlopen(index_url)
-        index_page_html = index_page.read().decode("utf-8")
-    except (urllib.error.URLError, urllib.error.HTTPError):
+    # get the HTML for the page with all groups
+    page_html = maybe_get_webpage(order)
+    if page_html is None:
         # we cannot access the webapage
         return None
 
     # extract section with the specified group
-    loc = index_page_html.find(f"<td>{order},{index}</td>")
+    loc = page_html.find(f"<td>{order},{index}</td>")
     if loc == -1:
-        raise ValueError(f"Group {order},{index} not found at {index_url}")
+        raise ValueError(f"Group {order},{index} not found on GroupNames.org")
 
-    end = loc + index_page_html[loc:].find("\n")
-    start = loc - index_page_html[:loc][::-1].find("\n")
-    section = index_page_html[start:end]
+    end = loc + page_html[loc:].find("\n")
+    start = loc - page_html[:loc][::-1].find("\n")
+    section = page_html[start:end]
 
     # extract first link from this section
     match = re.search(r'href="([^"]*)"', section)
     if match is None:
         raise ValueError(f"Webpage for group {order},{index} not found")
 
     # return url for the desired group
     return GROUPNAMES_URL + match.group(1)
 
 
-def get_generators_from_groupnames(order: int, index: int) -> GENERATORS_LIST | None:
+def get_generators_from_groupnames(group: str) -> GENERATORS_LIST | None:
     """Retrieve GAP group generators from GroupNames.org."""
 
+    # extract order and index of a SmallGroup
+    match = re.match(r"SmallGroup\(([0-9]+),([0-9]+)\)", group)
+    if match:
+        order, index = map(int, match.groups())
+    else:
+        # this group is not indexed in GroupNames.org
+        return None
+
     # load web page for the specified group
     group_url = get_group_url(order, index)
     if group_url is None:
         # we cannot access the webapage
         return None
     group_page = urllib.request.urlopen(group_url)
     group_page_html = group_page.read().decode("utf-8")
 
     # extract section with the generators we are after
-    loc = group_page_html.find("Permutation representations")
+    loc = group_page_html.lower().find("permutation representation")
     end = group_page_html[loc:].find("copytext")  # go until the first copy-able text
     section = group_page_html[loc : loc + end]
 
     # isolate generator text
     section = section[section.find("<pre") :]
     match = re.search(r">((?:.|\n)*?)<\/pre>", section)
     if match is None:
@@ -104,54 +118,49 @@
     """Is GAP 4 installed?"""
     commands = ["script", "-c", "gap --version", os.devnull]
     result = subprocess.run(commands, capture_output=True, text=True)
     lines = result.stdout.splitlines()
     return len(lines) == 2 and lines[1].startswith("GAP 4")
 
 
-def sanitize_gap_commands(commands: list[str]) -> list[str]:
+def sanitize_gap_commands(commands: Sequence[str]) -> tuple[str, ...]:
     """Sanitize GAP commands: don't format Print statements, and quit at the end."""
     stream = "__stream__"
     prefix = [
         f"{stream} := OutputTextUser();",
         f"SetPrintFormattingStatus({stream}, false);",
     ]
     suffix = ["QUIT;"]
     commands = [cmd.replace("Print(", f"PrintTo({stream}, ") for cmd in commands]
-    return prefix + commands + suffix
+    return tuple(prefix + commands + suffix)
 
 
-def get_gap_result(commands: list[str]) -> subprocess.CompletedProcess[str]:
+def get_gap_result(*commands: str) -> subprocess.CompletedProcess[str]:
     """Get the output from the given GAP commands."""
     commands = sanitize_gap_commands(commands)
-    with tempfile.NamedTemporaryFile(mode="w+", delete=False, suffix=".gap") as script:
-        script.write("\n".join(commands))
-        script_name = script.name
-    shell_commands = ["gap", "-q", "--quitonbreak", script_name]
+    shell_commands = ["gap", "-q", "--quitonbreak", "-c", " ".join(commands)]
     result = subprocess.run(shell_commands, capture_output=True, text=True)
-    os.remove(script_name)
     return result
 
 
-def get_generators_with_gap(order: int, index: int) -> GENERATORS_LIST | None:
+def get_generators_with_gap(group: str) -> GENERATORS_LIST | None:
     """Retrieve GAP group generators from GAP directly."""
 
     if not gap_is_installed():
         return None
 
     # run GAP commands
-    group = f"SmallGroup({order},{index})"
     commands = [
         f"G := {group};",
         "iso := IsomorphismPermGroup(G);",
         "permG := Image(iso, G);",
         "gens := GeneratorsOfGroup(permG);",
         r'for gen in gens do Print(gen, "\n"); od;',
     ]
-    result = get_gap_result(commands)
+    result = get_gap_result(*commands)
 
     if not result.stdout.strip():
         raise ValueError(f"Group not recognized by GAP: {group}")
 
     # collect generators
     generators = []
     for line in result.stdout.splitlines():
@@ -176,44 +185,64 @@
     cache_name: str,
 ) -> Callable[[Callable[..., Any]], Callable[..., Any]]:
     """Cache new results to disk, and retrieve existing results (if available) from the cache."""
 
     def decorator(func: Callable[..., Any]) -> Callable[..., Any]:
 
         @functools.wraps(func)
-        def wrapper(*args: Hashable) -> Any:
+        def wrapper(*args: Hashable, **kwargs: Hashable) -> Any:
 
             # retrieve results from cache, if available
             cache = diskcache.Cache(platformdirs.user_cache_dir(cache_name))
-            generators = cache.get(args, None)
-            if generators is not None:
-                return generators
+            key = args + tuple(kwargs.items())
+            if key in cache:
+                return cache[key]
 
             # compute results and save to cache
-            result = func(*args)
-            cache[args] = result
+            result = func(*args, **kwargs)
+            cache[key] = result
             return result
 
         return wrapper
 
     return decorator
 
 
 @use_disk_cache("qldpc_groups")
-def get_generators(order: int, index: int) -> GENERATORS_LIST:
+def get_generators(group: str) -> GENERATORS_LIST:
     """Retrieve GAP group generators."""
-    for get_generators_func in [
-        get_generators_with_gap,
-        get_generators_from_groupnames,
-    ]:
-        generators = get_generators_func(order, index)
-        if generators is not None:
-            return generators
 
-    # we could not find or retrieve the generators :(
+    generators = get_generators_with_gap(group)
+    if generators is not None:
+        return generators
+
+    generators = get_generators_from_groupnames(group)
+    if generators is not None:
+        return generators
+
     message = [
         "Cannot build GAP group:",
         "- local database does not contain the group",
-        "- GAP 4 not installed",
-        "- GroupNames.org is unreachable",
+        "- GAP 4 is not installed",
     ]
+    if group.startswith("SmallGroup"):
+        message.append("- GroupNames.org is unreachable")
+    else:
+        message.append("- group not indexed by GroupNames.org")
     raise ValueError("\n".join(message))
+
+
+@use_disk_cache("qldpc_groups")
+def get_small_group_number(order: int) -> int:
+    """Get the number of 'SmallGroup's of a given order."""
+    if gap_is_installed():
+        command = f"Print(NumberSmallGroups({order}));"
+        return int(get_gap_result(command).stdout)
+
+    # get the HTML for the page with all groups
+    page_html = maybe_get_webpage(order)
+    if page_html is None:
+        # we cannot access the webapage
+        raise ValueError("Cannot determine the number of small groups")
+
+    matches = re.findall(rf"<td>{order},([0-9]+)</td>", page_html)
+    return max(int(match) for match in matches)
```

### Comparing `qldpc-0.0.8/qldpc/small_groups_test.py` & `qldpc-0.0.9/qldpc/named_groups_test.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Unit tests for small_groups.py
+"""Unit tests for named_groups.py
 
    Copyright 2023 The qLDPC Authors and Infleqtion Inc.
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
@@ -17,19 +17,20 @@
 
 import subprocess
 import unittest.mock
 import urllib
 
 import pytest
 
-from qldpc import small_groups
+from qldpc import named_groups
 
 ORDER, INDEX = 2, 1
 GENERATORS = [[(0, 1)]]
-GROUP_URL = small_groups.GROUPNAMES_URL + "1/C2.html"
+GROUP = f"SmallGroup({ORDER},{INDEX})"
+GROUP_URL = named_groups.GROUPNAMES_URL + "1/C2.html"
 MOCK_INDEX_HTML = """<table class="gptable" columns="6" style='width: 70%;'>
 <tr><th width="12%"></th><th width="60%"></th><th width="5%"><a href='T.html'>d</a></th><th width="5%"><a href='R.html'>&rho;</a></th><th width="12%">Label</th><th width="7%">ID</th></tr><tr><td id="c2"><a href="1/C2.html">C<sub>2</sub></a></td><td><a href="cyclic.html">Cyclic</a> group</td><td><a href="T15.html#c2">2</a></td><td><a href="R.html#dim1+">1+</a></td><td>C2</td><td>2,1</td></tr>
 </table>"""  # pylint: disable=line-too-long  # noqa: E501
 MOCK_GROUP_HTML = """<b><a href='https://en.wikipedia.org/wiki/Group actions' title='See wikipedia' class='wiki'>Permutation representations of C<sub>2</sub></a></b><br><a id='shl1' class='shl' href="javascript:showhide('shs1','shl1','Regular action on 2 points');"><span class="nsgpn">&#x25ba;</span>Regular action on 2 points</a> - transitive group <a href="../T15.html#2t1">2T1</a><div id='shs1' class='shs'>Generators in S<sub>2</sub><br><pre class='pre' id='textgn1'>(1 2)</pre>&emsp;<button class='copytext' id='copygn1'>Copy</button><br>"""  # pylint: disable=line-too-long  # noqa: E501
 
 
 def get_mock_page(text: str) -> unittest.mock.MagicMock:
@@ -42,150 +43,188 @@
 def test_get_group_url() -> None:
     """Retrive url for group webpage on GroupNames.org."""
 
     # cannot connect to general webpage
     with unittest.mock.patch(
         "urllib.request.urlopen", side_effect=urllib.error.URLError("message")
     ):
-        assert small_groups.get_group_url(ORDER, INDEX) is None
+        assert named_groups.get_group_url(ORDER, INDEX) is None
 
     # cannot find group in the index
     mock_page = get_mock_page(MOCK_INDEX_HTML.replace(f"{ORDER},{INDEX}", ""))
     with (
         pytest.raises(ValueError, match="Group .* not found"),
         unittest.mock.patch("urllib.request.urlopen", return_value=mock_page),
     ):
-        small_groups.get_group_url(ORDER, INDEX)
+        named_groups.get_group_url(ORDER, INDEX)
 
     # cannot find link to group webpage
     mock_page = get_mock_page(MOCK_INDEX_HTML.replace("href", ""))
     with (
         pytest.raises(ValueError, match="Webpage .* not found"),
         unittest.mock.patch("urllib.request.urlopen", return_value=mock_page),
     ):
-        small_groups.get_group_url(ORDER, INDEX)
+        named_groups.get_group_url(ORDER, INDEX)
 
     # everything works as expected
     mock_page = get_mock_page(MOCK_INDEX_HTML)
     with unittest.mock.patch("urllib.request.urlopen", return_value=mock_page):
-        assert small_groups.get_group_url(ORDER, INDEX) == GROUP_URL
+        assert named_groups.get_group_url(ORDER, INDEX) == GROUP_URL
 
 
 def test_get_generators_from_groupnames() -> None:
     """Retrive generators from group webpage on GroupNames.org."""
 
+    # group not indexed
+    assert named_groups.get_generators_from_groupnames("") is None
+
     # group url not found
-    with unittest.mock.patch("qldpc.small_groups.get_group_url", return_value=None):
-        assert small_groups.get_generators_from_groupnames(ORDER, INDEX) is None
+    with unittest.mock.patch("qldpc.named_groups.get_group_url", return_value=None):
+        assert named_groups.get_generators_from_groupnames(GROUP) is None
 
     # cannot find generators
     mock_page = get_mock_page(MOCK_GROUP_HTML.replace("pre", ""))
     with (
         pytest.raises(ValueError, match="Generators .* not found"),
-        unittest.mock.patch("qldpc.small_groups.get_group_url", return_value=GROUP_URL),
+        unittest.mock.patch("qldpc.named_groups.get_group_url", return_value=GROUP_URL),
         unittest.mock.patch("urllib.request.urlopen", return_value=mock_page),
     ):
-        small_groups.get_generators_from_groupnames(ORDER, INDEX)
+        named_groups.get_generators_from_groupnames(GROUP)
 
     # everything works as expected
     mock_page = get_mock_page(MOCK_GROUP_HTML)
     with (
-        unittest.mock.patch("qldpc.small_groups.get_group_url", return_value=GROUP_URL),
+        unittest.mock.patch("qldpc.named_groups.get_group_url", return_value=GROUP_URL),
         unittest.mock.patch("urllib.request.urlopen", return_value=mock_page),
     ):
-        assert small_groups.get_generators_from_groupnames(ORDER, INDEX) == GENERATORS
+        assert named_groups.get_generators_from_groupnames(GROUP) == GENERATORS
 
 
 def get_mock_process(stdout: str) -> subprocess.CompletedProcess[str]:
     """Fake process with the given stdout."""
     return subprocess.CompletedProcess(args=[], returncode=0, stdout=stdout)
 
 
 def test_gap_is_installed() -> None:
     """Is GAP 4 installed?"""
     with unittest.mock.patch("subprocess.run", return_value=get_mock_process("")):
-        assert not small_groups.gap_is_installed()
+        assert not named_groups.gap_is_installed()
     with unittest.mock.patch("subprocess.run", return_value=get_mock_process("\nGAP 4")):
-        assert small_groups.gap_is_installed()
+        assert named_groups.gap_is_installed()
 
 
 def test_get_gap_result() -> None:
     """Run GAP commands and retrieve the GAP output."""
     output = "test"
     with unittest.mock.patch("subprocess.run", return_value=get_mock_process(output)):
-        assert small_groups.get_gap_result([]).stdout == output
+        assert named_groups.get_gap_result().stdout == output
 
 
 def test_get_generators_with_gap() -> None:
     """Retrive generators from GAP 4."""
 
     # GAP is not installed
-    with unittest.mock.patch("qldpc.small_groups.gap_is_installed", return_value=False):
-        assert small_groups.get_generators_with_gap(ORDER, INDEX) is None
+    with unittest.mock.patch("qldpc.named_groups.gap_is_installed", return_value=False):
+        assert named_groups.get_generators_with_gap(GROUP) is None
 
     # cannot extract cycle from string
     mock_process = get_mock_process("\n(1, 2a)\n")
     with (
         pytest.raises(ValueError, match="Cannot extract cycle"),
-        unittest.mock.patch("qldpc.small_groups.gap_is_installed", return_value=True),
-        unittest.mock.patch("qldpc.small_groups.get_gap_result", return_value=mock_process),
+        unittest.mock.patch("qldpc.named_groups.gap_is_installed", return_value=True),
+        unittest.mock.patch("qldpc.named_groups.get_gap_result", return_value=mock_process),
     ):
-        assert small_groups.get_generators_with_gap(ORDER, INDEX) is None
+        assert named_groups.get_generators_with_gap(GROUP) is None
 
     # group not recognized by GAP
     mock_process = get_mock_process("")
     with (
         pytest.raises(ValueError, match="not recognized by GAP"),
-        unittest.mock.patch("qldpc.small_groups.gap_is_installed", return_value=True),
-        unittest.mock.patch("qldpc.small_groups.get_gap_result", return_value=mock_process),
+        unittest.mock.patch("qldpc.named_groups.gap_is_installed", return_value=True),
+        unittest.mock.patch("qldpc.named_groups.get_gap_result", return_value=mock_process),
     ):
-        assert small_groups.get_generators_with_gap(ORDER, INDEX) is None
+        assert named_groups.get_generators_with_gap(GROUP) is None
 
     # everything works as expected
     mock_process = get_mock_process("\n(1, 2)\n")
     with (
-        unittest.mock.patch("qldpc.small_groups.gap_is_installed", return_value=True),
-        unittest.mock.patch("qldpc.small_groups.get_gap_result", return_value=mock_process),
+        unittest.mock.patch("qldpc.named_groups.gap_is_installed", return_value=True),
+        unittest.mock.patch("qldpc.named_groups.get_gap_result", return_value=mock_process),
     ):
-        assert small_groups.get_generators_with_gap(ORDER, INDEX) == GENERATORS
+        assert named_groups.get_generators_with_gap(GROUP) == GENERATORS
 
 
 def test_get_generators() -> None:
     """Retrieve generators somehow."""
 
     # use cache to save/retrieve results
     with unittest.mock.patch("diskcache.Cache", return_value={}):
         # compute and save result to cache
         with unittest.mock.patch(
-            "qldpc.small_groups.get_generators_with_gap", return_value=GENERATORS
+            "qldpc.named_groups.get_generators_with_gap", return_value=GENERATORS
         ):
-            assert small_groups.get_generators(ORDER, INDEX) == GENERATORS
+            assert named_groups.get_generators(GROUP) == GENERATORS
 
         # retrieve result from cache
-        assert small_groups.get_generators(ORDER, INDEX) == GENERATORS
+        assert named_groups.get_generators(GROUP) == GENERATORS
 
     # strip cache wrapper
-    if hasattr(small_groups.get_generators, "__wrapped__"):
-        small_groups.get_generators = small_groups.get_generators.__wrapped__
+    if hasattr(named_groups.get_generators, "__wrapped__"):
+        named_groups.get_generators = named_groups.get_generators.__wrapped__
 
     # retrieve from GAP
     with (
-        unittest.mock.patch("qldpc.small_groups.get_generators_with_gap", return_value=GENERATORS),
+        unittest.mock.patch("qldpc.named_groups.get_generators_with_gap", return_value=GENERATORS),
     ):
-        assert small_groups.get_generators(ORDER, INDEX) == GENERATORS
+        assert named_groups.get_generators(GROUP) == GENERATORS
 
     # retrieve from GroupNames.org
     with (
-        unittest.mock.patch("qldpc.small_groups.get_generators_with_gap", return_value=None),
+        unittest.mock.patch("qldpc.named_groups.get_generators_with_gap", return_value=None),
         unittest.mock.patch(
-            "qldpc.small_groups.get_generators_from_groupnames", return_value=GENERATORS
+            "qldpc.named_groups.get_generators_from_groupnames", return_value=GENERATORS
         ),
     ):
-        assert small_groups.get_generators(ORDER, INDEX) == GENERATORS
+        assert named_groups.get_generators(GROUP) == GENERATORS
 
     # fail to retrieve from anywhere :(
     with (
-        pytest.raises(ValueError, match="Cannot build GAP group"),
-        unittest.mock.patch("qldpc.small_groups.get_generators_with_gap", return_value=None),
-        unittest.mock.patch("qldpc.small_groups.get_generators_from_groupnames", return_value=None),
+        unittest.mock.patch("qldpc.named_groups.get_generators_with_gap", return_value=None),
+        unittest.mock.patch("qldpc.named_groups.get_generators_from_groupnames", return_value=None),
+    ):
+        with pytest.raises(ValueError, match="Cannot build GAP group"):
+            named_groups.get_generators(GROUP)
+        with pytest.raises(ValueError, match="Cannot build GAP group"):
+            named_groups.get_generators("CyclicGroup(2)")
+
+
+def test_get_small_group_number() -> None:
+    """Retrieve the number of groups of some order."""
+    # strip cache wrapper
+    if hasattr(named_groups.get_small_group_number, "__wrapped__"):
+        named_groups.get_small_group_number = named_groups.get_small_group_number.__wrapped__
+
+    order, number = 16, 14
+    text = rf"<td>{order},{number}</td>"
+
+    # fail to determine group number
+    with (
+        pytest.raises(ValueError, match="Cannot determine"),
+        unittest.mock.patch("qldpc.named_groups.maybe_get_webpage", return_value=None),
+        unittest.mock.patch("qldpc.named_groups.gap_is_installed", return_value=False),
+    ):
+        named_groups.get_small_group_number(order)
+
+    # retrieve from GAP
+    mock_process = get_mock_process(str(number))
+    with (
+        unittest.mock.patch("qldpc.named_groups.gap_is_installed", return_value=True),
+        unittest.mock.patch("qldpc.named_groups.get_gap_result", return_value=mock_process),
+    ):
+        assert named_groups.get_small_group_number(order) == number
+
+    # retrieve from GroupNames.org
+    with (
+        unittest.mock.patch("qldpc.named_groups.gap_is_installed", return_value=False),
+        unittest.mock.patch("qldpc.named_groups.maybe_get_webpage", return_value=text),
     ):
-        small_groups.get_generators(ORDER, INDEX)
+        assert named_groups.get_small_group_number(order) == number
```

### Comparing `qldpc-0.0.8/PKG-INFO` & `qldpc-0.0.9/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: qLDPC
-Version: 0.0.8
-Summary: Tools for constructing and analyzing quantum low density partity check (qLDPC) codes.
+Version: 0.0.9
+Summary: Tools for constructing and analyzing quantum low density parity check (qLDPC) codes.
 Home-page: https://github.com/Infleqtion/qLDPC
 License: Apache-2.0
 Keywords: quantum computing,quantum error correction,low density partiy check codes,LDPC
 Author: Michael A. Perlin
 Author-email: mika.perlin@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -27,21 +27,20 @@
 Requires-Dist: gurobipy (>=10.0.0)
 Requires-Dist: ldpc (>=0.1.0)
 Requires-Dist: networkx (>=2.6.2)
 Requires-Dist: numpy (>=1.22.0)
 Requires-Dist: platformdirs (>=4.0.0)
 Requires-Dist: pymatching (>=2.1.0)
 Requires-Dist: sympy (>=1.12)
-Requires-Dist: types-protobuf (<=4.24.0.4)
 Project-URL: Repository, https://github.com/Infleqtion/qLDPC
 Description-Content-Type: text/markdown
 
 # qLDPC
 
-This package contains tools for constructing and analyzing [quantum low density partity check (qLDPC) codes](https://errorcorrectionzoo.org/c/qldpc).
+This package contains tools for constructing and analyzing [quantum low density parity check (qLDPC) codes](https://errorcorrectionzoo.org/c/qldpc).
 
 ## 📦 Installation
 
 This package requires Python>=3.10, and can be installed from PyPI with
 ```
 pip install qldpc
 ```
@@ -51,26 +50,31 @@
 pip install -e qLDPC
 ```
 You can also `pip install -e 'qLDPC[dev]'` to additionally install some development tools.
 
 ## 🚀 Features
 
 Notable features include:
-- `abstract.py`: module for basic abstract algebra (groups, algebras, and representations thereof).
 - `ClassicalCode`: class for representing classical linear error-correcting codes over finite fields.
+  - Various pre-defined classical code families.
+  - Communication with the [GAP/GUAVA](https://www.gap-system.org/Packages/guava.html) package for [even more codes](https://docs.gap-system.org/pkg/guava/doc/chap5.html).
 - `QuditCode`: general class for constructing [Galois-qudit codes](https://errorcorrectionzoo.org/c/galois_into_galois).
 - `CSSCode`: general class for constructing [quantum CSS codes](https://errorcorrectionzoo.org/c/css) out of two mutually compatible `ClassicalCode`s.
   - `CSSCode.get_logical_ops`: method to construct a complete basis of nontrivial logical operators for a `CSSCode`.
-  - `CSSCode.get_distance`: method to compute the code distance (i.e., the minimum weight of a nontrivial logical operator) of a `CSSCode`.  Includes options for computing the exact code distance by brute force, as well as estimate (or upper bound) with the method of [arXiv:2308.07915](https://arxiv.org/abs/2308.07915).
+  - `CSSCode.get_distance`: method to compute the code distance (i.e., the minimum weight of a nontrivial logical operator) of a `CSSCode`.  Includes options for computing the exact code distance by brute force, as well as an estimate (or upper bound) with the method of [arXiv:2308.07915](https://arxiv.org/abs/2308.07915).
   - Includes options for applying local Hadamard transformations, which is useful for tailoring a `CSSCode` to biased noise (see [arXiv:2202.01702](https://arxiv.org/abs/2202.01702)).  Options to apply more general Clifford code deformations are pending.
 - `GBCode`: class for constructing [generalized bicycle codes](https://errorcorrectionzoo.org/c/generalized_bicycle), as described in [arXiv:1904.02703](https://arxiv.org/abs/1904.02703).
 - `QCCode`: class for constructing the [quasi-cyclic codes](https://errorcorrectionzoo.org/c/quantum_quasi_cyclic) in [arXiv:2308.07915](https://arxiv.org/abs/2308.07915).
 - `HGPCode`: class for constructing [hypergraph product codes](https://errorcorrectionzoo.org/c/hypergraph_product) out of two `ClassicalCode`s.
 - `LPCode`: class for constructing [lifted product codes](https://errorcorrectionzoo.org/c/lifted_product) out of two protographs (i.e., matrices whose entries are elements of a group algebra).  See [arXiv:2012.04068](https://arxiv.org/abs/2012.04068) and [arXiv:2202.01702](https://arxiv.org/abs/2202.01702).
 - `QTCode`: class for constructing [quantum Tanner codes](https://errorcorrectionzoo.org/c/quantum_tanner) out of (a) two symmetric subsets `A` and `B` of a group `G`, and (b) two `ClassicalCode`s with block lengths `|A|` and `|B|`.  See [arXiv:2202.13641](https://arxiv.org/abs/2202.13641) and [arXiv:2206.07571](https://arxiv.org/abs/2206.07571).
+- `abstract.py`: module for basic abstract algebra (groups, algebras, and representations thereof).
+  - Various pre-defined groups (mostly borrowed from [SymPy](https://docs.sympy.org/latest/modules/combinatorics/named_groups.html)).
+  - Communication with the [GAP](https://www.gap-system.org/) computer algebra system and [GroupNames.org](https://people.maths.bris.ac.uk/~matyd/GroupNames/) for constructing [even more groups](https://docs.gap-system.org/doc/ref/chap50.html).
+- `objects.py`: module for constructing and helper objects such as Cayley complexes and chain complexes, which are instrumental for the construction of various quantum codes.
 
 ## 🤔 Questions and issues
 
 If this project gains interest and traction, I'll add a documentation webpage and material to help users get started quickly.  I am also planning to write a paper that presents and explains this project.  In the meantime, you can explore the documentation and explanations in the source code.  `qldpc/codes_test.py` contains some examples of using the classes and methods described above.
 
 If you have any questions, feedback, or requests, please [open an issue on GitHub](https://github.com/Infleqtion/qLDPC/issues/new) or email me at [michael.perlin@infleqtion.com](mailto:michael.perlin@infleqtion.com)!
```

