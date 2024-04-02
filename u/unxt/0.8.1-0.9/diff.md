# Comparing `tmp/unxt-0.8.1.tar.gz` & `tmp/unxt-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Fri Mar 29 03:22:58 2024, max compression
+gzip compressed data, last modified: Tue Apr  2 18:21:24 2024, max compression
```

## Comparing `unxt-0.8.1.tar` & `unxt-0.9.tar`

### file list

```diff
@@ -1,46 +1,49 @@
--rw-r--r--   0        0        0      366 2024-03-29 03:22:58.000000 unxt-0.8.1/.copier-answers.yml
--rw-r--r--   0        0        0      125 2024-03-29 03:22:58.000000 unxt-0.8.1/.git_archival.txt
--rw-r--r--   0        0        0       32 2024-03-29 03:22:58.000000 unxt-0.8.1/.gitattributes
--rw-r--r--   0        0        0     2558 2024-03-29 03:22:58.000000 unxt-0.8.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      309 2024-03-29 03:22:58.000000 unxt-0.8.1/.readthedocs.yml
--rw-r--r--   0        0        0      439 2024-03-29 03:22:58.000000 unxt-0.8.1/conftest.py
--rw-r--r--   0        0        0     2809 2024-03-29 03:22:58.000000 unxt-0.8.1/noxfile.py
--rw-r--r--   0        0        0     2389 2024-03-29 03:22:58.000000 unxt-0.8.1/.github/CONTRIBUTING.md
--rw-r--r--   0        0        0      224 2024-03-29 03:22:58.000000 unxt-0.8.1/.github/dependabot.yml
--rw-r--r--   0        0        0      668 2024-03-29 03:22:58.000000 unxt-0.8.1/.github/matchers/pylint.json
--rw-r--r--   0        0        0     1540 2024-03-29 03:22:58.000000 unxt-0.8.1/.github/workflows/cd.yml
--rw-r--r--   0        0        0     1630 2024-03-29 03:22:58.000000 unxt-0.8.1/.github/workflows/ci.yml
--rw-r--r--   0        0        0      862 2024-03-29 03:22:58.000000 unxt-0.8.1/docs/conf.py
--rw-r--r--   0        0        0      191 2024-03-29 03:22:58.000000 unxt-0.8.1/docs/index.md
--rw-r--r--   0        0        0      912 2024-03-29 03:22:58.000000 unxt-0.8.1/src/unxt/__init__.py
--rw-r--r--   0        0        0    12664 2024-03-29 03:22:58.000000 unxt-0.8.1/src/unxt/_base.py
--rw-r--r--   0        0        0     1124 2024-03-29 03:22:58.000000 unxt-0.8.1/src/unxt/_compat.py
--rw-r--r--   0        0        0     6435 2024-03-29 03:22:58.000000 unxt-0.8.1/src/unxt/_core.py
--rw-r--r--   0        0        0     2572 2024-03-29 03:22:58.000000 unxt-0.8.1/src/unxt/_distance.py
--rw-r--r--   0        0        0      570 2024-03-29 03:22:58.000000 unxt-0.8.1/src/unxt/_fast.py
--rw-r--r--   0        0        0     3348 2024-03-29 03:22:58.000000 unxt-0.8.1/src/unxt/_register_dispatches.py
--rw-r--r--   0        0        0    89347 2024-03-29 03:22:58.000000 unxt-0.8.1/src/unxt/_register_primitives.py
--rw-r--r--   0        0        0      263 2024-03-29 03:22:58.000000 unxt-0.8.1/src/unxt/_typing.py
--rw-r--r--   0        0        0     1235 2024-03-29 03:22:58.000000 unxt-0.8.1/src/unxt/_utils.py
--rw-r--r--   0        0        0      411 2024-03-29 03:22:58.000000 unxt-0.8.1/src/unxt/_version.py
--rw-r--r--   0        0        0       82 2024-03-29 03:22:58.000000 unxt-0.8.1/src/unxt/_version.pyi
--rw-r--r--   0        0        0     4656 2024-03-29 03:22:58.000000 unxt-0.8.1/src/unxt/experimental.py
--rw-r--r--   0        0        0        0 2024-03-29 03:22:58.000000 unxt-0.8.1/src/unxt/py.typed
--rw-r--r--   0        0        0      404 2024-03-29 03:22:58.000000 unxt-0.8.1/src/unxt/unitsystems/__init__.py
--rw-r--r--   0        0        0     4351 2024-03-29 03:22:58.000000 unxt-0.8.1/src/unxt/unitsystems/_base.py
--rw-r--r--   0        0        0     2849 2024-03-29 03:22:58.000000 unxt-0.8.1/src/unxt/unitsystems/_core.py
--rw-r--r--   0        0        0      785 2024-03-29 03:22:58.000000 unxt-0.8.1/src/unxt/unitsystems/_realizations.py
--rw-r--r--   0        0        0     2705 2024-03-29 03:22:58.000000 unxt-0.8.1/src/unxt/unitsystems/_utils.py
--rw-r--r--   0        0        0       13 2024-03-29 03:22:58.000000 unxt-0.8.1/tests/__init__.py
--rw-r--r--   0        0        0      185 2024-03-29 03:22:58.000000 unxt-0.8.1/tests/test_package.py
--rw-r--r--   0        0        0      817 2024-03-29 03:22:58.000000 unxt-0.8.1/tests/test_plum.py
--rw-r--r--   0        0        0    12142 2024-03-29 03:22:58.000000 unxt-0.8.1/tests/test_quantity.py
--rw-r--r--   0        0        0     3716 2024-03-29 03:22:58.000000 unxt-0.8.1/tests/test_unitsystems.py
--rw-r--r--   0        0        0       13 2024-03-29 03:22:58.000000 unxt-0.8.1/tests/quaxed/__init__.py
--rw-r--r--   0        0        0    46354 2024-03-29 03:22:58.000000 unxt-0.8.1/tests/quaxed/test_array_api.py
--rw-r--r--   0        0        0      626 2024-03-29 03:22:58.000000 unxt-0.8.1/tests/quaxed/test_numpy.py
--rw-r--r--   0        0        0     2218 2024-03-29 03:22:58.000000 unxt-0.8.1/.gitignore
--rw-r--r--   0        0        0     1528 2024-03-29 03:22:58.000000 unxt-0.8.1/LICENSE
--rw-r--r--   0        0        0     1387 2024-03-29 03:22:58.000000 unxt-0.8.1/README.md
--rw-r--r--   0        0        0     5654 2024-03-29 03:22:58.000000 unxt-0.8.1/pyproject.toml
--rw-r--r--   0        0        0     5174 2024-03-29 03:22:58.000000 unxt-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0      366 2024-04-02 18:21:24.000000 unxt-0.9/.copier-answers.yml
+-rw-r--r--   0        0        0      125 2024-04-02 18:21:24.000000 unxt-0.9/.git_archival.txt
+-rw-r--r--   0        0        0       32 2024-04-02 18:21:24.000000 unxt-0.9/.gitattributes
+-rw-r--r--   0        0        0     2558 2024-04-02 18:21:24.000000 unxt-0.9/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      309 2024-04-02 18:21:24.000000 unxt-0.9/.readthedocs.yml
+-rw-r--r--   0        0        0      439 2024-04-02 18:21:24.000000 unxt-0.9/conftest.py
+-rw-r--r--   0        0        0     2809 2024-04-02 18:21:24.000000 unxt-0.9/noxfile.py
+-rw-r--r--   0        0        0     2389 2024-04-02 18:21:24.000000 unxt-0.9/.github/CONTRIBUTING.md
+-rw-r--r--   0        0        0      224 2024-04-02 18:21:24.000000 unxt-0.9/.github/dependabot.yml
+-rw-r--r--   0        0        0      668 2024-04-02 18:21:24.000000 unxt-0.9/.github/matchers/pylint.json
+-rw-r--r--   0        0        0     1540 2024-04-02 18:21:24.000000 unxt-0.9/.github/workflows/cd.yml
+-rw-r--r--   0        0        0     1630 2024-04-02 18:21:24.000000 unxt-0.9/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      862 2024-04-02 18:21:24.000000 unxt-0.9/docs/conf.py
+-rw-r--r--   0        0        0      191 2024-04-02 18:21:24.000000 unxt-0.9/docs/index.md
+-rw-r--r--   0        0        0      554 2024-04-02 18:21:24.000000 unxt-0.9/src/unxt/__init__.py
+-rw-r--r--   0        0        0      263 2024-04-02 18:21:24.000000 unxt-0.9/src/unxt/_typing.py
+-rw-r--r--   0        0        0      406 2024-04-02 18:21:24.000000 unxt-0.9/src/unxt/_version.py
+-rw-r--r--   0        0        0       82 2024-04-02 18:21:24.000000 unxt-0.9/src/unxt/_version.pyi
+-rw-r--r--   0        0        0     4692 2024-04-02 18:21:24.000000 unxt-0.9/src/unxt/experimental.py
+-rw-r--r--   0        0        0        0 2024-04-02 18:21:24.000000 unxt-0.9/src/unxt/py.typed
+-rw-r--r--   0        0        0      710 2024-04-02 18:21:24.000000 unxt-0.9/src/unxt/_quantity/__init__.py
+-rw-r--r--   0        0        0    15618 2024-04-02 18:21:24.000000 unxt-0.9/src/unxt/_quantity/base.py
+-rw-r--r--   0        0        0     3615 2024-04-02 18:21:24.000000 unxt-0.9/src/unxt/_quantity/base_parametric.py
+-rw-r--r--   0        0        0     1121 2024-04-02 18:21:24.000000 unxt-0.9/src/unxt/_quantity/compat.py
+-rw-r--r--   0        0        0     2938 2024-04-02 18:21:24.000000 unxt-0.9/src/unxt/_quantity/core.py
+-rw-r--r--   0        0        0     2570 2024-04-02 18:21:24.000000 unxt-0.9/src/unxt/_quantity/distance.py
+-rw-r--r--   0        0        0      569 2024-04-02 18:21:24.000000 unxt-0.9/src/unxt/_quantity/fast.py
+-rw-r--r--   0        0        0     3780 2024-04-02 18:21:24.000000 unxt-0.9/src/unxt/_quantity/functional.py
+-rw-r--r--   0        0        0     3375 2024-04-02 18:21:24.000000 unxt-0.9/src/unxt/_quantity/register_dispatches.py
+-rw-r--r--   0        0        0    90018 2024-04-02 18:21:24.000000 unxt-0.9/src/unxt/_quantity/register_primitives.py
+-rw-r--r--   0        0        0     1222 2024-04-02 18:21:24.000000 unxt-0.9/src/unxt/_quantity/utils.py
+-rw-r--r--   0        0        0      404 2024-04-02 18:21:24.000000 unxt-0.9/src/unxt/unitsystems/__init__.py
+-rw-r--r--   0        0        0     4407 2024-04-02 18:21:24.000000 unxt-0.9/src/unxt/unitsystems/_base.py
+-rw-r--r--   0        0        0     2849 2024-04-02 18:21:24.000000 unxt-0.9/src/unxt/unitsystems/_core.py
+-rw-r--r--   0        0        0      785 2024-04-02 18:21:24.000000 unxt-0.9/src/unxt/unitsystems/_realizations.py
+-rw-r--r--   0        0        0     2714 2024-04-02 18:21:24.000000 unxt-0.9/src/unxt/unitsystems/_utils.py
+-rw-r--r--   0        0        0       13 2024-04-02 18:21:24.000000 unxt-0.9/tests/__init__.py
+-rw-r--r--   0        0        0      185 2024-04-02 18:21:24.000000 unxt-0.9/tests/test_package.py
+-rw-r--r--   0        0        0      817 2024-04-02 18:21:24.000000 unxt-0.9/tests/test_plum.py
+-rw-r--r--   0        0        0    12184 2024-04-02 18:21:24.000000 unxt-0.9/tests/test_quantity.py
+-rw-r--r--   0        0        0     3716 2024-04-02 18:21:24.000000 unxt-0.9/tests/test_unitsystems.py
+-rw-r--r--   0        0        0       13 2024-04-02 18:21:24.000000 unxt-0.9/tests/quaxed/__init__.py
+-rw-r--r--   0        0        0    46419 2024-04-02 18:21:24.000000 unxt-0.9/tests/quaxed/test_array_api.py
+-rw-r--r--   0        0        0      626 2024-04-02 18:21:24.000000 unxt-0.9/tests/quaxed/test_numpy.py
+-rw-r--r--   0        0        0     2218 2024-04-02 18:21:24.000000 unxt-0.9/.gitignore
+-rw-r--r--   0        0        0     1528 2024-04-02 18:21:24.000000 unxt-0.9/LICENSE
+-rw-r--r--   0        0        0     1387 2024-04-02 18:21:24.000000 unxt-0.9/README.md
+-rw-r--r--   0        0        0     5690 2024-04-02 18:21:24.000000 unxt-0.9/pyproject.toml
+-rw-r--r--   0        0        0     5172 2024-04-02 18:21:24.000000 unxt-0.9/PKG-INFO
```

### Comparing `unxt-0.8.1/.pre-commit-config.yaml` & `unxt-0.9/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
   autoupdate_commit_msg: "chore: update pre-commit hooks"
   autofix_commit_msg: "style: pre-commit fixes"
 
 default_stages: [pre-commit, pre-push]
 
 repos:
   - repo: https://github.com/commitizen-tools/commitizen
