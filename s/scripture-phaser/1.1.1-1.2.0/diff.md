# Comparing `tmp/scripture_phaser-1.1.1.tar.gz` & `tmp/scripture_phaser-1.2.0.tar.gz`

## Comparing `scripture_phaser-1.1.1.tar` & `scripture_phaser-1.2.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     1308 2020-02-02 00:00:00.000000 scripture_phaser-1.1.1/RELEASE_CHECKLIST.md
--rw-r--r--   0        0        0     1721 2020-02-02 00:00:00.000000 scripture_phaser-1.1.1/requirements.txt
--rw-r--r--   0        0        0   247151 2020-02-02 00:00:00.000000 scripture_phaser-1.1.1/doc/demo.gif
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 scripture_phaser-1.1.1/doc/scripture_phaser.tape
--rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 scripture_phaser-1.1.1/src/__init__.py
--rw-r--r--   0        0        0     5347 2020-02-02 00:00:00.000000 scripture_phaser-1.1.1/src/agents.py
--rw-r--r--   0        0        0     8786 2020-02-02 00:00:00.000000 scripture_phaser-1.1.1/src/api.py
--rw-r--r--   0        0        0    23625 2020-02-02 00:00:00.000000 scripture_phaser-1.1.1/src/cli.py
--rw-r--r--   0        0        0    14548 2020-02-02 00:00:00.000000 scripture_phaser-1.1.1/src/enums.py
--rw-r--r--   0        0        0     2301 2020-02-02 00:00:00.000000 scripture_phaser-1.1.1/src/exceptions.py
--rw-r--r--   0        0        0     2309 2020-02-02 00:00:00.000000 scripture_phaser-1.1.1/src/models.py
--rw-r--r--   0        0        0     4411 2020-02-02 00:00:00.000000 scripture_phaser-1.1.1/src/passage.py
--rw-r--r--   0        0        0    17915 2020-02-02 00:00:00.000000 scripture_phaser-1.1.1/src/reference.py
--rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 scripture_phaser-1.1.1/src/scripture_phaser.py
--rw-r--r--   0        0        0     3620 2020-02-02 00:00:00.000000 scripture_phaser-1.1.1/src/stats.py
--rw-r--r--   0        0        0     5422 2020-02-02 00:00:00.000000 scripture_phaser-1.1.1/src/verse.py
--rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 scripture_phaser-1.1.1/test/__init__.py
--rw-r--r--   0        0        0     4893 2020-02-02 00:00:00.000000 scripture_phaser-1.1.1/test/test_api.py
--rwxr-xr-x   0        0        0     2457 2020-02-02 00:00:00.000000 scripture_phaser-1.1.1/test/test_base.py
--rw-r--r--   0        0        0     9528 2020-02-02 00:00:00.000000 scripture_phaser-1.1.1/test/test_passage.py
--rw-r--r--   0        0        0    11308 2020-02-02 00:00:00.000000 scripture_phaser-1.1.1/test/test_reference.py
--rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 scripture_phaser-1.1.1/test/test_verse.py
--rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 scripture_phaser-1.1.1/.gitignore
--rw-r--r--   0        0        0     1467 2020-02-02 00:00:00.000000 scripture_phaser-1.1.1/LICENSE
--rw-r--r--   0        0        0     3998 2020-02-02 00:00:00.000000 scripture_phaser-1.1.1/README.md
--rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 scripture_phaser-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     6621 2020-02-02 00:00:00.000000 scripture_phaser-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 scripture_phaser-1.2.0/RELEASE_CHECKLIST.md
+-rw-r--r--   0        0        0     1721 2020-02-02 00:00:00.000000 scripture_phaser-1.2.0/requirements.txt
+-rw-r--r--   0        0        0   289938 2020-02-02 00:00:00.000000 scripture_phaser-1.2.0/doc/demo.gif
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 scripture_phaser-1.2.0/doc/scripture_phaser.tape
+-rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 scripture_phaser-1.2.0/src/__init__.py
+-rw-r--r--   0        0        0     5347 2020-02-02 00:00:00.000000 scripture_phaser-1.2.0/src/agents.py
+-rw-r--r--   0        0        0     8675 2020-02-02 00:00:00.000000 scripture_phaser-1.2.0/src/api.py
+-rw-r--r--   0        0        0    20816 2020-02-02 00:00:00.000000 scripture_phaser-1.2.0/src/cli.py
+-rw-r--r--   0        0        0    14548 2020-02-02 00:00:00.000000 scripture_phaser-1.2.0/src/enums.py
+-rw-r--r--   0        0        0     2301 2020-02-02 00:00:00.000000 scripture_phaser-1.2.0/src/exceptions.py
+-rw-r--r--   0        0        0     2284 2020-02-02 00:00:00.000000 scripture_phaser-1.2.0/src/models.py
+-rw-r--r--   0        0        0     4353 2020-02-02 00:00:00.000000 scripture_phaser-1.2.0/src/passage.py
+-rw-r--r--   0        0        0    17915 2020-02-02 00:00:00.000000 scripture_phaser-1.2.0/src/reference.py
+-rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 scripture_phaser-1.2.0/src/scripture_phaser.py
+-rw-r--r--   0        0        0     3894 2020-02-02 00:00:00.000000 scripture_phaser-1.2.0/src/stats.py
+-rw-r--r--   0        0        0     5422 2020-02-02 00:00:00.000000 scripture_phaser-1.2.0/src/verse.py
+-rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 scripture_phaser-1.2.0/test/__init__.py
+-rw-r--r--   0        0        0     4893 2020-02-02 00:00:00.000000 scripture_phaser-1.2.0/test/test_api.py
+-rwxr-xr-x   0        0        0     2432 2020-02-02 00:00:00.000000 scripture_phaser-1.2.0/test/test_base.py
+-rw-r--r--   0        0        0     9458 2020-02-02 00:00:00.000000 scripture_phaser-1.2.0/test/test_passage.py
+-rw-r--r--   0        0        0    11308 2020-02-02 00:00:00.000000 scripture_phaser-1.2.0/test/test_reference.py
+-rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 scripture_phaser-1.2.0/test/test_verse.py
+-rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 scripture_phaser-1.2.0/.gitignore
+-rw-r--r--   0        0        0     1467 2020-02-02 00:00:00.000000 scripture_phaser-1.2.0/LICENSE
+-rw-r--r--   0        0        0     3303 2020-02-02 00:00:00.000000 scripture_phaser-1.2.0/README.md
+-rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 scripture_phaser-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     5926 2020-02-02 00:00:00.000000 scripture_phaser-1.2.0/PKG-INFO
```

### Comparing `scripture_phaser-1.1.1/RELEASE_CHECKLIST.md` & `scripture_phaser-1.2.0/RELEASE_CHECKLIST.md`

 * *Files 14% similar despite different names*

```diff
@@ -14,10 +14,10 @@
 
 6. Make sure that you don't have a preexisting dist folder in the root of the scripture_phaser repository. On the `MAJOR.MINOR.x` branch, run: `python -m build`.
 
 7. From the root of the scripture_phaser repository, run: `python -m twine upload --repository pypi dist/*`.
 
 8. Tag the commit on the `MAJOR.MINOR.x` branch with the MAJOR.MINOR.PATCH version number. `git tag MAJOR.MINOR.PATCH COMMIT`
 
