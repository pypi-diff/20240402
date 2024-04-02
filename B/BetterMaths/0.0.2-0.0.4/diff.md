# Comparing `tmp/bettermaths-0.0.2.tar.gz` & `tmp/bettermaths-0.0.4.tar.gz`

## Comparing `bettermaths-0.0.2.tar` & `bettermaths-0.0.4.tar`

### file list

```diff
@@ -1,20 +1,26 @@
--rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 bettermaths-0.0.2/generate.py
--rw-r--r--   0        0        0    37790 2020-02-02 00:00:00.000000 bettermaths-0.0.2/images/banner.png
--rw-r--r--   0        0        0    21551 2020-02-02 00:00:00.000000 bettermaths-0.0.2/images/logo transparent.png
--rw-r--r--   0        0        0    26707 2020-02-02 00:00:00.000000 bettermaths-0.0.2/images/logo.png
--rw-r--r--   0        0        0    23333 2020-02-02 00:00:00.000000 bettermaths-0.0.2/images/wiki/equation-page.png
--rw-r--r--   0        0        0    22228 2020-02-02 00:00:00.000000 bettermaths-0.0.2/images/wiki/geometry-page.png
--rw-r--r--   0        0        0    19633 2020-02-02 00:00:00.000000 bettermaths-0.0.2/images/wiki/home-page.png
--rw-r--r--   0        0        0    23092 2020-02-02 00:00:00.000000 bettermaths-0.0.2/images/wiki/probabilities-page.png
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 bettermaths-0.0.2/src/BetterMaths/__init__.py
--rw-r--r--   0        0        0    21932 2020-02-02 00:00:00.000000 bettermaths-0.0.2/src/BetterMaths/main.py
--rw-r--r--   0        0        0     4862 2020-02-02 00:00:00.000000 bettermaths-0.0.2/src/BetterMaths/main.pyi
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 bettermaths-0.0.2/src/BetterMaths/geometry/__init__.py
--rw-r--r--   0        0        0     3839 2020-02-02 00:00:00.000000 bettermaths-0.0.2/src/BetterMaths/geometry/main.py
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 bettermaths-0.0.2/src/BetterMaths/probability/__init__.py
--rw-r--r--   0        0        0     1224 2020-02-02 00:00:00.000000 bettermaths-0.0.2/src/BetterMaths/probability/main.py
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 bettermaths-0.0.2/.gitignore
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 bettermaths-0.0.2/LICENSE
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 bettermaths-0.0.2/README.md
--rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 bettermaths-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 bettermaths-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 bettermaths-0.0.4/generate.py
+-rw-r--r--   0        0        0    37790 2020-02-02 00:00:00.000000 bettermaths-0.0.4/images/banner.png
+-rw-r--r--   0        0        0    21551 2020-02-02 00:00:00.000000 bettermaths-0.0.4/images/logo transparent.png
+-rw-r--r--   0        0        0    26707 2020-02-02 00:00:00.000000 bettermaths-0.0.4/images/logo.png
+-rw-r--r--   0        0        0    23333 2020-02-02 00:00:00.000000 bettermaths-0.0.4/images/wiki/equation-page.png
+-rw-r--r--   0        0        0    22228 2020-02-02 00:00:00.000000 bettermaths-0.0.4/images/wiki/geometry-page.png
+-rw-r--r--   0        0        0    19633 2020-02-02 00:00:00.000000 bettermaths-0.0.4/images/wiki/home-page.png
+-rw-r--r--   0        0        0    23092 2020-02-02 00:00:00.000000 bettermaths-0.0.4/images/wiki/probabilities-page.png
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 bettermaths-0.0.4/src/BetterMaths/__init__.py
+-rw-r--r--   0        0        0    26874 2020-02-02 00:00:00.000000 bettermaths-0.0.4/src/BetterMaths/main.py
+-rw-r--r--   0        0        0     4962 2020-02-02 00:00:00.000000 bettermaths-0.0.4/src/BetterMaths/main.pyi
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 bettermaths-0.0.4/src/BetterMaths/geometry/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bettermaths-0.0.4/src/BetterMaths/geometry/main.py
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 bettermaths-0.0.4/src/BetterMaths/probability/__init__.py
+-rw-r--r--   0        0        0     2908 2020-02-02 00:00:00.000000 bettermaths-0.0.4/src/BetterMaths/probability/main.py
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 bettermaths-0.0.4/src/BetterMaths/sequences/__init__.py
+-rw-r--r--   0        0        0     8308 2020-02-02 00:00:00.000000 bettermaths-0.0.4/src/BetterMaths/sequences/main.py
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 bettermaths-0.0.4/src/BetterMaths/solidGeometry/__init__.py
+-rw-r--r--   0        0        0    14452 2020-02-02 00:00:00.000000 bettermaths-0.0.4/src/BetterMaths/solidGeometry/main.py
+-rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 bettermaths-0.0.4/tests/__init__.py
+-rw-r--r--   0        0        0     3813 2020-02-02 00:00:00.000000 bettermaths-0.0.4/tests/main.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 bettermaths-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 bettermaths-0.0.4/LICENSE
+-rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 bettermaths-0.0.4/README.md
+-rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 bettermaths-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     2588 2020-02-02 00:00:00.000000 bettermaths-0.0.4/PKG-INFO
```