-    rev: v3.20.0
+    rev: v3.21.3
     hooks:
       - id: commitizen
       # - id: commitizen-branch
       #   stages: [push]
 
   - repo: meta
     hooks:
@@ -39,22 +39,22 @@
     rev: "v1.10.0"
     hooks:
       - id: rst-backticks
       - id: rst-directive-colons
       - id: rst-inline-touching-normal
 
   - repo: https://github.com/python-jsonschema/check-jsonschema
-    rev: 0.28.0
+    rev: 0.28.1
     hooks:
       - id: check-dependabot
       - id: check-github-workflows
       - id: check-readthedocs
 
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: "v0.3.4"
+    rev: "v0.3.5"
     hooks:
       # Run the linter
       - id: ruff
         types_or: [python, pyi, jupyter]
         args: ["--fix", "--show-fixes"]
       # Run the formatter
       - id: ruff-format
```

### Comparing `unxt-0.8.1/noxfile.py` & `unxt-0.9/noxfile.py`

 * *Files identical despite different names*

### Comparing `unxt-0.8.1/.github/CONTRIBUTING.md` & `unxt-0.9/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `unxt-0.8.1/.github/matchers/pylint.json` & `unxt-0.9/.github/matchers/pylint.json`

 * *Files identical despite different names*

### Comparing `unxt-0.8.1/.github/workflows/cd.yml` & `unxt-0.9/.github/workflows/cd.yml`

 * *Files identical despite different names*

### Comparing `unxt-0.8.1/.github/workflows/ci.yml` & `unxt-0.9/.github/workflows/ci.yml`

 * *Files 0% similar despite different names*

```diff
@@ -62,8 +62,8 @@
 
       - name: Test package
         run: >-
           python -m pytest src docs tests -ra --cov --cov-report=xml
           --cov-report=term --durations=20
 
       - name: Upload coverage report
-        uses: codecov/codecov-action@v4.1.0
+        uses: codecov/codecov-action@v4.1.1
```

### Comparing `unxt-0.8.1/docs/conf.py` & `unxt-0.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `unxt-0.8.1/src/unxt/_base.py` & `unxt-0.9/src/unxt/_quantity/base.py`

 * *Files 15% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 def bool_op(op: Callable[[Any, Any], Any]) -> Callable[[Any, Any], Any]:
     # TODO: support operations on dimensionless quantities with array.
     def _op(self: "AbstractQuantity", other: Any) -> Shaped[Array, "..."]:
         if not isinstance(other, AbstractQuantity):
             return NotImplemented
 
         try:
-            other_value = other.to_value(self.unit)
+            other_value = other.to_units_value(self.unit)
         except UnitConversionError:
             return jnp.full(self.value.shape, fill_value=False, dtype=bool)
 
         return op(self.value, other_value)
 
     return _op
 
@@ -137,34 +137,77 @@
         cls: "type[AbstractQuantity]",
         value: ArrayLike,
         unit: Any,
         /,
         *,
         dtype: Any = None,
     ) -> "AbstractQuantity":
+        """Construct a `Quantity` from an array-like value and a unit.
+
+        Parameters
+        ----------
+        value : ArrayLike
+            The array-like value.
+        unit : Any
+            The unit of the value.
+
+        dtype : Any, optional
+            The data type of the array.
+
+        Returns
+        -------
+        AbstractQuantity
+
+        Examples
+        --------
+        For this example we'll use the `Quantity` class. The same applies to
+        any subclass of `AbstractQuantity`.
+
+        >>> import jax.numpy as jnp
+        >>> from unxt import Quantity
+
+        >>> x = jnp.array([1.0, 2, 3])
+        >>> Quantity.constructor(x, "m")
+        Quantity['length'](Array([1., 2., 3.], dtype=float32), unit='m')
+
+        """
         # Dispatch on both arguments.
         # Construct using the standard `__init__` method.
         return cls(xp.asarray(value, dtype=dtype), unit)
 
     @classmethod  # type: ignore[no-redef]
     @dispatcher
     def constructor(
         cls: "type[AbstractQuantity]", value: ArrayLike, *, unit: Any, dtype: Any = None
     ) -> "AbstractQuantity":
+        """Construct a `Quantity` from an array-like value and a unit kwarg.
+
+        This is a convenience method for constructing a `Quantity` when the
+        unit is given as a keyword argument. It is equivalent to calling
+        ``Quantity.constructor(value, unit)`` as positional arguments.
+        """
         # Dispatch on the `value` only. Dispatch to the full constructor.
         return cls.constructor(value, unit, dtype=dtype)
 
     @classmethod  # type: ignore[no-redef]
     @dispatcher
     def constructor(
         cls: "type[AbstractQuantity]", *, value: ArrayLike, unit: Any, dtype: Any = None
     ) -> "AbstractQuantity":
+        """Construct a `Quantity` from value and unit kwargs.
+
+        This is a convenience method for constructing a `Quantity` when both the
+        value and the unit are given as a keyword arguments. It is equivalent to
+        calling ``Quantity.constructor(value, unit)`` as positional arguments.
+        """
         # Dispatched on no argument. Dispatch to the full constructor.
         return cls.constructor(value, unit, dtype=dtype)
 
+    # See below for additional constructors.
+
     # ===============================================================
     # Quax
 
     @property
     def shape(self) -> tuple[int, ...]:
         """Shape of the array."""
         return self.value.shape
@@ -176,31 +219,87 @@
     def aval(self) -> jax.core.ShapedArray:
         return jax.core.get_aval(self.value)
 
     def enable_materialise(self, _: bool = True) -> Self:  # noqa: FBT001, FBT002
         return replace(self, value=self.value, unit=self.unit)
 
     # ===============================================================
-    # Quantity
+    # Quantity API
 
-    def to(self, units: Unit) -> "AbstractQuantity":
+    def to_units(self, units: Unit) -> "AbstractQuantity":
+        """Convert the quantity to the given units.
+
+        Parameters
+        ----------
+        units : Unit
+            The units to convert to.
+
+        Returns
+        -------
+        AbstractQuantity
+
+        Examples
+        --------
+        >>> from unxt import Quantity
+
+        >>> q = Quantity(1, "m")
+        >>> q.to_units("cm")
+        Quantity['length'](Array(100., dtype=float32, ...), unit='cm')
+
+        """
         return replace(self, value=self.value * self.unit.to(units), unit=units)
 
