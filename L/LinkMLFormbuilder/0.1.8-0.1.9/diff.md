# Comparing `tmp/linkmlformbuilder-0.1.8.tar.gz` & `tmp/linkmlformbuilder-0.1.9.tar.gz`

## Comparing `linkmlformbuilder-0.1.8.tar` & `linkmlformbuilder-0.1.9.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 linkmlformbuilder-0.1.8/src/LinkMLFormbuilder/__init__.py
--rw-r--r--   0        0        0   152766 2020-02-02 00:00:00.000000 linkmlformbuilder-0.1.8/src/LinkMLFormbuilder/bootstrap.css
--rw-r--r--   0        0        0     3568 2020-02-02 00:00:00.000000 linkmlformbuilder-0.1.8/src/LinkMLFormbuilder/constants.py
--rw-r--r--   0        0        0    10975 2020-02-02 00:00:00.000000 linkmlformbuilder-0.1.8/src/LinkMLFormbuilder/formbuilder.py
--rw-r--r--   0        0        0    10589 2020-02-02 00:00:00.000000 linkmlformbuilder-0.1.8/src/LinkMLFormbuilder/slot_code_generators.py
--rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 linkmlformbuilder-0.1.8/src/LinkMLFormbuilder/styles.css
--rw-r--r--   0        0        0     4317 2020-02-02 00:00:00.000000 linkmlformbuilder-0.1.8/src/LinkMLFormbuilder/utils.py
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 linkmlformbuilder-0.1.8/.gitignore
--rw-r--r--   0        0        0    35857 2020-02-02 00:00:00.000000 linkmlformbuilder-0.1.8/LICENSE
--rw-r--r--   0        0        0     3230 2020-02-02 00:00:00.000000 linkmlformbuilder-0.1.8/README.md
--rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 linkmlformbuilder-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     3798 2020-02-02 00:00:00.000000 linkmlformbuilder-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 linkmlformbuilder-0.1.9/src/LinkMLFormbuilder/__init__.py
+-rw-r--r--   0        0        0   152766 2020-02-02 00:00:00.000000 linkmlformbuilder-0.1.9/src/LinkMLFormbuilder/bootstrap.css
+-rw-r--r--   0        0        0     3568 2020-02-02 00:00:00.000000 linkmlformbuilder-0.1.9/src/LinkMLFormbuilder/constants.py
+-rw-r--r--   0        0        0    11328 2020-02-02 00:00:00.000000 linkmlformbuilder-0.1.9/src/LinkMLFormbuilder/formbuilder.py
+-rw-r--r--   0        0        0    10597 2020-02-02 00:00:00.000000 linkmlformbuilder-0.1.9/src/LinkMLFormbuilder/slot_code_generators.py
+-rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 linkmlformbuilder-0.1.9/src/LinkMLFormbuilder/styles.css
+-rw-r--r--   0        0        0     4387 2020-02-02 00:00:00.000000 linkmlformbuilder-0.1.9/src/LinkMLFormbuilder/utils.py
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 linkmlformbuilder-0.1.9/.gitignore
+-rw-r--r--   0        0        0    35857 2020-02-02 00:00:00.000000 linkmlformbuilder-0.1.9/LICENSE
+-rw-r--r--   0        0        0     3348 2020-02-02 00:00:00.000000 linkmlformbuilder-0.1.9/README.md
+-rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 linkmlformbuilder-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     3913 2020-02-02 00:00:00.000000 linkmlformbuilder-0.1.9/PKG-INFO
```

### Comparing `linkmlformbuilder-0.1.8/src/LinkMLFormbuilder/bootstrap.css` & `linkmlformbuilder-0.1.9/src/LinkMLFormbuilder/bootstrap.css`

 * *Files identical despite different names*

### Comparing `linkmlformbuilder-0.1.8/src/LinkMLFormbuilder/constants.py` & `linkmlformbuilder-0.1.9/src/LinkMLFormbuilder/constants.py`

 * *Files identical despite different names*

### Comparing `linkmlformbuilder-0.1.8/src/LinkMLFormbuilder/formbuilder.py` & `linkmlformbuilder-0.1.9/src/LinkMLFormbuilder/formbuilder.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,40 +3,42 @@
 from LinkMLFormbuilder import utils
 import os
 import pdfkit
 from LinkMLFormbuilder import slot_code_generators
 from shutil import which
 import pkg_resources
 from LinkMLFormbuilder import constants