### Comparing `bettermaths-0.0.2/generate.py` & `bettermaths-0.0.4/generate.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,9 +20,9 @@
 with open("pyproject.toml", "r") as file:
     toml_data = toml.load(file)
 
 version = toml_data["project"]["version"]
 
 subprocess.run(["pip", "install", f"dist/bettermaths-{version}-py3-none-any.whl"])
 
-# #Remove dist dir
-# shutil.rmtree("dist")
+#Remove dist dir
+#shutil.rmtree("dist")
```

### Comparing `bettermaths-0.0.2/images/banner.png` & `bettermaths-0.0.4/images/banner.png`

 * *Files identical despite different names*

### Comparing `bettermaths-0.0.2/images/logo transparent.png` & `bettermaths-0.0.4/images/logo transparent.png`

 * *Files identical despite different names*

### Comparing `bettermaths-0.0.2/images/logo.png` & `bettermaths-0.0.4/images/logo.png`

 * *Files identical despite different names*

### Comparing `bettermaths-0.0.2/images/wiki/equation-page.png` & `bettermaths-0.0.4/images/wiki/equation-page.png`

 * *Files identical despite different names*

### Comparing `bettermaths-0.0.2/images/wiki/geometry-page.png` & `bettermaths-0.0.4/images/wiki/geometry-page.png`

 * *Files identical despite different names*

### Comparing `bettermaths-0.0.2/images/wiki/home-page.png` & `bettermaths-0.0.4/images/wiki/home-page.png`

 * *Files identical despite different names*

### Comparing `bettermaths-0.0.2/images/wiki/probabilities-page.png` & `bettermaths-0.0.4/images/wiki/probabilities-page.png`

 * *Files identical despite different names*

### Comparing `bettermaths-0.0.2/src/BetterMaths/main.py` & `bettermaths-0.0.4/src/BetterMaths/main.py`

 * *Files 14% similar despite different names*

```diff
@@ -138,14 +138,72 @@
     Returns:
         The result of the resolved calculation.
     """
     equation = Equation(calcul, args=options)
     return equation.result()
 
 
+
+functions = {
+    "abs": lambda value, options: abs(value),
+    "floor": lambda value, options: math.floor(value),
+    "ceil": lambda value, options: math.ceil(value),
+    "sqrt": lambda value, options: math.sqrt(value),
+    "exp": lambda value, options: math.exp(value),
+    "log": lambda value, options: math.log(value, 10),
+    "ln": lambda value, options: math.log(value, math.e),
+    "cos": lambda value, options: cos(value, options["angles"]),
+    "sin": lambda value, options: sin(value, options["angles"]),
+    "tan": lambda value, options: tan(value, options["angles"]),
+    "acos": lambda value, options: acos(value, options["angles"]),
+    "asin": lambda value, options: asin(value, options["angles"]),
+    "atan": lambda value, options: atan(value, options["angles"]),
+    "atan2": lambda value, options: atan2(float(str(value).split(",")[0]), float(str(value).split(",")[1]), options["angles"]),
+    "cosh": lambda value, options: math.cosh(value),
+    "sinh": lambda value, options: math.sinh(value),
+    "tanh": lambda value, options: math.tanh(value),
+    "lcm": lambda value, options: math.lcm(*list(map(round, map(float, str(value).split(","))))),
+    "gcd": lambda value, options: math.gcd(*list(map(round, map(float, str(value).split(","))))),
+    "gcf": lambda value, options: math.gcd(*list(map(round, map(float, str(value).split(","))))),
+    "min": lambda value, options: min(str(value).split(",")),
+    "max": lambda value, options: max(str(value).split(",")),
+}
+minNameLenght = math.inf
+maxNameLenght = -1
+for key in functions:
+    if len(key) < minNameLenght:
+        minNameLenght = len(key)
+    elif len(key) > maxNameLenght:
+        maxNameLenght = len(key)
+# Because last index in range is exclude
+maxNameLenght += 1
+
+
+
+humanReadable = {
+    " ": "",
+    "++": "+",
+    "+-": "-",
+    "-+": "-",
+    "--": "+",
+}
+
+programReadable = {
+    "^": "**",
+    ")(": ")*("
+}
+for nbr in range(0, 10):
+    programReadable[str(nbr) + "("] = str(nbr) + "*("
+    for func in functions:
+        programReadable[str(nbr) + func] = str(nbr) + "*" + func
+for func in functions:
+        programReadable[")" + func] = ")*" + func
+
+programReadable["atan2*("] = "atan2("
+
 class Equation:
     """
     Represents a mathematical equation.
 
     Attributes:
         equation (str): The equation in program-readable format.
         humanEquation (str): The equation in human-readable format.