-    def to_value(self, units: Unit) -> ArrayLike:
+    def to_units_value(self, units: Unit) -> ArrayLike:
+        """Return the value in the given units.
+
+        Parameters
+        ----------
+        units : Unit
+            The units to convert to.
+
+        Returns
+        -------
+        ArrayLike
+
+        Examples
+        --------
+        >>> from unxt import Quantity
+
+        >>> q = Quantity(1, "m")
+        >>> q.to_units_value("cm")
+        Array(100., dtype=float32, weak_type=True)
+
+        """
         if units == self.unit:
             return self.value
         return self.value * self.unit.to(units)  # TODO: allow affine transforms
 
     def decompose(self, bases: Sequence[Unit]) -> "AbstractQuantity":
         """Decompose the quantity into the given bases."""
         du = self.unit.decompose(bases)  # decomposed units
         base_units = CompositeUnit(scale=1, bases=du.bases, powers=du.powers)
         return replace(self, value=self.value * du.scale, unit=base_units)
 
     # ===============================================================
+    # Astropy Quantity API
+
+    def to(self, units: Unit) -> "AbstractQuantity":
+        """Convert the quantity to the given units.
+
+        See :meth:`AbstractQuantity.to_units`.
+        """
+        return self.to_units(units)
+
+    def to_value(self, units: Unit) -> ArrayLike:
+        """Return the value in the given units.
+
+        See :meth:`AbstractQuantity.to_units_value`.
+        """
+
+    # ===============================================================
     # Array API
 
     def __array_namespace__(self, *, api_version: Any = None) -> "ArrayAPINamespace":
         return xp
 
     def __getitem__(self, key: Any) -> "AbstractQuantity":
         return replace(self, value=self.value[key])
@@ -300,15 +399,15 @@
         if not isinstance(other, AbstractQuantity):
             return NotImplemented
 
         if not can_convert_unit(other.unit, self.unit):
             raise UnitConversionError
 
         # TODO: figure out how to defer to quaxed (e.g. quaxed.operator.mod)
-        return replace(self, value=self.value % other.to_value(self.unit))
+        return replace(self, value=self.value % other.to_units_value(self.unit))
 
     # ===============================================================
     # Python stuff
 
     def __hash__(self) -> int:
         """Hash the object as the tuple of its field values.
 
@@ -350,31 +449,40 @@
     /,
     *,
     dtype: Any = None,
 ) -> AbstractQuantity:
     """Construct a `Quantity` from another `Quantity`.
 
     The `value` is converted to the new `unit`.
+
+    Examples
+    --------
+    >>> from unxt import Quantity
+
+    >>> q = Quantity(1, "m")
+    >>> Quantity.constructor(q, "cm")
+    Quantity['length'](Array(100., dtype=float32, ...), unit='cm')
+
     """
-    value = xp.asarray(value.to(unit), dtype=dtype)
+    value = xp.asarray(value.to_units(unit), dtype=dtype)
     return cls(value.value, unit)
 
 
 @AbstractQuantity.constructor._f.register  # type: ignore[no-redef] # noqa: SLF001
 def constructor(
     cls: type[AbstractQuantity],
     value: AbstractQuantity,
     /,
     *,
     unit: Any | None = None,
     dtype: Any = None,
 ) -> AbstractQuantity:
     """Construct a `Quantity` from another `Quantity`, with no unit change."""
     unit = value.unit if unit is None else unit
-    value = xp.asarray(value.to(unit), dtype=dtype)
+    value = xp.asarray(value.to_units(unit), dtype=dtype)
     return cls(value.value, unit)
 
 
 @AbstractQuantity.constructor._f.register  # type: ignore[no-redef] # noqa: SLF001
 def constructor(
     cls: type[AbstractQuantity], value: AstropyQuantity, *, dtype: Any = None
 ) -> AbstractQuantity:
```

### Comparing `unxt-0.8.1/src/unxt/_compat.py` & `unxt-0.9/src/unxt/_quantity/compat.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 
 __all__: list[str] = []
 
 
 from astropy.units import Quantity as AstropyQuantity
 from plum import conversion_method
 
-from ._base import AbstractQuantity
-from ._core import Quantity
-from ._fast import UncheckedQuantity
+from .base import AbstractQuantity
+from .core import Quantity
+from .fast import UncheckedQuantity
 
 
 @conversion_method(type_from=AbstractQuantity, type_to=AstropyQuantity)  # type: ignore[misc]
 def convert_quantity_to_astropyquantity(obj: AbstractQuantity, /) -> AstropyQuantity:
     """`AbstractQuantity` -> `astropy.AbstractQuantity`."""
     return AstropyQuantity(obj.value, obj.unit)
```

### Comparing `unxt-0.8.1/src/unxt/_distance.py` & `unxt-0.9/src/unxt/_quantity/distance.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 
 import astropy.units as u
 from plum import add_conversion_method, add_promotion_rule
 
 import quaxed.array_api as xp
 import quaxed.numpy as qnp
 
-from ._base import AbstractQuantity
-from ._core import Quantity
+from .base import AbstractQuantity
+from .core import Quantity
 
 FMT = TypeVar("FMT")
 
 parallax_base_length = Quantity(1, "AU")
 distance_modulus_base_distance = Quantity(10, "pc")
 length_dimension = u.get_physical_type("length")
```

### Comparing `unxt-0.8.1/src/unxt/_fast.py` & `unxt-0.9/src/unxt/_quantity/fast.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # pylint: disable=import-error, no-member, unsubscriptable-object
 #    b/c it doesn't understand dataclass fields
 
 __all__ = ["UncheckedQuantity"]
 
 from typing import Any
 
-from ._base import AbstractQuantity
+from .base import AbstractQuantity
 
 
 class UncheckedQuantity(AbstractQuantity):
     """A fast implementation of the Quantity class.
 
     This class is not parametrized by its dimensionality.
     """
```

### Comparing `unxt-0.8.1/src/unxt/_register_dispatches.py` & `unxt-0.9/src/unxt/_quantity/register_dispatches.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 import jax.core
 import jax.experimental.array_api as jax_xp
 from jax import Device
 
 from quaxed.array_api._dispatch import dispatcher as dispatcher_
 from quaxed.array_api._types import DType
 
-from ._base import AbstractQuantity
-from ._core import Quantity
-from ._utils import type_unparametrized as type_np
+from .base import AbstractQuantity
+from .core import Quantity
+from .utils import type_unparametrized as type_np
 
 T = TypeVar("T")
 
 
 def dispatcher(f: T) -> T:  # TODO: figure out mypy stub issue.
     """Dispatcher that makes mypy happy."""
     return dispatcher_(f)
@@ -34,16 +34,16 @@
     dtype: Any = None,
     device: Any = None,
 ) -> Quantity:
     unit = start.unit
     return Quantity(
         jax_xp.arange(
             start.value,
-            stop=stop.to_value(unit) if stop is not None else None,
-            step=step.to_value(unit) if step is not None else None,
+            stop=stop.to_units_value(unit) if stop is not None else None,
+            step=step.to_units_value(unit) if step is not None else None,
             dtype=dtype,
             device=device,
         ),
         unit=unit,
     )
 
 
@@ -78,15 +78,15 @@
     x: AbstractQuantity,
     fill_value: AbstractQuantity,
     /,
     *,
     dtype: Any = None,
     device: Any = None,
 ) -> AbstractQuantity:
-    fill_val = fill_value.to_value(x.unit)
+    fill_val = fill_value.to_units_value(x.unit)
     return type_np(x)(
         jax_xp.full_like(x.value, fill_val, dtype=dtype, device=device), unit=x.unit
     )
 
 
 @dispatcher  # type: ignore[no-redef]
 def full_like(
@@ -114,16 +114,16 @@
     dtype: DType | None = None,
     device: Device | None = None,
     endpoint: bool = True,
 ) -> Quantity:
     unit = start.unit
     return Quantity(
         jax_xp.linspace(
-            start.to_value(unit),
-            stop.to_value(unit),
+            start.to_units_value(unit),
+            stop.to_units_value(unit),
             num=num,
             dtype=dtype,
             device=device,
             endpoint=endpoint,
         ),
         unit=unit,
     )
```

### Comparing `unxt-0.8.1/src/unxt/_register_primitives.py` & `unxt-0.9/src/unxt/_quantity/register_primitives.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,32 +21,37 @@
 from jax._src.lax.slicing import GatherDimensionNumbers, GatherScatterMode
 from jax._src.typing import Shape
 from jax.core import Primitive
 from jaxtyping import Array, ArrayLike
 from plum import promote
 from quax import register as register_
 
-from ._base import AbstractQuantity, can_convert_unit
-from ._core import AbstractParametricQuantity, Quantity
-from ._distance import Distance
-from ._utils import type_unparametrized as type_np
+from .base import AbstractQuantity, can_convert_unit
+from .base_parametric import AbstractParametricQuantity
+from .core import Quantity
+from .distance import Distance
+from .utils import type_unparametrized as type_np
 
 T = TypeVar("T")
 
 Axes: TypeAlias = tuple[int, ...]
 UnitClasses: TypeAlias = UnitBase
 
 
 def register(primitive: Primitive) -> Callable[[T], T]:
     """:func`quax.register`, but makes mypy happy."""
     return register_(primitive)
 
 
 def _to_value_rad_or_one(q: AbstractQuantity) -> ArrayLike:
-    return q.to_value(radian) if can_convert_unit(q.unit, radian) else q.to_value(one)
+    return (
+        q.to_units_value(radian)
+        if can_convert_unit(q.unit, radian)
+        else q.to_units_value(one)
+    )
 
 
 ################################################################################
 # Registering Primitives
 
 # ==============================================================================
 
@@ -93,15 +98,15 @@
 
     >>> from unxt import Quantity
     >>> q = Quantity(-1, "")
     >>> xp.acos(q)
     Quantity['angle'](Array(3.1415927, dtype=float32), unit='rad')
 
     """
-    x_ = x.to_value(one)
+    x_ = x.to_units_value(one)
     return type_np(x)(value=lax.acos(x_), unit=radian)
 
 
 # ==============================================================================
 
 
 @register(lax.acosh_p)
