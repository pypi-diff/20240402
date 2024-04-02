# Comparing `tmp/gender-spacy-0.0.4.tar.gz` & `tmp/gender-spacy-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\gender-spacy-0.0.4.tar", last modified: Tue Jan 24 00:57:12 2023, max compression
+gzip compressed data, was "gender-spacy-0.0.5.tar", last modified: Tue Apr  2 02:17:35 2024, max compression
```

## Comparing `gender-spacy-0.0.4.tar` & `gender-spacy-0.0.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-01-24 00:57:12.965150 gender-spacy-0.0.4/
--rw-rw-rw-   0        0        0      150 2023-01-11 23:52:15.000000 gender-spacy-0.0.4/MANIFEST.in
--rw-rw-rw-   0        0        0     4556 2023-01-24 00:57:12.964152 gender-spacy-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     4268 2023-01-23 23:11:24.000000 gender-spacy-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-01-24 00:57:12.944206 gender-spacy-0.0.4/gender_spacy/
--rw-rw-rw-   0        0        0       39 2023-01-11 23:54:56.000000 gender-spacy-0.0.4/gender_spacy/__init__.py
--rw-rw-rw-   0        0        0     3833 2023-01-24 00:56:48.000000 gender-spacy-0.0.4/gender_spacy/components.py
-drwxrwxrwx   0        0        0        0 2023-01-24 00:57:12.963155 gender-spacy-0.0.4/gender_spacy/data/
--rw-rw-rw-   0        0        0      461 2023-01-05 15:46:17.000000 gender-spacy-0.0.4/gender_spacy/data/gender_pronouns.csv
--rw-rw-rw-   0        0        0     4689 2023-01-24 00:52:16.000000 gender-spacy-0.0.4/gender_spacy/data/project.toml
--rw-rw-rw-   0        0        0     2943 2023-01-05 21:53:58.000000 gender-spacy-0.0.4/gender_spacy/data/pronoun_patterns
--rw-rw-rw-   0        0        0     6639 2023-01-24 00:45:54.000000 gender-spacy-0.0.4/gender_spacy/gender_spacy.py
-drwxrwxrwx   0        0        0        0 2023-01-24 00:57:12.958207 gender-spacy-0.0.4/gender_spacy.egg-info/
--rw-rw-rw-   0        0        0     4556 2023-01-24 00:57:12.000000 gender-spacy-0.0.4/gender_spacy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      394 2023-01-24 00:57:12.000000 gender-spacy-0.0.4/gender_spacy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-24 00:57:12.000000 gender-spacy-0.0.4/gender_spacy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       98 2023-01-24 00:57:12.000000 gender-spacy-0.0.4/gender_spacy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-01-24 00:57:12.000000 gender-spacy-0.0.4/gender_spacy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-01-24 00:57:12.965150 gender-spacy-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      944 2023-01-24 00:46:43.000000 gender-spacy-0.0.4/setup.py
+drwxr-xr-x   0 wjbmattingly   (501) staff       (20)        0 2024-04-02 02:17:35.312579 gender-spacy-0.0.5/
+-rw-r--r--   0 wjbmattingly   (501) staff       (20)      146 2024-04-02 02:12:01.000000 gender-spacy-0.0.5/MANIFEST.in
+-rw-r--r--   0 wjbmattingly   (501) staff       (20)     4481 2024-04-02 02:17:35.312445 gender-spacy-0.0.5/PKG-INFO
+-rw-r--r--   0 wjbmattingly   (501) staff       (20)     4281 2024-04-02 02:12:01.000000 gender-spacy-0.0.5/README.md
+drwxr-xr-x   0 wjbmattingly   (501) staff       (20)        0 2024-04-02 02:17:35.310865 gender-spacy-0.0.5/gender_spacy/
+-rw-r--r--   0 wjbmattingly   (501) staff       (20)       39 2024-04-02 02:12:01.000000 gender-spacy-0.0.5/gender_spacy/__init__.py
+-rw-r--r--   0 wjbmattingly   (501) staff       (20)     3723 2024-04-02 02:12:01.000000 gender-spacy-0.0.5/gender_spacy/components.py
+drwxr-xr-x   0 wjbmattingly   (501) staff       (20)        0 2024-04-02 02:17:35.312101 gender-spacy-0.0.5/gender_spacy/data/
+-rw-r--r--   0 wjbmattingly   (501) staff       (20)      449 2024-04-02 02:12:01.000000 gender-spacy-0.0.5/gender_spacy/data/gender_pronouns.csv
+-rw-r--r--   0 wjbmattingly   (501) staff       (20)     4635 2024-04-02 02:12:01.000000 gender-spacy-0.0.5/gender_spacy/data/project.toml
+-rw-r--r--   0 wjbmattingly   (501) staff       (20)     2901 2024-04-02 02:12:01.000000 gender-spacy-0.0.5/gender_spacy/data/pronoun_patterns
+-rw-r--r--   0 wjbmattingly   (501) staff       (20)     6480 2024-04-02 02:12:01.000000 gender-spacy-0.0.5/gender_spacy/gender_spacy.py
+drwxr-xr-x   0 wjbmattingly   (501) staff       (20)        0 2024-04-02 02:17:35.311550 gender-spacy-0.0.5/gender_spacy.egg-info/
+-rw-r--r--   0 wjbmattingly   (501) staff       (20)     4481 2024-04-02 02:17:35.000000 gender-spacy-0.0.5/gender_spacy.egg-info/PKG-INFO
+-rw-r--r--   0 wjbmattingly   (501) staff       (20)      394 2024-04-02 02:17:35.000000 gender-spacy-0.0.5/gender_spacy.egg-info/SOURCES.txt
+-rw-r--r--   0 wjbmattingly   (501) staff       (20)        1 2024-04-02 02:17:35.000000 gender-spacy-0.0.5/gender_spacy.egg-info/dependency_links.txt
+-rw-r--r--   0 wjbmattingly   (501) staff       (20)       73 2024-04-02 02:17:35.000000 gender-spacy-0.0.5/gender_spacy.egg-info/requires.txt
+-rw-r--r--   0 wjbmattingly   (501) staff       (20)       13 2024-04-02 02:17:35.000000 gender-spacy-0.0.5/gender_spacy.egg-info/top_level.txt
+-rw-r--r--   0 wjbmattingly   (501) staff       (20)       38 2024-04-02 02:17:35.312625 gender-spacy-0.0.5/setup.cfg
+-rw-r--r--   0 wjbmattingly   (501) staff       (20)      923 2024-04-02 02:12:30.000000 gender-spacy-0.0.5/setup.py
```

### Comparing `gender-spacy-0.0.4/PKG-INFO` & `gender-spacy-0.0.5/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,88 +1,82 @@
-Metadata-Version: 2.1
-Name: gender-spacy
-Version: 0.0.4
-Summary: A spaCy component for identifying grammatical gender in English texts.
-Author: WJB Mattingly
-Description-Content-Type: text/markdown
-
-
-![gender spacy logo](https://github.com/sidatasciencelab/gender-spacy/raw/main/images/genderspacy-logo.png)
-
-# About
-
-Gender spaCy is a heuristic and machine learning pipeline that allows users to identify gender in an ethical way using gender-specific context. It is designed to sit alongside a standard spaCy pipeline (only English supported currently). The majority of the pipeline is rules-based, relying on titles and pronouns to identify gender as presented in the text. **It is important to note that this pipeline does not seek to assign gender to an individual, rather contextually identify an entity's gender within the context of a text.**
-
-There are Python libraries, such as gender-resolver that assign gender based on the statistical usage of first names in a given region. This, however, gets into problematic territory and is not as reliable as gender-based context (such as titles and pronouns). As a result, this pipeline opts out of leveraging these libraries. Instead, entities identified as PERSON by the spaCy NER model are altered to the span label of PERSON_UNKNOWN. Next, this pipeline leverages the new experimental coreference resolution model from ExplosionAI. It looks at all clusters of linked tokens. If any of them align with PERSON_UNKNOWN tags *and* gender-specific pronouns are used, the entity's label is changed to a gender-specific label, e.g. PERSON_FEMALE, PERSON_MALE, PERSON_NEUTRAL. In addition, terms that are nouns that are linked to a specific person receive the tag "REL_MALE/FEMALE_COREF".
-
-In addition to this, all gender-neutral pronouns are also identified and labeled as spans. This includes male, female, and gender neutral pronouns. Even transformer models have difficulty correctly parsing certain gender neutral pronouns due to their toponym nature, such as "per" which can function in English as an adverb (Per our discusion yesterday, I want to go to the store.) or as a gender neutral pronoun (Per went to the store yesterday). With a few extra rules, Gender spaCy corrects the POS tags for these toponyms in addition to placing all pronouns in the spans ruler.
-
-Users can access all gender span data under doc.spans["ruler].
-
-# Installation
-
-Because this pipeline leverages spaCy's new experimental coreference resolution model, it is best to install Gender spaCy in a fresh environment.
-
-First, it is good to create a new environment.
-
-```python
-conda create --name="gender-spacy" python=3.9
-```
-
-Now, activate the environment:
-
-```python
-conda activate gender-spacy
-```
-
-Next, install GenderSpaCy
-
-```python
-pip install gender-spacy
-```
-
-Finally, for the pipeline to perform coreference resolution, you should install the latest version of the spaCy experimental coreference resolution model.
-
-```python
-pip install https://github.com/explosion/spacy-experimental/releases/download/v0.6.0/en_coreference_web_trf-3.4.0a0-py3-none-any.whl
-```
-
-
-
-# Usage
-
-```python
-
-# import the library
-from gender_spacy import gender_spacy as gs
-
-# create the GenderParser nlp class.
-# This will take one argument: the spaCy model you wish to use
-nlp = gs.GenderParser("en_core_web_sm")
-
-# create a text and pass it to the the nlp via the process_doc() method.
-text = """
-During the year Miss Densmore arranged in final order 245 songs to accompany her manuscript on Seminole music and revised portions of the text to conform to this arrangement of the material. 
-
-In December 1941 Miss Densmore was appointed as consultant at The National Archives for work in connection with the Smithsonian Densmore collection of sound recordings of American Indian music, and duiing the ensuing months she was engaged in planning the organization of the collection.
-"""
-doc = nlp.process_doc(text)
-
-# perform coreference resolution on the doc container
-# This part of the library comes from spacy-experimental
-doc = nlp.coref_resolution()
-
-# Visualize the result:
-nlp.visualize()
-```
-
-## Expected Result
-
-![result demo](https://github.com/sidatasciencelab/gender-spacy/raw/main/images/result.JPG)
-
-
-
-# CITATIONS
-Source for gender pronouns: https://uwm.edu/lgbtrc/support/gender-pronouns/
-
-Source for Coreference Resolution: https://explosion.ai/blog/coref
-Discussion for Coref Code: https://github.com/explosion/spaCy/discussions/11585
+
+![gender spacy logo](https://github.com/sidatasciencelab/gender-spacy/raw/main/images/genderspacy-logo.png)
+
+# About
+
+Gender spaCy is a heuristic and machine learning pipeline that allows users to identify gender in an ethical way using gender-specific context. It is designed to sit alongside a standard spaCy pipeline (only English supported currently). The majority of the pipeline is rules-based, relying on titles and pronouns to identify gender as presented in the text. **It is important to note that this pipeline does not seek to assign gender to an individual, rather contextually identify an entity's gender within the context of a text.**
+
+There are Python libraries, such as gender-resolver that assign gender based on the statistical usage of first names in a given region. This, however, gets into problematic territory and is not as reliable as gender-based context (such as titles and pronouns). As a result, this pipeline opts out of leveraging these libraries. Instead, entities identified as PERSON by the spaCy NER model are altered to the span label of PERSON_UNKNOWN. Next, this pipeline leverages the new experimental coreference resolution model from ExplosionAI. It looks at all clusters of linked tokens. If any of them align with PERSON_UNKNOWN tags *and* gender-specific pronouns are used, the entity's label is changed to a gender-specific label, e.g. PERSON_FEMALE, PERSON_MALE, PERSON_NEUTRAL. In addition, terms that are nouns that are linked to a specific person receive the tag "REL_MALE/FEMALE_COREF".
+
+In addition to this, all gender-neutral pronouns are also identified and labeled as spans. This includes male, female, and gender neutral pronouns. Even transformer models have difficulty correctly parsing certain gender neutral pronouns due to their toponym nature, such as "per" which can function in English as an adverb (Per our discusion yesterday, I want to go to the store.) or as a gender neutral pronoun (Per went to the store yesterday). With a few extra rules, Gender spaCy corrects the POS tags for these toponyms in addition to placing all pronouns in the spans ruler.
+
+Users can access all gender span data under doc.spans["ruler].
+
+# Installation
+
+Because this pipeline leverages spaCy's new experimental coreference resolution model, it is best to install Gender spaCy in a fresh environment.
+
+First, it is good to create a new environment.
+
+```python
+conda create --name="gender-spacy" python=3.9
+```
+
+Now, activate the environment:
+
+```python
+conda activate gender-spacy
+```
+
+Next, install GenderSpaCy
+
+```python
+pip install gender-spacy
+```
+
+Finally, for the pipeline to perform coreference resolution, you should install the latest version of the spaCy experimental coreference resolution model.
+
+```python
+pip install https://github.com/explosion/spacy-experimental/releases/download/v0.6.0/en_coreference_web_trf-3.4.0a0-py3-none-any.whl
+```
+
+
+
+# Usage
+
+```python
+
+# import the library
+from gender_spacy import gender_spacy as gs
+
+# create the GenderParser nlp class.
+# This will take one argument: the spaCy model you wish to use
+nlp = gs.GenderParser("en_core_web_sm")
+
+# create a text and pass it to the the nlp via the process_doc() method.
+text = """
+Maya Angelou was an American memoirist, popular poet, and civil rights activist. She published seven autobiographies, three books of essays, several books of poetry, and is credited with a list of plays, movies, and television shows spanning over 50 years.
+
+Jerome Allen Seinfeld is an American stand-up comedian, actor, writer, and producer. He is best known for playing a semi-fictionalized version of himself in the sitcom Seinfeld (1989–1998), which he created and wrote with Larry David.
+"""
+doc = nlp.process_doc(text)
+
+# perform coreference resolution on the doc container
+# This part of the library comes from spacy-experimental
+doc = nlp.coref_resolution()
+
+# Visualize the result:
+nlp.visualize()
+```
+
+## Expected Result
+
+![result demo](https://github.com/sidatasciencelab/gender-spacy/raw/main/images/demo.JPG)
+
+
+
+# CITATIONS
+Source for gender pronouns: https://uwm.edu/lgbtrc/support/gender-pronouns/
+
+Source for Coreference Resolution: https://explosion.ai/blog/coref
+
+Discussion for Coref Code: https://github.com/explosion/spaCy/discussions/11585
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `gender-spacy-0.0.4/README.md` & `gender-spacy-0.0.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+Metadata-Version: 2.1
+Name: gender-spacy
+Version: 0.0.5
+Summary: A spaCy component for identifying grammatical gender in English texts.
+Author: WJB Mattingly
+Description-Content-Type: text/markdown
+
 
 ![gender spacy logo](https://github.com/sidatasciencelab/gender-spacy/raw/main/images/genderspacy-logo.png)
 
 # About
 
 Gender spaCy is a heuristic and machine learning pipeline that allows users to identify gender in an ethical way using gender-specific context. It is designed to sit alongside a standard spaCy pipeline (only English supported currently). The majority of the pipeline is rules-based, relying on titles and pronouns to identify gender as presented in the text. **It is important to note that this pipeline does not seek to assign gender to an individual, rather contextually identify an entity's gender within the context of a text.**
 
@@ -50,32 +57,33 @@
 
 # create the GenderParser nlp class.
 # This will take one argument: the spaCy model you wish to use
 nlp = gs.GenderParser("en_core_web_sm")
 
 # create a text and pass it to the the nlp via the process_doc() method.
 text = """
-During the year Miss Densmore arranged in final order 245 songs to accompany her manuscript on Seminole music and revised portions of the text to conform to this arrangement of the material. 
+Maya Angelou was an American memoirist, popular poet, and civil rights activist. She published seven autobiographies, three books of essays, several books of poetry, and is credited with a list of plays, movies, and television shows spanning over 50 years.
 
-In December 1941 Miss Densmore was appointed as consultant at The National Archives for work in connection with the Smithsonian Densmore collection of sound recordings of American Indian music, and duiing the ensuing months she was engaged in planning the organization of the collection.
+Jerome Allen Seinfeld is an American stand-up comedian, actor, writer, and producer. He is best known for playing a semi-fictionalized version of himself in the sitcom Seinfeld (1989–1998), which he created and wrote with Larry David.
 """
 doc = nlp.process_doc(text)
 
 # perform coreference resolution on the doc container
 # This part of the library comes from spacy-experimental
 doc = nlp.coref_resolution()
 
 # Visualize the result:
 nlp.visualize()
 ```
 
 ## Expected Result
 
-![result demo](https://github.com/sidatasciencelab/gender-spacy/raw/main/images/result.JPG)
+![result demo](https://github.com/sidatasciencelab/gender-spacy/raw/main/images/demo.JPG)
 
 
 
 # CITATIONS
 Source for gender pronouns: https://uwm.edu/lgbtrc/support/gender-pronouns/
 
 Source for Coreference Resolution: https://explosion.ai/blog/coref
-Discussion for Coref Code: https://github.com/explosion/spaCy/discussions/11585
+
+Discussion for Coref Code: https://github.com/explosion/spaCy/discussions/11585
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `gender-spacy-0.0.4/gender_spacy/components.py` & `gender-spacy-0.0.5/gender_spacy/components.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,110 +1,110 @@
-import pandas as pd
-import spacy
-from spacy.language import Language
-from spacy.tokens import Token, Span, Doc
-import re
-import string
-
-import toml
-import srsly
-
-import os
-from pathlib import Path
-from distutils.sysconfig import get_python_lib
-
-BASE_DIR = None
-if os.path.isfile(get_python_lib() + "/genderspacy"):
-  BASE_DIR = get_python_lib() + "/genderspacy"
-else:
-  BASE_DIR = os.path.dirname(__file__)
-
-gender_pronoun_file = BASE_DIR + "/data/gender_pronouns.csv"
-project_toml = BASE_DIR + "/data/project.toml"
-pronoun_patterns = BASE_DIR + "/data/pronoun_patterns"
-
-project_data = toml.load(project_toml)
-
-regex = project_data["regex"]
-titles = project_data["titles"]
-pipeline_data = project_data["pipeline_data"]
-
-
-regex_patterns = {}
-all_titles = ""
-for title_name, title_list in titles.items():
-    title_combined = "|".join(title_list)
-    all_titles = all_titles+f"{title_combined}|"
-    pattern = regex["individual"].replace("<GENDER_TITLES>", title_combined).replace("\\\\", "\\")
-    regex_patterns[title_name] = pattern
-regex_patterns["spouse"] = regex["spouse"].replace("<GENDER_TITLES>", all_titles).replace("\\\\", "\\").replace("|)", ")")
-all_titles = all_titles[:-1]
-
-
-df = pd.read_csv(gender_pronoun_file)
-pronouns = df.values.tolist()
-
-unique_pronouns = []
-for p in pronouns:
-    for item in p[1:]:
-        unique_pronouns.append(item)
-unique_pronouns = list(set(unique_pronouns))
-unique_pronouns.sort()
-
-@Language.component("people_and_spouse")
-def people_and_spouse(doc):
-    original_ents = list(doc.spans["ruler"])
-    text = doc.text
-    for label, pattern in regex_patterns.items():
-        if label == "spouse":
-            label=f"COLLECTIVE_SPOUSAL"
-        else:
-            label=f"PERSON_{label.upper()}"
-        text = doc.text
-        new_ents = []
-        for match in re.finditer(pattern, doc.text):
-            start, end = match.span()
-            span = doc.char_span(start, end, alignment_mode="expand")
-            if span != None:
-                if span.text[-1] in string.punctuation:
-                    span.end = span.end-1
-                start, end, name = span.start, span.end, span.text
-                tmp_span = Span(doc, start, end, label=label)
-                for i, token in enumerate(tmp_span):
-                    if i > 2 and doc[(tmp_span.start+i)-2].text not in pattern.replace("\\", ""):
-                        if token.is_sent_start == True:
-                            tmp_span.end=tmp_span.start+i-1
-                original_ents.append(tmp_span)
-    doc.spans["ruler"] = original_ents
-    return doc
-
-@Language.component("pronoun_id")
-def pronoun_id(doc):
-    original_spans = list(doc.spans["ruler"])
-    new_spans = []
-    for span in doc.spans["ruler"]:
-        if any(span.text.lower() in p for p in pronouns):
-            for option in pronouns:
-                if span.text.lower() in option:
-                    span.label_ = f"{option[0].upper()}_PRONOUN"
-                    new_spans.append(span)
-                    break
-        else:
-            new_spans.append(span)
-    doc.spans["ruler"] = new_spans
-    return doc
-
-@Language.component("pronoun_resolver")
-def pronoun_resolver(doc):
-    for i, token in enumerate(doc):
-        if any(token.text.lower() in p for p in pronouns):
-            if token.text.lower() == "per" and token.pos_ != "PRON":
-                if doc[i-1].lemma_ != "as" and token.is_sent_start == False:
-                    token.pos_ = "PRON"
-                elif doc[i+1].pos_ not in ["PRON", "DET"]:
-                    # print(doc[i+1].pos_)
-                    token.pos_ = "PRON"
-                else:
-                    token.pos_ = "ADP"
-            else:
-                token.pos_ = "PRON"
-    return doc
+import pandas as pd
+import spacy
+from spacy.language import Language
+from spacy.tokens import Token, Span, Doc
+import re
+import string
+
+import toml
+import srsly
+
+import os
+from pathlib import Path
+from distutils.sysconfig import get_python_lib
+
+BASE_DIR = None
+if os.path.isfile(get_python_lib() + "/genderspacy"):
+  BASE_DIR = get_python_lib() + "/genderspacy"
+else:
+  BASE_DIR = os.path.dirname(__file__)
+
+gender_pronoun_file = BASE_DIR + "/data/gender_pronouns.csv"
+project_toml = BASE_DIR + "/data/project.toml"
+pronoun_patterns = BASE_DIR + "/data/pronoun_patterns"
+
+project_data = toml.load(project_toml)
+
+regex = project_data["regex"]
+titles = project_data["titles"]
+pipeline_data = project_data["pipeline_data"]
+
+
+regex_patterns = {}
+all_titles = ""
+for title_name, title_list in titles.items():
+    title_combined = "|".join(title_list)
+    all_titles = all_titles+f"{title_combined}|"
+    pattern = regex["individual"].replace("<GENDER_TITLES>", title_combined).replace("\\\\", "\\")
+    regex_patterns[title_name] = pattern
+regex_patterns["spouse"] = regex["spouse"].replace("<GENDER_TITLES>", all_titles).replace("\\\\", "\\").replace("|)", ")")
+all_titles = all_titles[:-1]
+
+
+df = pd.read_csv(gender_pronoun_file)
+pronouns = df.values.tolist()
+
+unique_pronouns = []
+for p in pronouns:
+    for item in p[1:]:
+        unique_pronouns.append(item)
+unique_pronouns = list(set(unique_pronouns))
+unique_pronouns.sort()
+
+@Language.component("people_and_spouse")
+def people_and_spouse(doc):
+    original_ents = list(doc.spans["ruler"])
+    text = doc.text
+    for label, pattern in regex_patterns.items():
+        if label == "spouse":
+            label=f"COLLECTIVE_SPOUSAL"
+        else:
+            label=f"PERSON_{label.upper()}"
+        text = doc.text
+        new_ents = []
+        for match in re.finditer(pattern, doc.text):
+            start, end = match.span()
+            span = doc.char_span(start, end, alignment_mode="expand")
+            if span != None:
+                if span.text[-1] in string.punctuation:
+                    span.end = span.end-1
+                start, end, name = span.start, span.end, span.text
+                tmp_span = Span(doc, start, end, label=label)
+                for i, token in enumerate(tmp_span):
+                    if i > 2 and doc[(tmp_span.start+i)-2].text not in pattern.replace("\\", ""):
+                        if token.is_sent_start == True:
+                            tmp_span.end=tmp_span.start+i-1
+                original_ents.append(tmp_span)
+    doc.spans["ruler"] = original_ents
+    return doc
+
+@Language.component("pronoun_id")
+def pronoun_id(doc):
+    original_spans = list(doc.spans["ruler"])
+    new_spans = []
+    for span in doc.spans["ruler"]:
+        if any(span.text.lower() in p for p in pronouns):
+            for option in pronouns:
+                if span.text.lower() in option:
+                    span.label_ = f"{option[0].upper()}_PRONOUN"
+                    new_spans.append(span)
+                    break
+        else:
+            new_spans.append(span)
+    doc.spans["ruler"] = new_spans
+    return doc
+
+@Language.component("pronoun_resolver")
+def pronoun_resolver(doc):
+    for i, token in enumerate(doc):
+        if any(token.text.lower() in p for p in pronouns):
+            if token.text.lower() == "per" and token.pos_ != "PRON":
+                if doc[i-1].lemma_ != "as" and token.is_sent_start == False:
+                    token.pos_ = "PRON"
+                elif doc[i+1].pos_ not in ["PRON", "DET"]:
+                    # print(doc[i+1].pos_)
+                    token.pos_ = "PRON"
+                else:
+                    token.pos_ = "ADP"
+            else:
+                token.pos_ = "PRON"
+    return doc
```

### Comparing `gender-spacy-0.0.4/gender_spacy/data/project.toml` & `gender-spacy-0.0.5/gender_spacy/data/project.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,294 +1,290 @@
-00000000: 5b70 6970 656c 696e 655f 6461 7461 5d0d  [pipeline_data].
-00000010: 0a6e 616d 6520 3d20 2267 656e 6465 7273  .name = "genders
-00000020: 7061 6379 220d 0a61 7574 686f 7220 3d20  pacy"..author = 
-00000030: 2257 2e4a 2e42 2e20 4d61 7474 696e 676c  "W.J.B. Mattingl
-00000040: 7922 0d0a 7572 6c20 3d20 2268 7474 7073  y"..url = "https
-00000050: 3a2f 2f67 6974 6875 622e 636f 6d2f 776a  ://github.com/wj
-00000060: 626d 6174 7469 6e67 6c79 2f67 656e 6465  bmattingly/gende
-00000070: 7273 7061 6379 220d 0a76 6572 7369 6f6e  rspacy"..version
-00000080: 203d 2022 302e 302e 3122 0d0a 6465 7363   = "0.0.1"..desc
-00000090: 7269 7074 696f 6e20 3d20 2254 6869 7320  ription = "This 
-000000a0: 6973 2061 2073 7061 4379 2070 6970 656c  is a spaCy pipel
-000000b0: 696e 6520 666f 7220 6865 6c70 696e 6720  ine for helping 
-000000c0: 6964 656e 7469 6679 2067 656e 6465 7220  identify gender 
-000000d0: 696e 2074 6578 7473 2e20 4974 2069 7320  in texts. It is 
-000000e0: 696e 636c 7573 6976 6520 6f66 2066 656d  inclusive of fem
-000000f0: 616c 652c 206d 616c 652c 2061 6e64 206e  ale, male, and n
-00000100: 6575 7472 616c 2067 656e 6465 7220 7072  eutral gender pr
-00000110: 6f6e 6f75 6e73 2f74 6974 6c65 732e 220d  onouns/titles.".
-00000120: 0a0d 0a5b 636f 6c6f 7273 5d0d 0a4e 4555  ...[colors]..NEU
-00000130: 5452 414c 5f50 524f 4e4f 554e 3d22 2366  TRAL_PRONOUN="#f
-00000140: 6662 3666 3822 0d0a 5045 5253 4f4e 5f4e  fb6f8"..PERSON_N
-00000150: 4555 5452 414c 3d22 2366 6662 3666 3822  EUTRAL="#ffb6f8"
-00000160: 0d0a 5245 4c5f 4e45 5554 5241 4c5f 434f  ..REL_NEUTRAL_CO
-00000170: 5245 463d 2223 6666 6236 6638 220d 0a0d  REF="#ffb6f8"...
-00000180: 0a46 454d 414c 455f 5052 4f4e 4f55 4e3d  .FEMALE_PRONOUN=
-00000190: 2223 6236 6666 6637 220d 0a50 4552 534f  "#b6fff7"..PERSO
-000001a0: 4e5f 4645 4d41 4c45 3d22 2362 3666 6666  N_FEMALE="#b6fff
-000001b0: 3722 0d0a 5045 5253 4f4e 5f46 454d 414c  7"..PERSON_FEMAL
-000001c0: 455f 434f 5245 463d 2223 6236 6666 6637  E_COREF="#b6fff7
-000001d0: 220d 0a52 454c 5f46 454d 414c 455f 434f  "..REL_FEMALE_CO
-000001e0: 5245 463d 2223 6236 6666 6637 220d 0a0d  REF="#b6fff7"...
-000001f0: 0a4d 414c 455f 5052 4f4e 4f55 4e3d 2223  .MALE_PRONOUN="#
-00000200: 6236 6237 6666 220d 0a50 4552 534f 4e5f  b6b7ff"..PERSON_
-00000210: 4d41 4c45 3d22 2362 3662 3766 6622 0d0a  MALE="#b6b7ff"..
-00000220: 5045 5253 4f4e 5f4d 414c 455f 434f 5245  PERSON_MALE_CORE
-00000230: 463d 2223 6236 6237 6666 220d 0a52 454c  F="#b6b7ff"..REL
-00000240: 5f4d 414c 455f 434f 5245 463d 2223 6236  _MALE_COREF="#b6
-00000250: 6237 6666 220d 0a0d 0a43 4f4c 4c45 4354  b7ff"....COLLECT
-00000260: 4956 455f 5350 4f55 5341 4c3d 2223 6637  IVE_SPOUSAL="#f7
-00000270: 6666 6236 220d 0a0d 0a5b 7072 6f6e 6f75  ffb6"....[pronou
-00000280: 6e73 5d0d 0a6d 616c 653d 205b 2768 6527  ns]..male= ['he'
-00000290: 2c20 2768 696d 272c 2027 6869 7327 2c20  , 'him', 'his', 
-000002a0: 2768 6973 272c 2027 6869 6d73 656c 6627  'his', 'himself'
-000002b0: 5d0d 0a66 656d 616c 6520 3d20 5b27 7368  ]..female = ['sh
-000002c0: 6527 2c20 2768 6572 272c 2027 6865 7227  e', 'her', 'her'
-000002d0: 2c20 2768 6572 7327 2c20 2768 6572 7365  , 'hers', 'herse
-000002e0: 6c66 275d 0d0a 6e65 7574 7261 6c20 3d20  lf']..neutral = 
-000002f0: 5b27 6661 6527 2c20 2766 6165 7227 2c20  ['fae', 'faer', 
-00000300: 2766 6165 7227 2c20 2766 6165 7273 272c  'faer', 'faers',
-00000310: 2027 6661 6572 7365 6c66 272c 0d0a 2020   'faerself',..  
-00000320: 2020 2020 2020 2020 2020 2761 6527 2c20            'ae', 
-00000330: 2761 6572 272c 2027 6165 7227 2c20 2766  'aer', 'aer', 'f
-00000340: 6165 7273 272c 2027 6661 6572 7365 6c66  aers', 'faerself
-00000350: 272c 0d0a 2020 2020 2020 2020 2020 2020  ',..            
-00000360: 2765 272c 2027 656d 272c 2027 6569 7227  'e', 'em', 'eir'
-00000370: 2c20 2765 6972 7327 2c20 2765 6972 7365  , 'eirs', 'eirse
-00000380: 6c66 272c 0d0a 2020 2020 2020 2020 2020  lf',..          
-00000390: 2020 2765 7927 2c20 2765 6d27 2c20 2765    'ey', 'em', 'e
-000003a0: 6972 272c 2027 6569 7273 272c 2027 6569  ir', 'eirs', 'ei
-000003b0: 7273 656c 6627 2c0d 0a20 2020 2020 2020  rself',..       
-000003c0: 2020 2020 2027 7065 7227 2c20 2770 6572       'per', 'per
-000003d0: 272c 2027 7065 7273 272c 2027 7065 7273  ', 'pers', 'pers
-000003e0: 272c 2027 7065 7273 656c 6627 2c0d 0a20  ', 'perself',.. 
-000003f0: 2020 2020 2020 2020 2020 2027 7468 6579             'they
-00000400: 272c 2027 7468 656d 272c 2027 7468 6569  ', 'them', 'thei
-00000410: 7227 2c20 2774 6865 6972 7327 2c20 2774  r', 'theirs', 't
-00000420: 6865 6d73 656c 6627 2c0d 0a20 2020 2020  hemself',..     
-00000430: 2020 2020 2020 2027 7665 272c 2027 7665         've', 've
-00000440: 7227 2c20 2776 6973 272c 2027 7669 7327  r', 'vis', 'vis'
-00000450: 2c20 2776 6572 6573 656c 6627 2c0d 0a20  , 'vereself',.. 
-00000460: 2020 2020 2020 2020 2020 2027 7865 272c             'xe',
-00000470: 2027 7865 6d27 2c20 2778 7972 272c 2027   'xem', 'xyr', '
-00000480: 7879 7273 272c 2027 7865 6d73 656c 6627  xyrs', 'xemself'
-00000490: 2c27 7a65 272c 0d0a 2020 2020 2020 2020  ,'ze',..        
-000004a0: 2020 2020 2768 6972 272c 2027 6869 7227      'hir', 'hir'
-000004b0: 2c20 2768 6972 7327 2c20 2768 6972 7365  , 'hirs', 'hirse
-000004c0: 6c66 272c 0d0a 2020 2020 2020 2020 2020  lf',..          
-000004d0: 2020 277a 6965 272c 2027 6869 7227 2c20    'zie', 'hir', 
-000004e0: 2768 6972 272c 2027 6869 7273 272c 2027  'hir', 'hirs', '
-000004f0: 6869 7273 656c 6627 5d0d 0a0d 0a5b 7669  hirself']....[vi
-00000500: 7375 616c 697a 655f 7061 7261 6d73 5d0d  sualize_params].
-00000510: 0a73 7061 6e73 5f6b 6579 3d22 7275 6c65  .spans_key="rule
-00000520: 7222 0d0a 0d0a 5b72 6567 6578 5d0d 0a69  r"....[regex]..i
-00000530: 6e64 6976 6964 7561 6c20 3d20 2228 3c47  ndividual = "(<G
-00000540: 454e 4445 525f 5449 544c 4553 3e29 285c  ENDER_TITLES>)(\
-00000550: 5c2e 292a 205b 412d 5a5d 5b61 2d7a 5d2a  \.)* [A-Z][a-z]*
-00000560: 2820 5b41 2d5a 5d5b 612d 7a5d 2a29 2a22  ( [A-Z][a-z]*)*"
-00000570: 0d0a 7370 6f75 7365 203d 2022 283c 4745  ..spouse = "(<GE
-00000580: 4e44 4552 5f54 4954 4c45 533e 2928 5c5c  NDER_TITLES>)(\\
-00000590: 2e29 2a20 2861 6e64 7c26 2920 283c 4745  .)* (and|&) (<GE
-000005a0: 4e44 4552 5f54 4954 4c45 533e 2928 5c5c  NDER_TITLES>)(\\
-000005b0: 2e29 2a20 5b41 2d5a 5d5b 612d 7a5d 2a28  .)* [A-Z][a-z]*(
-000005c0: 205b 412d 5a5d 5b61 2d7a 5d2a 292a 220d   [A-Z][a-z]*)*".
-000005d0: 0a0d 0a5b 7469 746c 6573 5d0d 0a66 656d  ...[titles]..fem
-000005e0: 616c 6520 3d20 5b22 4d72 7322 2c20 224d  ale = ["Mrs", "M
-000005f0: 7322 2c20 224d 6973 7322 2c20 224d 6164  s", "Miss", "Mad
-00000600: 616d 222c 2022 4d64 6d22 5d0d 0a6d 616c  am", "Mdm"]..mal
-00000610: 6520 3d20 5b22 4d72 225d 0d0a 6e65 7574  e = ["Mr"]..neut
-00000620: 7261 6c20 3d20 5b22 4d78 222c 2022 496e  ral = ["Mx", "In
-00000630: 6422 2c20 224d 7372 222c 2022 4d72 6522  d", "Msr", "Mre"
-00000640: 2c20 224d 6973 6322 2c20 2250 7222 2c0d  , "Misc", "Pr",.
-00000650: 0a0d 0a20 2020 2020 2020 2020 2023 2050  ...          # P
-00000660: 726f 6665 7373 696f 6e61 6c0d 0a20 2020  rofessional..   
-00000670: 2020 2020 2020 2022 4472 222c 2022 446f         "Dr", "Do
-00000680: 6374 6f72 222c 2022 5072 6f66 222c 2022  ctor", "Prof", "
-00000690: 5072 6f66 6573 736f 7222 2c0d 0a20 2020  Professor",..   
-000006a0: 2020 2020 2020 2023 204d 696c 6974 6172         # Militar
-000006b0: 790d 0a20 2020 2020 2020 2020 2027 314c  y..          '1L
-000006c0: 5427 2c20 2731 4c74 272c 2027 3153 4727  T', '1Lt', '1SG'
-000006d0: 2c20 2731 5367 272c 2027 3153 7420 4c74  , '1Sg', '1St Lt
-000006e0: 272c 2027 3153 746c 7427 2c20 2731 5374  ', '1Stlt', '1St
-000006f0: 7367 7427 2c20 2731 7374 204c 7427 2c20  sgt', '1st Lt', 
-00000700: 2731 7374 4c74 272c 2027 3173 7453 6774  '1stLt', '1stSgt
-00000710: 272c 2027 3244 204c 7427 2c20 2732 4c54  ', '2D Lt', '2LT
-00000720: 272c 2027 324c 7427 2c20 2732 4e64 6c74  ', '2Lt', '2Ndlt
-00000730: 272c 2027 3264 204c 7427 2c20 2732 6e64  ', '2d Lt', '2nd
-00000740: 4c74 272c 2027 4131 4327 2c20 2741 4227  Lt', 'A1C', 'AB'
-00000750: 2c20 2741 444d 272c 2027 4162 272c 2027  , 'ADM', 'Ab', '
-00000760: 4164 6d27 2c20 2741 646d 6972 616c 2043  Adm', 'Admiral C
-00000770: 6869 6566 206f 6620 4e61 7661 6c20 4f70  hief of Naval Op
-00000780: 6572 6174 696f 6e73 272c 2027 4169 726d  erations', 'Airm
-00000790: 616e 272c 2027 4169 726d 616e 2042 6173  an', 'Airman Bas
-000007a0: 6963 272c 2027 4169 726d 616e 2046 6972  ic', 'Airman Fir
-000007b0: 7374 2043 6c61 7373 272c 2027 416d 6e27  st Class', 'Amn'
-000007c0: 2c20 2742 4727 2c20 2742 4765 6e27 2c20  , 'BG', 'BGen', 
-000007d0: 2742 6727 2c20 2742 6765 6e27 2c20 2742  'Bg', 'Bgen', 'B
-000007e0: 7269 6720 4765 6e27 2c20 2742 7269 6761  rig Gen', 'Briga
-000007f0: 6469 6572 2047 656e 6572 616c 272c 2027  dier General', '
-00000800: 4341 5054 272c 2027 4343 4d27 2c20 2743  CAPT', 'CCM', 'C
-00000810: 4452 272c 2027 434d 5341 4627 2c20 2743  DR', 'CMSAF', 'C
-00000820: 4d53 6774 272c 2027 434f 4c27 2c20 2743  MSgt', 'COL', 'C
-00000830: 504c 272c 2027 4350 4f27 2c20 2743 5054  PL', 'CPO', 'CPT
-00000840: 272c 2027 4353 4d27 2c20 2743 5732 272c  ', 'CSM', 'CW2',
-00000850: 2027 4357 3327 2c20 2743 5734 272c 2027   'CW3', 'CW4', '
-00000860: 4357 3527 2c20 2743 574f 3227 2c20 2743  CW5', 'CWO2', 'C
-00000870: 574f 3327 2c20 2743 574f 3427 2c20 2743  WO3', 'CWO4', 'C
-00000880: 574f 3527 2c20 2743 6170 7427 2c20 2743  WO5', 'Capt', 'C
-00000890: 6170 7461 696e 272c 2027 4363 6d27 2c20  aptain', 'Ccm', 
-000008a0: 2743 6472 272c 2027 4368 6965 6620 4d61  'Cdr', 'Chief Ma
-000008b0: 7374 6572 2053 6572 6765 616e 7427 2c20  ster Sergeant', 
-000008c0: 2743 6869 6566 204d 6173 7465 7220 5365  'Chief Master Se
-000008d0: 7267 6561 6e74 206f 6620 7468 6520 4169  rgeant of the Ai
-000008e0: 7220 466f 7263 6527 2c20 2743 6869 6566  r Force', 'Chief
-000008f0: 2050 6574 7479 204f 6666 6963 6572 272c   Petty Officer',
-00000900: 2027 4368 6965 6620 5761 7272 616e 7420   'Chief Warrant 
-00000910: 4f66 6669 6365 7220 3227 2c20 2743 6869  Officer 2', 'Chi
-00000920: 6566 2057 6172 7261 6e74 204f 6666 6963  ef Warrant Offic
-00000930: 6572 2033 272c 2027 4368 6965 6620 5761  er 3', 'Chief Wa
-00000940: 7272 616e 7420 4f66 6669 6365 7220 3427  rrant Officer 4'
-00000950: 2c20 2743 6869 6566 2057 6172 7261 6e74  , 'Chief Warrant
-00000960: 204f 6666 6963 6572 2035 272c 2027 436d   Officer 5', 'Cm
-00000970: 7361 6627 2c20 2743 6d73 6774 272c 2027  saf', 'Cmsgt', '
-00000980: 436f 6c27 2c20 2743 6f6c 6f6e 656c 272c  Col', 'Colonel',
-00000990: 2027 436f 6d6d 616e 6420 4368 6965 6620   'Command Chief 
-000009a0: 4d61 7374 6572 2053 6572 6765 616e 7427  Master Sergeant'
-000009b0: 2c20 2743 6f6d 6d61 6e64 204d 6173 7465  , 'Command Maste
-000009c0: 7220 4368 6965 6620 5065 7474 7920 4f66  r Chief Petty Of
-000009d0: 6669 6365 7227 2c20 2743 6f6d 6d61 6e64  ficer', 'Command
-000009e0: 2053 6572 6765 616e 7420 4d61 6a6f 7227   Sergeant Major'
-000009f0: 2c20 2743 6f6d 6d61 6e64 616e 7420 6f66  , 'Commandant of
-00000a00: 2074 6865 2043 6f61 7374 2047 7561 7264   the Coast Guard
-00000a10: 272c 2027 436f 6d6d 616e 6465 7227 2c20  ', 'Commander', 
-00000a20: 2743 6f72 706f 7261 6c27 2c20 2743 706c  'Corporal', 'Cpl
-00000a30: 272c 2027 4370 6f27 2c20 2743 7074 272c  ', 'Cpo', 'Cpt',
-00000a40: 2027 4373 6d27 2c20 2743 7732 272c 2027   'Csm', 'Cw2', '
-00000a50: 4377 3327 2c20 2743 7734 272c 2027 4377  Cw3', 'Cw4', 'Cw
-00000a60: 3527 2c20 2743 776f 3227 2c20 2743 776f  5', 'Cwo2', 'Cwo
-00000a70: 3327 2c20 2743 776f 3427 2c20 2743 776f  3', 'Cwo4', 'Cwo
-00000a80: 3527 2c20 2745 4e53 272c 2027 456e 7327  5', 'ENS', 'Ens'
-00000a90: 2c20 2745 6e73 6967 6e27 2c20 2746 4144  , 'Ensign', 'FAD
-00000aa0: 4d27 2c20 2746 4c54 434d 272c 2027 464f  M', 'FLTCM', 'FO
-00000ab0: 5243 4d27 2c20 2746 6164 6d27 2c20 2746  RCM', 'Fadm', 'F
-00000ac0: 6972 7374 204c 6965 7574 656e 616e 7427  irst Lieutenant'
-00000ad0: 2c20 2746 6972 7374 2053 6572 6765 616e  , 'First Sergean
-00000ae0: 7427 2c20 2746 6c65 6574 2041 646d 6972  t', 'Fleet Admir
-00000af0: 616c 272c 2027 466c 6565 7420 4d61 7374  al', 'Fleet Mast
-00000b00: 6572 2043 6869 6566 2050 6574 7479 204f  er Chief Petty O
-00000b10: 6666 6963 6572 272c 2027 466c 7463 6d27  fficer', 'Fltcm'
-00000b20: 2c20 2746 6f72 6365 204d 6173 7465 7220  , 'Force Master 
-00000b30: 4368 6965 6620 5065 7474 7920 4f66 6669  Chief Petty Offi
-00000b40: 6365 7227 2c20 2746 6f72 636d 272c 2027  cer', 'Forcm', '
-00000b50: 4741 272c 2027 4745 4e27 2c20 2747 4f41  GA', 'GEN', 'GOA
-00000b60: 4627 2c20 2747 6127 2c20 2747 656e 272c  F', 'Ga', 'Gen',
-00000b70: 2027 4765 6e65 7261 6c27 2c20 2747 656e   'General', 'Gen
-00000b80: 6572 616c 2041 6972 2046 6f72 6365 2043  eral Air Force C
-00000b90: 6869 6566 206f 6620 5374 6166 6627 2c20  hief of Staff', 
-00000ba0: 2747 656e 6572 616c 206f 6620 7468 6520  'General of the 
-00000bb0: 4169 7220 466f 7263 6527 2c20 2747 656e  Air Force', 'Gen
-00000bc0: 6572 616c 206f 6620 7468 6520 4172 6d79  eral of the Army
-00000bd0: 272c 2027 476f 6166 272c 2027 4775 6e6e  ', 'Goaf', 'Gunn
-00000be0: 6572 7920 5365 7267 6561 6e74 272c 2027  ery Sergeant', '
-00000bf0: 4779 5367 7427 2c20 2747 7973 6774 272c  GySgt', 'Gysgt',
-00000c00: 2027 4c43 4452 272c 2027 4c43 706c 272c   'LCDR', 'LCpl',
-00000c10: 2027 4c54 272c 2027 4c54 4327 2c20 274c   'LT', 'LTC', 'L
-00000c20: 5447 272c 2027 4c54 4a47 272c 2027 4c61  TG', 'LTJG', 'La
-00000c30: 6e63 6520 436f 7270 6f72 616c 272c 2027  nce Corporal', '
-00000c40: 4c63 6472 272c 2027 4c63 706c 272c 2027  Lcdr', 'Lcpl', '
-00000c50: 4c69 6575 7465 6e61 6e74 272c 2027 4c69  Lieutenant', 'Li
-00000c60: 6575 7465 6e61 6e74 2043 6f6c 6f6e 656c  eutenant Colonel
-00000c70: 272c 2027 4c69 6575 7465 6e61 6e74 2043  ', 'Lieutenant C
-00000c80: 6f6d 6d61 6e64 6572 272c 2027 4c69 6575  ommander', 'Lieu
-00000c90: 7465 6e61 6e74 2047 656e 6572 616c 272c  tenant General',
-00000ca0: 2027 4c69 6575 7465 6e61 6e74 2c20 4a75   'Lieutenant, Ju
-00000cb0: 6e69 6f72 2047 7261 6465 272c 2027 4c74  nior Grade', 'Lt
-00000cc0: 272c 2027 4c74 2043 6f6c 272c 2027 4c74  ', 'Lt Col', 'Lt
-00000cd0: 2047 656e 272c 2027 4c74 436f 6c27 2c20   Gen', 'LtCol', 
-00000ce0: 274c 7447 656e 272c 2027 4c74 6327 2c20  'LtGen', 'Ltc', 
-00000cf0: 274c 7463 6f6c 272c 2027 4c74 6727 2c20  'Ltcol', 'Ltg', 
-00000d00: 274c 7467 656e 272c 2027 4c74 6a67 272c  'Ltgen', 'Ltjg',
-00000d10: 2027 4d41 4a27 2c20 274d 4350 4f27 2c20   'MAJ', 'MCPO', 
-00000d20: 274d 4350 4f43 272c 2027 4d43 504f 4e27  'MCPOC', 'MCPON'
-00000d30: 2c20 274d 4727 2c20 274d 4779 5367 7427  , 'MG', 'MGySgt'
-00000d40: 2c20 274d 5043 4f43 4727 2c20 274d 5347  , 'MPCOCG', 'MSG
-00000d50: 272c 2027 4d53 6774 272c 2027 4d61 6a27  ', 'MSgt', 'Maj'
-00000d60: 2c20 274d 616a 2047 656e 272c 2027 4d61  , 'Maj Gen', 'Ma
-00000d70: 6a47 656e 272c 2027 4d61 6a67 656e 272c  jGen', 'Majgen',
-00000d80: 2027 4d61 6a6f 7227 2c20 274d 616a 6f72   'Major', 'Major
-00000d90: 2047 656e 6572 616c 272c 2027 4d61 7374   General', 'Mast
-00000da0: 6572 2043 6869 6566 2050 6574 7479 204f  er Chief Petty O
-00000db0: 6666 6963 6572 272c 2027 4d61 7374 6572  fficer', 'Master
-00000dc0: 2043 6869 6566 2050 6574 7479 204f 6666   Chief Petty Off
-00000dd0: 6963 6572 206f 6620 7468 6520 436f 6173  icer of the Coas
-00000de0: 7420 4775 6172 6427 2c20 274d 6173 7465  t Guard', 'Maste
-00000df0: 7220 4368 6965 6620 5065 7474 7920 4f66  r Chief Petty Of
-00000e00: 6669 6365 7220 6f66 2074 6865 204e 6176  ficer of the Nav
-00000e10: 7927 2c20 274d 6173 7465 7220 4775 6e6e  y', 'Master Gunn
-00000e20: 6572 7920 5365 7267 6561 6e74 272c 2027  ery Sergeant', '
-00000e30: 4d61 7374 6572 2053 6572 6765 616e 7427  Master Sergeant'
-00000e40: 2c20 274d 6370 6f27 2c20 274d 6370 6f63  , 'Mcpo', 'Mcpoc
-00000e50: 272c 2027 4d63 706f 6e27 2c20 274d 6727  ', 'Mcpon', 'Mg'
-00000e60: 2c20 274d 6779 7367 7427 2c20 274d 7063  , 'Mgysgt', 'Mpc
-00000e70: 6f63 6727 2c20 274d 7367 272c 2027 4d73  ocg', 'Msg', 'Ms
-00000e80: 6774 272c 2027 5046 4327 2c20 2750 4f31  gt', 'PFC', 'PO1
-00000e90: 272c 2027 504f 3227 2c20 2750 4f33 272c  ', 'PO2', 'PO3',
-00000ea0: 2027 5056 3227 2c20 2750 5654 272c 2027   'PV2', 'PVT', '
-00000eb0: 5065 7474 7920 4f66 6669 6365 7220 3173  Petty Officer 1s
-00000ec0: 7420 436c 6173 7327 2c20 2750 6574 7479  t Class', 'Petty
-00000ed0: 204f 6666 6963 6572 2032 6e64 2043 6c61   Officer 2nd Cla
-00000ee0: 7373 272c 2027 5065 7474 7920 4f66 6669  ss', 'Petty Offi
-00000ef0: 6365 7220 3372 6420 436c 6173 7327 2c20  cer 3rd Class', 
-00000f00: 2750 6663 272c 2027 506f 3127 2c20 2750  'Pfc', 'Po1', 'P
-00000f10: 6f32 272c 2027 506f 3327 2c20 2750 7269  o2', 'Po3', 'Pri
-00000f20: 7661 7465 272c 2027 5072 6976 6174 6520  vate', 'Private 
-00000f30: 3227 2c20 2750 7269 7661 7465 2046 6972  2', 'Private Fir
-00000f40: 7374 2043 6c61 7373 272c 2027 5076 3227  st Class', 'Pv2'
-00000f50: 2c20 2750 7674 272c 2027 5241 444d 272c  , 'Pvt', 'RADM',
-00000f60: 2027 5244 4d4c 272c 2027 5261 646d 272c   'RDML', 'Radm',
-00000f70: 2027 5264 6d6c 272c 2027 5265 6172 2041   'Rdml', 'Rear A
-00000f80: 646d 6972 616c 2028 6c6f 7765 7220 6861  dmiral (lower ha
-00000f90: 6c66 2927 2c20 2752 6561 7220 4164 6d69  lf)', 'Rear Admi
-00000fa0: 7261 6c20 2875 7070 6572 2068 616c 6629  ral (upper half)
-00000fb0: 272c 2027 5341 272c 2027 5343 504f 272c  ', 'SA', 'SCPO',
-00000fc0: 2027 5346 4327 2c20 2753 474d 272c 2027   'SFC', 'SGM', '
-00000fd0: 5347 5427 2c20 2753 4d41 272c 2027 534d  SGT', 'SMA', 'SM
-00000fe0: 5367 7427 2c20 2753 4e27 2c20 2753 5043  Sgt', 'SN', 'SPC
-00000ff0: 272c 2027 5352 272c 2027 5353 4727 2c20  ', 'SR', 'SSG', 
-00001000: 2753 5367 7427 2c20 2753 6127 2c20 2753  'SSgt', 'Sa', 'S
-00001010: 6370 6f27 2c20 2753 6561 6d61 6e27 2c20  cpo', 'Seaman', 
-00001020: 2753 6561 6d61 6e20 4170 7072 656e 7469  'Seaman Apprenti
-00001030: 6365 272c 2027 5365 616d 616e 2052 6563  ce', 'Seaman Rec
-00001040: 7275 6974 272c 2027 5365 636f 6e64 204c  ruit', 'Second L
-00001050: 6965 7574 656e 616e 7427 2c20 2753 656e  ieutenant', 'Sen
-00001060: 696f 7220 4169 726d 616e 206f 7220 5365  ior Airman or Se
-00001070: 7267 6561 6e74 272c 2027 5365 6e69 6f72  rgeant', 'Senior
-00001080: 2043 6869 6566 2050 6574 7479 204f 6666   Chief Petty Off
-00001090: 6963 6572 272c 2027 5365 6e69 6f72 204d  icer', 'Senior M
-000010a0: 6173 7465 7220 5365 7267 6561 6e74 272c  aster Sergeant',
-000010b0: 2027 5365 7267 6561 6e74 272c 2027 5365   'Sergeant', 'Se
-000010c0: 7267 6561 6e74 2046 6972 7374 2043 6c61  rgeant First Cla
-000010d0: 7373 272c 2027 5365 7267 6561 6e74 204d  ss', 'Sergeant M
-000010e0: 616a 6f72 272c 2027 5365 7267 6561 6e74  ajor', 'Sergeant
-000010f0: 204d 616a 6f72 206f 6620 7468 6520 4172   Major of the Ar
-00001100: 6d79 272c 2027 5365 7267 6561 6e74 204d  my', 'Sergeant M
-00001110: 616a 6f72 206f 6620 7468 6520 4d61 7269  ajor of the Mari
-00001120: 6e65 2043 6f72 7073 272c 2027 5366 6327  ne Corps', 'Sfc'
-00001130: 2c20 2753 676d 272c 2027 5367 7427 2c20  , 'Sgm', 'Sgt', 
-00001140: 2753 6774 4d61 6a27 2c20 2753 6774 4d61  'SgtMaj', 'SgtMa
-00001150: 6a4d 6172 436f 7227 2c20 2753 6774 6d61  jMarCor', 'Sgtma
-00001160: 6a27 2c20 2753 6774 6d61 6a6d 6172 636f  j', 'Sgtmajmarco
-00001170: 7227 2c20 2753 6d61 272c 2027 536d 7367  r', 'Sma', 'Smsg
-00001180: 7427 2c20 2753 6e27 2c20 2753 7063 272c  t', 'Sn', 'Spc',
-00001190: 2027 5370 6563 6961 6c69 7374 272c 2027   'Specialist', '
-000011a0: 5372 272c 2027 5372 4127 2c20 2753 7261  Sr', 'SrA', 'Sra
-000011b0: 272c 2027 5373 6727 2c20 2753 7367 7427  ', 'Ssg', 'Ssgt'
-000011c0: 2c20 2753 7461 6666 2053 6572 6765 616e  , 'Staff Sergean
-000011d0: 7427 2c20 2754 5367 7427 2c20 2754 6563  t', 'TSgt', 'Tec
-000011e0: 686e 6963 616c 2053 6572 6765 616e 7427  hnical Sergeant'
-000011f0: 2c20 2754 7367 7427 2c20 2756 4144 4d27  , 'Tsgt', 'VADM'
-00001200: 2c20 2756 6164 6d27 2c20 2756 6963 6520  , 'Vadm', 'Vice 
-00001210: 4164 6d69 7261 6c27 2c20 2757 4f31 272c  Admiral', 'WO1',
-00001220: 2027 5761 7272 616e 7420 4f66 6669 6365   'Warrant Office
-00001230: 7227 2c20 2757 6172 7261 6e74 204f 6666  r', 'Warrant Off
-00001240: 6963 6572 2031 272c 2027 576f 3127 5d0d  icer 1', 'Wo1'].
-00001250: 0a                                       .
+00000000: 5b70 6970 656c 696e 655f 6461 7461 5d0a  [pipeline_data].
+00000010: 6e61 6d65 203d 2022 6765 6e64 6572 7370  name = "gendersp
+00000020: 6163 7922 0a61 7574 686f 7220 3d20 2257  acy".author = "W
+00000030: 2e4a 2e42 2e20 4d61 7474 696e 676c 7922  .J.B. Mattingly"
+00000040: 0a75 726c 203d 2022 6874 7470 733a 2f2f  .url = "https://
+00000050: 6769 7468 7562 2e63 6f6d 2f77 6a62 6d61  github.com/wjbma
+00000060: 7474 696e 676c 792f 6765 6e64 6572 7370  ttingly/gendersp
+00000070: 6163 7922 0a76 6572 7369 6f6e 203d 2022  acy".version = "
+00000080: 302e 302e 3122 0a64 6573 6372 6970 7469  0.0.1".descripti
+00000090: 6f6e 203d 2022 5468 6973 2069 7320 6120  on = "This is a 
+000000a0: 7370 6143 7920 7069 7065 6c69 6e65 2066  spaCy pipeline f
+000000b0: 6f72 2068 656c 7069 6e67 2069 6465 6e74  or helping ident
+000000c0: 6966 7920 6765 6e64 6572 2069 6e20 7465  ify gender in te
+000000d0: 7874 732e 2049 7420 6973 2069 6e63 6c75  xts. It is inclu
+000000e0: 7369 7665 206f 6620 6665 6d61 6c65 2c20  sive of female, 
+000000f0: 6d61 6c65 2c20 616e 6420 6e65 7574 7261  male, and neutra
+00000100: 6c20 6765 6e64 6572 2070 726f 6e6f 756e  l gender pronoun
+00000110: 732f 7469 746c 6573 2e22 0a0a 5b63 6f6c  s/titles."..[col
+00000120: 6f72 735d 0a4e 4555 5452 414c 5f50 524f  ors].NEUTRAL_PRO
+00000130: 4e4f 554e 3d22 2366 6662 3666 3822 0a50  NOUN="#ffb6f8".P
+00000140: 4552 534f 4e5f 4e45 5554 5241 4c3d 2223  ERSON_NEUTRAL="#
+00000150: 6666 6236 6638 220a 5245 4c5f 4e45 5554  ffb6f8".REL_NEUT
+00000160: 5241 4c5f 434f 5245 463d 2223 6666 6236  RAL_COREF="#ffb6
+00000170: 6638 220a 0a46 454d 414c 455f 5052 4f4e  f8"..FEMALE_PRON
+00000180: 4f55 4e3d 2223 6236 6666 6637 220a 5045  OUN="#b6fff7".PE
+00000190: 5253 4f4e 5f46 454d 414c 453d 2223 6236  RSON_FEMALE="#b6
+000001a0: 6666 6637 220a 5045 5253 4f4e 5f46 454d  fff7".PERSON_FEM
+000001b0: 414c 455f 434f 5245 463d 2223 6236 6666  ALE_COREF="#b6ff
+000001c0: 6637 220a 5245 4c5f 4645 4d41 4c45 5f43  f7".REL_FEMALE_C
+000001d0: 4f52 4546 3d22 2362 3666 6666 3722 0a0a  OREF="#b6fff7"..
+000001e0: 4d41 4c45 5f50 524f 4e4f 554e 3d22 2362  MALE_PRONOUN="#b
+000001f0: 3662 3766 6622 0a50 4552 534f 4e5f 4d41  6b7ff".PERSON_MA
+00000200: 4c45 3d22 2362 3662 3766 6622 0a50 4552  LE="#b6b7ff".PER
+00000210: 534f 4e5f 4d41 4c45 5f43 4f52 4546 3d22  SON_MALE_COREF="
+00000220: 2362 3662 3766 6622 0a52 454c 5f4d 414c  #b6b7ff".REL_MAL
+00000230: 455f 434f 5245 463d 2223 6236 6237 6666  E_COREF="#b6b7ff
+00000240: 220a 0a43 4f4c 4c45 4354 4956 455f 5350  "..COLLECTIVE_SP
+00000250: 4f55 5341 4c3d 2223 6637 6666 6236 220a  OUSAL="#f7ffb6".
+00000260: 0a5b 7072 6f6e 6f75 6e73 5d0a 6d61 6c65  .[pronouns].male
+00000270: 3d20 5b27 6865 272c 2027 6869 6d27 2c20  = ['he', 'him', 
+00000280: 2768 6973 272c 2027 6869 7327 2c20 2768  'his', 'his', 'h
+00000290: 696d 7365 6c66 275d 0a66 656d 616c 6520  imself'].female 
+000002a0: 3d20 5b27 7368 6527 2c20 2768 6572 272c  = ['she', 'her',
+000002b0: 2027 6865 7227 2c20 2768 6572 7327 2c20   'her', 'hers', 
+000002c0: 2768 6572 7365 6c66 275d 0a6e 6575 7472  'herself'].neutr
+000002d0: 616c 203d 205b 2766 6165 272c 2027 6661  al = ['fae', 'fa
+000002e0: 6572 272c 2027 6661 6572 272c 2027 6661  er', 'faer', 'fa
+000002f0: 6572 7327 2c20 2766 6165 7273 656c 6627  ers', 'faerself'
+00000300: 2c0a 2020 2020 2020 2020 2020 2020 2761  ,.            'a
+00000310: 6527 2c20 2761 6572 272c 2027 6165 7227  e', 'aer', 'aer'
+00000320: 2c20 2766 6165 7273 272c 2027 6661 6572  , 'faers', 'faer
+00000330: 7365 6c66 272c 0a20 2020 2020 2020 2020  self',.         
+00000340: 2020 2027 6527 2c20 2765 6d27 2c20 2765     'e', 'em', 'e
+00000350: 6972 272c 2027 6569 7273 272c 2027 6569  ir', 'eirs', 'ei
+00000360: 7273 656c 6627 2c0a 2020 2020 2020 2020  rself',.        
+00000370: 2020 2020 2765 7927 2c20 2765 6d27 2c20      'ey', 'em', 
+00000380: 2765 6972 272c 2027 6569 7273 272c 2027  'eir', 'eirs', '
+00000390: 6569 7273 656c 6627 2c0a 2020 2020 2020  eirself',.      
+000003a0: 2020 2020 2020 2770 6572 272c 2027 7065        'per', 'pe
+000003b0: 7227 2c20 2770 6572 7327 2c20 2770 6572  r', 'pers', 'per
+000003c0: 7327 2c20 2770 6572 7365 6c66 272c 0a20  s', 'perself',. 
+000003d0: 2020 2020 2020 2020 2020 2027 7468 6579             'they
+000003e0: 272c 2027 7468 656d 272c 2027 7468 6569  ', 'them', 'thei
+000003f0: 7227 2c20 2774 6865 6972 7327 2c20 2774  r', 'theirs', 't
+00000400: 6865 6d73 656c 6627 2c0a 2020 2020 2020  hemself',.      
+00000410: 2020 2020 2020 2776 6527 2c20 2776 6572        've', 'ver
+00000420: 272c 2027 7669 7327 2c20 2776 6973 272c  ', 'vis', 'vis',
+00000430: 2027 7665 7265 7365 6c66 272c 0a20 2020   'vereself',.   
+00000440: 2020 2020 2020 2020 2027 7865 272c 2027           'xe', '
+00000450: 7865 6d27 2c20 2778 7972 272c 2027 7879  xem', 'xyr', 'xy
+00000460: 7273 272c 2027 7865 6d73 656c 6627 2c27  rs', 'xemself','
+00000470: 7a65 272c 0a20 2020 2020 2020 2020 2020  ze',.           
+00000480: 2027 6869 7227 2c20 2768 6972 272c 2027   'hir', 'hir', '
+00000490: 6869 7273 272c 2027 6869 7273 656c 6627  hirs', 'hirself'
+000004a0: 2c0a 2020 2020 2020 2020 2020 2020 277a  ,.            'z
+000004b0: 6965 272c 2027 6869 7227 2c20 2768 6972  ie', 'hir', 'hir
+000004c0: 272c 2027 6869 7273 272c 2027 6869 7273  ', 'hirs', 'hirs
+000004d0: 656c 6627 5d0a 0a5b 7669 7375 616c 697a  elf']..[visualiz
+000004e0: 655f 7061 7261 6d73 5d0a 7370 616e 735f  e_params].spans_
+000004f0: 6b65 793d 2272 756c 6572 220a 0a5b 7265  key="ruler"..[re
+00000500: 6765 785d 0a69 6e64 6976 6964 7561 6c20  gex].individual 
+00000510: 3d20 2228 3c47 454e 4445 525f 5449 544c  = "(<GENDER_TITL
+00000520: 4553 3e29 285c 5c2e 292a 205b 412d 5a5d  ES>)(\\.)* [A-Z]
+00000530: 5b61 2d7a 5d2a 2820 5b41 2d5a 5d5b 612d  [a-z]*( [A-Z][a-
+00000540: 7a5d 2a29 2a22 0a73 706f 7573 6520 3d20  z]*)*".spouse = 
+00000550: 2228 3c47 454e 4445 525f 5449 544c 4553  "(<GENDER_TITLES
+00000560: 3e29 285c 5c2e 292a 2028 616e 647c 2629  >)(\\.)* (and|&)
+00000570: 2028 3c47 454e 4445 525f 5449 544c 4553   (<GENDER_TITLES
+00000580: 3e29 285c 5c2e 292a 205b 412d 5a5d 5b61  >)(\\.)* [A-Z][a
+00000590: 2d7a 5d2a 2820 5b41 2d5a 5d5b 612d 7a5d  -z]*( [A-Z][a-z]
+000005a0: 2a29 2a22 0a0a 5b74 6974 6c65 735d 0a66  *)*"..[titles].f
+000005b0: 656d 616c 6520 3d20 5b22 4d72 7322 2c20  emale = ["Mrs", 
+000005c0: 224d 7322 2c20 224d 6973 7322 2c20 224d  "Ms", "Miss", "M
+000005d0: 6164 616d 222c 2022 4d64 6d22 5d0a 6d61  adam", "Mdm"].ma
+000005e0: 6c65 203d 205b 224d 7222 5d0a 6e65 7574  le = ["Mr"].neut
+000005f0: 7261 6c20 3d20 5b22 4d78 222c 2022 496e  ral = ["Mx", "In
+00000600: 6422 2c20 224d 7372 222c 2022 4d72 6522  d", "Msr", "Mre"
+00000610: 2c20 224d 6973 6322 2c20 2250 7222 2c0a  , "Misc", "Pr",.
+00000620: 0a20 2020 2020 2020 2020 2023 2050 726f  .          # Pro
+00000630: 6665 7373 696f 6e61 6c0a 2020 2020 2020  fessional.      
+00000640: 2020 2020 2244 7222 2c20 2244 6f63 746f      "Dr", "Docto
+00000650: 7222 2c20 2250 726f 6622 2c20 2250 726f  r", "Prof", "Pro
+00000660: 6665 7373 6f72 222c 0a20 2020 2020 2020  fessor",.       
+00000670: 2020 2023 204d 696c 6974 6172 790a 2020     # Military.  
+00000680: 2020 2020 2020 2020 2731 4c54 272c 2027          '1LT', '
+00000690: 314c 7427 2c20 2731 5347 272c 2027 3153  1Lt', '1SG', '1S
+000006a0: 6727 2c20 2731 5374 204c 7427 2c20 2731  g', '1St Lt', '1
+000006b0: 5374 6c74 272c 2027 3153 7473 6774 272c  Stlt', '1Stsgt',
+000006c0: 2027 3173 7420 4c74 272c 2027 3173 744c   '1st Lt', '1stL
+000006d0: 7427 2c20 2731 7374 5367 7427 2c20 2732  t', '1stSgt', '2
+000006e0: 4420 4c74 272c 2027 324c 5427 2c20 2732  D Lt', '2LT', '2
+000006f0: 4c74 272c 2027 324e 646c 7427 2c20 2732  Lt', '2Ndlt', '2
+00000700: 6420 4c74 272c 2027 326e 644c 7427 2c20  d Lt', '2ndLt', 
+00000710: 2741 3143 272c 2027 4142 272c 2027 4144  'A1C', 'AB', 'AD
+00000720: 4d27 2c20 2741 6227 2c20 2741 646d 272c  M', 'Ab', 'Adm',
+00000730: 2027 4164 6d69 7261 6c20 4368 6965 6620   'Admiral Chief 
+00000740: 6f66 204e 6176 616c 204f 7065 7261 7469  of Naval Operati
+00000750: 6f6e 7327 2c20 2741 6972 6d61 6e27 2c20  ons', 'Airman', 
+00000760: 2741 6972 6d61 6e20 4261 7369 6327 2c20  'Airman Basic', 
+00000770: 2741 6972 6d61 6e20 4669 7273 7420 436c  'Airman First Cl
+00000780: 6173 7327 2c20 2741 6d6e 272c 2027 4247  ass', 'Amn', 'BG
+00000790: 272c 2027 4247 656e 272c 2027 4267 272c  ', 'BGen', 'Bg',
+000007a0: 2027 4267 656e 272c 2027 4272 6967 2047   'Bgen', 'Brig G
+000007b0: 656e 272c 2027 4272 6967 6164 6965 7220  en', 'Brigadier 
+000007c0: 4765 6e65 7261 6c27 2c20 2743 4150 5427  General', 'CAPT'
+000007d0: 2c20 2743 434d 272c 2027 4344 5227 2c20  , 'CCM', 'CDR', 
+000007e0: 2743 4d53 4146 272c 2027 434d 5367 7427  'CMSAF', 'CMSgt'
+000007f0: 2c20 2743 4f4c 272c 2027 4350 4c27 2c20  , 'COL', 'CPL', 
+00000800: 2743 504f 272c 2027 4350 5427 2c20 2743  'CPO', 'CPT', 'C
+00000810: 534d 272c 2027 4357 3227 2c20 2743 5733  SM', 'CW2', 'CW3
+00000820: 272c 2027 4357 3427 2c20 2743 5735 272c  ', 'CW4', 'CW5',
+00000830: 2027 4357 4f32 272c 2027 4357 4f33 272c   'CWO2', 'CWO3',
+00000840: 2027 4357 4f34 272c 2027 4357 4f35 272c   'CWO4', 'CWO5',
+00000850: 2027 4361 7074 272c 2027 4361 7074 6169   'Capt', 'Captai
+00000860: 6e27 2c20 2743 636d 272c 2027 4364 7227  n', 'Ccm', 'Cdr'
+00000870: 2c20 2743 6869 6566 204d 6173 7465 7220  , 'Chief Master 
+00000880: 5365 7267 6561 6e74 272c 2027 4368 6965  Sergeant', 'Chie
+00000890: 6620 4d61 7374 6572 2053 6572 6765 616e  f Master Sergean
+000008a0: 7420 6f66 2074 6865 2041 6972 2046 6f72  t of the Air For
+000008b0: 6365 272c 2027 4368 6965 6620 5065 7474  ce', 'Chief Pett
+000008c0: 7920 4f66 6669 6365 7227 2c20 2743 6869  y Officer', 'Chi
+000008d0: 6566 2057 6172 7261 6e74 204f 6666 6963  ef Warrant Offic
+000008e0: 6572 2032 272c 2027 4368 6965 6620 5761  er 2', 'Chief Wa
+000008f0: 7272 616e 7420 4f66 6669 6365 7220 3327  rrant Officer 3'
+00000900: 2c20 2743 6869 6566 2057 6172 7261 6e74  , 'Chief Warrant
+00000910: 204f 6666 6963 6572 2034 272c 2027 4368   Officer 4', 'Ch
+00000920: 6965 6620 5761 7272 616e 7420 4f66 6669  ief Warrant Offi
+00000930: 6365 7220 3527 2c20 2743 6d73 6166 272c  cer 5', 'Cmsaf',
+00000940: 2027 436d 7367 7427 2c20 2743 6f6c 272c   'Cmsgt', 'Col',
+00000950: 2027 436f 6c6f 6e65 6c27 2c20 2743 6f6d   'Colonel', 'Com
+00000960: 6d61 6e64 2043 6869 6566 204d 6173 7465  mand Chief Maste
+00000970: 7220 5365 7267 6561 6e74 272c 2027 436f  r Sergeant', 'Co
+00000980: 6d6d 616e 6420 4d61 7374 6572 2043 6869  mmand Master Chi
+00000990: 6566 2050 6574 7479 204f 6666 6963 6572  ef Petty Officer
+000009a0: 272c 2027 436f 6d6d 616e 6420 5365 7267  ', 'Command Serg
+000009b0: 6561 6e74 204d 616a 6f72 272c 2027 436f  eant Major', 'Co
+000009c0: 6d6d 616e 6461 6e74 206f 6620 7468 6520  mmandant of the 
+000009d0: 436f 6173 7420 4775 6172 6427 2c20 2743  Coast Guard', 'C
+000009e0: 6f6d 6d61 6e64 6572 272c 2027 436f 7270  ommander', 'Corp
+000009f0: 6f72 616c 272c 2027 4370 6c27 2c20 2743  oral', 'Cpl', 'C
+00000a00: 706f 272c 2027 4370 7427 2c20 2743 736d  po', 'Cpt', 'Csm
+00000a10: 272c 2027 4377 3227 2c20 2743 7733 272c  ', 'Cw2', 'Cw3',
+00000a20: 2027 4377 3427 2c20 2743 7735 272c 2027   'Cw4', 'Cw5', '
+00000a30: 4377 6f32 272c 2027 4377 6f33 272c 2027  Cwo2', 'Cwo3', '
+00000a40: 4377 6f34 272c 2027 4377 6f35 272c 2027  Cwo4', 'Cwo5', '
+00000a50: 454e 5327 2c20 2745 6e73 272c 2027 456e  ENS', 'Ens', 'En
+00000a60: 7369 676e 272c 2027 4641 444d 272c 2027  sign', 'FADM', '
+00000a70: 464c 5443 4d27 2c20 2746 4f52 434d 272c  FLTCM', 'FORCM',
+00000a80: 2027 4661 646d 272c 2027 4669 7273 7420   'Fadm', 'First 
+00000a90: 4c69 6575 7465 6e61 6e74 272c 2027 4669  Lieutenant', 'Fi
+00000aa0: 7273 7420 5365 7267 6561 6e74 272c 2027  rst Sergeant', '
+00000ab0: 466c 6565 7420 4164 6d69 7261 6c27 2c20  Fleet Admiral', 
+00000ac0: 2746 6c65 6574 204d 6173 7465 7220 4368  'Fleet Master Ch
+00000ad0: 6965 6620 5065 7474 7920 4f66 6669 6365  ief Petty Office
+00000ae0: 7227 2c20 2746 6c74 636d 272c 2027 466f  r', 'Fltcm', 'Fo
+00000af0: 7263 6520 4d61 7374 6572 2043 6869 6566  rce Master Chief
+00000b00: 2050 6574 7479 204f 6666 6963 6572 272c   Petty Officer',
+00000b10: 2027 466f 7263 6d27 2c20 2747 4127 2c20   'Forcm', 'GA', 
+00000b20: 2747 454e 272c 2027 474f 4146 272c 2027  'GEN', 'GOAF', '
+00000b30: 4761 272c 2027 4765 6e27 2c20 2747 656e  Ga', 'Gen', 'Gen
+00000b40: 6572 616c 272c 2027 4765 6e65 7261 6c20  eral', 'General 
+00000b50: 4169 7220 466f 7263 6520 4368 6965 6620  Air Force Chief 
+00000b60: 6f66 2053 7461 6666 272c 2027 4765 6e65  of Staff', 'Gene
+00000b70: 7261 6c20 6f66 2074 6865 2041 6972 2046  ral of the Air F
+00000b80: 6f72 6365 272c 2027 4765 6e65 7261 6c20  orce', 'General 
+00000b90: 6f66 2074 6865 2041 726d 7927 2c20 2747  of the Army', 'G
+00000ba0: 6f61 6627 2c20 2747 756e 6e65 7279 2053  oaf', 'Gunnery S
+00000bb0: 6572 6765 616e 7427 2c20 2747 7953 6774  ergeant', 'GySgt
+00000bc0: 272c 2027 4779 7367 7427 2c20 274c 4344  ', 'Gysgt', 'LCD
+00000bd0: 5227 2c20 274c 4370 6c27 2c20 274c 5427  R', 'LCpl', 'LT'
+00000be0: 2c20 274c 5443 272c 2027 4c54 4727 2c20  , 'LTC', 'LTG', 
+00000bf0: 274c 544a 4727 2c20 274c 616e 6365 2043  'LTJG', 'Lance C
+00000c00: 6f72 706f 7261 6c27 2c20 274c 6364 7227  orporal', 'Lcdr'
+00000c10: 2c20 274c 6370 6c27 2c20 274c 6965 7574  , 'Lcpl', 'Lieut
+00000c20: 656e 616e 7427 2c20 274c 6965 7574 656e  enant', 'Lieuten
+00000c30: 616e 7420 436f 6c6f 6e65 6c27 2c20 274c  ant Colonel', 'L
+00000c40: 6965 7574 656e 616e 7420 436f 6d6d 616e  ieutenant Comman
+00000c50: 6465 7227 2c20 274c 6965 7574 656e 616e  der', 'Lieutenan
+00000c60: 7420 4765 6e65 7261 6c27 2c20 274c 6965  t General', 'Lie
+00000c70: 7574 656e 616e 742c 204a 756e 696f 7220  utenant, Junior 
+00000c80: 4772 6164 6527 2c20 274c 7427 2c20 274c  Grade', 'Lt', 'L
+00000c90: 7420 436f 6c27 2c20 274c 7420 4765 6e27  t Col', 'Lt Gen'
+00000ca0: 2c20 274c 7443 6f6c 272c 2027 4c74 4765  , 'LtCol', 'LtGe
+00000cb0: 6e27 2c20 274c 7463 272c 2027 4c74 636f  n', 'Ltc', 'Ltco
+00000cc0: 6c27 2c20 274c 7467 272c 2027 4c74 6765  l', 'Ltg', 'Ltge
+00000cd0: 6e27 2c20 274c 746a 6727 2c20 274d 414a  n', 'Ltjg', 'MAJ
+00000ce0: 272c 2027 4d43 504f 272c 2027 4d43 504f  ', 'MCPO', 'MCPO
+00000cf0: 4327 2c20 274d 4350 4f4e 272c 2027 4d47  C', 'MCPON', 'MG
+00000d00: 272c 2027 4d47 7953 6774 272c 2027 4d50  ', 'MGySgt', 'MP
+00000d10: 434f 4347 272c 2027 4d53 4727 2c20 274d  COCG', 'MSG', 'M
+00000d20: 5367 7427 2c20 274d 616a 272c 2027 4d61  Sgt', 'Maj', 'Ma
+00000d30: 6a20 4765 6e27 2c20 274d 616a 4765 6e27  j Gen', 'MajGen'
+00000d40: 2c20 274d 616a 6765 6e27 2c20 274d 616a  , 'Majgen', 'Maj
+00000d50: 6f72 272c 2027 4d61 6a6f 7220 4765 6e65  or', 'Major Gene
+00000d60: 7261 6c27 2c20 274d 6173 7465 7220 4368  ral', 'Master Ch
+00000d70: 6965 6620 5065 7474 7920 4f66 6669 6365  ief Petty Office
+00000d80: 7227 2c20 274d 6173 7465 7220 4368 6965  r', 'Master Chie
+00000d90: 6620 5065 7474 7920 4f66 6669 6365 7220  f Petty Officer 
+00000da0: 6f66 2074 6865 2043 6f61 7374 2047 7561  of the Coast Gua
+00000db0: 7264 272c 2027 4d61 7374 6572 2043 6869  rd', 'Master Chi
+00000dc0: 6566 2050 6574 7479 204f 6666 6963 6572  ef Petty Officer
+00000dd0: 206f 6620 7468 6520 4e61 7679 272c 2027   of the Navy', '
+00000de0: 4d61 7374 6572 2047 756e 6e65 7279 2053  Master Gunnery S
+00000df0: 6572 6765 616e 7427 2c20 274d 6173 7465  ergeant', 'Maste
+00000e00: 7220 5365 7267 6561 6e74 272c 2027 4d63  r Sergeant', 'Mc
+00000e10: 706f 272c 2027 4d63 706f 6327 2c20 274d  po', 'Mcpoc', 'M
+00000e20: 6370 6f6e 272c 2027 4d67 272c 2027 4d67  cpon', 'Mg', 'Mg
+00000e30: 7973 6774 272c 2027 4d70 636f 6367 272c  ysgt', 'Mpcocg',
+00000e40: 2027 4d73 6727 2c20 274d 7367 7427 2c20   'Msg', 'Msgt', 
+00000e50: 2750 4643 272c 2027 504f 3127 2c20 2750  'PFC', 'PO1', 'P
+00000e60: 4f32 272c 2027 504f 3327 2c20 2750 5632  O2', 'PO3', 'PV2
+00000e70: 272c 2027 5056 5427 2c20 2750 6574 7479  ', 'PVT', 'Petty
+00000e80: 204f 6666 6963 6572 2031 7374 2043 6c61   Officer 1st Cla
+00000e90: 7373 272c 2027 5065 7474 7920 4f66 6669  ss', 'Petty Offi
+00000ea0: 6365 7220 326e 6420 436c 6173 7327 2c20  cer 2nd Class', 
+00000eb0: 2750 6574 7479 204f 6666 6963 6572 2033  'Petty Officer 3
+00000ec0: 7264 2043 6c61 7373 272c 2027 5066 6327  rd Class', 'Pfc'
+00000ed0: 2c20 2750 6f31 272c 2027 506f 3227 2c20  , 'Po1', 'Po2', 
+00000ee0: 2750 6f33 272c 2027 5072 6976 6174 6527  'Po3', 'Private'
+00000ef0: 2c20 2750 7269 7661 7465 2032 272c 2027  , 'Private 2', '
+00000f00: 5072 6976 6174 6520 4669 7273 7420 436c  Private First Cl
+00000f10: 6173 7327 2c20 2750 7632 272c 2027 5076  ass', 'Pv2', 'Pv
+00000f20: 7427 2c20 2752 4144 4d27 2c20 2752 444d  t', 'RADM', 'RDM
+00000f30: 4c27 2c20 2752 6164 6d27 2c20 2752 646d  L', 'Radm', 'Rdm
+00000f40: 6c27 2c20 2752 6561 7220 4164 6d69 7261  l', 'Rear Admira
+00000f50: 6c20 286c 6f77 6572 2068 616c 6629 272c  l (lower half)',
+00000f60: 2027 5265 6172 2041 646d 6972 616c 2028   'Rear Admiral (
+00000f70: 7570 7065 7220 6861 6c66 2927 2c20 2753  upper half)', 'S
+00000f80: 4127 2c20 2753 4350 4f27 2c20 2753 4643  A', 'SCPO', 'SFC
+00000f90: 272c 2027 5347 4d27 2c20 2753 4754 272c  ', 'SGM', 'SGT',
+00000fa0: 2027 534d 4127 2c20 2753 4d53 6774 272c   'SMA', 'SMSgt',
+00000fb0: 2027 534e 272c 2027 5350 4327 2c20 2753   'SN', 'SPC', 'S
+00000fc0: 5227 2c20 2753 5347 272c 2027 5353 6774  R', 'SSG', 'SSgt
+00000fd0: 272c 2027 5361 272c 2027 5363 706f 272c  ', 'Sa', 'Scpo',
+00000fe0: 2027 5365 616d 616e 272c 2027 5365 616d   'Seaman', 'Seam
+00000ff0: 616e 2041 7070 7265 6e74 6963 6527 2c20  an Apprentice', 
+00001000: 2753 6561 6d61 6e20 5265 6372 7569 7427  'Seaman Recruit'
+00001010: 2c20 2753 6563 6f6e 6420 4c69 6575 7465  , 'Second Lieute
+00001020: 6e61 6e74 272c 2027 5365 6e69 6f72 2041  nant', 'Senior A
+00001030: 6972 6d61 6e20 6f72 2053 6572 6765 616e  irman or Sergean
+00001040: 7427 2c20 2753 656e 696f 7220 4368 6965  t', 'Senior Chie
+00001050: 6620 5065 7474 7920 4f66 6669 6365 7227  f Petty Officer'
+00001060: 2c20 2753 656e 696f 7220 4d61 7374 6572  , 'Senior Master
+00001070: 2053 6572 6765 616e 7427 2c20 2753 6572   Sergeant', 'Ser
+00001080: 6765 616e 7427 2c20 2753 6572 6765 616e  geant', 'Sergean
+00001090: 7420 4669 7273 7420 436c 6173 7327 2c20  t First Class', 
+000010a0: 2753 6572 6765 616e 7420 4d61 6a6f 7227  'Sergeant Major'
+000010b0: 2c20 2753 6572 6765 616e 7420 4d61 6a6f  , 'Sergeant Majo
+000010c0: 7220 6f66 2074 6865 2041 726d 7927 2c20  r of the Army', 
+000010d0: 2753 6572 6765 616e 7420 4d61 6a6f 7220  'Sergeant Major 
+000010e0: 6f66 2074 6865 204d 6172 696e 6520 436f  of the Marine Co
+000010f0: 7270 7327 2c20 2753 6663 272c 2027 5367  rps', 'Sfc', 'Sg
+00001100: 6d27 2c20 2753 6774 272c 2027 5367 744d  m', 'Sgt', 'SgtM
+00001110: 616a 272c 2027 5367 744d 616a 4d61 7243  aj', 'SgtMajMarC
+00001120: 6f72 272c 2027 5367 746d 616a 272c 2027  or', 'Sgtmaj', '
+00001130: 5367 746d 616a 6d61 7263 6f72 272c 2027  Sgtmajmarcor', '
+00001140: 536d 6127 2c20 2753 6d73 6774 272c 2027  Sma', 'Smsgt', '
+00001150: 536e 272c 2027 5370 6327 2c20 2753 7065  Sn', 'Spc', 'Spe
+00001160: 6369 616c 6973 7427 2c20 2753 7227 2c20  cialist', 'Sr', 
+00001170: 2753 7241 272c 2027 5372 6127 2c20 2753  'SrA', 'Sra', 'S
+00001180: 7367 272c 2027 5373 6774 272c 2027 5374  sg', 'Ssgt', 'St
+00001190: 6166 6620 5365 7267 6561 6e74 272c 2027  aff Sergeant', '
+000011a0: 5453 6774 272c 2027 5465 6368 6e69 6361  TSgt', 'Technica
+000011b0: 6c20 5365 7267 6561 6e74 272c 2027 5473  l Sergeant', 'Ts
+000011c0: 6774 272c 2027 5641 444d 272c 2027 5661  gt', 'VADM', 'Va
+000011d0: 646d 272c 2027 5669 6365 2041 646d 6972  dm', 'Vice Admir
+000011e0: 616c 272c 2027 574f 3127 2c20 2757 6172  al', 'WO1', 'War
+000011f0: 7261 6e74 204f 6666 6963 6572 272c 2027  rant Officer', '
+00001200: 5761 7272 616e 7420 4f66 6669 6365 7220  Warrant Officer 
+00001210: 3127 2c20 2757 6f31 275d 0a              1', 'Wo1'].
```

### Comparing `gender-spacy-0.0.4/gender_spacy/data/pronoun_patterns` & `gender-spacy-0.0.5/gender_spacy/data/pronoun_patterns`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-{"pattern":[{"LOWER":"ae","POS":"PRON"}],"label":"GENDER_PRONOUN"}
-{"pattern":[{"LOWER":"aer","POS":"PRON"}],"label":"GENDER_PRONOUN"}
-{"pattern":[{"LOWER":"e","POS":"PRON"}],"label":"GENDER_PRONOUN"}
-{"pattern":[{"LOWER":"eir","POS":"PRON"}],"label":"GENDER_PRONOUN"}
-{"pattern":[{"LOWER":"eirs","POS":"PRON"}],"label":"GENDER_PRONOUN"}
-{"pattern":[{"LOWER":"eirself","POS":"PRON"}],"label":"GENDER_PRONOUN"}
-{"pattern":[{"LOWER":"em","POS":"PRON"}],"label":"GENDER_PRONOUN"}
-{"pattern":[{"LOWER":"ey","POS":"PRON"}],"label":"GENDER_PRONOUN"}
-{"pattern":[{"LOWER":"fae","POS":"PRON"}],"label":"GENDER_PRONOUN"}
-{"pattern":[{"LOWER":"faer","POS":"PRON"}],"label":"GENDER_PRONOUN"}
-{"pattern":[{"LOWER":"faers","POS":"PRON"}],"label":"GENDER_PRONOUN"}
-{"pattern":[{"LOWER":"faerself","POS":"PRON"}],"label":"GENDER_PRONOUN"}
-{"pattern":[{"LOWER":"he","POS":"PRON"}],"label":"GENDER_PRONOUN"}
-{"pattern":[{"LOWER":"her","POS":"PRON"}],"label":"GENDER_PRONOUN"}
-{"pattern":[{"LOWER":"hers","POS":"PRON"}],"label":"GENDER_PRONOUN"}
-{"pattern":[{"LOWER":"herself","POS":"PRON"}],"label":"GENDER_PRONOUN"}
-{"pattern":[{"LOWER":"him","POS":"PRON"}],"label":"GENDER_PRONOUN"}
-{"pattern":[{"LOWER":"himself","POS":"PRON"}],"label":"GENDER_PRONOUN"}
-{"pattern":[{"LOWER":"hir","POS":"PRON"}],"label":"GENDER_PRONOUN"}
-{"pattern":[{"LOWER":"hirs","POS":"PRON"}],"label":"GENDER_PRONOUN"}
-{"pattern":[{"LOWER":"hirself","POS":"PRON"}],"label":"GENDER_PRONOUN"}
-{"pattern":[{"LOWER":"his","POS":"PRON"}],"label":"GENDER_PRONOUN"}
-{"pattern":[{"LOWER":"per","POS":"PRON"}],"label":"GENDER_PRONOUN"}
-{"pattern":[{"LOWER":"pers","POS":"PRON"}],"label":"GENDER_PRONOUN"}
-{"pattern":[{"LOWER":"perself","POS":"PRON"}],"label":"GENDER_PRONOUN"}
-{"pattern":[{"LOWER":"she","POS":"PRON"}],"label":"GENDER_PRONOUN"}
-{"pattern":[{"LOWER":"their","POS":"PRON"}],"label":"GENDER_PRONOUN"}
-{"pattern":[{"LOWER":"theirs","POS":"PRON"}],"label":"GENDER_PRONOUN"}
-{"pattern":[{"LOWER":"them","POS":"PRON"}],"label":"GENDER_PRONOUN"}
-{"pattern":[{"LOWER":"themself","POS":"PRON"}],"label":"GENDER_PRONOUN"}
-{"pattern":[{"LOWER":"they","POS":"PRON"}],"label":"GENDER_PRONOUN"}
-{"pattern":[{"LOWER":"ve","POS":"PRON"}],"label":"GENDER_PRONOUN"}
-{"pattern":[{"LOWER":"ver","POS":"PRON"}],"label":"GENDER_PRONOUN"}
-{"pattern":[{"LOWER":"vereself","POS":"PRON"}],"label":"GENDER_PRONOUN"}
-{"pattern":[{"LOWER":"vis","POS":"PRON"}],"label":"GENDER_PRONOUN"}
-{"pattern":[{"LOWER":"xe","POS":"PRON"}],"label":"GENDER_PRONOUN"}
-{"pattern":[{"LOWER":"xem","POS":"PRON"}],"label":"GENDER_PRONOUN"}
-{"pattern":[{"LOWER":"xemself","POS":"PRON"}],"label":"GENDER_PRONOUN"}
-{"pattern":[{"LOWER":"xyr","POS":"PRON"}],"label":"GENDER_PRONOUN"}
-{"pattern":[{"LOWER":"xyrs","POS":"PRON"}],"label":"GENDER_PRONOUN"}
-{"pattern":[{"LOWER":"ze","POS":"PRON"}],"label":"GENDER_PRONOUN"}
-{"pattern":[{"LOWER":"zie","POS":"PRON"}],"label":"GENDER_PRONOUN"}
+{"pattern":[{"LOWER":"ae","POS":"PRON"}],"label":"GENDER_PRONOUN"}
+{"pattern":[{"LOWER":"aer","POS":"PRON"}],"label":"GENDER_PRONOUN"}
+{"pattern":[{"LOWER":"e","POS":"PRON"}],"label":"GENDER_PRONOUN"}
+{"pattern":[{"LOWER":"eir","POS":"PRON"}],"label":"GENDER_PRONOUN"}
+{"pattern":[{"LOWER":"eirs","POS":"PRON"}],"label":"GENDER_PRONOUN"}
+{"pattern":[{"LOWER":"eirself","POS":"PRON"}],"label":"GENDER_PRONOUN"}
+{"pattern":[{"LOWER":"em","POS":"PRON"}],"label":"GENDER_PRONOUN"}
+{"pattern":[{"LOWER":"ey","POS":"PRON"}],"label":"GENDER_PRONOUN"}
+{"pattern":[{"LOWER":"fae","POS":"PRON"}],"label":"GENDER_PRONOUN"}
+{"pattern":[{"LOWER":"faer","POS":"PRON"}],"label":"GENDER_PRONOUN"}
+{"pattern":[{"LOWER":"faers","POS":"PRON"}],"label":"GENDER_PRONOUN"}
+{"pattern":[{"LOWER":"faerself","POS":"PRON"}],"label":"GENDER_PRONOUN"}
+{"pattern":[{"LOWER":"he","POS":"PRON"}],"label":"GENDER_PRONOUN"}
+{"pattern":[{"LOWER":"her","POS":"PRON"}],"label":"GENDER_PRONOUN"}
+{"pattern":[{"LOWER":"hers","POS":"PRON"}],"label":"GENDER_PRONOUN"}
+{"pattern":[{"LOWER":"herself","POS":"PRON"}],"label":"GENDER_PRONOUN"}
+{"pattern":[{"LOWER":"him","POS":"PRON"}],"label":"GENDER_PRONOUN"}
+{"pattern":[{"LOWER":"himself","POS":"PRON"}],"label":"GENDER_PRONOUN"}
+{"pattern":[{"LOWER":"hir","POS":"PRON"}],"label":"GENDER_PRONOUN"}
+{"pattern":[{"LOWER":"hirs","POS":"PRON"}],"label":"GENDER_PRONOUN"}
+{"pattern":[{"LOWER":"hirself","POS":"PRON"}],"label":"GENDER_PRONOUN"}
+{"pattern":[{"LOWER":"his","POS":"PRON"}],"label":"GENDER_PRONOUN"}
+{"pattern":[{"LOWER":"per","POS":"PRON"}],"label":"GENDER_PRONOUN"}
+{"pattern":[{"LOWER":"pers","POS":"PRON"}],"label":"GENDER_PRONOUN"}
+{"pattern":[{"LOWER":"perself","POS":"PRON"}],"label":"GENDER_PRONOUN"}
+{"pattern":[{"LOWER":"she","POS":"PRON"}],"label":"GENDER_PRONOUN"}
+{"pattern":[{"LOWER":"their","POS":"PRON"}],"label":"GENDER_PRONOUN"}
+{"pattern":[{"LOWER":"theirs","POS":"PRON"}],"label":"GENDER_PRONOUN"}
+{"pattern":[{"LOWER":"them","POS":"PRON"}],"label":"GENDER_PRONOUN"}
+{"pattern":[{"LOWER":"themself","POS":"PRON"}],"label":"GENDER_PRONOUN"}
+{"pattern":[{"LOWER":"they","POS":"PRON"}],"label":"GENDER_PRONOUN"}
+{"pattern":[{"LOWER":"ve","POS":"PRON"}],"label":"GENDER_PRONOUN"}
+{"pattern":[{"LOWER":"ver","POS":"PRON"}],"label":"GENDER_PRONOUN"}
+{"pattern":[{"LOWER":"vereself","POS":"PRON"}],"label":"GENDER_PRONOUN"}
+{"pattern":[{"LOWER":"vis","POS":"PRON"}],"label":"GENDER_PRONOUN"}
+{"pattern":[{"LOWER":"xe","POS":"PRON"}],"label":"GENDER_PRONOUN"}
+{"pattern":[{"LOWER":"xem","POS":"PRON"}],"label":"GENDER_PRONOUN"}
+{"pattern":[{"LOWER":"xemself","POS":"PRON"}],"label":"GENDER_PRONOUN"}
+{"pattern":[{"LOWER":"xyr","POS":"PRON"}],"label":"GENDER_PRONOUN"}
+{"pattern":[{"LOWER":"xyrs","POS":"PRON"}],"label":"GENDER_PRONOUN"}
+{"pattern":[{"LOWER":"ze","POS":"PRON"}],"label":"GENDER_PRONOUN"}
+{"pattern":[{"LOWER":"zie","POS":"PRON"}],"label":"GENDER_PRONOUN"}
```

### Comparing `gender-spacy-0.0.4/gender_spacy/gender_spacy.py` & `gender-spacy-0.0.5/gender_spacy/gender_spacy.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,160 +1,160 @@
-import spacy
-from spacy import displacy
-from spacy.tokens import Doc, Span
-
-import itertools
-import pathlib
-from typing import List, Union
-
-import requests
-import tqdm  # progress bar
-
-import srsly
-from . import components
-import toml
-
-import os
-from pathlib import Path
-from distutils.sysconfig import get_python_lib
-
-BASE_DIR = None
-if os.path.isfile(get_python_lib() + "/genderspacy"):
-  BASE_DIR = get_python_lib() + "/genderspacy"
-else:
-  BASE_DIR = os.path.dirname(__file__)
-
-pronoun_patterns = BASE_DIR + "/data/pronoun_patterns"
-pronoun_patterns = list(srsly.read_jsonl(pronoun_patterns))
-
-project_toml = BASE_DIR + "/data/project.toml"
-project_data = toml.load(project_toml)
-
-colors = project_data["colors"]
-visualize_params = project_data["visualize_params"]
-visualize_params["colors"] = colors
-
-pronouns = project_data["pronouns"]
-
-
-class GenderParser:
-    """
-    Args:
-        model_name (str): the spaCy model you wish to use, e.g. en_core_web_lg
-    """
-    def __init__(self, model_name):
-        try:
-            nlp = spacy.load(model_name)
-        except:
-            OSError
-            print(f"Downloading {model_name}...")
-            try:
-                os.system(f"python -m spacy download {model_name}")
-                nlp = spacy.load(model_name)
-            except:
-                OSError
-                raise Exception(f"{model_name} is not a recognized spaCy model.")
-
-        nlp_coref = spacy.load("en_coreference_web_trf")
-
-        # use replace_listeners for the coref components
-        nlp_coref.replace_listeners("transformer", "coref", ["model.tok2vec"])
-        nlp_coref.replace_listeners("transformer", "span_resolver", ["model.tok2vec"])
-
-        # we won't copy over the span cleaner
-        nlp.add_pipe("coref", source=nlp_coref)
-        nlp.add_pipe("span_resolver", source=nlp_coref)
-
-        nlp.add_pipe("pronoun_resolver")
-        ruler = nlp.add_pipe("span_ruler")
-        nlp.add_pipe("pronoun_id")
-        nlp.add_pipe('people_and_spouse')
-        ruler.add_patterns(pronoun_patterns)
-        self.nlp = nlp
-    
-    def process_doc(self, text):
-        """
-        Creates the spaCy doc container and iterates over the entities found by the spaCy NER model.
-        Args:
-            text (str): the text that will be processed.
-        
-        Returns:
-            doc (spaCy Doc): the doc container that contains all the data about gender spans
-        """
-        doc = self.nlp(text)
-
-        original_spans  = list(doc.spans["ruler"])
-        for ent in doc.ents:
-            if ent.label_=="PERSON":
-                ent.label_ = "PERSON_UNKNOWN"
-                original_spans.append(ent)
-        doc.spans["ruler"] = original_spans
-        self.doc = doc
-        return doc
-    def coref_resolution(self):
-        """
-        Uses the spaCy Experimental Coref Model to identify all connections between PERSON entities and pronouns.
-        If there is a cluster where a PERSON entity has a gender-specific pronoun, the span labels are adjusted accordingly.
-        """
-        spans = list(self.doc.spans["ruler"])
-        # pronouns = {"female": ["she", "her", "hers", "herself"], "male": ["he", "him", "his", "himself"]}
-
-        def parse_gender(token, pronoun_set, gender):
-            if token.text.lower() not in pronoun_set:
-                span = self.doc.char_span(token.start_char, token.end_char, label=gender.upper())
-                span = Span(self.doc, span.start, span.end, label=f"PERSON_{gender.upper()}_COREF")
-                return span
-
-        for key, cluster in self.doc.spans.items():
-            if "head" in key:
-                head_tokens = [token.text.lower() for token in cluster]
-                for gender, pronoun_set in pronouns.items():
-                    if any(pronoun in head_tokens for pronoun in pronoun_set):
-                        for token in cluster:
-                            gender_res = parse_gender(token, pronoun_set, gender.upper())
-                            if gender_res != None:
-                                num = key.split("_")[-1]
-                                res_cluster = self.doc.spans[f"coref_clusters_{num}"]
-                                for token_set in res_cluster:
-                                    for token2 in token_set:
-                                        if token2.pos_ in "PROPN":
-                                            span = self.doc.char_span(token2.idx, token2.idx+len(token2.text), label=gender.upper())
-                                            span = Span(self.doc, span.start, span.end, label=f"PERSON_{gender.upper()}_COREF")
-                                            spans.append(span)
-                                        # elif token2.pos_ == "NOUN":
-                                        #     span = self.doc.char_span(token2.idx, token2.idx+len(token2.text), label=gender.upper())
-                                        #     span = Span(self.doc, span.start, span.end, label=f"REL_{gender.upper()}_COREF")                  
-                                        #     spans.append(span)
-        def connect_spans(spans):
-            for i, span in enumerate(spans):
-                for span2 in spans:
-                    if span.end == span2.start:
-                        if (self.doc[span.start].pos_ and self.doc[span2.start].pos_) == "PROPN":
-                            new_span = Span(self.doc, span.start, span.end+1, label=span.label_)
-                            spans.append(new_span)
-            return spans
-        spans = connect_spans(spans)
-        # spans = connect_spans(spans)
-        final_spans = []
-        for span in spans:
-            rem = False
-            if span.label_ == "PERSON_UNKNOWN":
-                for span2 in spans:
-                    if span2.start == span.start:
-                        rem = True
-            if rem == False:
-                final_spans.append(span)
-        merged_spans = spacy.util.filter_spans(final_spans)
-        self.doc.spans["ruler"] = merged_spans
-        return self.doc
-
-    def visualize(self, jupyter=True):
-        """
-        visualizes the spaCy doc Container on the spans
-        Args:
-            jupyter (Bool): affects if the visualization loads in Jupyter or as HTML
-        """
-        if jupyter==True:
-            displacy.render(self.doc, style="span", options=visualize_params, jupyter=True)
-        else:
-            displacy.render(self.doc, style="span", options={"spans_key": "ruler"})
+import spacy
+from spacy import displacy
+from spacy.tokens import Doc, Span
+
+import itertools
+import pathlib
+from typing import List, Union
+
+import requests
+import tqdm  # progress bar
+
+import srsly
+from . import components
+import toml
+
+import os
+from pathlib import Path
+from distutils.sysconfig import get_python_lib
+
+BASE_DIR = None
+if os.path.isfile(get_python_lib() + "/genderspacy"):
+  BASE_DIR = get_python_lib() + "/genderspacy"
+else:
+  BASE_DIR = os.path.dirname(__file__)
+
+pronoun_patterns = BASE_DIR + "/data/pronoun_patterns"
+pronoun_patterns = list(srsly.read_jsonl(pronoun_patterns))
+
+project_toml = BASE_DIR + "/data/project.toml"
+project_data = toml.load(project_toml)
+
+colors = project_data["colors"]
+visualize_params = project_data["visualize_params"]
+visualize_params["colors"] = colors
+
+pronouns = project_data["pronouns"]
+
+
+class GenderParser:
+    """
+    Args:
+        model_name (str): the spaCy model you wish to use, e.g. en_core_web_lg
+    """
+    def __init__(self, model_name):
+        try:
+            nlp = spacy.load(model_name)
+        except:
+            OSError
+            print(f"Downloading {model_name}...")
+            try:
+                os.system(f"python -m spacy download {model_name}")
+                nlp = spacy.load(model_name)
+            except:
+                OSError
+                raise Exception(f"{model_name} is not a recognized spaCy model.")
+
+        nlp_coref = spacy.load("en_coreference_web_trf")
+
+        # use replace_listeners for the coref components
+        nlp_coref.replace_listeners("transformer", "coref", ["model.tok2vec"])
+        nlp_coref.replace_listeners("transformer", "span_resolver", ["model.tok2vec"])
+
+        # we won't copy over the span cleaner
+        nlp.add_pipe("coref", source=nlp_coref)
+        nlp.add_pipe("span_resolver", source=nlp_coref)
+
+        nlp.add_pipe("pronoun_resolver")
+        ruler = nlp.add_pipe("span_ruler")
+        nlp.add_pipe("pronoun_id")
+        nlp.add_pipe('people_and_spouse')
+        ruler.add_patterns(pronoun_patterns)
+        self.nlp = nlp
+    
+    def process_doc(self, text):
+        """
+        Creates the spaCy doc container and iterates over the entities found by the spaCy NER model.
+        Args:
+            text (str): the text that will be processed.
+        
+        Returns:
+            doc (spaCy Doc): the doc container that contains all the data about gender spans
+        """
+        doc = self.nlp(text)
+
+        original_spans  = list(doc.spans["ruler"])
+        for ent in doc.ents:
+            if ent.label_=="PERSON":
+                ent.label_ = "PERSON_UNKNOWN"
+                original_spans.append(ent)
+        doc.spans["ruler"] = original_spans
+        self.doc = doc
+        return doc
+    def coref_resolution(self):
+        """
+        Uses the spaCy Experimental Coref Model to identify all connections between PERSON entities and pronouns.
+        If there is a cluster where a PERSON entity has a gender-specific pronoun, the span labels are adjusted accordingly.
+        """
+        spans = list(self.doc.spans["ruler"])
+        # pronouns = {"female": ["she", "her", "hers", "herself"], "male": ["he", "him", "his", "himself"]}
+
+        def parse_gender(token, pronoun_set, gender):
+            if token.text.lower() not in pronoun_set:
+                span = self.doc.char_span(token.start_char, token.end_char, label=gender.upper())
+                span = Span(self.doc, span.start, span.end, label=f"PERSON_{gender.upper()}_COREF")
+                return span
+
+        for key, cluster in self.doc.spans.items():
+            if "head" in key:
+                head_tokens = [token.text.lower() for token in cluster]
+                for gender, pronoun_set in pronouns.items():
+                    if any(pronoun in head_tokens for pronoun in pronoun_set):
+                        for token in cluster:
+                            gender_res = parse_gender(token, pronoun_set, gender.upper())
+                            if gender_res != None:
+                                num = key.split("_")[-1]
+                                res_cluster = self.doc.spans[f"coref_clusters_{num}"]
+                                for token_set in res_cluster:
+                                    for token2 in token_set:
+                                        if token2.pos_ in "PROPN":
+                                            span = self.doc.char_span(token2.idx, token2.idx+len(token2.text), label=gender.upper())
+                                            span = Span(self.doc, span.start, span.end, label=f"PERSON_{gender.upper()}_COREF")
+                                            spans.append(span)
+                                        # elif token2.pos_ == "NOUN":
+                                        #     span = self.doc.char_span(token2.idx, token2.idx+len(token2.text), label=gender.upper())
+                                        #     span = Span(self.doc, span.start, span.end, label=f"REL_{gender.upper()}_COREF")                  
+                                        #     spans.append(span)
+        def connect_spans(spans):
+            for i, span in enumerate(spans):
+                for span2 in spans:
+                    if span.end == span2.start:
+                        if (self.doc[span.start].pos_ and self.doc[span2.start].pos_) == "PROPN":
+                            new_span = Span(self.doc, span.start, span.end+1, label=span.label_)
+                            spans.append(new_span)
+            return spans
+        spans = connect_spans(spans)
+        # spans = connect_spans(spans)
+        final_spans = []
+        for span in spans:
+            rem = False
+            if span.label_ == "PERSON_UNKNOWN":
+                for span2 in spans:
+                    if span2.start == span.start:
+                        rem = True
+            if rem == False:
+                final_spans.append(span)
+        merged_spans = spacy.util.filter_spans(final_spans)
+        self.doc.spans["ruler"] = merged_spans
+        return self.doc
+
+    def visualize(self, jupyter=True):
+        """
+        visualizes the spaCy doc Container on the spans
+        Args:
+            jupyter (Bool): affects if the visualization loads in Jupyter or as HTML
+        """
+        if jupyter==True:
+            displacy.render(self.doc, style="span", options=visualize_params, jupyter=True)
+        else:
+            displacy.render(self.doc, style="span", options={"spans_key": "ruler"})
```

### Comparing `gender-spacy-0.0.4/gender_spacy.egg-info/PKG-INFO` & `gender-spacy-0.0.5/gender_spacy.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,88 +1,89 @@
-Metadata-Version: 2.1
-Name: gender-spacy
-Version: 0.0.4
-Summary: A spaCy component for identifying grammatical gender in English texts.
-Author: WJB Mattingly
-Description-Content-Type: text/markdown
-
-
-![gender spacy logo](https://github.com/sidatasciencelab/gender-spacy/raw/main/images/genderspacy-logo.png)
-
-# About
-
-Gender spaCy is a heuristic and machine learning pipeline that allows users to identify gender in an ethical way using gender-specific context. It is designed to sit alongside a standard spaCy pipeline (only English supported currently). The majority of the pipeline is rules-based, relying on titles and pronouns to identify gender as presented in the text. **It is important to note that this pipeline does not seek to assign gender to an individual, rather contextually identify an entity's gender within the context of a text.**
-
-There are Python libraries, such as gender-resolver that assign gender based on the statistical usage of first names in a given region. This, however, gets into problematic territory and is not as reliable as gender-based context (such as titles and pronouns). As a result, this pipeline opts out of leveraging these libraries. Instead, entities identified as PERSON by the spaCy NER model are altered to the span label of PERSON_UNKNOWN. Next, this pipeline leverages the new experimental coreference resolution model from ExplosionAI. It looks at all clusters of linked tokens. If any of them align with PERSON_UNKNOWN tags *and* gender-specific pronouns are used, the entity's label is changed to a gender-specific label, e.g. PERSON_FEMALE, PERSON_MALE, PERSON_NEUTRAL. In addition, terms that are nouns that are linked to a specific person receive the tag "REL_MALE/FEMALE_COREF".
-
-In addition to this, all gender-neutral pronouns are also identified and labeled as spans. This includes male, female, and gender neutral pronouns. Even transformer models have difficulty correctly parsing certain gender neutral pronouns due to their toponym nature, such as "per" which can function in English as an adverb (Per our discusion yesterday, I want to go to the store.) or as a gender neutral pronoun (Per went to the store yesterday). With a few extra rules, Gender spaCy corrects the POS tags for these toponyms in addition to placing all pronouns in the spans ruler.
-
-Users can access all gender span data under doc.spans["ruler].
-
-# Installation
-
-Because this pipeline leverages spaCy's new experimental coreference resolution model, it is best to install Gender spaCy in a fresh environment.
-
-First, it is good to create a new environment.
-
-```python
-conda create --name="gender-spacy" python=3.9
-```
-
-Now, activate the environment:
-
-```python
-conda activate gender-spacy
-```
-
-Next, install GenderSpaCy
-
-```python
-pip install gender-spacy
-```
-
-Finally, for the pipeline to perform coreference resolution, you should install the latest version of the spaCy experimental coreference resolution model.
-
-```python
-pip install https://github.com/explosion/spacy-experimental/releases/download/v0.6.0/en_coreference_web_trf-3.4.0a0-py3-none-any.whl
-```
-
-
-
-# Usage
-
-```python
-
-# import the library
-from gender_spacy import gender_spacy as gs
-
-# create the GenderParser nlp class.
-# This will take one argument: the spaCy model you wish to use
-nlp = gs.GenderParser("en_core_web_sm")
-
-# create a text and pass it to the the nlp via the process_doc() method.
-text = """
-During the year Miss Densmore arranged in final order 245 songs to accompany her manuscript on Seminole music and revised portions of the text to conform to this arrangement of the material. 
-
-In December 1941 Miss Densmore was appointed as consultant at The National Archives for work in connection with the Smithsonian Densmore collection of sound recordings of American Indian music, and duiing the ensuing months she was engaged in planning the organization of the collection.
-"""
-doc = nlp.process_doc(text)
-
-# perform coreference resolution on the doc container
-# This part of the library comes from spacy-experimental
-doc = nlp.coref_resolution()
-
-# Visualize the result:
-nlp.visualize()
-```
-
-## Expected Result
-
-![result demo](https://github.com/sidatasciencelab/gender-spacy/raw/main/images/result.JPG)
-
-
-
-# CITATIONS
-Source for gender pronouns: https://uwm.edu/lgbtrc/support/gender-pronouns/
-
-Source for Coreference Resolution: https://explosion.ai/blog/coref
-Discussion for Coref Code: https://github.com/explosion/spaCy/discussions/11585
+Metadata-Version: 2.1
+Name: gender-spacy
+Version: 0.0.5
+Summary: A spaCy component for identifying grammatical gender in English texts.
+Author: WJB Mattingly
+Description-Content-Type: text/markdown
+
+
+![gender spacy logo](https://github.com/sidatasciencelab/gender-spacy/raw/main/images/genderspacy-logo.png)
+
+# About
+
+Gender spaCy is a heuristic and machine learning pipeline that allows users to identify gender in an ethical way using gender-specific context. It is designed to sit alongside a standard spaCy pipeline (only English supported currently). The majority of the pipeline is rules-based, relying on titles and pronouns to identify gender as presented in the text. **It is important to note that this pipeline does not seek to assign gender to an individual, rather contextually identify an entity's gender within the context of a text.**
+
+There are Python libraries, such as gender-resolver that assign gender based on the statistical usage of first names in a given region. This, however, gets into problematic territory and is not as reliable as gender-based context (such as titles and pronouns). As a result, this pipeline opts out of leveraging these libraries. Instead, entities identified as PERSON by the spaCy NER model are altered to the span label of PERSON_UNKNOWN. Next, this pipeline leverages the new experimental coreference resolution model from ExplosionAI. It looks at all clusters of linked tokens. If any of them align with PERSON_UNKNOWN tags *and* gender-specific pronouns are used, the entity's label is changed to a gender-specific label, e.g. PERSON_FEMALE, PERSON_MALE, PERSON_NEUTRAL. In addition, terms that are nouns that are linked to a specific person receive the tag "REL_MALE/FEMALE_COREF".
+
+In addition to this, all gender-neutral pronouns are also identified and labeled as spans. This includes male, female, and gender neutral pronouns. Even transformer models have difficulty correctly parsing certain gender neutral pronouns due to their toponym nature, such as "per" which can function in English as an adverb (Per our discusion yesterday, I want to go to the store.) or as a gender neutral pronoun (Per went to the store yesterday). With a few extra rules, Gender spaCy corrects the POS tags for these toponyms in addition to placing all pronouns in the spans ruler.
+
+Users can access all gender span data under doc.spans["ruler].
+
+# Installation
+
+Because this pipeline leverages spaCy's new experimental coreference resolution model, it is best to install Gender spaCy in a fresh environment.
+
+First, it is good to create a new environment.
+
+```python
+conda create --name="gender-spacy" python=3.9
+```
+
+Now, activate the environment:
+
+```python
+conda activate gender-spacy
+```
+
+Next, install GenderSpaCy
+
+```python
+pip install gender-spacy
+```
+
+Finally, for the pipeline to perform coreference resolution, you should install the latest version of the spaCy experimental coreference resolution model.
+
+```python
+pip install https://github.com/explosion/spacy-experimental/releases/download/v0.6.0/en_coreference_web_trf-3.4.0a0-py3-none-any.whl
+```
+
+
+
+# Usage
+
+```python
+
+# import the library
+from gender_spacy import gender_spacy as gs
+
+# create the GenderParser nlp class.
+# This will take one argument: the spaCy model you wish to use
+nlp = gs.GenderParser("en_core_web_sm")
+
+# create a text and pass it to the the nlp via the process_doc() method.
+text = """
+Maya Angelou was an American memoirist, popular poet, and civil rights activist. She published seven autobiographies, three books of essays, several books of poetry, and is credited with a list of plays, movies, and television shows spanning over 50 years.
+
+Jerome Allen Seinfeld is an American stand-up comedian, actor, writer, and producer. He is best known for playing a semi-fictionalized version of himself in the sitcom Seinfeld (1989–1998), which he created and wrote with Larry David.
+"""
+doc = nlp.process_doc(text)
+
+# perform coreference resolution on the doc container
+# This part of the library comes from spacy-experimental
+doc = nlp.coref_resolution()
+
+# Visualize the result:
+nlp.visualize()
+```
+
+## Expected Result
+
+![result demo](https://github.com/sidatasciencelab/gender-spacy/raw/main/images/demo.JPG)
+
+
+
+# CITATIONS
+Source for gender pronouns: https://uwm.edu/lgbtrc/support/gender-pronouns/
+
+Source for Coreference Resolution: https://explosion.ai/blog/coref
+
+Discussion for Coref Code: https://github.com/explosion/spaCy/discussions/11585
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