@@ -179,235 +237,281 @@
         __eq__(self, other) -> bool: Checks if the current equation is equal to the other equation or value.
         __ne__(self, other) -> bool: Checks if the current equation is not equal to the other equation or value.
         __lt__(self, other) -> bool: Checks if the current equation is less than the other equation or value.
         __le__(self, other) -> bool: Checks if the current equation is less than or equal to the other equation or value.
     """
     
     def __init__(self, equation: str, **args):
+        for froms in humanReadable:
+            if froms in equation: # Just for optimisation
+                equation = equation.replace(froms, humanReadable.get(froms))
+        #If we have +number at the beginning
+        while equation.startswith("+"):
+            equation = equation[1:]
         self.humanEquation = equation
-        self.toHumanRedeable()
-        self.equation = equation
-        self.toProgramRedeable()
+        
+        self.equation = self.humanEquation
+        a = self.__getProgramReadable__()
+        for froms in a:
+            if froms in self.equation: # Just for optimisation
+                self.equation = self.equation.replace(froms, a.get(froms))
 
         self.options = {}
         if "args" in args and len(args.get("args")) != 0:
             self.options = args.get("args")
         else:
             self.options["angles"] = args.get("angles", Option.DEGREES)
-    
+
+
     def setOption(self, options: dict):
         self.options = options
 
-    def toHumanRedeable(self):
-        replacables = {
-            " ": "",
-            "++": "+",
-            "+-": "-",
-            "--": "-",
-            "--": "+",
-        }
-
-        for froms, to in replacables.items():
-            self.humanEquation = self.humanEquation.replace(froms, to)
+    def toHumanRedeable(self) -> str:
         return self.humanEquation
     
-    def toProgramRedeable(self)->str:
-        self.toHumanRedeable()
-
-        replacables = {
-            "^": "**",
-        }
-        for nbr in range(0, 10):
-            replacables[str(nbr) + "("] = str(nbr) + "*("
-            for func in ["sqrt", "abs", "exp", "log", "cos", "sin", "tan", "acos", "asin", "atan", "atan2"]:
-                replacables[str(nbr) + func] = str(nbr) + "*" + func
-                
-        replacables["atan2*("] = "atan2("
-
-        for froms, to in replacables.items():
-            self.equation = self.equation.replace(froms, to)
+    def toProgramRedeable(self) -> str:
         return self.equation
+    
+    def __getProgramReadable__(self) -> dict:
+        return programReadable
 
-    def result(self)->float:
-        equation = self.toProgramRedeable()
+    def result(self) -> float:
+        try:
+            return self.__resolve__(self.equation)
+        except OverflowError:
+            return math.inf
+        
+    
+    def sum(self, equation: str) -> float:
+        values = equation.split("+")
         result = 0
+        for value in values:
+            result += self.__resolve__(value)
+        return result
+    
+    def sub(self, equation: str):
+        return eval(equation)
+    
+    def pow(self, equation: str) -> float:
+        values = equation.split("*")
+        result = self.__resolve__(values.pop())
+        for value in values:
+            result *= self.__resolve__(value)
+        return result
+    
+    def power(self, equation: str) -> float:
+        values = equation.split("**")
+        result = self.__resolve__(values.pop())
+        while len(values) > 0:
+            result = self.__resolve__(values.pop()) ** result
+        return result
+    
+    def divide(self, equation: str) -> float:
+        values = equation.split("/")
+        result = self.__resolve__(values.pop(0))
+        for value in values:
+            result /= self.__resolve__(value)
+        return result
+    
+    def floordivide(self, equation: str) -> float:
+        values = equation.split("//")
+        result = self.__resolve__(values.pop(0))
+        for value in values:
+            result //= self.__resolve__(value)
+        return result
+    
+    def modulo(self, equation: str) -> float:
+        values = equation.split("%")
+        result = self.__resolve__(values.pop(0))
+        for value in values:
+            result %= self.__resolve__(value)
+        return result
+
+    def __resolve__(self, equation: str) -> float:
         if "(" in equation:
             start = equation.find("(")
             nbrCanBePassed = 1
             end = -1
             for i in range(start + 1, len(equation)):
                 element = equation[i]
                 if element == "(":
                     nbrCanBePassed += 1
                 elif element == ")":
                     nbrCanBePassed -= 1
                     if nbrCanBePassed == 0:
                         end = i
                         break
-            value = resolve(equation[start + 1:end], self.options)
-            functions = {
-                "sqrt": lambda: math.sqrt(value),
-                "abs": lambda: abs(value),
-                "exp": lambda: math.exp(value),
-                "log": lambda: math.log(value, math.e),
-                "cos": lambda: cos(value, self.options["angles"]),
-                "sin": lambda: sin(value, self.options["angles"]),
-                "tan": lambda: tan(value, self.options["angles"]),
-                "acos": lambda: acos(value, self.options["angles"]),
-                "asin": lambda: asin(value, self.options["angles"]),
-                "atan": lambda: atan(value, self.options["angles"]),
-                "atan2": lambda: atan2(float(str(value).split(",")[0]), float(str(value).split(",")[1]), self.options["angles"]),
-            }
-            for key, func in functions.items():
-                if key == equation[start - len(key):start]:
-                    value = func()
-                    start -= len(key)
+
+            inParenthese = equation[start + 1:end]
+            if "," in inParenthese:
+                value = ",".join([str(self.__resolve__(v)) for v in inParenthese.split(",")])
+            else:
+                value = self.__resolve__(inParenthese)
+            
+            for key in range(minNameLenght, maxNameLenght):
+                func = functions.get(equation[start - key:start])
+                if func != None:
+                    value = func(value, self.options)
+                    start -= key
                     break
 
-            return resolve(equation[:start] + str(value) + equation[end + 1:], self.options)
+            return self.__resolve__(equation[:start] + str(value) + equation[end + 1:])
         #Factorial
         elif "!" in equation:
             start = equation.find("!")
             mustBeFactorial = ""
             for i in range(start - 1, -1, -1):
                 if equation[i] in ["0", "1", "2", "3", "4", "5", "6", "7", "8", "9"]:
                     mustBeFactorial = equation[i] + mustBeFactorial
                 else:
                     break
-            return resolve(equation[:start - len(mustBeFactorial)] + str(math.factorial(int(mustBeFactorial))) + equation[start + 1:], self.options)
-        elif "," in equation:
-            if "pi" in equation:
-                equation = equation.replace("pi", str(math.pi))
-            return equation
-        else:
-            if "pi" in equation:
-                equation = equation.replace("pi", str(math.pi))
-            result = eval(equation)
-        return result
+            return self.__resolve__(equation[:start - len(mustBeFactorial)] + str(math.factorial(int(mustBeFactorial))) + equation[start + 1:])
+        elif "+" in equation:
+            return self.sum(equation)
+        elif "-" in equation:
+            return self.sub(equation)
+        elif "//" in equation:
+            return self.floordivide(equation)
+        elif "/" in equation:
+            return self.divide(equation)
+        elif "%" in equation:
+            return self.modulo(equation)
+        elif "**" in equation:
+            return self.power(equation)
+        elif "*" in equation:
+            return self.pow(equation)
+
+        if "pi" in equation:
+            equation = equation.replace("pi", str(math.pi))
+        if "tau" in equation:
+            equation = equation.replace("tau", str(math.tau))
+        if "e" in equation:
+            equation = equation.replace("e", str(math.e))
+        return float(equation)
     
 
-    def split(self, separator)->"list[Equation]":
+    def split(self, separator) -> "list[Equation]":
         splitedEquations = self.humanEquation.split(separator)
         result = []
         for splitedEquation in splitedEquations:
             newEquation = Equation(splitedEquation)
             newEquation.setOption(self.options)
             result.append(newEquation)
         return result
     
 
-    def __transformOther__(self, other)->"tuple[str, dict[Option]]":
+    def __transformOther__(self, other) -> "tuple[str, dict[Option]]":
         otherEquation = ""
         options = self.options
         if type(other) != Equation:
             otherEquation = str(other)
         else:
             otherEquation = other.humanEquation
             for key, value in other.options.items():
                 options[key] = value
         return otherEquation, options
 
 
-    def __add__(self, other)->"Equation":
+    def __add__(self, other) -> "Equation":
         otherEquation, options = self.__transformOther__(other)
 
         new = Equation(self.humanEquation + "+" + otherEquation)
         new.setOption(options)
         return new
 
 
-    def __radd__(self, other)->"Equation":
+    def __radd__(self, other) -> "Equation":
         return self.__add__(other)
 
 
-    def __sub__(self, other)->"Equation":
+    def __sub__(self, other) -> "Equation":
         otherEquation, options = self.__transformOther__(other)
         
         new = Equation(self.humanEquation + "-(" + otherEquation + ")")
         new.setOption(options)
         return new
 
 
-    def __rsub__(self, other)->"Equation":
+    def __rsub__(self, other) -> "Equation":
         otherEquation, options = self.__transformOther__(other)
         
         new = Equation(otherEquation + "-(" + self.humanEquation + ")")
         new.setOption(options)
         return new
 
 
-    def __mul__(self, other)->"Equation":
+    def __mul__(self, other) -> "Equation":
         otherEquation, options = self.__transformOther__(other)
 
         new = Equation("(" + otherEquation + ")*(" + self.humanEquation + ")")
         new.setOption(options)
         return new
 
 
-    def __rmul__(self, other)->"Equation":
+    def __rmul__(self, other) -> "Equation":
         return self.__mul__(other)
 
 
-    def __pow__(self, other, mod: int = None)->"Equation":
+    def __pow__(self, other, mod: int = None) -> "Equation":
         otherEquation, options = self.__transformOther__(other)
 
         new = Equation("(" + self.humanEquation + ")**(" + otherEquation + ")")
         new.setOption(options)
         return new
     
 
-    def __rpow__(self, other, mod: int = None)->"Equation":
+    def __rpow__(self, other, mod: int = None) -> "Equation":
         otherEquation, options = self.__transformOther__(other)
 
         new = Equation("(" + otherEquation + ")**(" + self.humanEquation + ")")
         new.setOption(options)
         return new
 
 
-    def __floordiv__(self, other)->"Equation":
+    def __floordiv__(self, other) -> "Equation":
         otherEquation, options = self.__transformOther__(other)
 
         new = Equation("(" + self.humanEquation + ")//(" + otherEquation + ")")
         new.setOption(options)
         return new
 
 
-    def __rfloordiv__(self, other)->"Equation":
+    def __rfloordiv__(self, other) -> "Equation":
         otherEquation, options = self.__transformOther__(other)
 
         new = Equation("(" + otherEquation + ")//(" + self.humanEquation + ")")
         new.setOption(options)
         return new
 
 
-    def __truediv__(self, other)->"Equation":
+    def __truediv__(self, other) -> "Equation":
         otherEquation, options = self.__transformOther__(other)
 
         new = Equation("(" + self.humanEquation + ")/(" + otherEquation + ")")
         new.setOption(options)
         return new
 
 
-    def __rtruediv__(self, other)->"Equation":
+    def __rtruediv__(self, other) -> "Equation":
         otherEquation, options = self.__transformOther__(other)
 
         new = Equation("(" + otherEquation + ")/(" + self.humanEquation + ")")
         new.setOption(options)
         return new
 
 
-    def __mod__(self, other)->"Equation":
+    def __mod__(self, other) -> "Equation":
         otherEquation, options = self.__transformOther__(other)
 
         new = Equation("(" + self.humanEquation + ")%(" + otherEquation + ")")
         new.setOption(options)
         return new
 
 
-    def __rmod__(self, other)->"Equation":
+    def __rmod__(self, other) -> "Equation":
         otherEquation, options = self.__transformOther__(other)
 
         new = Equation("(" + otherEquation + ")%(" + self.humanEquation + ")")
         new.setOption(options)
         return new
     
 
@@ -427,135 +531,135 @@
         if type(other) != Equation:
             otherResult = float(other)
         else:
             otherResult = other.result()
         return (otherResult // result, otherResult % result)
 
 
-    def __neg__(self)->"Equation":
+    def __neg__(self) -> "Equation":
         new = Equation("-(" + self.humanEquation + ")")
         new.setOption(self.options)
         return new
     
 
-    def __eq__(self, other)->bool:
+    def __eq__(self, other) -> bool:
         otherResult = ""
         if type(other) != Equation:
             otherResult = resolve(str(other))
         else:
             otherResult = other.result()
 
         return self.result() == otherResult
     
-    def __ne__(self, other)->bool:
+    def __ne__(self, other) -> bool:
         otherResult = ""
         if type(other) != Equation:
             otherResult = resolve(str(other))
         else:
             otherResult = other.result()
 
         return self.result() != otherResult
     
-    def __lt__(self, other)->bool:
+    def __lt__(self, other) -> bool:
         otherResult = ""
         if type(other) != Equation:
             otherResult = resolve(str(other))
         else:
             otherResult = other.result()
 
         return self.result() < otherResult
 
 
-    def __le__(self, other)->bool:
+    def __le__(self, other) -> bool:
         otherResult = ""
         if type(other) != Equation:
             otherResult = resolve(str(other))
         else:
             otherResult = other.result()
 
         return self.result() <= otherResult
 
 
-    def __gt__(self, other)->bool:
+    def __gt__(self, other) -> bool:
         otherResult = ""
         if type(other) != Equation:
             otherResult = resolve(str(other))
         else:
             otherResult = other.result()
 
         return self.result() > otherResult
 
 
-    def __ge__(self, other)->bool:
+    def __ge__(self, other) -> bool:
         otherResult = ""
         if type(other) != Equation:
             otherResult = resolve(str(other))
         else:
             otherResult = other.result()
 
         return self.result() >= otherResult
     
 
-    def __float__(self)->float:
+    def __float__(self) -> float:
         return float(self.result())
 
 
-    def __int__(self)->int:
+    def __int__(self) -> int:
         return int(self.result())
 
 
-    def __abs__(self)->int:
+    def __abs__(self) -> int:
         return abs(self.result())
     
 
     #TODO: ndigits must be SupportsIndex
-    def __round__(self, ndigits: None = None)->int:
+    def __round__(self, ndigits: None = None) -> int:
         return round(self.result(), ndigits)
     
 
-    def __ceil__(self)->int:
+    def __ceil__(self) -> int:
         return math.ceil(self.result())
 
 
-    def __floor__(self)->int:
+    def __floor__(self) -> int:
         return math.floor(self.result())
 
 
-    def __str__(self)->str:
+    def __str__(self) -> str:
         return self.humanEquation
 
 
 
 class Function(Equation):
     def __init__(self, equation, name = "x", **args):
         self.name = name
         super().__init__(equation, **args)
 
         self.cachedResults = {}
+        self.hasUnknow = self.equation.find(name) != -1
     
-    def toProgramRedeable(self):
-        super().toProgramRedeable()
-
-        replacables = {}
+    def __getProgramReadable__(self) -> dict:
+        replacables = super().__getProgramReadable__()
         for nbr in range(0, 10):
             replacables[str(nbr) + self.name] = str(nbr) + "*" + self.name
-        
-        for froms, to in replacables.items():
-            self.equation = self.equation.replace(froms, to)
-        return self.equation
+        return replacables
+
 
     def result(self, value: float) -> float:
         value = str(value)
         if value in self.cachedResults:
             return self.cachedResults[value]
-        r = resolve(self.equation.replace(self.name, str(value)), self.options)
+        if self.hasUnknow:
+            r = resolve(self.equation.replace(self.name, value), self.options)
+        else:
+            r = resolve(self.equation, self.options)
         self.cachedResults[value] = r
         return r
     
-    def prime(self)->"Function":
+    def prime(self) -> "Function":
         variable = self.equation.find(self.name)
         result = 1
         for i in range(variable, 0, -1):
             if self.equation[i] == "*":
                 result *= self.equation[i - 1]
                 i -= 1
         for i in range(variable, len(self.equation), 1):
@@ -563,82 +667,112 @@
                 result *= self.equation[i + 1]
                 i += 1
         return result
 
 
 
 
-class Sum(Function):
+class Sum(Equation):
     def __init__(self, start, end, equation, unknow = "x"):
         self.start = start
         self.end = end
-        super().__init__(equation, unknow)
 
+        self.name = unknow
 
-    def resolve(self):
-        result = 0
-        for i in range(self.start, self.end + 1):
-            result += self.result(i)
-        return result
+        super().__init__(equation)
 
-    def toFunction(self):
-        equation = [self.equation for i in range(self.start, self.end + 1)]
-        return Function("+".join(equation))
-
-    def toEquation(self, value):
-        equation = [self.equation.replace(self.name, str(value)) for i in range(self.start, self.end + 1)]
-        return Equation("+".join(equation))
+        self.hasUnknow = self.equation.find(self.name) != -1
+
+        if self.hasUnknow:
+            self.equation = "+".join([self.equation.replace(self.name, str(i)) for i in range(self.start, self.end + 1)])
+        else:
+            self.equation = str((self.end + 1) - self.start) + "*" + self.equation
+    
+
+    def __getProgramReadable__(self) -> dict:
+        replacables = super().__getProgramReadable__()
+        for nbr in range(0, 10):
+            replacables[str(nbr) + self.name] = str(nbr) + "*" + self.name
+        return replacables
+
+    def result(self):
+        return super().result()
+
+    def toFunction(self) -> Function:
+        return Function(self.equation)
+
+    def toEquation(self) -> Equation:
+        return Equation(self.equation)
 
 
     def __add__(self, other):
         if type(other) != Sum:
-            return
+            raise BaseException("Cannot sum " + str(self) + " and " + str(other))
 
+        newEquation = None
         if other.start == self.start and other.end == self.end:
-            new = Sum(self.start, self.end, self.humanEquation + other.humanEquation)
-            new.setOption(self.options)
-            return new
+            newEquation = Sum(self.start, self.end, self.humanEquation + "+" + other.humanEquation)
+        elif other.humanEquation == self.humanEquation:
+            if other.start == self.end or other.end == self.start:
+                newEquation = Sum(min(self.start, other.start), max(self.end, other.end) + 1, self.humanEquation)
+            elif other.start - 1 == self.end or other.end + 1 == self.start:
+                newEquation = Sum(min(self.start, other.start), max(self.end, other.end), self.humanEquation)
+        else:
+            newStart = min(self.start, other.start)
+            newEnd = min(self.end, other.end)
+
+            result = None
+            if other.end > self.end:
+                result = other.end / self.end
+            else:
+                result = self.end / other.end
+
+            humanEquation = None
+            if other.start > self.start:
+                humanEquation = other.start / self.start
+            else:
+                humanEquation = self.start / other.start
 
+            newEquation = Sum(newStart, newEnd, str(humanEquation) + "+" + str(result))
+        
+        if newEquation != None and newEquation.result() == (self.result() + other.result()):
+            newEquation.setOption(self.options)
+            return newEquation
+        raise BaseException("Cannot sum " + str(self) + " and " + str(other))
 
-    def __radd__(self, other)->"Equation":
+
+    def __radd__(self, other) -> "Equation":
         return self.__add__(other)
 
-class EquaDiff(Function):
-    """
-    Represents an equation differential function.
 