-9. Push the tag to GitHub. `git push tag MAJOR.MINOR.PATCH`.
+9. Push the tag to GitHub. `git push origin MAJOR.MINOR.PATCH`.
 
 10. Create a release on GitHub by clicking the tags button to the right of the branch selection dropdown. Provide a detailed description of the release and select the tag that was just pushed to mark the release. Upload the contents of the dist folder in the scripture_phaser directory to the release.
```

### Comparing `scripture_phaser-1.1.1/requirements.txt` & `scripture_phaser-1.2.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `scripture_phaser-1.1.1/src/__init__.py` & `scripture_phaser-1.2.0/src/__init__.py`

 * *Files identical despite different names*

### Comparing `scripture_phaser-1.1.1/src/agents.py` & `scripture_phaser-1.2.0/src/agents.py`

 * *Files identical despite different names*

### Comparing `scripture_phaser-1.1.1/src/api.py` & `scripture_phaser-1.2.0/src/api.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,15 +40,14 @@
 from src.enums import App
 from src.enums import AppDefaults
 from src.stats import Stats
 from src.models import Attempt
 from src.passage import Passage
 from src.enums import Translations
 from src.reference import Reference
-from src.exceptions import EditorNotFound
 from src.exceptions import InvalidReference
 from src.exceptions import InvalidTranslation
 
 
 class API:
     def __init__(self):
         self.stats = Stats()
@@ -175,16 +174,14 @@
             ans = self.get_fast_recitation_ans(reference)
 
             if text == ans:
                 score = 1
             else:
                 n_correct = sum([1 for i in range(len(ans)) if text[i] == ans[i]])
                 score = n_correct / len(ans)
-
-                passage_words = self.passage.show().split()
         else:
             ans = self.get_recitation_ans(reference)
 
             if text == ans:
                 score = 1
             else:
                 n_correct_chars, n_incorrect_chars = 0, 0
@@ -197,15 +194,15 @@
                     elif tag == "insert":
                         n_incorrect_chars += j2 - j1
                     elif tag == "equal":
                         n_correct_chars += i2 - i1
 
                 score = n_correct_chars / (n_correct_chars + n_incorrect_chars)
 