+import warnings
 
 def retrieveFileContent(yamlfile):
     try:
         stream = open(os.path.abspath(yamlfile), "r")
         return yaml.safe_load(stream)
     except yaml.YAMLError:
         print("File could not be parsed")
         exit(1)
     except Exception:
         print("Could not retrieve file content, please make sure the path is correct")
         exit(1)
 
-def getSlotFormCode(slotCode, content, default_range, subclasses, level):
-    if (constants.NAME not in slotCode): raise TypeError("Missing field: name")
+def getSlotFormCode(slotCode, content, default_range, subclasses, level, key):
+    if (slotCode is None): return ""
+    # if (constants.NAME not in slotCode): raise TypeError("Missing field: name")
     desc = utils.extractDescription(slotCode)
     required = constants.REQUIRED if (constants.REQUIRED in slotCode and slotCode.get(constants.REQUIRED) == True) else ""
     propertyName = slotCode.get(constants.NAME)
-    title = utils.extractSlotName(slotCode)
+    title = utils.extractSlotName(slotCode, key)
     
-    if (constants.VALUES_FROM in slotCode or (constants.RANGE in slotCode and slotCode.get(constants.RANGE) in content.get(constants.ENUMS))):
+    if (constants.VALUES_FROM in slotCode or (constants.RANGE in slotCode and constants.ENUMS in content and slotCode.get(constants.RANGE) in content.get(constants.ENUMS))):
         return slot_code_generators.getEnumSlotCode(slotCode, content, desc, required, propertyName, title)
     elif (constants.ENUM_RANGE in slotCode): # inlined enum
         return slot_code_generators.getInlineEnumSlotCode(slotCode, desc, required, propertyName, title)
     elif (constants.RANGE in slotCode):
         if (slotCode.get(constants.RANGE) in content.get(constants.CLASSES)):
-            return getClassFormCode(content.get(constants.CLASSES).get(slotCode.get(constants.RANGE)), content, default_range, subclasses, level + 1) # the range is a class itself and should be treated as such
+            return getClassFormCode(content.get(constants.CLASSES).get(slotCode.get(constants.RANGE)), content, default_range, subclasses, level + 1, key) # the range is a class itself and should be treated as such
         elif (slotCode.get(constants.RANGE) == "integer" or slotCode.get(constants.RANGE) == "float"):
             return slot_code_generators.getNumberSlotCode(slotCode, desc, required, propertyName, title)
         elif (slotCode.get(constants.RANGE) == "string"): #assume textarea
             return slot_code_generators.getTextareaSlotCode(desc, required, propertyName, title, slotCode)
         elif (slotCode.get(constants.RANGE) == "boolean"):
             return slot_code_generators.getBooleanSlotCode(desc, required, propertyName, title)
         else: # this is a basic pdf, so datetime should not be a datetime field, but a textfield
@@ -48,68 +50,69 @@
             elif (default_range == "string"): #assume textarea
                 return slot_code_generators.getTextareaSlotCode(desc, required, propertyName, title, slotCode)
             elif (default_range == "boolean"):
                 return slot_code_generators.getBooleanSlotCode(desc, required, propertyName, title)
             else: # this is a basic pdf, so datetime should not be a datetime field, but a textfield
                 return slot_code_generators.getStringSlotCode(desc, required, propertyName, title, slotCode)
         else:
-            raise TypeError("Invalid LinkML. There should either be a explicitly defined range for slot {slot}, or a default_range.".format(slot=utils.extractName(slotCode)))
+            raise TypeError("Invalid LinkML. There should either be a explicitly defined range for slot {slot}, or a default_range.".format(slot=utils.extractName(slotCode, key)))
 