@@ -118,15 +123,15 @@
 
     >>> from unxt import Quantity
     >>> q = Quantity(2.0, "")
     >>> xp.acosh(q)
     Quantity['angle'](Array(1.316958, dtype=float32), unit='rad')
 
     """
-    x_ = x.to_value(one)
+    x_ = x.to_units_value(one)
     return type_np(x)(value=lax.acosh(x_), unit=radian)
 
 
 # ==============================================================================
 # Addition
 
 
@@ -151,15 +156,15 @@
     >>> q2 = Quantity(500.0, "m")
     >>> xp.add(q1, q2)
     Quantity['length'](Array(1.5, dtype=float32), unit='km')
     >>> q1 + q2
     Quantity['length'](Array(1.5, dtype=float32, weak_type=True), unit='km')
 
     """
-    return replace(x, value=lax.add(x.value, y.to_value(x.unit)))
+    return replace(x, value=lax.add(x.value, y.to_units_value(x.unit)))
 
 
 @register(lax.add_p)
 def _add_p_vaq(x: ArrayLike, y: AbstractQuantity) -> AbstractQuantity:
     """Add a value and a quantity.
 
     Examples
@@ -191,15 +196,15 @@
     >>> xp.add(x1, q2)
     Quantity['dimensionless'](Array(600., dtype=float32), unit='')
     >>> x1 + q2
     Quantity['dimensionless'](Array(600., dtype=float32, weak_type=True), unit='')
 
     """
     y = eqx.error_if(y, y.unit != one, "Cannot add a non-quantity and quantity.")
-    return replace(y, value=lax.add(x, y.to_value(one)))
+    return replace(y, value=lax.add(x, y.to_units_value(one)))
 
 
 @register(lax.add_p)
 def _add_p_aqv(x: AbstractQuantity, y: ArrayLike) -> AbstractQuantity:
     """Add a quantity and a value.
 
     Examples
@@ -235,15 +240,15 @@
     >>> xp.add(q1, y)
     Quantity[...](Array(600., dtype=float32), unit='')
     >>> q1 + y
     Quantity[...](Array(600., dtype=float32, weak_type=True), unit='')
 
     """
     x = eqx.error_if(x, x.unit != one, "Cannot add a quantity and a non-quantity.")
-    return replace(x, value=lax.add(x.to_value(one), y))
+    return replace(x, value=lax.add(x.to_units_value(one), y))
 
 
 # ==============================================================================
 
 
 @register(add_any_p)
 def _add_any_p(
@@ -296,15 +301,15 @@
     >>> from unxt import Quantity
     >>> x1 = Quantity(1, "")
     >>> x2 = Quantity(2, "")
     >>> xp.bitwise_and(x1, x2)
     Array(0, dtype=int32)
 
     """
-    return lax.and_p.bind(x1.to_value(one), x2.to_value(one))
+    return lax.and_p.bind(x1.to_units_value(one), x2.to_units_value(one))
 
 
 # ==============================================================================
 
 
 @register(lax.approx_top_k_p)
 def _approx_top_k_p() -> AbstractQuantity:
@@ -375,15 +380,15 @@
     >>> import quaxed.array_api as xp
     >>> from unxt import UncheckedQuantity
     >>> q = UncheckedQuantity(1, "")
     >>> xp.asin(q)
     UncheckedQuantity(Array(1.5707964, dtype=float32), unit='rad')
 
     """
-    return type_np(x)(lax.asin(x.to_value(one)), unit=radian)
+    return type_np(x)(lax.asin(x.to_units_value(one)), unit=radian)
 
 
 @register(lax.asin_p)
 def _asin_p_q(
     x: AbstractParametricQuantity["dimensionless"],
 ) -> AbstractParametricQuantity["angle"]:
     """Inverse sine of a quantity.
@@ -393,15 +398,15 @@
     >>> import quaxed.array_api as xp
     >>> from unxt import Quantity
     >>> q = Quantity(1, "")
     >>> xp.asin(q)
     Quantity['angle'](Array(1.5707964, dtype=float32), unit='rad')
 
     """
-    return type_np(x)(lax.asin(x.to_value(one)), unit=radian)
+    return type_np(x)(lax.asin(x.to_units_value(one)), unit=radian)
 
 
 # ==============================================================================
 
 
 @register(lax.asinh_p)
 def _asinh_p_aq(x: AbstractQuantity) -> AbstractQuantity:
@@ -412,15 +417,15 @@
     >>> import quaxed.array_api as xp
     >>> from unxt import UncheckedQuantity
     >>> q = UncheckedQuantity(2, "")
     >>> xp.asinh(q)
     UncheckedQuantity(Array(1.4436355, dtype=float32), unit='rad')
 
     """
-    return type_np(x)(lax.asinh(x.to_value(one)), unit=radian)
+    return type_np(x)(lax.asinh(x.to_units_value(one)), unit=radian)
 
 
 @register(lax.asinh_p)
 def _asinh_p_q(
     x: AbstractParametricQuantity["dimensionless"],
 ) -> AbstractParametricQuantity["angle"]:
     """Inverse hyperbolic sine of a quantity.
@@ -430,15 +435,15 @@
     >>> import quaxed.array_api as xp
     >>> from unxt import Quantity
     >>> q = Quantity(2, "")
     >>> xp.asinh(q)
     Quantity['angle'](Array(1.4436355, dtype=float32), unit='rad')
 
     """
-    return type_np(x)(lax.asinh(x.to_value(one)), unit=radian)
+    return type_np(x)(lax.asinh(x.to_units_value(one)), unit=radian)
 
 
 # ==============================================================================
 
 
 @register(lax.atan2_p)
 def _atan2_p_aqaq(x: AbstractQuantity, y: AbstractQuantity) -> AbstractQuantity:
@@ -451,15 +456,15 @@
     >>> q1 = UncheckedQuantity(1, "m")
     >>> q2 = UncheckedQuantity(3, "m")
     >>> xp.atan2(q1, q2)
     UncheckedQuantity(Array(0.32175055, dtype=float32), unit='rad')
 
     """
     x, y = promote(x, y)  # e.g. Distance -> Quantity
-    y_ = y.to_value(x.unit)
+    y_ = y.to_units_value(x.unit)
     return type_np(x)(lax.atan2(x.value, y_), unit=radian)
 
 
 @register(lax.atan2_p)
 def _atan2_p_qq(
     x: AbstractParametricQuantity, y: AbstractParametricQuantity
 ) -> AbstractParametricQuantity["radian"]:
@@ -472,15 +477,15 @@
     >>> q1 = Quantity(1, "m")
     >>> q2 = Quantity(3, "m")
     >>> xp.atan2(q1, q2)
     Quantity['angle'](Array(0.32175055, dtype=float32), unit='rad')
 
     """
     x, y = promote(x, y)  # e.g. Distance -> Quantity
-    y_ = y.to_value(x.unit)
+    y_ = y.to_units_value(x.unit)
     return type_np(x)(lax.atan2(x.value, y_), unit=radian)
 
 
 # ---------------------------
 
 
 @register(lax.atan2_p)
@@ -493,15 +498,15 @@
     >>> from unxt import UncheckedQuantity
     >>> x1 = xp.asarray(1.0)
     >>> q2 = UncheckedQuantity(3.0, "")
     >>> xp.atan2(x1, q2)
     UncheckedQuantity(Array(0.32175055, dtype=float32), unit='rad')
 
     """
-    y_ = y.to_value(one)
+    y_ = y.to_units_value(one)
     return type_np(y)(lax.atan2(x, y_), unit=radian)
 
 
 @register(lax.atan2_p)
 def _atan2_p_vq(
     x: ArrayLike, y: AbstractParametricQuantity["dimensionless"]
 ) -> AbstractParametricQuantity["angle"]:
@@ -513,15 +518,15 @@
     >>> from unxt import Quantity
     >>> x1 = xp.asarray(1.0)
     >>> q2 = Quantity(3.0, "")
     >>> xp.atan2(x1, q2)
     Quantity['angle'](Array(0.32175055, dtype=float32), unit='rad')
 
     """
-    y_ = y.to_value(one)
+    y_ = y.to_units_value(one)
     return Quantity(lax.atan2(x, y_), unit=radian)
 
 
 # ---------------------------
 
 
 @register(lax.atan2_p)
@@ -534,15 +539,15 @@
     >>> from unxt import UncheckedQuantity
     >>> q1 = UncheckedQuantity(1.0, "")
     >>> x2 = xp.asarray(3.0)
     >>> xp.atan2(q1, x2)
     UncheckedQuantity(Array(0.32175055, dtype=float32), unit='rad')
 
     """
-    x_ = x.to_value(one)
+    x_ = x.to_units_value(one)
     return type_np(x)(lax.atan2(x_, y), unit=radian)
 
 
 @register(lax.atan2_p)
 def _atan2_p_qv(
     x: AbstractParametricQuantity["dimensionless"], y: ArrayLike
 ) -> AbstractParametricQuantity["angle"]:
@@ -554,15 +559,15 @@
     >>> from unxt import Quantity
     >>> q1 = Quantity(1.0, "")
     >>> x2 = xp.asarray(3.0)
     >>> xp.atan2(q1, x2)
     Quantity['angle'](Array(0.32175055, dtype=float32), unit='rad')
 
     """
-    x_ = x.to_value(one)
+    x_ = x.to_units_value(one)
     return type_np(x)(lax.atan2(x_, y), unit=radian)
 
 
 # ==============================================================================
 
 
 @register(lax.atan_p)
@@ -574,15 +579,15 @@
     >>> import quaxed.array_api as xp
     >>> from unxt import UncheckedQuantity
     >>> q = UncheckedQuantity(1, "")
     >>> xp.atan(q)
     UncheckedQuantity(Array(0.7853982, dtype=float32), unit='rad')
 
     """
-    return type_np(x)(lax.atan(x.to_value(one)), unit=radian)
+    return type_np(x)(lax.atan(x.to_units_value(one)), unit=radian)
 
 
 @register(lax.atan_p)
 def _atan_p_q(
     x: AbstractParametricQuantity["dimensionless"],
 ) -> AbstractParametricQuantity["angle"]:
     """Arctangent of a quantity.
@@ -592,15 +597,15 @@
     >>> import quaxed.array_api as xp
     >>> from unxt import Quantity
     >>> q = Quantity(1, "")
     >>> xp.atan(q)
     Quantity['angle'](Array(0.7853982, dtype=float32), unit='rad')
 
     """
-    return Quantity(lax.atan(x.to_value(one)), unit=radian)
+    return Quantity(lax.atan(x.to_units_value(one)), unit=radian)
 
 
 # ==============================================================================
 
 
 @register(lax.atanh_p)
 def _atanh_p_aq(x: AbstractQuantity) -> AbstractQuantity:
@@ -611,15 +616,15 @@
     >>> import quaxed.array_api as xp
     >>> from unxt import UncheckedQuantity
     >>> q = UncheckedQuantity(2, "")
     >>> xp.atanh(q)
     UncheckedQuantity(Array(nan, dtype=float32), unit='rad')
 
     """
-    return type_np(x)(lax.atanh(x.to_value(one)), unit=radian)
+    return type_np(x)(lax.atanh(x.to_units_value(one)), unit=radian)
 
 
 @register(lax.atanh_p)
 def _atanh_p_q(
     x: AbstractParametricQuantity["dimensionless"],
 ) -> AbstractParametricQuantity["angle"]:
     """Inverse hyperbolic tangent of a quantity.
@@ -629,15 +634,15 @@
     >>> import quaxed.array_api as xp
     >>> from unxt import Quantity
     >>> q = Quantity(2, "")
     >>> xp.atanh(q)
     Quantity['angle'](Array(nan, dtype=float32), unit='rad')
 
     """
-    return type_np(x)(lax.atanh(x.to_value(one)), unit=radian)
+    return type_np(x)(lax.atanh(x.to_units_value(one)), unit=radian)
 
 
 # ==============================================================================
 
 
 @register(lax.axis_index_p)
 def _axis_index_p() -> AbstractQuantity:
@@ -775,17 +780,17 @@
     >>> lax.clamp(min, q, max)
     Quantity['length'](Array([0, 1, 2], dtype=int32), unit='m')
 
     """
     return replace(
         x,
         value=lax.clamp(
-            min.to_value(x.unit),
+            min.to_units_value(x.unit),
             x.value,
-            max.to_value(x.unit),
+            max.to_units_value(x.unit),
         ),
     )
 
 
 # ---------------------------
 
 
@@ -811,15 +816,17 @@
     >>> min = xp.asarray(0)
     >>> max = Quantity(2, "")
     >>> q = Quantity([-1, 1, 3], "")
     >>> lax.clamp(min, q, max)
     Quantity['dimensionless'](Array([0, 1, 2], dtype=int32), unit='')
 
     """
-    return replace(x, value=lax.clamp(min, x.to_value(one), max.to_value(one)))
+    return replace(
+        x, value=lax.clamp(min, x.to_units_value(one), max.to_units_value(one))
+    )
 
 
 # ---------------------------
 
 
 @register(lax.clamp_p)
 def _clamp_p_aqvaq(
@@ -836,15 +843,15 @@
     >>> min = UncheckedQuantity(0, "")
     >>> max = UncheckedQuantity(2, "")
     >>> x = xp.asarray([-1, 1, 3])
     >>> lax.clamp(min, x, max)
     Array([0, 1, 2], dtype=int32)
 
     """
-    return lax.clamp(min.to_value(one), x, max.to_value(one))
+    return lax.clamp(min.to_units_value(one), x, max.to_units_value(one))
 
 
 @register(lax.clamp_p)
 def _clamp_p_qvq(
     min: AbstractParametricQuantity["dimensionless"],
     x: ArrayLike,
     max: AbstractParametricQuantity["dimensionless"],
@@ -860,15 +867,15 @@
     >>> min = Quantity(0, "")
     >>> max = Quantity(2, "")
     >>> x = xp.asarray([-1, 1, 3])
     >>> lax.clamp(min, x, max)
     Array([0, 1, 2], dtype=int32)
 
     """
-    return lax.clamp(min.to_value(one), x, max.to_value(one))
+    return lax.clamp(min.to_units_value(one), x, max.to_units_value(one))
 
 
 # ---------------------------
 
 
 @register(lax.clamp_p)
 def _clamp_p_aqaqv(
@@ -885,15 +892,17 @@
     >>> min = UncheckedQuantity(0, "")
     >>> max = xp.asarray(2)
     >>> q = UncheckedQuantity([-1, 1, 3], "")
     >>> lax.clamp(min, q, max)
     UncheckedQuantity(Array([0, 1, 2], dtype=int32), unit='')
 
     """
-    return replace(x, value=lax.clamp(min.to_value(one), x.to_value(one), max))
+    return replace(
+        x, value=lax.clamp(min.to_units_value(one), x.to_units_value(one), max)
+    )
 
 
 @register(lax.clamp_p)
 def _clamp_p_qqv(
     min: AbstractParametricQuantity["dimensionless"],
     x: AbstractParametricQuantity["dimensionless"],
     max: ArrayLike,
@@ -909,15 +918,17 @@
     >>> min = Quantity(0, "")
     >>> max = xp.asarray(2)
     >>> q = Quantity([-1, 1, 3], "")
     >>> lax.clamp(min, q, max)
     Quantity['dimensionless'](Array([0, 1, 2], dtype=int32), unit='')
 
     """
-    return replace(x, value=lax.clamp(min.to_value(one), x.to_value(one), max))
+    return replace(
+        x, value=lax.clamp(min.to_units_value(one), x.to_units_value(one), max)
+    )
 
 
 # ==============================================================================
 
 
 @register(lax.clz_p)
 def _clz_p() -> AbstractQuantity:
@@ -944,15 +955,15 @@
     >>> x = Quantity(1.0, "m")
     >>> y = Quantity(2.0, "m")
     >>> lax.complex(x, y)
     Quantity['length'](Array(1.+2.j, dtype=complex64, weak_type=True), unit='m')
 
     """
     x, y = promote(x, y)  # e.g. Distance -> Quantity
-    y_ = y.to_value(x.unit)
+    y_ = y.to_units_value(x.unit)
     return replace(x, value=lax.complex(x.value, y_))
 
 
 # ==============================================================================
 # Concatenation
 
 
@@ -978,15 +989,15 @@
 
     """
     operand0 = operands[0]
     units = operand0.unit
     return replace(
         operand0,
         value=lax.concatenate(
-            [op.to_value(units) for op in operands], dimension=dimension
+            [op.to_units_value(units) for op in operands], dimension=dimension
         ),
     )
 
 
 # ---------------------------
 
 
@@ -1012,15 +1023,15 @@
                          [ 0.        ,  0.        ,  1.        ]], dtype=float32),
                   unit='')
 
     """
     return type_np(operand0)(
         lax.concatenate(
             [
-                (op.to_value(one) if hasattr(op, "unit") else op)
+                (op.to_units_value(one) if hasattr(op, "unit") else op)
                 for op in (operand0, *operands)
             ],
             dimension=dimension,
         ),
         unit=one,
     )
 
@@ -1047,15 +1058,15 @@
                          [ 0.        ,  0.70710677,  0.70710677]], dtype=float32),
                   unit='')
 
     """
     return Quantity(
         lax.concatenate(
             [
-                (op.to_value(one) if hasattr(op, "unit") else op)
+                (op.to_units_value(one) if hasattr(op, "unit") else op)
                 for op in (operand0, *operands)
             ],
             dimension=dimension,
         ),
         unit=one,
     )
 
@@ -1350,15 +1361,15 @@
     >>> q = Quantity([1, 2, 3], "")
     >>> lax.cumprod(q)
     Quantity['dimensionless'](Array([1, 2, 6], dtype=int32), unit='')
 
     """
     return replace(
         operand,
-        value=lax.cumprod(operand.to_value(one), axis=axis, reverse=reverse),
+        value=lax.cumprod(operand.to_units_value(one), axis=axis, reverse=reverse),
     )
 
 
 # ==============================================================================
 
 
 @register(lax.cumsum_p)