-        attempt = Attempt.create(
+        Attempt.create(
             random_single_verse=self.random_single_verse,
             reference=reference.ref_str,
             score=score,
             attempt=text,
             datetime=datetime.datetime.now()
         )
 
@@ -222,10 +219,10 @@
         text = "".join([char for char in raw_text if char.isalnum() or char.isspace()])
         return [word[0] for word in text.split()]
 
     def get_recitation_ans(self, reference):
         if self.random_single_verse:
             passage = Passage(reference, self.translation)
             passage.populate([v.text for v in self.passage.verses if v.reference.ref_str == reference.ref_str])
-            ans = passage.show()
+            return passage.show()
         else:
-            ans = self.passage.show()
+            return self.passage.show()
```

### Comparing `scripture_phaser-1.1.1/src/cli.py` & `scripture_phaser-1.2.0/src/cli.py`

 * *Files 13% similar despite different names*

```diff
@@ -31,39 +31,37 @@
 # ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
 # POSSIBILITY OF SUCH DAMAGE.
 
 import os
 import platform
 import readchar
 import argparse
-import datetime
 import subprocess
 from shutil import which
 from src.api import API
 from src.enums import App
 from difflib import SequenceMatcher
 from src.enums import TermColours as TC
 from src.exceptions import EditorNotFound
-from src.exceptions import InvalidDateFilter
 from src.exceptions import InvalidTranslation
 
+NUM_DAYS_FOR_GOOD_STREAK = 7
+GOOD_YEARLY_ATTEMPT_COUNT = 180
+GOOD_SCORE = 0.75
+
 
 class CLISTR:
     def __init__(self, api):
         self.api = api
 
     @staticmethod
     def CLI_PROMPT():
         return "> "
 
     @staticmethod
-    def STATS_CLI_PROMPT():
-        return f"{TC.WHITE}[{TC.GREEN}STATS{TC.WHITE}] > "
-
-    @staticmethod
     def DESCRIPTION():
         return "scripture_phaser helps you to memorize the Bible."
 
     @staticmethod
     def LICENSE():
         return App.license.value
 
@@ -78,40 +76,29 @@
     @staticmethod
     def LICENSE_HELP():
         return "show the license"
 
     @staticmethod
     def WELCOME():
         return (
-            f"scripture_phaser helps you to memorize the Bible.\n"
-            f"Copyright (C) 2023-2024 Nolan McMahon"
-        )
-
-    @staticmethod
-    def WELCOME_STATS():
-        return (
-            f"You are now in the statistics viewer!\n"
-            f"To exit back to the main prompt, press 'q'."
+            "scripture_phaser helps you to memorize the Bible.\n"
+            "Copyright (C) 2023-2024 Nolan McMahon"
         )
 
     @staticmethod
     def NO_REFERENCE():
         return f"Reference:{TC.RED} No reference set{TC.WHITE}"
 
     @staticmethod
     def STATS_RESET_WARNING():
         return (
             f"Are you sure that you want to reset your statistics? [{TC.RED}y{TC.WHITE}/{TC.GREEN}N{TC.WHITE}] "
         )
 
     @staticmethod
-    def CLEAR_STATS_FILTERS():
-        return f"Clearing start date and end date filters."
-
-    @staticmethod
     def STATS_RESET():
         return f"Statistics reset{TC.WHITE}"
 
     @staticmethod
     def HELP():
         return (
             f"This is the {TC.CYAN}Normal Mode{TC.WHITE}.\n\n"
@@ -121,38 +108,22 @@
             f"\t{TC.BLUE}H{TC.WHITE} - Prints this help message\n"
             f"\t{TC.BLUE}I{TC.WHITE} - List available translations\n"
             f"\t{TC.BLUE}L{TC.WHITE} - Lists selected reference, random single verse recitations and translation\n"
             f"\t{TC.BLUE}M{TC.WHITE} - Toggles whether or not to practice random single verses\n"
             f"\t{TC.BLUE}N{TC.WHITE} - Toggles whether or not to include the passage numbers\n"
             f"\t{TC.BLUE}P{TC.WHITE} - Practice the current reference\n"
             f"\t{TC.BLUE}R{TC.WHITE} - Sets the reference\n"
-            f"\t{TC.BLUE}S{TC.WHITE} - View your statistics\n"
+            f"\t{TC.BLUE}S{TC.WHITE} - View recitation statistics\n"
+            f"\t{TC.BLUE}D{TC.WHITE} - Deletes all past statistics\n"
             f"\t{TC.BLUE}T{TC.WHITE} - Set the translation\n"
             f"\t{TC.BLUE}V{TC.WHITE} - Preview current reference\n"
             f"\t{TC.BLUE}Q{TC.WHITE} - Quits"
         )
 
     @staticmethod
-    def STATS_HELP():
-        return (
-            f"This is the {TC.CYAN}Statistics Mode{TC.WHITE}.\n\n"
-            "Here you can view summary statistics based on your "
-            "past recitation attempts.\n\n"
-            f"The {TC.CYAN}Statistics Mode{TC.WHITE} can be "
-            "controlled using:\n"
-            f"\t{TC.BLUE}SD{TC.WHITE} - Set the start date used to filter your statistics\n"
-            f"\t{TC.BLUE}ED{TC.WHITE} - Set the end date used to filter your statistics\n"
-            f"\t{TC.BLUE}L{TC.WHITE}  - Show all filters and their values\n"
-            f"\t{TC.BLUE}C{TC.WHITE}  - Clear all filters\n"
-            f"\t{TC.BLUE}A{TC.WHITE}  - List all verses attempted\n"
-            f"\t{TC.BLUE}R{TC.WHITE}  - Rank all attempted passages by average score\n"
-            f"\t{TC.BLUE}D{TC.WHITE}  - Reset statistics"
-        )
-
-    @staticmethod
     def FAST_HELP():
         return (
             f"This is the {TC.CYAN}Fast Recitation Mode{TC.WHITE}.\n\n"
             f"Type the first letter of the next word in the passage "
             f"(it is case sensitive) to advance the recitation by one word. "
             f"If you type the wrong letter twice, the reciation will "
             f"advance by one word and will reveal the correct word in red.\n\n"
@@ -160,111 +131,118 @@
             "can be controlled using:\n"
             f"\t{TC.BLUE}?{TC.WHITE}        - Print this help message\n"
             f"\t{TC.BLUE}Ctrl + c{TC.WHITE} - Stop the recitation\n"
         )
 
     @staticmethod
     def REFERENCE_PROMPT():
-        return f"Reference: "
+        return "Reference: "
 
     @staticmethod
     def TRANSLATION_PROMPT():
-        return f"Translation: "
-
-    @staticmethod
-    def SET_START_DATE():
-        return f"Set Start Date to Filter by: (Leave Blank to Unset)"
-
-    @staticmethod
-    def SET_END_DATE():
-        return f"Set End Date to Filter by: (Leave Blank to Unset):"
-
-    @staticmethod
-    def YEAR_PROMPT():
-        return f"Year (yyyy): "
-
-    @staticmethod
-    def MONTH_PROMPT():
-        return f"Month (mm): "
-
-    @staticmethod
-    def DAY_PROMPT():
-        return f"Day (dd): "
+        return "Translation: "
 
     @staticmethod
     def NO_EDITOR():
         return (
             f"{TC.RED}No editor found! {TC.WHITE}"
             "Try setting your 'EDITOR' environmental variable and "
             "restarting scripture_phaser or reciting with "
             f"{TC.CYAN}Fast Recitation Mode{TC.WHITE}."
         )
 
     @staticmethod
     def EXIT_TO_NORMAL_MODE():
         return "Exiting to Normal Mode!"
 
-    def START_DATE(self): return f"Start Date (yyyy-mm-dd):{TC.YELLOW} {self.api.stats.start_date}{TC.WHITE}"
-
-    def END_DATE(self):
-        return f"End Date (yyyy-mm-dd):{TC.YELLOW} {self.api.stats.end_date}{TC.WHITE}"
-
-    def ALL_ATTEMPTED_VERSES(self):
-        start = self.api.stats.start_date
-        if isinstance(start, datetime.date):
-            start = start.strftime("%B %d, %Y")
-
-        end = self.api.stats.end_date
-        if isinstance(end, datetime.date):
-            end = end.strftime("%B %d, %Y")
-
-        refs = self.api.stats.all_attempted_verses()
-        if len(refs) == 0:
-            string = "You haven't recorded any attempts yet!"
-        else:
-            last_ref = refs.pop()
-            if len(refs) == 0:
-                ref_str = last_ref
-            else:
-                ref_str = ", ".join(refs) + f" and {last_ref}"
-
-            if start is not None and end is not None:
-                string = f"Between {start} and {end}, you've attempted {ref_str}."
-            elif start is not None:
-                string = f"Since {start}, you've attempted {ref_str}."
-            elif end is not None:
-                string = f"Prior to {end}, you've attempted {ref_str}."
-            else:
-                string = f"You've attempted {ref_str} before."
-        return string
-
     def ALL_VERSES_RANKED(self):
-        start = self.api.stats.start_date
-        if isinstance(start, datetime.date):
-            start = start.strftime("%B %d, %Y")
-
-        end = self.api.stats.end_date
-        if isinstance(end, datetime.date):
-            end = end.strftime("%B %d, %Y")
+        verse_scores, verse_counts = self.api.stats.all_verses_ranked()
 
-        verses = self.api.stats.all_verses_ranked()
-        if len(verses) == 0:
+        # Used to Make Output Columnar
+        max_attempt_width = len(str(max(verse_counts.values())))
+
+        if len(verse_counts) == 0:
             string = "You haven't recorded any attempts yet!"
         else:
             string = ""
-            sorted_verses = sorted(verses.items(), key=lambda item: item[1], reverse=True)
+            sorted_verses = sorted(verse_scores.items(), key=lambda item: item[1], reverse=True)
             for ref, score in sorted_verses:
+                attempt_count = verse_counts[ref]
+                if attempt_count == 1:
+                    string += "[1 Attempt] "
+                    string += " " * max_attempt_width
+                else:
+                    string += f"[{attempt_count} Attempts] "
+                    string += " " * (max_attempt_width - 1)
+
                 score = round(score * 100, 1)
-                if score > 75:
+                if score == 100:
                     string += f"({TC.GREEN}{score}%{TC.WHITE}) {ref}\n"
+                elif score > 75:
+                    string += f"({TC.GREEN}{score}%{TC.WHITE})  {ref}\n"
+                elif score >= 10:
+                    string += f"({TC.RED}{score}%{TC.WHITE})  {ref}\n"
                 else:
-                    string += f"({TC.RED}{score}%{TC.WHITE}) {ref}\n"
+                    string += f"({TC.RED}{score}%{TC.WHITE})   {ref}\n"
+
             string = string[:-1]
         return string
 
+    def STATS_GAMIFICATION(self):
+        streak = self.api.stats.get_streak()
+        if streak < NUM_DAYS_FOR_GOOD_STREAK:
+            streak_str = f"Current Recititation Streak is {TC.RED}{streak}{TC.WHITE}."
+        else:
+            streak_str = f"Current Recitation Streak is {TC.GREEN}{streak}{TC.WHITE}!"
+
+        past_year_attempt_count = self.api.stats.get_num_attempts_past_year()
+        if past_year_attempt_count < GOOD_YEARLY_ATTEMPT_COUNT:
+            past_year_attempt_count_str = f"{TC.RED}{past_year_attempt_count}{TC.WHITE} recitations in the past year."
+        else:
+            past_year_attempt_count_str = f"{TC.GREEN}{past_year_attempt_count}{TC.WHITE} recitations in the past year!"
+
+        attempts_by_day = self.api.stats.get_num_attempts_past_year_by_day()
+
+        max_attempts = max(attempts_by_day)
+        few_threshold = 0
+        some_threshold = max_attempts / 3
+        many_threshold = 2 * max_attempts / 3
+
+        blank, few, some, many = ".", "\u2591", "\u2592", "\u2593"
+        for i, day in enumerate(attempts_by_day):
+            if day > many_threshold:
+                attempts_by_day[i] = many
+            elif day > some_threshold:
+                attempts_by_day[i] = some
+            elif day > few_threshold:
+                attempts_by_day[i] = few
+            else:
+                attempts_by_day[i] = blank
+
+        mon, tue, wed, thr, fri, sat, sun = "MON ", "TUE ", "WED ", "THR ", "FRI ", "SAT ", "SUN "
+        mon += "".join(attempts_by_day[::7])
+        tue += "".join(attempts_by_day[1::7])
+        wed += "".join(attempts_by_day[2::7])
+        thr += "".join(attempts_by_day[3::7])
+        fri += "".join(attempts_by_day[4::7])
+        sat += "".join(attempts_by_day[5::7])
+        sun += "".join(attempts_by_day[6::7])
+
+        return (
+            f"{streak_str}\n"
+            f"{past_year_attempt_count_str}\n\n"
+            f"{mon}\n{tue}\n{wed}\n{thr}\n{fri}\n{sat}\n{sun}\n\n"
+            f"{many} = >{int(many_threshold)} Attempt" + \
+                    ("s" if int(many_threshold) != 1 else "") + "   "
+            f"{some} = >{int(some_threshold)} Attempt" + \
+                    ("s" if int(some_threshold) != 1 else "") + "   "
+            f"{few} = >0 Attempts   "
+            ". = 0 Attempts\n"
+        )
+
     def REFERENCE(self):
         return f"Reference:{TC.YELLOW} {self.api.passage.reference.ref_str}{TC.WHITE}"
 
     def TRANSLATION(self):
         return f"Translation:{TC.YELLOW} {self.api.translation}{TC.WHITE}"
 
     def RANDOM_SINGLE_VERSE(self):
@@ -292,27 +270,27 @@
         return f"Available Translations:\n{TC.YELLOW}" + "\n".join(self.api.view_translation()) + f"{TC.WHITE}"
 
     def PASSAGE(self):
         return f"{TC.CYAN}{self.api.view_passage()}{TC.WHITE}"
 
     def TEXT_SCORE(self, score, diff):
         if score == 1.0:
-            return f"{TC.GREEN}Perfect!{TC.WHITE}"
-        elif score > 0.75:
-            return f"{TC.PINK}Not bad: {TC.GREEN}{round(score * 100, 0)}%{TC.WHITE}\n{TC.CYAN}{diff}{TC.WHITE}"
+            return f"({TC.GREEN}100%{TC.WHITE})"
+        elif score > GOOD_SCORE:
+            return f"({TC.GREEN}{round(score * 100, 0)}%{TC.WHITE})\n{TC.CYAN}{diff}{TC.WHITE}"
         else:
-            return f"{TC.RED}Not quite...{TC.WHITE}\n{TC.CYAN}{diff}{TC.WHITE}"
+            return f"({TC.RED}{round(score * 100, 0)}%{TC.WHITE})\n{TC.CYAN}{diff}{TC.WHITE}"
 
     def FAST_SCORE(self, score):
         if score == 1.0:
-            return f"{TC.GREEN}Perfect!{TC.WHITE}"
+            return f"({TC.GREEN}100%{TC.WHITE})"
         elif score > 0.75:
-            return f"{TC.PINK}Not bad: {round(score * 100, 0)}%{TC.WHITE}"
+            return f"({TC.GREEN}{round(score * 100, 0)}%{TC.WHITE})"
         else:
-            return f"{TC.RED}Not quite...{TC.WHITE}"
+            return f"({TC.RED}{round(score * 100, 0)}%{TC.WHITE})"
 
 
 class CLI:
     def __init__(self):
         self.api = API()
         self.messages = CLISTR(self.api)
 
@@ -429,37 +407,38 @@
 
             if i == len(passage_words):
                 score = self.api.finish_recitation(ref, recitation)
                 print(self.messages.FAST_SCORE(score))
                 break
 
     def text_recitation(self, ref):
-        if self.editor == None:
+        if self.editor is None:
             print(self.messages.NO_EDITOR())
         else:
             if self.is_windows:
-                windows_filename = f"{reference.ref_str}".replace(":", ";")
+                windows_filename = f"{ref.ref_str}".replace(":", ";")
                 filename = self.api.cache_path / windows_filename
             else:
-                filename = self.api.cache_path / f"{reference.ref_str}"
+                filename = self.api.cache_path / f"{ref.ref_str}"
 
             filename.touch(exist_ok=True)
             subprocess.run([self.editor, filename])
 
             if not filename.exists():
                 text = ""
             else:
                 with open(filename, "r") as file:
                     text = file.readlines()
                     text = "".join(text).strip()
 
                 if filename.exists():
                     os.remove(filename)
 
-            score = self.api.finish_recitation(reference, text)
+            score = self.api.finish_recitation(ref, text)
+            ans = self.api.get_recitation_ans(ref)
 
             diff = ""
             result = SequenceMatcher(a=text, b=ans).get_opcodes()
             for tag, i1, i2, j1, j2 in result:
                 if tag == "replace":
                     segment = f"{TC.RED}{text[i1:i2]}{TC.GREEN}{ans[j1:j2]}{TC.WHITE}"
                     segment = segment.replace(" ", "_")
@@ -549,88 +528,20 @@
                     if self.api.fast_recitations:
                         self.fast_recitation(reference)
                     else:
                         self.text_recitation(reference)
 
             # Show Stats
             elif user_input == "s" or user_input == "stats":
-                self.stats_mainloop()
-
-            # Print Help
-            else:
-                print(self.messages.HELP())
-
-    def stats_mainloop(self):
-        print(self.messages.WELCOME_STATS())
-
-        while True:
-            user_input = input(self.messages.STATS_CLI_PROMPT()).strip().lower()
-
-            # Current State
-            if user_input == "l" or user_input == "list":
-                print(self.messages.START_DATE())
-                print(self.messages.END_DATE())
-
-            # Clear Filters
-            elif user_input == "c" or user_input == "clear":
-                print(self.messages.CLEAR_STATS_FILTERS())
-                self.api.stats.clear_filters()
-
-            # Set Start Date
-            elif user_input == "sd" or user_input == "start":
-                print(self.messages.SET_START_DATE())
-                year = input(self.messages.YEAR_PROMPT())
-                month = input(self.messages.MONTH_PROMPT())
-                day = input(self.messages.DAY_PROMPT())
-
-                if not (year.isdecimal() and month.isdecimal() and day.isdecimal()):
-                    self.api.stats.set_start_date(None)
-                else:
-                    try:
-                        self.api.stats.set_start_date(datetime.date(int(year), int(month), int(day)))
-                    except ValueError as e:
-                        print(e.__str__().capitalize())
-
-                    except InvalidDateFilter as e:
-                        print(e.__str__())
-
-            # Set End Date
-            elif user_input == "ed" or user_input == "end":
-                print(self.messages.SET_END_DATE())
-                year = input(self.messages.YEAR_PROMPT())
-                month = input(self.messages.MONTH_PROMPT())
-                day = input(self.messages.DAY_PROMPT())
-
-                if not (year.isdecimal() and month.isdecimal() and day.isdecimal()):
-                    self.api.stats.set_end_date(None)
-                else:
-                    try:
-                        self.api.stats.set_end_date(datetime.date(int(year), int(month), int(day)))
-
-                    except ValueError as e:
-                        print(e.__str__().capitalize())
-
-                    except InvalidDateFilter as e:
-                        print(e.__str__())
-
-            # See All Attempted Verses
-            elif user_input == "a" or user_input == "all":
-                print(self.messages.ALL_ATTEMPTED_VERSES())
-
-            # See All Verses Ranked By Score
-            elif user_input == "r" or user_input == "rank":
+                print(self.messages.STATS_GAMIFICATION())
                 print(self.messages.ALL_VERSES_RANKED())
 
             # Reset Statistics
             elif user_input == "d" or user_input == "delete":
                 confirmation = input(self.messages.STATS_RESET_WARNING()).strip().lower()
                 if confirmation == "y" or confirmation == "yes":
                     self.api.stats.reset_db()
                     print(self.messages.STATS_RESET())
 
-            # Exit Stats
-            elif user_input == "q" or user_input == "quit":
-                break
-
-            # Print Stats Help
+            # Print Help
             else:
-                print(self.messages.STATS_HELP())
+                print(self.messages.HELP())
```

### Comparing `scripture_phaser-1.1.1/src/enums.py` & `scripture_phaser-1.2.0/src/enums.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,16 +32,16 @@
 # POSSIBILITY OF SUCH DAMAGE.
 
 import os
 import enum
 import platform
 from pathlib import Path
 
-VERSION = "1.1.1"
-RELEASE_DATE = "2024-03-27"
+VERSION = "1.2.0"
+RELEASE_DATE = "2024-04-01"
 
 if platform.system() == "Windows":
     CONFIG_DIR = Path(os.environ["HOMEPATH"]) / ".config"
     CACHE_DIR = Path(os.environ["HOMEPATH"]) / ".cache"
     DATA_DIR = Path(os.environ["HOMEPATH"]) / ".local/share"
 else:
     try:
```

### Comparing `scripture_phaser-1.1.1/src/exceptions.py` & `scripture_phaser-1.2.0/src/exceptions.py`

 * *Files identical despite different names*

### Comparing `scripture_phaser-1.1.1/src/models.py` & `scripture_phaser-1.2.0/src/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,14 @@
 # CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
 # SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
 # INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
 # CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
 # ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
 # POSSIBILITY OF SUCH DAMAGE.
 
-from pathlib import Path
 from peewee import Model
 from peewee import TextField
 from peewee import CharField
 from peewee import FloatField
 from peewee import BooleanField
 from peewee import DateTimeField
 from peewee import SqliteDatabase
```

### Comparing `scripture_phaser-1.1.1/src/passage.py` & `scripture_phaser-1.2.0/src/passage.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,18 +27,16 @@
 # CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
 # SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
 # INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
 # CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
 # ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
 # POSSIBILITY OF SUCH DAMAGE.
 
-from src.enums import Bible
 from src.verse import Verse
 from src.agents import Agents
-from src.enums import Reverse_Bible_Books
 from src.exceptions import InvalidReference
 
 
 class Passage:
     def __init__(self, reference, translation):
         self.agent = Agents[translation]
         self.reference = reference
@@ -49,15 +47,16 @@
         self.populated = True
         if texts is None:
             texts = self.agent.get(self.reference)
         for verse, text in zip(self.verses, texts):
             verse.initialize(text, require_passage_numbers)
 
     def show(self, with_verse=False, with_ref=False):
-        if not self.populated: return ""
+        if not self.populated:
+            return ""
         else:
             if with_verse:
                 texts = [verse.show(with_verse=True) for verse in self.verses]
             else:
                 texts = [verse.show() for verse in self.verses]
 
             text = " ".join(texts)
```

### Comparing `scripture_phaser-1.1.1/src/reference.py` & `scripture_phaser-1.2.0/src/reference.py`

 * *Files identical despite different names*

### Comparing `scripture_phaser-1.1.1/src/scripture_phaser.py` & `scripture_phaser-1.2.0/src/scripture_phaser.py`

 * *Files identical despite different names*

### Comparing `scripture_phaser-1.1.1/src/stats.py` & `scripture_phaser-1.2.0/src/stats.py`

 * *Files 21% similar despite different names*

```diff
@@ -28,66 +28,74 @@
 # SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
 # INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
 # CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
 # ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
 # POSSIBILITY OF SUCH DAMAGE.
 
 import datetime
+from peewee import fn
 from src.models import Attempt
-from src.exceptions import InvalidDateFilter
 
 
 class Stats:
     def __init__(self):
-        self.start_date = None
-        self.end_date = None
+        if not Attempt.table_exists():
+            Attempt.create_table()
 
     @staticmethod
     def reset_db():
         if Attempt.table_exists():
             Attempt.drop_table()
         Attempt.create_table()
 
-    def clear_filters(self):
-        self.start_date = None
-        self.end_date = None
-
-    def validate_filters(self):
-        if self.start_date is not None and self.end_date is not None:
-            if self.start_date > self.end_date:
-                self.clear_filters()
-                raise InvalidDateFilter()
-
-    def set_start_date(self, date=None):
-        self.start_date = date
-        self.validate_filters()
-
-    def set_end_date(self, date=None):
-        self.end_date = date
-        self.validate_filters()
-
-    def apply_filters(self, query):
-        if self.start_date is not None:
-            query = query.where(Attempt.datetime >= self.start_date)
-        if self.end_date is not None:
-            query = query.where(Attempt.datetime <= self.end_date)
-        return query
-
-    def all_attempted_verses(self):
-        attempts = self.apply_filters(Attempt.select(Attempt.reference))
-        return {attempt.reference for attempt in attempts}
-
-    def all_verses_ranked(self):
-        verses = {}
-        for ref in self.all_attempted_verses():
-            attempts = self.apply_filters(
-                Attempt.select(Attempt.score).where(Attempt.reference == ref)
-            )
-            scores = [attempt.score for attempt in attempts]
-            verses[ref] = sum(scores) / len(scores)
-        return verses
+    @staticmethod
+    def get_streak():
+        datetimes = Attempt.select(Attempt.datetime).order_by(Attempt.datetime.desc())
+        dates = {dt.datetime.date() for dt in datetimes}
+
+        streak = 0
+        date = datetime.date.today()
+        while True:
+            if date in dates:
+                streak += 1
+                date -= datetime.timedelta(days=1)
+            else:
+                break
+
+        return streak
 
-    def verse_by_reference(self, ref):
-        attempts = self.apply_filters(
-            Attempt.select(Attempt.datetime, Attempt.score).where(Attempt.reference == ref).order_by(Attempt.id)
-        )
-        return [(a.datetime, a.score) for a in attempts]
+    @staticmethod
+    def get_num_attempts_past_year():
+        one_year_ago = datetime.date.today() - datetime.timedelta(days=365)
+        return Attempt.select().where(Attempt.datetime > one_year_ago).count()
+
+    @staticmethod
+    def get_num_attempts_past_year_by_day():
+        today = datetime.date.today()
+        days_since_monday = today.weekday()
+        start_date = today - datetime.timedelta(days=days_since_monday, weeks=52)
+        results = [0] * ((today - start_date).days + 1)
+        day_counts = Attempt \
+            .select(
+                Attempt.datetime,
+                fn.COUNT(Attempt.id).alias("num")
+            ) \
+            .where(Attempt.datetime > start_date) \
+            .group_by(fn.date_trunc("day", Attempt.datetime)) \
+            .order_by(Attempt.datetime)
+
+        for day in day_counts:
+            results[(day.datetime.date() - start_date).days] = day.num
+
+        return results
+
+    @staticmethod
+    def all_verses_ranked():
+        verse_scores, verse_counts = {}, {}
+        all_attempts = Attempt.select(Attempt.reference)
+        for reference in all_attempts:
+            ref = reference.reference
+            attempts = Attempt.select(Attempt.score).where(Attempt.reference == ref)
+            scores = [attempt.score for attempt in attempts]
+            verse_scores[ref] = sum(scores) / len(scores)
+            verse_counts[ref] = len(scores)
+        return verse_scores, verse_counts
```

### Comparing `scripture_phaser-1.1.1/src/verse.py` & `scripture_phaser-1.2.0/src/verse.py`

 * *Files identical despite different names*

### Comparing `scripture_phaser-1.1.1/test/__init__.py` & `scripture_phaser-1.2.0/test/__init__.py`

 * *Files identical despite different names*

### Comparing `scripture_phaser-1.1.1/test/test_api.py` & `scripture_phaser-1.2.0/test/test_api.py`

 * *Files identical despite different names*

### Comparing `scripture_phaser-1.1.1/test/test_base.py` & `scripture_phaser-1.2.0/test/test_base.py`

 * *Files 14% similar despite different names*

```diff
@@ -29,15 +29,14 @@
 # INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
 # CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
 # ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
 # POSSIBILITY OF SUCH DAMAGE.
 
 import os
 import unittest
-from pathlib import Path
 from src.enums import App
 from src.enums import CONFIG_DIR
 
 
 class BaseTest(unittest.TestCase):
     @classmethod
     def setUpClass(cls):
```

### Comparing `scripture_phaser-1.1.1/test/test_passage.py` & `scripture_phaser-1.2.0/test/test_passage.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,19 +27,17 @@
 # SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
 # INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
 # CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
 # ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
 # POSSIBILITY OF SUCH DAMAGE.
 
 from unittest.mock import MagicMock
-from src.enums import App
 from src.verse import Verse
 from src.passage import Passage
 from src.reference import Reference
-from src.exceptions import InvalidReference
 from test.test_base import BaseTest
 
 
 class PassageTests(BaseTest):
     """
     Test the Passage Object
     """
```

### Comparing `scripture_phaser-1.1.1/test/test_reference.py` & `scripture_phaser-1.2.0/test/test_reference.py`

 * *Files identical despite different names*

### Comparing `scripture_phaser-1.1.1/test/test_verse.py` & `scripture_phaser-1.2.0/test/test_verse.py`

 * *Files identical despite different names*

### Comparing `scripture_phaser-1.1.1/.gitignore` & `scripture_phaser-1.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `scripture_phaser-1.1.1/LICENSE` & `scripture_phaser-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `scripture_phaser-1.1.1/README.md` & `scripture_phaser-1.2.0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -27,30 +27,19 @@
 * m/single      - Toggles whether or not to practice random single verses
 * f/fast        - Toggles whether or not to use fast recitation mode when reciting
 * r/reference   - Sets the reference
 * t/translation - Set the translation
 * i/inquire     - List available translations
 * p/practice    - Practice the current reference
 * v/view        - Preview current reference
-* s/stats       - Enter statistics mode
+* s/stats       - Prints recitation statistics
+* d/delete      - Deletes all past statistics
 * h/help        - Prints this help message
 * q/quit        - Quits scripture_phaser
 
-You can enter statistics mode by pressing "s" in standard mode ("\[STATS\] >" prompt). In statistics mode, the following commands are available to you:
-
-* sd/start      - Sets the earliest date to use when fetching past recitation attempts
-* ed/end        - Sets the latest date to use when fetching past recitation attempts
-* l/list        - List current filters used in data selection (start/end date)
-* c/clear       - Clears all current filters used in data selection (start/end date)
-* a/all         - List all references ever attempted
-* r/rank        - Rank all attempted verses by average recall accuracy
-* d/delete      - Reset all statistics
-* h/help        - Prints stats mode help message
-* q/quit        - Return to the standard mode
-
 You can enter fast recitation mode if you have fast recitations set to True and you press "p" to practice the passage (blank prompt). In fast recitation mode, the following commands are available to you:
 
 * a-z A-Z 0-9   - Advances the recitation of the verse by one word
 * ?             - Prints fast mode help message
 * Ctrl + C      - Return to standard mode
 
 ## Uninstallation
```

### Comparing `scripture_phaser-1.1.1/pyproject.toml` & `scripture_phaser-1.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 
 [tool.hatch.build.targets.wheel]
 packages = ["src"]
 
 [project]
 name = "scripture_phaser"
-version = "1.1.1"
+version = "1.2.0"
 dependencies = [
 	"meaningless==1.0.0",
 	"peewee==3.17.0",
         "readchar==4.0.5"
 ]
 requires-python = ">=3.8"
 authors = [
```

### Comparing `scripture_phaser-1.1.1/PKG-INFO` & `scripture_phaser-1.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: scripture_phaser
-Version: 1.1.1
+Version: 1.2.0
 Summary: scripture_phaser helps you to memorize the Bible.
 Project-URL: Homepage, https://nolanmcmahon.net/projects/scripture_phaser.html
 Project-URL: Repository, https://github.com/NolantheNerd/scripture_phaser
 Author-email: Nolan McMahon <nolan@nolanmcmahon.net>
 License: Copyright 2023-2024 Nolan McMahon
         
         Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
@@ -64,30 +64,19 @@
 * m/single      - Toggles whether or not to practice random single verses
 * f/fast        - Toggles whether or not to use fast recitation mode when reciting
 * r/reference   - Sets the reference
 * t/translation - Set the translation
 * i/inquire     - List available translations
 * p/practice    - Practice the current reference
 * v/view        - Preview current reference
-* s/stats       - Enter statistics mode
+* s/stats       - Prints recitation statistics
+* d/delete      - Deletes all past statistics
 * h/help        - Prints this help message
 * q/quit        - Quits scripture_phaser
 
-You can enter statistics mode by pressing "s" in standard mode ("\[STATS\] >" prompt). In statistics mode, the following commands are available to you:
-
-* sd/start      - Sets the earliest date to use when fetching past recitation attempts
-* ed/end        - Sets the latest date to use when fetching past recitation attempts
-* l/list        - List current filters used in data selection (start/end date)
-* c/clear       - Clears all current filters used in data selection (start/end date)
-* a/all         - List all references ever attempted
-* r/rank        - Rank all attempted verses by average recall accuracy
-* d/delete      - Reset all statistics
-* h/help        - Prints stats mode help message
-* q/quit        - Return to the standard mode
-
 You can enter fast recitation mode if you have fast recitations set to True and you press "p" to practice the passage (blank prompt). In fast recitation mode, the following commands are available to you:
 
 * a-z A-Z 0-9   - Advances the recitation of the verse by one word
 * ?             - Prints fast mode help message
 * Ctrl + C      - Return to standard mode
 
 ## Uninstallation
```