-def getClassFormCode(classCode, content, default_range, subclasses, level):
-    title = utils.extractName(classCode)
+def getClassFormCode(classCode, content, default_range, subclasses, level, key):
+    title = utils.extractName(classCode, key)
     code = '''<h{level}>{title}</h{level}>\n'''.format(level = level + 1, title = title)
     code += "<p class='form-description'>Form description: " + utils.capitalizeLabel(utils.extractDescription(classCode)) + "</p>\n"
     if (constants.IS_A in classCode): # process superclass first
         superClassName = classCode.get(constants.IS_A)
         superClassCode = content.get(constants.CLASSES).get(superClassName)
         for slot in superClassCode.get(constants.SLOTS):
             if (slot not in classCode.get("slot_usage")): # this slot is not further specified in the class itself
                 slotCode = content.get(constants.SLOTS).get(slot)
-                code += getSlotFormCode(slotCode, content, default_range, subclasses, level)
+                code += getSlotFormCode(slotCode, content, default_range, subclasses, level, slot)
     if (constants.MIXINS in classCode): # then process mixins
         for key in classCode.get(constants.MIXINS):
             mixinCode = content.get(constants.CLASSES).get(key)
             for slot in mixinCode.get(constants.SLOTS):
                 if (slot not in classCode.get("slot_usage")): # this slot is not further specified in the class itself
                     slotCode = content.get(constants.SLOTS).get(slot)
-                    code += getSlotFormCode(slotCode, content, default_range, subclasses, level)
+                    code += getSlotFormCode(slotCode, content, default_range, subclasses, level, slot)
     
-    gen = (slot for slot in classCode.get(constants.SLOTS) if content.get(constants.SLOTS).get(slot).get(constants.RANGE) not in subclasses)
-    gen2 = (slot for slot in classCode.get(constants.SLOTS) if content.get(constants.SLOTS).get(slot).get(constants.RANGE) in subclasses)
     if (constants.SLOTS in classCode):
+        gen = (slot for slot in classCode.get(constants.SLOTS) if (content.get(constants.SLOTS).get(slot).get(constants.RANGE) not in subclasses and content.get(constants.SLOTS).get(slot) is not None))
         for slot in gen: #process slots of this class
             slotCode = content.get(constants.SLOTS).get(slot)
-            code += getSlotFormCode(slotCode, content, default_range, subclasses, level)
+            code += getSlotFormCode(slotCode, content, default_range, subclasses, level, slot)
     if (constants.ATTRIBUTES in classCode): #inline slots
         for slot in classCode.get(constants.ATTRIBUTES):
             slotCode = classCode.get(constants.ATTRIBUTES).get(slot)
-            code += getSlotFormCode(slotCode, content, default_range, subclasses, level)
+            code += getSlotFormCode(slotCode, content, default_range, subclasses, level, slot)
     if (constants.SLOTS in classCode):
+        gen2 = (slot for slot in classCode.get(constants.SLOTS) if (content.get(constants.SLOTS).get(slot).get(constants.RANGE) in subclasses and content.get(constants.SLOTS).get(slot) is not None))
         for slot in gen2: #process slots of this class where the range is a subclass
             slotCode = content.get(constants.SLOTS).get(slot)
-            code += getSlotFormCode(slotCode, content, default_range, subclasses, level)
+            code += getSlotFormCode(slotCode, content, default_range, subclasses, level, slot)
     return code
 
 
 def buildForm(content, html_only, output_directory, name, testEnv = False):
-    if (constants.NAME not in content and name == constants.DEFAULT): raise TypeError("The model metadata does not contain a 'name' field. Please make sure your model is valid")
-    NAME = name if (name != constants.DEFAULT) else content.get(constants.NAME)
+    if (constants.NAME not in content and name == constants.DEFAULT): 
+        warnings.warn("WARNING: The model metadata does not contain a 'name' field. Please make sure your model is valid")
+    NAME = name if (name != constants.DEFAULT) else (content.get(constants.NAME) if constants.NAME in content else "formDefault")
     OUTPUT_DIR = os.getcwd() if (output_directory == constants.CWD) else os.path.abspath(output_directory)
     HTML_PATH = os.path.join(OUTPUT_DIR, NAME + constants.HTML_EXT)
     
     with open(HTML_PATH, "w", encoding="utf-8") as f:
         if (html_only == True):
             f.write(constants.HTML_START_HTML_ONLY)
         else:
             f.write(constants.HTML_START)
             f.write(pkg_resources.resource_string(__name__, "bootstrap.css").decode('utf-8'))
             f.write("\n")
             f.write(pkg_resources.resource_string(__name__, "styles.css").decode('utf-8'))
             f.write(constants.HTML_START_PART2)