@@ -1428,15 +1439,15 @@
 
     >>> from unxt import Quantity
     >>> q = Quantity(1.0, "")
     >>> lax.digamma(q)
     Quantity['dimensionless'](Array(-0.5772154, dtype=float32, weak_type=True), unit='')
 
     """
-    return replace(x, value=lax.digamma(x.to_value(one)))
+    return replace(x, value=lax.digamma(x.to_units_value(one)))
 
 
 # ==============================================================================
 # Division
 
 
 @register(lax.div_p)
@@ -1739,15 +1750,15 @@
     >>> q2 = Quantity(1, "m")
     >>> xp.equal(q1, q2)
     Array(True, dtype=bool)
     >>> q1 == q2
     Array(True, dtype=bool, weak_type=True)
 
     """
-    return lax.eq(x.value, y.to_value(x.unit))
+    return lax.eq(x.value, y.to_units_value(x.unit))
 
 
 @register(lax.eq_p)
 def _eq_p_vq(x: ArrayLike, y: AbstractQuantity) -> ArrayLike:
     """Equality of an array and a quantity.
 
     Examples
@@ -1762,15 +1773,15 @@
 
     >>> from unxt import Quantity
     >>> q = Quantity(2.0, "")
     >>> xp.equal(x, q)
     Array([False,  True, False], dtype=bool)
 
     """
-    return lax.eq(x, y.to_value(one))
+    return lax.eq(x, y.to_units_value(one))
 
 
 @register(lax.eq_p)
 def _eq_p_aqv(x: AbstractQuantity, y: ArrayLike) -> ArrayLike:
     """Equality of an array and a quantity.
 
     Examples
@@ -1797,15 +1808,15 @@
     False
 
     """
     # TODO: better support for jit
     if not y.shape and (y in (0, jnp.inf)):
         return lax.eq(x.value, y)
 