-    Args:
-        equation (str): The equation to be solved.
-        name (str, optional): The name of the variable in the equation. Defaults to "x".
-        **args: Additional arguments to be passed to the parent class.
 
-    Attributes:
-        equation (str): The equation to be solved.
-        name (str): The name of the variable in the equation.
-        options (dict): Additional options for solving the equation.
+class Prod(Equation):
+    def __init__(self, start, end, equation, unknow = "x"):
+        self.start = start
+        self.end = end
 
-    Methods:
-        result(value=""): Computes the result of the equation for a given value.
+        self.name = unknow
 
-    """
+        super().__init__(equation)
+        
+        self.hasUnknow = self.equation.find(self.name) != -1
+
+        if self.hasUnknow:
+            self.equation = "*" .join(["(" + self.equation.replace(self.name, str(i)) + ")" for i in range(self.start, self.end + 1)])
+        else:
+            self.equation =  "(" + self.equation + ")**" + str((self.end + 1) - self.start)
+
+        
+    def __getProgramReadable__(self) -> dict:
+        replacables = super().__getProgramReadable__()
+        for nbr in range(0, 10):
+            replacables[str(nbr) + self.name] = str(nbr) + "*" + self.name
+        return replacables
+
+    def result(self):
+        return super().result()
 
-    def __init__(self, equation, name="x", **args):
-        super().__init__(equation, name, **args)
+    def toFunction(self) -> Function:
+        return Function(self.equation)
 
-    def result(self, value=""):
-        """
-        Computes the result of the equation for a given value.
-
-        Args:
-            value (str, optional): The value to substitute for the variable in the equation. Defaults to "".
-
-        Returns:
-            str: The result of the equation with the substituted value.
-
-        """
-        a = self.equation.split("+")[0]
-        a = a.replace(self.name, value)
-        a = resolve(a, self.options)
-        b = self.equation.split("+")[1]
-        self.equation = "Cexp(" + str(a) + self.name + ") + " + str(-int(b) / int(a))
-        print(self.equation)
-        return self.toHumanRedeable()
+    def toEquation(self) -> Equation:
+        return Equation(self.equation)
```

### Comparing `bettermaths-0.0.2/src/BetterMaths/main.pyi` & `bettermaths-0.0.4/src/BetterMaths/main.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -81,19 +81,22 @@
 
 
 class Function(Equation):
     def result(self, value: _SupportsFloatOrIndex) -> float: ...
     def prime(self) -> "Function": ...
 
 
-class Sum(Function):
-    def resolve(self) -> float: ...
+class Sum(Equation):
+    def result(self) -> float: ...
 
     def toFunction(self) -> Function: ...
     def toEquation(self, value) -> Equation: ...
 
-    def __add__(self, other: Sum) -> Sum: ...
-    def __radd__(self, other) -> Sum: ...
+    def __add__(self, other: "Sum") -> "Sum": ...
+    def __radd__(self, other: "Sum") -> "Sum": ...
 
 
-class EquaDiff(Function):
-    def result(self, value = ""): ...
+class Prod(Equation):
+    def result(self) -> float: ...
+
+    def toFunction(self) -> Function: ...
+    def toEquation(self, value) -> Equation: ...
```

### Comparing `bettermaths-0.0.2/LICENSE` & `bettermaths-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `bettermaths-0.0.2/pyproject.toml` & `bettermaths-0.0.4/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,33 +1,36 @@
-[build-system]
-requires = ["hatchling"]
-build-backend = "hatchling.build"
-
-[project]
-name = "BetterMaths"
-version = "0.0.2"
-authors = [
-  { name="Dhaiven", email="bettermath.get.help@gmail.com" },
-  { name="algorythmTTV", email="bettermath.get.help@gmail.com" },
-]
-description = "Python mathematics made easier"
-readme = "README.md"
-requires-python = ">=3.4"
-classifiers = [
-    "Programming Language :: Python :: 3.4",
-    "Programming Language :: Python :: 3.5",
-    "Programming Language :: Python :: 3.6",
-    "Programming Language :: Python :: 3.7",
-    "Programming Language :: Python :: 3.8",
-    "Programming Language :: Python :: 3.9",
-    "Programming Language :: Python :: 3.10",
-    "Programming Language :: Python :: 3.11",
-    "Programming Language :: Python :: 3.12",
-    "License :: OSI Approved :: MIT License",
-    "Operating System :: OS Independent",
-]
-keywords = ["math", "mathematics", "better", "easier", "simple", "easy"]
-
-[project.urls]
-Homepage = "https://dhaiven.github.io/"
-Documentation = "https://dhaiven.github.io/BetterMaths/wiki"
+[build-system]
+requires = ["hatchling"]
+build-backend = "hatchling.build"
+
+[project]
+name = "BetterMaths"
+version = "0.0.4"
+dependencies = [
+  "sympy"
+]
+authors = [
+  { name="Dhaiven", email="bettermath.get.help@gmail.com" },
+  { name="algorythmTTV", email="bettermath.get.help@gmail.com" },
+]
+description = "Python mathematics made easier"
+readme = "README.md"
+requires-python = ">=3.4"
+classifiers = [
+    "Programming Language :: Python :: 3.4",
+    "Programming Language :: Python :: 3.5",
+    "Programming Language :: Python :: 3.6",
+    "Programming Language :: Python :: 3.7",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
+    "License :: OSI Approved :: MIT License",
+    "Operating System :: OS Independent",
+]
+keywords = ["math", "mathematics", "better", "easier", "simple", "easy"]
+
+[project.urls]
+Homepage = "https://dhaiven.github.io/"
+Documentation = "https://github.com/Dhaiven/BetterMaths/wiki"
 Repository = "https://github.com/Dhaiven/BetterMaths"
```

### Comparing `bettermaths-0.0.2/PKG-INFO` & `bettermaths-0.0.4/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.3
 Name: BetterMaths
-Version: 0.0.2
+Version: 0.0.4
 Summary: Python mathematics made easier
 Project-URL: Homepage, https://dhaiven.github.io/
-Project-URL: Documentation, https://dhaiven.github.io/BetterMaths/wiki
+Project-URL: Documentation, https://github.com/Dhaiven/BetterMaths/wiki
 Project-URL: Repository, https://github.com/Dhaiven/BetterMaths
 Author-email: Dhaiven <bettermath.get.help@gmail.com>, algorythmTTV <bettermath.get.help@gmail.com>
 License-File: LICENSE
 Keywords: better,easier,easy,math,mathematics,simple
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.4
@@ -16,24 +16,45 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.4
+Requires-Dist: sympy
 Description-Content-Type: text/markdown
 
-![alt text](images/banner.png "Title")
-
+![BeterMaths Banner](https://github.com/Dhaiven/BetterMaths/blob/main/images/banner.png)
 
 [![MIT License](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
 > [!WARNING]
 > This module is in beta phase
 
-#### See the [Wiki](https://github.com/Dhaiven/BetterMaths/wiki) for documentations
+
+## Little documentation
+This module add ```Equation``` class that allow resolve equation in string
+```python
+# Create an equation
+equation = Equation("2+7*8cos(3)")
+# Resolve this equation
+equation.result() # 57.92325394625613
+```
+
+### Why use ```Equation``` and not ```eval``` ?
+- ```Equation``` is faster than ```eval``` (See [tests/main.py](https://github.com/Dhaiven/BetterMaths/blob/main/tests/main.py))
+- ```Equation``` support parenthese, mathematical formulas like ```cos``` and magics numbers like ```π```
+
+
+### See the [Wiki](https://github.com/Dhaiven/BetterMaths/wiki) for more documentations
+
+## Instalation
+Open your terminal and put ```pip install BetterMaths```
+<br> For upgrade the version, put ```pip install --upgrade BetterMaths```
 
 ## Contribution
-BetterMaths accepts community contributions!
+BetterMaths accepts community contributions! <br>
+This contributions must case no error tests folder.
+Launch __init__ file, put ```y``` for take your changes and checks if there are error.
 
 ## Authors
-  - <img src="https://www.github.com/Dhaiven.png" width="3%" height="3%"/> [@Dhaiven](https://www.github.com/Dhaiven) for code
-  - <img src="https://www.github.com/algorythmTTV.png" width="3%" height="3%"/> [@algorythmTTV](https://www.github.com/algorythmTTV) for images and site
+  - <img src="https://www.github.com/Dhaiven.png" width="3%" height="3%"/> [@Dhaiven](https://www.github.com/Dhaiven) for code, optimisation and tests
+  - <img src="https://www.github.com/algorythmTTV.png" width="3%" height="3%"/> [@algorythmTTV](https://www.github.com/algorythmTTV) for images, site ans code
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