-        title = utils.extractName(content)
+        title = utils.extractName(content, "default")
         f.write("<h1>" + title + "</h1>\n")
         default_range = content.get(constants.DEFAULT_RANGE) if (constants.DEFAULT_RANGE in content) else None
         classes = []
         superClasses = []
         subClasses = [] # all classes that are technically containers/subclasses
         if (constants.SLOTS in content):
             for key in content.get(constants.SLOTS):
@@ -133,15 +136,15 @@
                         subClasses.append(slotCode.get(constants.RANGE))
 
             if (key not in superClasses and key not in subClasses):
                 classes.append(key)
         for key in classes:
             classCode = content.get(constants.CLASSES).get(key)
             if ("abstract" not in classCode or classCode.get("abstract") == False): # if the class is abstract, it should not be in the form
-                f.write(getClassFormCode(classCode, content, default_range, subClasses, 1))
+                f.write(getClassFormCode(classCode, content, default_range, subClasses, 1, key))
         f.write(constants.HTML_END)
         f.close()
         if (not html_only):
             options = { 
             'margin-bottom': '1cm', 
             'footer-right': '[page] of [topage]',
             }
```

### Comparing `linkmlformbuilder-0.1.8/src/LinkMLFormbuilder/slot_code_generators.py` & `linkmlformbuilder-0.1.9/src/LinkMLFormbuilder/slot_code_generators.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
        for enum in slotCode.get(constants.VALUES_FROM): enumList.append(enum)
     if (constants.RANGE in slotCode and constants.RANGE in content.get(constants.ENUMS)): enumList.append(slotCode.get(constants.RANGE))
     
     for enum in enumList:
       if (enum not in content.get(constants.ENUMS)):
           return getTextareaSlotCode(desc, required, propertyName, title, slotCode)
       enumCode = content.get(constants.ENUMS).get(enum)
-      enumName = utils.extractName(enumCode)
+      enumName = utils.extractName(enumCode, "")
       if (constants.PERMISSIBLE_VALUES in enumCode):
         code += getPermissibleValuesCode(enumCode.get(constants.PERMISSIBLE_VALUES), enumName, multivalued, required)
       else:
         code += '''<div class='answer-options'>\n<span class='values-from-dynamic'>{enumName}:</span>\n<textarea rows="6" class="form-control" id="{propertyName}"></textarea></div>'''.format(enumName = utils.capitalizeLabel(enumName), propertyName = enumCode.get(constants.NAME))
     code += "</div>\n"        
     return code
 
@@ -89,15 +89,15 @@
 
     code = '''<div class="mb-3">
             <div class="input-group">\n'''
     code += '''<span class="input-group-text">{slotName}</span>\n'''.format(slotName = utils.capitalizeLabel(title))
     code += '''<input type="text" class="form-control hideField">\n</div>\n'''
     code += '''<div class="form-text" id="{propertyName}-description">{desc}</div>\n'''.format(propertyName = propertyName, desc = utils.capitalizeLabel(desc))
     enumCode = slotCode.get(constants.ENUM_RANGE)
-    enumName = utils.extractName(slotCode) + " valueset" #inlined enums don't have names and titles, so it's generated from the slot itself
+    enumName = utils.extractName(slotCode, "") + " valueset" #inlined enums don't have names and titles, so it's generated from the slot itself
     if (constants.PERMISSIBLE_VALUES in enumCode):
         code += getPermissibleValuesCode(enumCode.get(constants.PERMISSIBLE_VALUES), enumName, multivalued, required)
     else:
       code += '''<div class='answer-options'>\n<span class='values-from-dynamic'>{enumName}:</span>\n<textarea rows="6" class="form-control" id="{enumNameNoSpace}"></textarea>\n</div>\n'''.format(enumName = utils.capitalizeLabel(enumName), propertyName = enumCode.get(constants.NAME), enumNameNoSpace = enumName.replace(" ", "_"))
     code += "</div>\n"     
     return code