-    return lax.eq(x.to_value(one), y)
+    return lax.eq(x.to_units_value(one), y)
 
 
 @register(lax.eq_p)
 def _eq_p_aq0(x: AbstractQuantity, y: float | int) -> ArrayLike:
     """Equality of a quantity and 0."""
     y = eqx.error_if(
         y,
@@ -1842,15 +1853,15 @@
     >>> from unxt import Quantity
     >>> q = Quantity(0.5, "")
     >>> lax.erf_inv(q)
     Quantity['dimensionless'](Array(0.47693628, dtype=float32, ...), unit='')
 
     """
     # TODO: can this support non-dimensionless quantities?
-    return replace(x, value=lax.erf_inv(x.to_value(one)))
+    return replace(x, value=lax.erf_inv(x.to_units_value(one)))
 
 
 # ==============================================================================
 
 
 @register(lax.erf_p)
 def _erf_p(x: AbstractQuantity) -> AbstractQuantity:
@@ -1869,15 +1880,15 @@
     >>> from unxt import Quantity
     >>> q = Quantity(0.5, "")
     >>> lax.erf(q)
     Quantity['dimensionless'](Array(0.5204999, dtype=float32, ...), unit='')
 
     """
     # TODO: can this support non-dimensionless quantities?
-    return replace(x, value=lax.erf(x.to_value(one)))
+    return replace(x, value=lax.erf(x.to_units_value(one)))
 
 
 # ==============================================================================
 
 
 @register(lax.erfc_p)
 def _erfc_p(x: AbstractQuantity) -> AbstractQuantity:
@@ -1895,15 +1906,15 @@
     >>> from unxt import Quantity
     >>> q = Quantity(0.5, "")
     >>> lax.erfc(q)
     Quantity['dimensionless'](Array(0.47950017, dtype=float32, ...), unit='')
 
     """
     # TODO: can this support non-dimensionless quantities?
-    return replace(x, value=lax.erfc(x.to_value(one)))
+    return replace(x, value=lax.erfc(x.to_units_value(one)))
 
 
 # ==============================================================================
 
 
 @register(lax.exp2_p)
 def _exp2_p(x: AbstractQuantity) -> AbstractQuantity:
@@ -1920,15 +1931,15 @@
 
     >>> from unxt import Quantity
     >>> q = Quantity(3, "")
     >>> jnp.exp2(q)
     Quantity['dimensionless'](Array(8., dtype=float32), unit='')
 
     """
-    return replace(x, value=lax.exp2(x.to_value(one)))
+    return replace(x, value=lax.exp2(x.to_units_value(one)))
 
 
 # ==============================================================================
 
 
 @register(lax.exp_p)
 def _exp_p(x: AbstractQuantity) -> AbstractQuantity:
@@ -1953,15 +1964,15 @@
     >>> xp.exp(Quantity(xp.pi * 1j, "")) + 1
     Quantity['dimensionless'](Array(0.-8.742278e-08j, dtype=complex64), unit='')
 
     Pretty close to zero!
 
     """
     # TODO: more meaningful error message.
-    return replace(x, value=lax.exp(x.to_value(one)))
+    return replace(x, value=lax.exp(x.to_units_value(one)))
 
 
 # ==============================================================================
 
 
 @register(lax.expm1_p)
 def _expm1_p(x: AbstractQuantity) -> AbstractQuantity:
@@ -1978,15 +1989,15 @@
 
     >>> from unxt import Quantity
     >>> q = Quantity(0, "")
     >>> xp.expm1(q)
     Quantity['dimensionless'](Array(0., dtype=float32), unit='')
 
     """
-    return replace(x, value=lax.expm1(x.to_value(one)))
+    return replace(x, value=lax.expm1(x.to_units_value(one)))
 
 
 # ==============================================================================
 
 
 @register(lax.fft_p)
 def _fft_p(x: AbstractQuantity, *, fft_type: Any, fft_lengths: Any) -> AbstractQuantity:
@@ -2008,15 +2019,15 @@
     Quantity['dimensionless'](Array([ 6. +0.j       , -1.5+0.8660254j, -1.5-0.8660254j],
                                     dtype=complex64), unit='')
 
     """
     # TODO: what units can this support?
     return replace(
         x,
-        value=lax.fft(x.to_value(one), fft_type, fft_lengths),
+        value=lax.fft(x.to_units_value(one), fft_type, fft_lengths),
     )
 
 
 # ==============================================================================
 
 
 @register(lax.floor_p)
@@ -2097,15 +2108,15 @@
     >>> q2 = Quantity(1., "km")
     >>> xp.greater_equal(q1, q2)
     Array(True, dtype=bool)
     >>> q1 >= q2
     Array(True, dtype=bool, weak_type=True)
 
     """
-    return lax.ge(x.value, y.to_value(x.unit))
+    return lax.ge(x.value, y.to_units_value(x.unit))
 
 
 @register(lax.ge_p)
 def _ge_p_vq(x: ArrayLike, y: AbstractQuantity) -> ArrayLike:
     """Greater than or equal to of an array and a quantity.
 
     Examples
@@ -2121,15 +2132,15 @@
 
     >>> from unxt import Quantity
     >>> q2 = Quantity(1., "")
     >>> xp.greater_equal(x, q2)
     Array(True, dtype=bool)
 
     """
-    return lax.ge(x, y.to_value(one))
+    return lax.ge(x, y.to_units_value(one))
 
 
 @register(lax.ge_p)
 def _ge_p_qv(x: AbstractQuantity, y: ArrayLike) -> ArrayLike:
     """Greater than or equal to of a quantity and an array.
 
     Examples
@@ -2147,15 +2158,15 @@
     >>> q1 = Quantity(1., "")
     >>> xp.greater_equal(q1, y)
     Array(True, dtype=bool)
 
     """
     # if jnp.array_equal(y, 0):
     #     return lax.ge(x.value, y)
-    return lax.ge(x.to_value(one), y)
+    return lax.ge(x.to_units_value(one), y)
 
 
 # ==============================================================================
 
 
 @register(lax.gt_p)
 def _gt_p_qq(x: AbstractQuantity, y: AbstractQuantity) -> ArrayLike:
@@ -2174,15 +2185,15 @@
     >>> from unxt import Quantity
     >>> q1 = Quantity(1_001., "m")
     >>> q2 = Quantity(1., "km")
     >>> xp.greater_equal(q1, q2)
     Array(True, dtype=bool)
 
     """
-    return lax.gt(x.value, y.to_value(x.unit))
+    return lax.gt(x.value, y.to_units_value(x.unit))
 
 
 @register(lax.gt_p)
 def _gt_p_vq(x: ArrayLike, y: AbstractQuantity) -> ArrayLike:
     """Greater than of an array and a quantity.
 
     Examples
@@ -2198,15 +2209,15 @@
 
     >>> from unxt import Quantity
     >>> q2 = Quantity(1., "")
     >>> xp.greater_equal(x, q2)
     Array(True, dtype=bool)
 
     """
-    return lax.gt(x, y.to_value(one))
+    return lax.gt(x, y.to_units_value(one))
 
 
 @register(lax.gt_p)
 def _gt_p_qv(x: AbstractQuantity, y: ArrayLike) -> ArrayLike:
     """Greater than or equal to of a quantity and an array.
 
     Examples
@@ -2222,15 +2233,15 @@
 
     >>> from unxt import Quantity
     >>> q1 = Quantity(1., "")
     >>> xp.greater_equal(q1, y)
     Array(True, dtype=bool)
 
     """
-    return lax.gt(x.to_value(one), y)
+    return lax.gt(x.to_units_value(one), y)
 
 
 @register(lax.gt_p)
 def _gt_p_qi(x: AbstractQuantity, y: int) -> ArrayLike:
     """Greater than or equal to of a quantity and an array.
 
     Examples
@@ -2246,15 +2257,15 @@
 
     >>> from unxt import Quantity
     >>> q1 = Quantity(1., "")
     >>> jnp.greater(q1, y)
     Array(True, dtype=bool, weak_type=True)
 
     """
-    return lax.gt(x.to_value(one), y)
+    return lax.gt(x.to_units_value(one), y)
 
 
 # ==============================================================================
 
 
 @register(lax.igamma_grad_a_p)
 def _igamma_grad_a_p() -> AbstractQuantity:
@@ -2390,15 +2401,15 @@
     >>> from unxt import Quantity
     >>> q1 = Quantity(1_001., "m")
     >>> q2 = Quantity(1., "km")
     >>> xp.less_equal(q1, q2)
     Array(False, dtype=bool)
 
     """
-    return lax.le(x.value, y.to_value(x.unit))
+    return lax.le(x.value, y.to_units_value(x.unit))
 
 
 @register(lax.le_p)
 def _le_p_vq(x: ArrayLike, y: AbstractQuantity) -> ArrayLike:
     """Less than or equal to of an array and a quantity.
 
     Examples
@@ -2414,15 +2425,15 @@
 
     >>> from unxt import Quantity
     >>> q2 = Quantity(1., "")
     >>> xp.less_equal(x1, q2)
     Array(False, dtype=bool)
 
     """
-    return lax.le(x, y.to_value(one))
+    return lax.le(x, y.to_units_value(one))
 
 
 @register(lax.le_p)
 def _le_p_qv(x: AbstractQuantity, y: ArrayLike) -> ArrayLike:
     """Less than or equal to of a quantity and an array.
 
     Examples
@@ -2438,15 +2449,15 @@
 
     >>> from unxt import Quantity
     >>> q1 = Quantity(1., "")
     >>> xp.less_equal(q1, y1)
     Array(False, dtype=bool)
 
     """
-    return lax.le(x.to_value(one), y)
+    return lax.le(x.to_units_value(one), y)
 
 
 # ==============================================================================
 
 
 @register(lax.le_to_p)
 def _le_to_p() -> AbstractParametricQuantity:
@@ -2472,15 +2483,15 @@
     >>> from unxt import Quantity
     >>> q = Quantity(3, "")
     >>> jsp.special.gammaln(q)
     Quantity['dimensionless'](Array(0.6931474, dtype=float32), unit='')
 
     """
     # TODO: are there any units that this can support?
-    return replace(x, value=lax.lgamma(x.to_value(one)))
+    return replace(x, value=lax.lgamma(x.to_units_value(one)))
 
 
 # ==============================================================================
 
 
 @register(lax.linear_solve_p)
 def _linear_solve_p() -> AbstractQuantity:
@@ -2488,49 +2499,49 @@
 
 
 # ==============================================================================
 
 
 @register(lax.log1p_p)
 def _log1p_p(x: AbstractQuantity) -> AbstractQuantity:
-    return replace(x, value=lax.log1p(x.to_value(one)))
+    return replace(x, value=lax.log1p(x.to_units_value(one)))
 
 
 # ==============================================================================
 
 
 @register(lax.log_p)
 def _log_p(x: AbstractQuantity) -> AbstractQuantity:
-    return replace(x, value=lax.log(x.to_value(one)))
+    return replace(x, value=lax.log(x.to_units_value(one)))
 
 
 # ==============================================================================
 
 
 @register(lax.logistic_p)
 def _logistic_p(x: AbstractQuantity) -> AbstractQuantity:
-    return replace(x, value=lax.logistic(x.to_value(one)))
+    return replace(x, value=lax.logistic(x.to_units_value(one)))
 
 
 # ==============================================================================
 
 
 @register(lax.lt_p)
 def _lt_p_qq(x: AbstractQuantity, y: AbstractQuantity) -> ArrayLike:
-    return lax.lt(x.value, y.to_value(x.unit))
+    return lax.lt(x.value, y.to_units_value(x.unit))
 
 
 @register(lax.lt_p)
 def _lt_p_vq(x: ArrayLike, y: AbstractQuantity) -> ArrayLike:
-    return lax.lt(x, y.to_value(one))
+    return lax.lt(x, y.to_units_value(one))
 
 
 @register(lax.lt_p)
 def _lt_p_qv(x: AbstractQuantity, y: ArrayLike) -> ArrayLike:
-    return lax.lt(x.to_value(one), y)
+    return lax.lt(x.to_units_value(one), y)
 
 
 # ==============================================================================
 
 
 @register(lax.lt_to_p)
 def _lt_to_p() -> ArrayLike:
@@ -2538,43 +2549,43 @@
 
 
 # ==============================================================================
 
 
 @register(lax.max_p)
 def _max_p_qq(x: AbstractQuantity, y: AbstractQuantity) -> AbstractQuantity:
-    return replace(x, value=lax.max(x.value, y.to_value(x.unit)))
+    return replace(x, value=lax.max(x.value, y.to_units_value(x.unit)))
 
 
 @register(lax.max_p)
 def _max_p_vq(x: ArrayLike, y: AbstractQuantity) -> AbstractQuantity:
-    return replace(y, value=lax.max(x, y.to_value(one)))
+    return replace(y, value=lax.max(x, y.to_units_value(one)))
 
 
 @register(lax.max_p)
 def _max_p_qv(x: AbstractQuantity, y: ArrayLike) -> AbstractQuantity:
-    return replace(x, value=lax.max(x.to_value(one), y))
+    return replace(x, value=lax.max(x.to_units_value(one), y))
 
 
 # ==============================================================================
 
 
 @register(lax.min_p)
 def _min_p_qq(x: AbstractQuantity, y: AbstractQuantity) -> AbstractQuantity:
-    return replace(x, value=lax.min(x.value, y.to_value(x.unit)))
+    return replace(x, value=lax.min(x.value, y.to_units_value(x.unit)))
 
 
 @register(lax.min_p)
 def _min_p_vq(x: ArrayLike, y: AbstractQuantity) -> AbstractQuantity:
-    return replace(y, value=lax.min(x, y.to_value(one)))
+    return replace(y, value=lax.min(x, y.to_units_value(one)))
 
 
 @register(lax.min_p)
 def _min_p_qv(x: AbstractQuantity, y: ArrayLike) -> AbstractQuantity:
-    return replace(x, value=lax.min(x.to_value(one), y))
+    return replace(x, value=lax.min(x.to_units_value(one), y))
 
 
 # ==============================================================================
 # Multiplication
 
 
 @register(lax.mul_p)
@@ -2594,28 +2605,28 @@
 
 
 # ==============================================================================
 
 
 @register(lax.ne_p)
 def _ne_p_qq(x: AbstractQuantity, y: AbstractQuantity) -> ArrayLike:
-    return lax.ne(x.value, y.to_value(x.unit))
+    return lax.ne(x.value, y.to_units_value(x.unit))
 
 
 @register(lax.ne_p)
 def _ne_p_vq(x: ArrayLike, y: AbstractQuantity) -> ArrayLike:
-    return lax.ne(x, y.to_value(one))
+    return lax.ne(x, y.to_units_value(one))
 
 
 @register(lax.ne_p)
 def _ne_p_qv(x: AbstractQuantity, y: ArrayLike) -> ArrayLike:
     # special-case for scalar value=0, unit=one
     if y.shape == () and y == 0:  # TODO: proper jax
         return lax.ne(x.value, y)
-    return lax.ne(x.to_value(one), y)
+    return lax.ne(x.to_units_value(one), y)
 
 
 # @register(lax.ne_p)
 # def _ne_p_qv(x: AbstractParametricQuantity, y: ArrayLike) -> ArrayLike:
 #     return lax.
 
 
@@ -2702,15 +2713,15 @@
 # ==============================================================================
 
 
 @register(lax.pow_p)
 def _pow_p_qq(
     x: AbstractQuantity, y: AbstractParametricQuantity["dimensionless"]
 ) -> AbstractQuantity:
-    y_: Array = y.to_value(one)
+    y_: Array = y.to_units_value(one)
     y0 = y_[(0,) * y_.ndim]
     y_ = eqx.error_if(y_, any(y_ != y0), "power must be a scalar")
     return type_np(x)(value=lax.pow(x.value, y0), unit=x.unit**y0)
 
 
 @register(lax.pow_p)
 def _pow_p_qf(x: AbstractQuantity, y: ArrayLike) -> AbstractQuantity:
@@ -2907,15 +2918,15 @@
     >>> from unxt import Distance
     >>> q1 = Distance(10, "m")
     >>> q2 = Quantity(3, "m")
     >>> q1 % q2
     Distance(Array(1, dtype=int32, ...), unit='m')
 
     """
-    return replace(x, value=lax.rem(x.value, y.to_value(x.unit)))
+    return replace(x, value=lax.rem(x.value, y.to_units_value(x.unit)))
 
 
 # ==============================================================================
 
 
 @register(lax.reshape_p)
 def _reshape_p(
@@ -2982,15 +2993,18 @@
     updates: AbstractQuantity,
     **kwargs: Any,
 ) -> AbstractQuantity:
     """Scatter-add operator."""
     return replace(
         operand,
         value=lax.scatter_add_p.bind(
-            operand.value, scatter_indices, updates.to_value(operand.units), **kwargs
+            operand.value,
+            scatter_indices,
+            updates.to_units_value(operand.units),
+            **kwargs,
         ),
     )
 
 
 @register(lax.scatter_add_p)
 def _scatter_add_p_vvq(
     operand: ArrayLike,
@@ -3069,26 +3083,26 @@
 
 # ==============================================================================
 
 
 @register(lax.select_n_p)
 def _select_n_p(which: AbstractQuantity, *cases: AbstractQuantity) -> AbstractQuantity:
     unit = cases[0].unit
-    cases_ = (case.to_value(unit) for case in cases)
-    return type_np(which)(lax.select_n(which.to_value(one), *cases_), unit=unit)
+    cases_ = (case.to_units_value(unit) for case in cases)
+    return type_np(which)(lax.select_n(which.to_units_value(one), *cases_), unit=unit)
 
 
 @register(lax.select_n_p)
 def _select_n_p_vq(
     which: AbstractQuantity, case0: AbstractQuantity, case1: ArrayLike
 ) -> AbstractQuantity:
     # encountered from jnp.hypot
     unit = case0.unit
     return type_np(which)(
-        lax.select_n(which.to_value(one), case0.to_value(unit), case1),
+        lax.select_n(which.to_units_value(one), case0.to_units_value(unit), case1),
         unit=unit,
     )
 
 
 @register(lax.select_n_p)
 def _select_n_p_jjq(
     which: ArrayLike, case0: ArrayLike, case1: AbstractQuantity
@@ -3107,15 +3121,17 @@
 
 @register(lax.select_n_p)
 def _select_n_p_jqq(
     which: ArrayLike, case0: AbstractQuantity, case1: AbstractQuantity
 ) -> AbstractQuantity:
     # used by `jnp.hypot`
     unit = case0.unit
-    return replace(case0, value=lax.select_n(which, case0.value, case1.to_value(unit)))
+    return replace(
+        case0, value=lax.select_n(which, case0.value, case1.to_units_value(unit))
+    )
 
 
 # ==============================================================================
 
 
 @register(lax.sharding_constraint_p)
 def _sharding_constraint_p() -> AbstractQuantity:
@@ -3248,15 +3264,15 @@
 
 # ==============================================================================
 # Subtraction
 
 
 @register(lax.sub_p)
 def _sub_p_qq(x: AbstractQuantity, y: AbstractQuantity) -> AbstractQuantity:
-    return replace(x, value=lax.sub(x.to_value(x.unit), y.to_value(x.unit)))
+    return replace(x, value=lax.sub(x.to_units_value(x.unit), y.to_units_value(x.unit)))
 
 
 @register(lax.sub_p)
 def _sub_p_vq(x: ArrayLike, y: AbstractQuantity) -> AbstractQuantity:
     return replace(y, value=lax.sub(x, y.value))
```

### Comparing `unxt-0.8.1/src/unxt/_utils.py` & `unxt-0.9/src/unxt/_quantity/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 Copyright (c) 2023 Galactic Dynamics. All rights reserved.
 """
 
 __all__ = ["type_unparametrized"]
 
 from plum.parametric import ParametricTypeMeta
 
-from ._base import AbstractQuantity
+from .base import AbstractQuantity
 
 
 # TODO: upstream to `plum`
 def type_unparametrized(q: AbstractQuantity) -> type[AbstractQuantity]:
     """Return the non-parametric type of a Quantity.
 
     :mod:`plum.parametric` produces parametric subtypes of Quantity.  This
@@ -24,24 +24,24 @@
     >>> from unxt import UncheckedQuantity, Quantity
 
     >>> q = UncheckedQuantity(1, "m")
     >>> q
     UncheckedQuantity(Array(1, dtype=int32, weak_type=True), unit='m')
 
     >>> type_unparametrized(q)
-    <class 'unxt._fast.UncheckedQuantity'>
+    <class 'unxt...UncheckedQuantity'>
 
     >>> q = Quantity(1, "m")
     >>> q
     Quantity['length'](Array(1, dtype=int32, weak_type=True), unit='m')
 
     >>> type_unparametrized(q)
-    <class 'unxt._core.Quantity'>
+    <class 'unxt...Quantity'>
 
     This is different from `type` for parametric types.
 
     >>> type(q)
-    <class 'unxt._core.Quantity[PhysicalType('length')]'>
+    <class 'unxt...Quantity[PhysicalType('length')]'>
 
     """
     typ = type(q)
     return typ.mro()[1] if isinstance(typ, ParametricTypeMeta) else typ
```

### Comparing `unxt-0.8.1/src/unxt/experimental.py` & `unxt-0.9/src/unxt/experimental.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 from typing import ParamSpec, TypeVar
 
 import equinox as eqx
 import jax
 from astropy.units import UnitBase as Unit
 from jaxtyping import ArrayLike
 
-from ._core import Quantity
-from ._utils import type_unparametrized
+from ._quantity.core import Quantity
+from ._quantity.utils import type_unparametrized
 
 P = ParamSpec("P")
 R = TypeVar("R", bound=Quantity)
 
 
 def grad(
     fun: Callable[P, R], argnums: int = 0, *, units: tuple[Unit, ...]
@@ -36,15 +36,15 @@
         )
         return fun(*args_).value
 
     def gradfun(*args: P.args, **kw: P.kwargs) -> R:
         # Get the value of the args. They are turned back into Quantity
         # inside the function we are taking the grad of.
         args_ = tuple(
-            (a if unit is None else a.to_value(unit))  # type: ignore[attr-defined]
+            (a if unit is None else a.to_units_value(unit))  # type: ignore[attr-defined]
             for a, unit in zip(args, units, strict=True)
         )
         # Call the grad, returning a Quantity
         value = fun(*args)
         grad_value = gradfun_mag(*args_)
         # Adjust the Quantity by the units of the derivative
         # TODO: get Quantity[unit] / unit2 -> Quantity[unit/unit2] working
@@ -79,15 +79,15 @@
         )
         return fun(*args_)
 
     def jacfun(*args: P.args, **kw: P.kwargs) -> R:
         # Get the value of the args. They are turned back into Quantity
         # inside the function we are taking the Jacobian of.
         args_ = tuple(
-            (a if unit is None else a.to_value(unit))  # type: ignore[attr-defined]
+            (a if unit is None else a.to_units_value(unit))  # type: ignore[attr-defined]
             for a, unit in zip(args, units, strict=True)
         )
         # Call the Jacobian, returning a Quantity
         value = jacfun_mag(*args_)
         # Adjust the Quantity by the units of the derivative
         # TODO: check the unit correction
         # TODO: get Quantity[unit] / unit2 -> Quantity[unit/unit2] working
@@ -115,15 +115,15 @@
         )
         return fun(*args_)
 
     def hessfun(*args: P.args, **kw: P.kwargs) -> R:
         # Get the value of the args. They are turned back into Quantity
         # inside the function we are taking the hessian of.
         args_ = tuple(
-            (a if unit is None else a.to_value(unit))  # type: ignore[attr-defined]
+            (a if unit is None else a.to_units_value(unit))  # type: ignore[attr-defined]
             for a, unit in zip(args, units, strict=True)
         )
         # Call the hessian, returning a Quantity
         value = hessfun_mag(*args_)
         # Adjust the Quantity by the units of the derivative
         # TODO: check the unit correction
         # TODO: get Quantity[unit] / unit2 -> Quantity[unit/unit2] working
```

### Comparing `unxt-0.8.1/src/unxt/unitsystems/_base.py` & `unxt-0.9/src/unxt/unitsystems/_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 from collections.abc import Iterator
 from typing import ClassVar, Union, cast
 
 import astropy.units as u
 from astropy.units.physical import _physical_unit_mapping
 
-from unxt._base import AbstractQuantity
-from unxt._core import Quantity
+from unxt._quantity.base import AbstractQuantity
+from unxt._quantity.core import Quantity
 from unxt._typing import Unit
 
 
 class AbstractUnitSystem:
     """Represents a system of units.
 
     This class behaves like a dictionary with keys set by physical types (i.e. "length",
@@ -115,8 +115,9 @@
         if key in self._registry:
             return self._registry[key]
         return self[key]
 
     def as_preferred(self, quantity: AbstractQuantity | u.Quantity) -> Quantity:
         """Convert a quantity to the preferred unit for this unit system."""
         unit = self.preferred(quantity.unit.physical_type)
+        # Note that it's necessary to
         return cast(AbstractQuantity, Quantity.constructor(quantity.to(unit), unit))
```

### Comparing `unxt-0.8.1/src/unxt/unitsystems/_core.py` & `unxt-0.9/src/unxt/unitsystems/_core.py`

 * *Files identical despite different names*

### Comparing `unxt-0.8.1/src/unxt/unitsystems/_realizations.py` & `unxt-0.9/src/unxt/unitsystems/_realizations.py`

 * *Files identical despite different names*

### Comparing `unxt-0.8.1/src/unxt/unitsystems/_utils.py` & `unxt-0.9/src/unxt/unitsystems/_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 import astropy.units as u
 from plum import dispatch
 
 from ._base import AbstractUnitSystem
 from ._core import DimensionlessUnitSystem, UnitSystem
 from ._realizations import NAMED_UNIT_SYSTEMS, dimensionless
-from unxt._base import AbstractQuantity
+from unxt._quantity.base import AbstractQuantity
 from unxt._typing import Unit
 
 
 @dispatch
 def unitsystem(units: AbstractUnitSystem, /) -> AbstractUnitSystem:
     """Convert a UnitSystem or tuple of arguments to a UnitSystem.
```

### Comparing `unxt-0.8.1/tests/test_plum.py` & `unxt-0.9/tests/test_plum.py`

 * *Files identical despite different names*

### Comparing `unxt-0.8.1/tests/test_quantity.py` & `unxt-0.9/tests/test_quantity.py`

 * *Files 4% similar despite different names*

```diff
@@ -110,24 +110,24 @@
 
 
 def test_array_namespace():
     """Test the array namespace."""
     assert Quantity(1, u.m).__array_namespace__() is quaxed.array_api
 
 
-def test_to():
-    """Test the ``Quantity.to`` method."""
+def test_to_units():
+    """Test the ``Quantity.to_units`` method."""
     q = Quantity(1, u.m)
-    assert qnp.equal(q.to(u.km), Quantity(0.001, u.km))
+    assert qnp.equal(q.to_units(u.km), Quantity(0.001, u.km))
 
 
-def test_to_value():
-    """Test the ``Quantity.to`` method."""
+def test_to_units_value():
+    """Test the ``Quantity.to_units_value`` method."""
     q = Quantity(1, u.m)
-    assert q.to_value(u.km) == Quantity(0.001, u.km).value
+    assert q.to_units_value(u.km) == Quantity(0.001, u.km).value
 
 
 @pytest.mark.skip("TODO")
 def test_getitem():
     """Test the ``Quantity.__getitem__`` method."""
     raise NotImplementedError
```

### Comparing `unxt-0.8.1/tests/test_unitsystems.py` & `unxt-0.9/tests/test_unitsystems.py`

 * *Files identical despite different names*

### Comparing `unxt-0.8.1/tests/quaxed/test_array_api.py` & `unxt-0.9/tests/quaxed/test_array_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,29 +76,33 @@
 
 
 def test_arange_stop():
     """Test `arange`."""
     start = Quantity(2, u.m)
     stop = Quantity(10, u.km)
     got = xp.arange(start, stop)
-    expected = Quantity(xp.arange(start.value, stop.to_value(start.unit)), u.m)
+    expected = Quantity(xp.arange(start.value, stop.to_units_value(start.unit)), u.m)
 
     assert isinstance(got, Quantity)
     assert got.unit == expected.unit
     assert jnp.array_equal(got.value, expected.value)
 
 
 def test_arange_step():
     """Test `arange`."""
     start = Quantity(2, u.m)
     stop = Quantity(10, u.km)
     step = Quantity(2, u.m)
     got = xp.arange(start, stop, step)
     expected = Quantity(
-        xp.arange(start.value, stop.to_value(start.unit), step.to_value(start.unit)),
+        xp.arange(
+            start.value,
+            stop.to_units_value(start.unit),
+            step.to_units_value(start.unit),
+        ),
         u.m,
     )
 
     assert isinstance(got, Quantity)
     assert got.unit == expected.unit
     assert jnp.array_equal(got.value, expected.value)
```

### Comparing `unxt-0.8.1/tests/quaxed/test_numpy.py` & `unxt-0.9/tests/quaxed/test_numpy.py`

 * *Files identical despite different names*

### Comparing `unxt-0.8.1/.gitignore` & `unxt-0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `unxt-0.8.1/LICENSE` & `unxt-0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `unxt-0.8.1/README.md` & `unxt-0.9/README.md`

 * *Files identical despite different names*

### Comparing `unxt-0.8.1/pyproject.toml` & `unxt-0.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -73,14 +73,15 @@
     features = ["test"]
     scripts.test = "pytest {args}"
 
 
 [tool.pytest.ini_options]
   addopts = [
     "-ra",
+    "-p no:doctest",  # using sybil
     "--arraydiff",
     "--showlocals",
     "--strict-markers",
     "--strict-config",
   ]
   filterwarnings = [
     "error",
```

### Comparing `unxt-0.8.1/PKG-INFO` & `unxt-0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: unxt
-Version: 0.8.1
+Version: 0.9
 Summary: Quantities in JAX
 Project-URL: Bug Tracker, https://github.com/GalacticDynamics/unxt/issues
 Project-URL: Changelog, https://github.com/GalacticDynamics/unxt/releases
 Project-URL: Discussions, https://github.com/GalacticDynamics/unxt/discussions
 Project-URL: Homepage, https://github.com/GalacticDynamics/unxt
 Author-email: Nathaniel Starkman <nstarman@users.noreply.github.com>
 License: BSD 3-Clause License
```