```

### Comparing `linkmlformbuilder-0.1.8/src/LinkMLFormbuilder/styles.css` & `linkmlformbuilder-0.1.9/src/LinkMLFormbuilder/styles.css`

 * *Files identical despite different names*

### Comparing `linkmlformbuilder-0.1.8/src/LinkMLFormbuilder/utils.py` & `linkmlformbuilder-0.1.9/src/LinkMLFormbuilder/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import re
 from LinkMLFormbuilder import constants
+import warnings
 
 def extractAliases(sourceCode):
     name = ""
     if (constants.ALIASES in sourceCode or constants.STRUCTURED_ALIASES in sourceCode or constants.LOCAL_NAMES in sourceCode):
         name += " ("
         if (constants.ALIASES in sourceCode):
             for alias in sourceCode.get(constants.ALIASES):
@@ -17,35 +18,37 @@
                     name += structured_alias.get("literal_form") + constants.SEPARATOR
         if (constants.LOCAL_NAMES in sourceCode):
             for local_name in sourceCode.get(constants.LOCAL_NAMES):
                 name += local_name.get("local_name_value") + constants.SEPARATOR
         name = name[:-3] + ")"
     return name
 
-def extractName(classCode):
-    if (constants.NAME not in classCode): raise TypeError("Missing field: name")
+def extractName(classCode, key):
+    if (constants.NAME not in classCode): 
+        warnings.warn("WARNING: missing field name")
+        return key
     return (classCode.get(constants.TITLE) if (constants.TITLE in classCode) else classCode.get(constants.NAME)) + extractAliases(classCode)
 
 def extractDescription(itemCode):
     description = ""
     if (constants.DESCRIPTION in itemCode):
         description = normalize_description(itemCode.get(constants.DESCRIPTION))
     if (constants.ALT_DESCRIPTIONS in itemCode):
         description += " ("
         for alt_description in itemCode.get(constants.ALT_DESCRIPTIONS):
             description += normalize_description(alt_description.get(constants.DESCRIPTION)) + constants.SEPARATOR
         description = description[:-3] + ")"
     return description
 
-def extractSlotName(slotCode):
+def extractSlotName(slotCode, slot):
     name = ""
     if (((constants.MULTIVALUED in slotCode and slotCode.get(constants.MULTIVALUED) == False) or (constants.MAXIMUM_CARDINALITY in slotCode and slotCode.get(constants.MAXIMUM_CARDINALITY) == 1)) and constants.SINGULAR_NAME in slotCode):
         name = slotCode.get(constants.SINGULAR_NAME) # cardinality is either 0..1 or 1..1
     else:
-        name += extractName(slotCode)
+        name += extractName(slotCode, slot)
     return name
 
 def normalize_description(desc): # remove html tags <p><div>, remove anything in <i> and <img>
     p = re.compile(r'<.*?>')
     return p.sub('', desc).strip()
 
 def capitalizeLabel(label):
```

### Comparing `linkmlformbuilder-0.1.8/LICENSE` & `linkmlformbuilder-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `linkmlformbuilder-0.1.8/README.md` & `linkmlformbuilder-0.1.9/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 This tool was built as part of a larger project by a programmer who is not part of the LinkML development team. Therefore, errors in the interpretation of slots of the modelling language are possible. 
 
 ## Installation
 Under the hood, this tool uses the python adaptation of [PDFKIT](https://pypi.org/project/pdfkit/). It requires [wkhtmltopdf](https://wkhtmltopdf.org/index.html) to be installed on your system.
 
 Installation steps:
-1. Install and add wkhtmltopath
+1. Install and add wkhtmltopdf to path
     1. [Download here](https://wkhtmltopdf.org/downloads.html)
     2. Add the /bin to the path variable in your system's environment variables
 2. ```pip install linkmlformbuilder```
 
 ## Build from source
 1. Make sure the working directory contains the pyproject.toml file
 2. ```pip install build```
@@ -44,14 +44,17 @@
                         flag is missing
   --name [NAME]         Specify an alternative file name, do not specify a
                         file extension. By default, the filename of the
                         yamlfile is used for the HTML and optionally PDF files
 ```
 
 ## Changelog
+### Version 0.1.9
+- Missing 'name' field error is now a warning
+- Default options for missing 'name' fields
 ### Version 0.1.8
 - Throw error when field 'name' is missing from a model element
 - Auto close file on error (with statement)
 ### Version 0.1.7
 - Apply cardinality to slots
 ### Version 0.1.6
 - Overwrite existing output file(s) instead of throwing fileExists errors
```

### Comparing `linkmlformbuilder-0.1.8/pyproject.toml` & `linkmlformbuilder-0.1.9/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [tool.hatch.build.targets.sdist]
 include = [
     "src/LinkMLFormbuilder"
 ]
 
 [project]
 name = "LinkMLFormbuilder"
-version = "0.1.8"
+version = "0.1.9"
 authors = [
   { name="N. van Brummelen" },
 ]
 description = "Build forms from LinkML. Export to HTML or (basic) PDF"
 dependencies = ["pdfkit", "pyyaml"]
 readme = "README.md"
 requires-python = ">=3"
@@ -38,15 +38,15 @@
 [project.scripts]
 linkmlformbuilder = "LinkMLFormbuilder.formbuilder:cli"
 
 [tool.pytest.ini_options]
 minversion = "6.0"
 addopts = ["-ra", "--showlocals", "--strict-markers", "--strict-config"]
 xfail_strict = true
-filterwarnings = ["error"]
+filterwarnings = ["error", "ignore::UserWarning"]
 log_cli_level = "info"
 testpaths = [
   "tests",
 ]
 pythonpath = [
   "src"
 ]
```

### Comparing `linkmlformbuilder-0.1.8/PKG-INFO` & `linkmlformbuilder-0.1.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LinkMLFormbuilder
-Version: 0.1.8
+Version: 0.1.9
 Summary: Build forms from LinkML. Export to HTML or (basic) PDF
 Project-URL: Homepage, https://github.com/AmsterdamUMC/LinkMLFormBuilder#
 Project-URL: Issues, https://github.com/AmsterdamUMC/LinkMLFormBuilder/issues
 Author: N. van Brummelen
 License-Expression: GPL-3.0-only
 License-File: LICENSE
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -22,15 +22,15 @@
 
 This tool was built as part of a larger project by a programmer who is not part of the LinkML development team. Therefore, errors in the interpretation of slots of the modelling language are possible. 
 
 ## Installation
 Under the hood, this tool uses the python adaptation of [PDFKIT](https://pypi.org/project/pdfkit/). It requires [wkhtmltopdf](https://wkhtmltopdf.org/index.html) to be installed on your system.
 
 Installation steps:
-1. Install and add wkhtmltopath
+1. Install and add wkhtmltopdf to path
     1. [Download here](https://wkhtmltopdf.org/downloads.html)
     2. Add the /bin to the path variable in your system's environment variables
 2. ```pip install linkmlformbuilder```
 
 ## Build from source
 1. Make sure the working directory contains the pyproject.toml file
 2. ```pip install build```
@@ -61,14 +61,17 @@
                         flag is missing
   --name [NAME]         Specify an alternative file name, do not specify a
                         file extension. By default, the filename of the
                         yamlfile is used for the HTML and optionally PDF files
 ```
 
 ## Changelog
+### Version 0.1.9
+- Missing 'name' field error is now a warning
+- Default options for missing 'name' fields
 ### Version 0.1.8
 - Throw error when field 'name' is missing from a model element
 - Auto close file on error (with statement)
 ### Version 0.1.7
 - Apply cardinality to slots
 ### Version 0.1.6
 - Overwrite existing output file(s) instead of throwing fileExists errors
```

