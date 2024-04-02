# Comparing `tmp/hearthstone-7.9.0.tar.gz` & `tmp/hearthstone-8.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hearthstone-7.9.0.tar", last modified: Tue Nov  7 21:42:37 2023, max compression
+gzip compressed data, was "hearthstone-8.0.0.tar", last modified: Tue Apr  2 11:16:16 2024, max compression
```

## Comparing `hearthstone-7.9.0.tar` & `hearthstone-8.0.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-07 21:42:37.339273 hearthstone-7.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2023-11-07 21:42:32.000000 hearthstone-7.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1935 2023-11-07 21:42:37.339273 hearthstone-7.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1229 2023-11-07 21:42:32.000000 hearthstone-7.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-07 21:42:37.339273 hearthstone-7.9.0/hearthstone/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2023-11-07 21:42:32.000000 hearthstone-7.9.0/hearthstone/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3047 2023-11-07 21:42:32.000000 hearthstone-7.9.0/hearthstone/bountyxml.py
--rw-r--r--   0 runner    (1001) docker     (127)    14283 2023-11-07 21:42:32.000000 hearthstone-7.9.0/hearthstone/cardxml.py
--rw-r--r--   0 runner    (1001) docker     (127)     4185 2023-11-07 21:42:32.000000 hearthstone-7.9.0/hearthstone/dbf.py
--rw-r--r--   0 runner    (1001) docker     (127)     5393 2023-11-07 21:42:32.000000 hearthstone-7.9.0/hearthstone/deckstrings.py
--rw-r--r--   0 runner    (1001) docker     (127)    10283 2023-11-07 21:42:32.000000 hearthstone-7.9.0/hearthstone/entities.py
--rw-r--r--   0 runner    (1001) docker     (127)    62292 2023-11-07 21:42:32.000000 hearthstone-7.9.0/hearthstone/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     6985 2023-11-07 21:42:32.000000 hearthstone-7.9.0/hearthstone/mercenaryxml.py
--rw-r--r--   0 runner    (1001) docker     (127)     1803 2023-11-07 21:42:32.000000 hearthstone-7.9.0/hearthstone/stringsfile.py
--rw-r--r--   0 runner    (1001) docker     (127)       97 2023-11-07 21:42:32.000000 hearthstone-7.9.0/hearthstone/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-07 21:42:37.339273 hearthstone-7.9.0/hearthstone/utils/
--rw-r--r--   0 runner    (1001) docker     (127)    15879 2023-11-07 21:42:32.000000 hearthstone-7.9.0/hearthstone/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      671 2023-11-07 21:42:32.000000 hearthstone-7.9.0/hearthstone/xmlutils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-07 21:42:37.339273 hearthstone-7.9.0/hearthstone.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1935 2023-11-07 21:42:37.000000 hearthstone-7.9.0/hearthstone.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      533 2023-11-07 21:42:37.000000 hearthstone-7.9.0/hearthstone.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-07 21:42:37.000000 hearthstone-7.9.0/hearthstone.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2023-11-07 21:42:37.000000 hearthstone-7.9.0/hearthstone.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2023-11-07 21:42:37.000000 hearthstone-7.9.0/hearthstone.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-07 21:42:37.000000 hearthstone-7.9.0/hearthstone.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      840 2023-11-07 21:42:37.339273 hearthstone-7.9.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)       62 2023-11-07 21:42:32.000000 hearthstone-7.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 11:16:16.751590 hearthstone-8.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-04-02 11:16:11.000000 hearthstone-8.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-04-02 11:16:16.751590 hearthstone-8.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-04-02 11:16:11.000000 hearthstone-8.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 11:16:16.751590 hearthstone-8.0.0/hearthstone/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-02 11:16:11.000000 hearthstone-8.0.0/hearthstone/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-04-02 11:16:11.000000 hearthstone-8.0.0/hearthstone/bountyxml.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14369 2024-04-02 11:16:11.000000 hearthstone-8.0.0/hearthstone/cardxml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4185 2024-04-02 11:16:11.000000 hearthstone-8.0.0/hearthstone/dbf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5811 2024-04-02 11:16:11.000000 hearthstone-8.0.0/hearthstone/deckstrings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10283 2024-04-02 11:16:11.000000 hearthstone-8.0.0/hearthstone/entities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65012 2024-04-02 11:16:11.000000 hearthstone-8.0.0/hearthstone/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6985 2024-04-02 11:16:11.000000 hearthstone-8.0.0/hearthstone/mercenaryxml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-04-02 11:16:11.000000 hearthstone-8.0.0/hearthstone/stringsfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-02 11:16:11.000000 hearthstone-8.0.0/hearthstone/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 11:16:16.751590 hearthstone-8.0.0/hearthstone/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)    16605 2024-04-02 11:16:11.000000 hearthstone-8.0.0/hearthstone/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-02 11:16:11.000000 hearthstone-8.0.0/hearthstone/xmlutils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 11:16:16.751590 hearthstone-8.0.0/hearthstone.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-04-02 11:16:16.000000 hearthstone-8.0.0/hearthstone.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-02 11:16:16.000000 hearthstone-8.0.0/hearthstone.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 11:16:16.000000 hearthstone-8.0.0/hearthstone.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-02 11:16:16.000000 hearthstone-8.0.0/hearthstone.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-02 11:16:16.000000 hearthstone-8.0.0/hearthstone.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 11:16:16.000000 hearthstone-8.0.0/hearthstone.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-04-02 11:16:16.751590 hearthstone-8.0.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)       62 2024-04-02 11:16:11.000000 hearthstone-8.0.0/setup.py
```

### Comparing `hearthstone-7.9.0/LICENSE` & `hearthstone-8.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hearthstone-7.9.0/PKG-INFO` & `hearthstone-8.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hearthstone
-Version: 7.9.0
+Version: 8.0.0
 Summary: CardDefs.xml parser and Hearthstone enums for Python
 Home-page: https://github.com/HearthSim/python-hearthstone/
 Download-URL: https://github.com/HearthSim/python-hearthstone/tarball/master
 Author: Jerome Leclanche
 Author-email: jerome@leclan.ch
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `hearthstone-7.9.0/README.md` & `hearthstone-8.0.0/README.md`

 * *Files identical despite different names*

### Comparing `hearthstone-7.9.0/hearthstone/bountyxml.py` & `hearthstone-8.0.0/hearthstone/bountyxml.py`

 * *Files identical despite different names*

### Comparing `hearthstone-7.9.0/hearthstone/cardxml.py` & `hearthstone-8.0.0/hearthstone/cardxml.py`

 * *Files 0% similar despite different names*

```diff
@@ -369,26 +369,28 @@
 	deathrattle = prop(GameTag.DEATHRATTLE, bool)
 	discover = prop(GameTag.DISCOVER, bool)
 	divine_shield = prop(GameTag.DIVINE_SHIELD, bool)
 	double_spelldamage_bonus = prop(GameTag.RECEIVES_DOUBLE_SPELLDAMAGE_BONUS, bool)
 	dredge = prop(GameTag.DREDGE, bool)
 	echo = prop(GameTag.ECHO, bool)
 	elite = prop(GameTag.ELITE, bool)
+	elusive = prop(GameTag.ELUSIVE, bool)
 	evil_glow = prop(GameTag.EVIL_GLOW, bool)
 	forge = prop(GameTag.FORGE, bool)
 	forgetful = prop(GameTag.FORGETFUL, bool)
 	ghostly = prop(GameTag.GHOSTLY, bool)
 	hide_health = prop(GameTag.HIDE_HEALTH, bool)
 	hide_stats = prop(GameTag.HIDE_STATS, bool)
 	hide_cost = prop(GameTag.HIDE_COST, bool)
 	immune = prop(GameTag.IMMUNE, bool)
 	inspire = prop(GameTag.INSPIRE, bool)
 	jade_golem = prop(GameTag.JADE_GOLEM, bool)
 	lifesteal = prop(GameTag.LIFESTEAL, bool)
 	magnetic = prop(GameTag.MODULAR, bool)
+	miniaturize = prop(GameTag.MINIATURIZE, bool)
 	one_turn_effect = prop(GameTag.TAG_ONE_TURN_EFFECT, bool)
 	outcast = prop(GameTag.OUTCAST, bool)
 	overheal = prop(GameTag.OVERHEAL, bool)
 	overkill = prop(GameTag.OVERKILL, bool)
 	poisonous = prop(GameTag.POISONOUS, bool)
 	quest = prop(GameTag.QUEST, bool)
 	reborn = prop(GameTag.REBORN, bool)
```

### Comparing `hearthstone-7.9.0/hearthstone/dbf.py` & `hearthstone-8.0.0/hearthstone/dbf.py`

 * *Files identical despite different names*

### Comparing `hearthstone-7.9.0/hearthstone/deckstrings.py` & `hearthstone-8.0.0/hearthstone/deckstrings.py`

 * *Files 12% similar despite different names*

```diff
@@ -51,33 +51,33 @@
 	@classmethod
 	def from_deckstring(cls, deckstring: str) -> "Deck":
 		instance = cls()
 		(
 			instance.cards,
 			instance.heroes,
 			instance.format,
-			instance.sideboard,
+			instance.sideboards,
 		) = parse_deckstring(deckstring)
 		return instance
 
 	def __init__(self):
 		self.cards: CardIncludeList = []
-		self.sideboard: SideboardList = []
+		self.sideboards: SideboardList = []
 		self.heroes: CardList = []
 		self.format: FormatType = FormatType.FT_UNKNOWN
 
 	@property
 	def as_deckstring(self) -> str:
-		return write_deckstring(self.cards, self.heroes, self.format, self.sideboard)
+		return write_deckstring(self.cards, self.heroes, self.format, self.sideboards)
 
 	def get_dbf_id_list(self) -> CardIncludeList:
 		return sorted(self.cards, key=lambda x: x[0])
 
 	def get_sideboard_dbf_id_list(self) -> SideboardList:
-		return sorted(self.sideboard, key=lambda x: x[0])
+		return sorted(self.sideboards, key=lambda x: x[0])
 
 
 def trisort_cards(cards: Sequence[tuple]) -> Tuple[
 	List[tuple], List[tuple], List[tuple]
 ]:
 	cards_x1: List[tuple] = []
 	cards_x2: List[tuple] = []
@@ -108,33 +108,41 @@
 
 def parse_deckstring(deckstring) -> (
 	Tuple[CardIncludeList, CardList, FormatType, SideboardList]
 ):
 	decoded = base64.b64decode(deckstring)
 	data = BytesIO(decoded)
 
+	# Header section
+
 	if data.read(1) != b"\0":
 		raise ValueError("Invalid deckstring")
 
 	version = _read_varint(data)
 	if version != DECKSTRING_VERSION:
 		raise ValueError("Unsupported deckstring version %r" % (version))
 
 	format = _read_varint(data)
 	try:
 		format = FormatType(format)
 	except ValueError:
 		raise ValueError("Unsupported FormatType in deckstring %r" % (format))
 
+	# Heroes section
+
 	heroes: CardList = []
 	num_heroes = _read_varint(data)
 	for i in range(num_heroes):
 		heroes.append(_read_varint(data))
+	heroes.sort()
+
+	# Cards section
 
 	cards: CardIncludeList = []
+
 	num_cards_x1 = _read_varint(data)
 	for i in range(num_cards_x1):
 		card_id = _read_varint(data)
 		cards.append((card_id, 1))
 
 	num_cards_x2 = _read_varint(data)
 	for i in range(num_cards_x2):
@@ -143,86 +151,99 @@
 
 	num_cards_xn = _read_varint(data)
 	for i in range(num_cards_xn):
 		card_id = _read_varint(data)
 		count = _read_varint(data)
 		cards.append((card_id, count))
 
-	sideboard = []
+	cards.sort()
+
+	# Sideboards section
 
-	has_sideboard = data.read(1) == b"\1"
+	sideboards = []
 
-	if has_sideboard:
-		num_sideboard_x1 = _read_varint(data)
-		for i in range(num_sideboard_x1):
+	has_sideboards = data.read(1) == b"\1"
+
+	if has_sideboards:
+		num_sideboards_x1 = _read_varint(data)
+		for i in range(num_sideboards_x1):
 			card_id = _read_varint(data)
 			sideboard_owner = _read_varint(data)
-			sideboard.append((card_id, 1, sideboard_owner))
+			sideboards.append((card_id, 1, sideboard_owner))
 
-		num_sideboard_x2 = _read_varint(data)
-		for i in range(num_sideboard_x2):
+		num_sideboards_x2 = _read_varint(data)
+		for i in range(num_sideboards_x2):
 			card_id = _read_varint(data)
 			sideboard_owner = _read_varint(data)
-			sideboard.append((card_id, 2, sideboard_owner))
+			sideboards.append((card_id, 2, sideboard_owner))
 
-		num_sideboard_xn = _read_varint(data)
-		for i in range(num_sideboard_xn):
+		num_sideboards_xn = _read_varint(data)
+		for i in range(num_sideboards_xn):
 			card_id = _read_varint(data)
 			count = _read_varint(data)
 			sideboard_owner = _read_varint(data)
-			sideboard.append((card_id, count, sideboard_owner))
+			sideboards.append((card_id, count, sideboard_owner))
+
+	sideboards.sort(key=lambda x: (x[2], x[0]))
 
-	return cards, heroes, format, sideboard
+	return cards, heroes, format, sideboards
 
 
 def write_deckstring(
 	cards: CardIncludeList,
 	heroes: CardList,
 	format: FormatType,
-	sideboard: Optional[SideboardList] = None,
+	sideboards: Optional[SideboardList] = None,
 ) -> str:
-	if sideboard is None:
-		sideboard = []
+	if sideboards is None:
+		sideboards = []
 
 	data = BytesIO()
 	data.write(b"\0")
 	_write_varint(data, DECKSTRING_VERSION)
 	_write_varint(data, int(format))
 
 	if len(heroes) != 1:
 		raise ValueError("Unsupported hero count %i" % (len(heroes)))
 	_write_varint(data, len(heroes))
-	for hero in heroes:
+	for hero in sorted(heroes):
 		_write_varint(data, hero)
 
 	cards_x1, cards_x2, cards_xn = trisort_cards(cards)
 
-	for cardlist in cards_x1, cards_x2:
+	sort_key = lambda x: x[0]
+
+	for cardlist in sorted(cards_x1, key=sort_key), sorted(cards_x2, key=sort_key):
 		_write_varint(data, len(cardlist))
 		for cardid, _ in cardlist:
 			_write_varint(data, cardid)
 
 	_write_varint(data, len(cards_xn))
-	for cardid, count in cards_xn:
+	for cardid, count in sorted(cards_xn, key=sort_key):
 		_write_varint(data, cardid)
 		_write_varint(data, count)
 
-	if len(sideboard) > 0:
+	if len(sideboards) > 0:
 		data.write(b"\1")
 
-		sideboard_x1, sideboard_x2, sideboard_xn = trisort_cards(sideboard)
+		sideboards_x1, sideboards_x2, sideboards_xn = trisort_cards(sideboards)
+
+		sb_sort_key = lambda x: (x[2], x[0])
 
-		for cardlist in sideboard_x1, sideboard_x2:
+		for cardlist in (
+			sorted(sideboards_x1, key=sb_sort_key),
+			sorted(sideboards_x2, key=sb_sort_key)
+		):
 			_write_varint(data, len(cardlist))
 			for cardid, _, sideboard_owner in cardlist:
 				_write_varint(data, cardid)
 				_write_varint(data, sideboard_owner)
 
-		_write_varint(data, len(cards_xn))
-		for cardid, count, sideboard_owner in sideboard_xn:
+		_write_varint(data, len(sideboards_xn))
+		for cardid, count, sideboard_owner in sorted(sideboards_xn, key=sb_sort_key):
 			_write_varint(data, cardid)
 			_write_varint(data, count)
 			_write_varint(data, sideboard_owner)
 
 	else:
 		data.write(b"\0")
```

### Comparing `hearthstone-7.9.0/hearthstone/entities.py` & `hearthstone-8.0.0/hearthstone/entities.py`

 * *Files identical despite different names*

### Comparing `hearthstone-7.9.0/hearthstone/enums.py` & `hearthstone-8.0.0/hearthstone/enums.py`

 * *Files 4% similar despite different names*

```diff
@@ -165,14 +165,15 @@
 	DEATHRATTLE_RETURN_ZONE = 382
 	STEADY_SHOT_CAN_TARGET = 383
 	DISPLAYED_CREATOR = 385
 	POWERED_UP = 386
 	SPARE_PART = 388
 	FORGETFUL = 389
 	CAN_SUMMON_MAXPLUSONE_MINION = 390
+	OBFUSCATED = 391
 	BURNING = 392
 	OVERLOAD_LOCKED = 393
 	NUM_TIMES_HERO_POWER_USED_THIS_GAME = 394
 	CURRENT_HEROPOWER_DAMAGE_BONUS = 395
 	HEROPOWER_DAMAGE = 396
 	NUM_FRIENDLY_MINIONS_THAT_DIED_THIS_TURN = 398
 	NUM_CARDS_DRAWN_THIS_TURN = 399
@@ -217,15 +218,15 @@
 	SCORE_LABELID_1 = 450
 	SCORE_VALUE_1 = 451
 	SCORE_LABELID_2 = 452
 	SCORE_LABELID_3 = 454
 	SCORE_VALUE_2 = 453
 	SCORE_VALUE_3 = 455
 	CANT_BE_FATIGUED = 456
-	AUTOATTACK = 457
+	AUTO_ATTACK = 457
 	ARMS_DEALING = 458
 	QUEST = 462
 	TAG_LAST_KNOWN_COST_IN_HAND = 466
 	DEFINING_ENCHANTMENT = 469
 	FINISH_ATTACK_SPELL_ON_DAMAGE = 470
 	MODULAR_ENTITY_PART_1 = 471
 	MODULAR_ENTITY_PART_2 = 472
@@ -314,15 +315,15 @@
 	ECHOING_OOZE_SPELL = 963
 	COLLECTIONMANAGER_FILTER_MANA_EVEN = 956
 	COLLECTIONMANAGER_FILTER_MANA_ODD = 957
 	AMOUNT_HEALED_THIS_GAME = 958
 	ZOMBEAST_DEBUG_CURRENT_BEAST_DATABASE_ID = 964
 	ZOMBEAST_DEBUG_CURRENT_ITERATION = 965
 	ZOMBEAST_DEBUG_MAX_ITERATIONS = 966
-	START_OF_GAME = 968
+	START_OF_GAME_KEYWORD = 968
 	ENCHANTMENT_INVISIBLE = 976
 	PUZZLE = 979
 	PUZZLE_PROGRESS = 980
 	PUZZLE_PROGRESS_TOTAL = 981
 	PUZZLE_TYPE = 982
 	PUZZLE_COMPLETED = 984
 	CONCEDE_BUTTON_ALTERNATIVE_TEXT = 985
@@ -349,15 +350,15 @@
 	LUNAHIGHLIGHTHINT = 1054
 	SUPPRESS_JOBS_DONE_VO = 1055
 	SHRINE = 1057
 	ALL_HEALING_DOUBLE = 1058
 	BLOCK_ALL_INPUT = 1071
 	PUZZLE_MODE = 1073
 	CARD_DOES_NOTHING = 1075
-	CASTSWHENDRAWN = 1077
+	CASTS_WHEN_DRAWN = 1077
 	DISPLAY_CARD_ON_MOUSEOVER = 1078
 	DECK_POWER_UP = 1080
 	SIDEKICK = 1081
 	SIDEKICK_HERO_POWER = 1082
 	REBORN = 1085
 	SQUELCH_NON_GAME_TRIGGERS_AND_MODIFIERS = 1087
 	QUEST_REWARD_DATABASE_ID = 1089
@@ -380,32 +381,33 @@
 	EXTRA_DEATHRATTLES_ADDITIONAL = 1131
 	ALTERNATE_MOUSE_OVER_CARD = 1132
 	ENCHANTMENT_BANNER_TEXT = 1135
 	MOUSE_OVER_CARD_APPEARANCE = 1142
 	IS_ADVENTURE_SCENARIO = 1172
 	TWINSPELL_COPY = 1186
 	PROXY_GALAKROND = 1190
-	SIDEQUEST = 1192
+	SIDE_QUEST = 1192
 	TWINSPELL = 1193
 	GALAKROND_IN_PLAY = 1194
 	COIN_MANA_GEM = 1199
 	MEGA_WINDFURY = 1207
+	ELUSIVE = 1211
 	EMPOWER = 1263
 	EMPOWER_PRIEST = 1264
 	EMPOWER_ROGUE = 1265
 	EMPOWER_SHAMAN = 1266
 	EMPOWER_WARLOCK = 1267
 	EMPOWER_WARRIOR = 1268
 	TWINSPELLPENDING = 1269
 	DRUSTVAR_HORROR_DEBUG_CURRENT_SPELL_DATABASE_ID = 1280
 	DRUSTVAR_HORROR_DEBUG_CURRENT_ITERATION = 1281
 	HEROIC_HERO_POWER = 1282
 	DRUSTVAR_HORROR_DEBUG_MAX_ITERATIONS = 1283
 	CREATOR_DBID = 1284
-	FATIGUEREFERENCE = 1290
+	FATIGUE_REFERENCE = 1290
 	HERO_FLYING = 1293
 	UI_BUFF_HEALTH_UP = 1294
 	UI_BUFF_SET_COST_ZERO = 1295
 	UI_BUFF_COST_DOWN = 1296
 	UI_BUFF_ATK_UP = 1297
 	UI_BUFF_COST_UP = 1298
 	DEBUG_DISPLAY_TAG_BOTTOM_RIGHT = 1313
@@ -471,15 +473,15 @@
 	DORMANT_AWAKEN_CONDITION_ENCHANT = 1519
 	SUPPRESS_SUMMON_VO_FOR_PLAYER = 1521
 	CORRUPT = 1524
 	ALLOW_GAME_SPEEDUP = 1526
 	POISONOUS_INSTANT = 1528
 	FORCE_NO_CUSTOM_SPELLS = 1529
 	START_OF_COMBAT = 1531
-	CORRUPTEDCARD = 1551
+	CORRUPTED_CARD = 1551
 	BACON_HERO_EARLY_ACCESS = 1554
 	SPAWN_TIME_COUNT = 1556
 	SKIP_MULLIGAN = 1561
 	COPIED_FROM_ENTITY_ID = 1565
 	BACON_SELL_VALUE = 1587
 	BACON_VERDANTSPHERES = 1598
 	OPPONENT_SIDE_GHOSTLY = 1609
@@ -557,15 +559,15 @@
 	BACON_BLOODGEMBUFFATKVALUE = 1844
 	CANT_MOVE_MINION = 1848
 	LETTUCE_MERCENARY_EXPERIENCE = 1852
 	LETTUCE_IS_EQUPIMENT = 1855
 	LETTUCE_EQUIPMENT_ID = 1856
 	DARKMOON_FAIRE_PRIZES_ACTIVE = 1895
 	IGNORE_DECK_RULESET = 1896
-	HONORABLEKILL = 1920
+	HONORABLE_KILL = 1920
 	HAS_DIAMOND_QUALITY = 1932
 	CURRENT_SPELLPOWER_ARCANE = 1936
 	CURRENT_SPELLPOWER_FIRE = 1937
 	CURRENT_SPELLPOWER_FROST = 1938
 	CURRENT_SPELLPOWER_NATURE = 1939
 	CURRENT_SPELLPOWER_HOLY = 1940
 	CURRENT_SPELLPOWER_SHADOW = 1941
@@ -576,17 +578,17 @@
 	SPELLPOWER_FIRE = 1946
 	SPELLPOWER_FROST = 1947
 	SPELLPOWER_NATURE = 1948
 	SPELLPOWER_HOLY = 1949
 	SPELLPOWER_SHADOW = 1950
 	SPELLPOWER_FEL = 1951
 	SPELLPOWER_PHYSICAL = 1952
-	ENRAGED_TOOLTIP = 1954
+	ENRAGE_TOOLTIP = 1954
 	IMP = 1965
-	BLOOD_GEM = 1966
+	BACON_BLOOD_GEM_TOOLTIP = 1966
 	LETTUCE_HAS_MANUALLY_SELECTED_ABILITY = 1967
 	LETTUCE_KEEP_LAST_STANDING_MINION_ACTOR = 1976
 	GOLDSPARKLES_HINT = 1984
 	LETTUCE_USE_DETERMINISTIC_TEAM_ABILITY_QUEUING = 1990
 	LETTUCE_SELECTED_ABILITY_QUEUE_ORDER = 1991
 	QUESTLINE_FINAL_REWARD_DATABASE_ID = 1992
 	QUESTLINE_PART = 1993
@@ -597,39 +599,40 @@
 	MAX_SLOTS_PER_PLAYER_OVERRIDE = 2017
 	FAKE_CONTROLLER = 2032
 	BACON_SKIN = 2038
 	BACON_SKIN_PARENT_ID = 2039
 	GAME_SEED = 2042
 	IS_USING_TRADE_OPTION = 2045
 	BACON_BOB_SKIN = 2049
+	COIN_CARD = 2088
 	BACON_COMBAT_DAMAGE_CAP = 2089
-	REFRESH = 2104
+	BACON_REFRESH_TOOLTIP = 2104
 	TARGETING_ARROW_TYPE = 2108
 	LETTUCE_CURRENT_BOUNTY_ID = 2120
 	LETTUCE_OVERTIME = 2123
 	AVENGE = 2129
 	BACON_COMPANION_ID = 2130
-	SPELLRESISTANCE_ARCANE = 2138
-	SPELLRESISTANCE_FIRE = 2139
-	SPELLRESISTANCE_FROST = 2140
-	SPELLRESISTANCE_NATURE = 2141
-	SPELLRESISTANCE_HOLY = 2142
-	SPELLRESISTANCE_SHADOW = 2143
-	SPELLRESISTANCE_FEL = 2144
-	SPELLWEAKNESS_ARCANE = 2145
-	SPELLWEAKNESS_FIRE = 2146
-	SPELLWEAKNESS_FROST = 2147
-	SPELLWEAKNESS_NATURE = 2148
-	SPELLWEAKNESS_HOLY = 2149
-	SPELLWEAKNESS_SHADOW = 2150
-	SPELLWEAKNESS_FEL = 2151
+	SPELL_RESISTANCE_ARCANE = 2138
+	SPELL_RESISTANCE_FIRE = 2139
+	SPELL_RESISTANCE_FROST = 2140
+	SPELL_RESISTANCE_NATURE = 2141
+	SPELL_RESISTANCE_HOLY = 2142
+	SPELL_RESISTANCE_SHADOW = 2143
+	SPELL_RESISTANCE_FEL = 2144
+	SPELL_WEAKNESS_ARCANE = 2145
+	SPELL_WEAKNESS_FIRE = 2146
+	SPELL_WEAKNESS_FROST = 2147
+	SPELL_WEAKNESS_NATURE = 2148
+	SPELL_WEAKNESS_HOLY = 2149
+	SPELL_WEAKNESS_SHADOW = 2150
+	SPELL_WEAKNESS_FEL = 2151
 	BACON_BUDDY = 2154
 	BACON_STARSTOBOUNCEOFF = 2155
-	LETTUCE_ATTACK = 2159
-	LETTUCE_SPELLCOMBO = 2160
+	LETTUCE_KEYWORD_ATTACK = 2159
+	LETTUCE_KEYWORD_SPELL_COMBO = 2160
 	LETTUCE_BOUNTY_BOSS = 2168
 	LETTUCE_IS_TREASURE_CARD = 2170
 	LETTUCE_SPELLDAMAGEARCANE = 2171
 	LETTUCE_SPELLDAMAGEFEL = 2172
 	LETTUCE_SPELLDAMAGEFIRE = 2173
 	LETTUCE_SPELLDAMAGEFROST = 2174
 	LETTUCE_SPELLDAMAGEHOLY = 2175
@@ -650,17 +653,17 @@
 	COST_BLOOD = 2196
 	COST_FROST = 2197
 	COST_UNHOLY = 2198
 	COST_DEATH = 2199
 	HAS_BLOOD_PLAGUE = 2211
 	HAS_FROST_PLAGUE = 2212
 	HAS_UNHOLY_PLAGUE = 2213
-	BLEED = 2214
-	CRITICALDAMAGE = 2219
-	ROOT = 2220
+	LETTUCE_BLEED = 2214
+	LETTUCE_KEYWORD_CRITICAL_DAMAGE = 2219
+	LETTUCE_KEYWORD_ROOT = 2220
 	LETTUCE_SHOW_OPPOSING_FAKE_HAND = 2224
 	BACON_DIABLO_FIGHT_DIABLO_PLAYER_ID = 2226
 	LETTUCE_VERSUS_SPELL_STATE = 2228
 	LETTUCE_START_OF_GAME_ABILITY = 2241
 	COLOSSAL = 2247
 	COLOSSAL_LIMB = 2248
 	CURRENT_TEMP_SPELLPOWER_ARCANE = 2250
@@ -683,32 +686,32 @@
 	CURRENT_HEALING_POWER = 2333
 	EARLY_CONCEDE_POPUP_AVAILABLE = 2340
 	BACON_PLAYER_NUM_HERO_BUDDIES_GAINED = 2346
 	BATTLEGROUNDS_FAVORITE_FINISHER = 2348
 	LOCATION_ACTION_COST = 2352
 	LOCATION_ACTION_COOLDOWN = 2353
 	WHELP = 2355
-	SPELLCRAFT = 2359
+	BACON_SPELLCRAFT_ID = 2359
 	BACON_HERO_BUDDY_PROGRESS = 2364
 	REVIVE = 2369
 	BACON_HEROPOWER_BASE_HERO_ID = 2376
 	LETTUCE_CURSED_ABILITY_VISUAL = 2381
 	BACON_OMIT_WHEN_OUT_OF_ROTATION = 2387
 	ALLIED = 2388
-	LETTUCE_HEALINGPOWER = 2434
+	LETTUCE_KEYWORD_HEALING_POWER = 2434
 	DONT_SUPPRESS_SUMMON_VO = 2440
 	BACON_NUMBER_HERO_REFRESH_AVAILABLE = 2452
 	BACON_FREEZE_TOOLTIP = 2455
 	INFUSE = 2456
 	INFUSED = 2457
 	HAS_DRAG_TO_BUY = 2458
 	ENTITY_TAG_THRESHOLD_TAG_ID = 2459
 	ENTITY_TAG_THRESHOLD_VALUE = 2460
-	MERCS_SPELLWEAKNESS = 2464
-	MERCS_SPELLRESISTANCE = 2465
+	MERCENARIES_SPELL_WEAKNESS = 2464
+	MERCENARIES_SPELL_RESISTANCE = 2465
 	BACON_QUESTS_ACTIVE = 2468
 	COLOSSAL_LIMB_ON_LEFT = 2469
 	LETTUCE_ABILITY_TILE_VISUAL_PUBLIC_SPEED = 2470
 	BACON_DIED_LAST_COMBAT = 2483
 	LETTUCE_ABILITY_TIER = 2493
 	LETTUCE_EQUIPMENT_TIER = 2494
 	MANATHIRST = 2498
@@ -722,15 +725,15 @@
 	BACON_MINION_TYPE_REWARD = 2571
 	COPIED_HINT = 2572
 	BLEEDING = 2575
 	HAS_SIGNATURE_QUALITY = 2589
 	IMMOLATESTAGE = 2600
 	EVIL_TWIN_MUSTACHE = 2611
 	SINFUL_BRAND = 2613
-	LETTUCE_SILENCE = 2631
+	LETTUCE_KEYWORD_SILENCE = 2631
 	BACON_QUEST_COMPLETED = 2633
 	CORPSES_SPENT_THIS_GAME = 2639
 	HAUNTED_SECRET = 2634
 	DONT_SUPPRESS_KEYWORD_VO = 2636
 	CARD_BACK_OVERRIDE = 2637
 	CARDTEXT_ENTITY_0 = 2655
 	CARDTEXT_ENTITY_1 = 2656
@@ -779,26 +782,26 @@
 	HAS_ACTIVATE_POWER = 2840
 	EMOTECLASS = 2851
 	VENOMOUS = 2853
 	MAGNETIC_TO_RACE = 2859
 	BACON_MAX_LEADERBOARD_ARMOR = 2867
 	IS_USING_FORGE_OPTION = 2869
 	BACON_REBORN_TOOLTIP = 2870
-	BACON_PUTRICIDESCREATION_TOOLTIP = 2875
+	BACON_PUTRICIDES_CREATION_TOOLTIP = 2875
 	TAG_SCRIPT_DATA_NUM_3 = 2889
 	CARD_NAME_DATA_1 = 2890
 	BACON_GLOBAL_ANOMALY_DBID = 2897
 	QUICKDRAW = 2905
 	BACON_COSTS_HEALTH_TO_BUY = 2911
 	TAG_SCRIPT_DATA_NUM_4 = 2919
 	TAG_SCRIPT_DATA_NUM_5 = 2920
 	TAG_SCRIPT_DATA_NUM_6 = 2921
 	DECK_SWAP_ACTIVE = 2929
 	MAX_SIDEBOARD_CARDS = 2931
-	BONUSEFFECTS = 2934
+	BONUS_EFFECTS = 2934
 	BACON_USE_COIN_BASED_BUDDY_METER = 2935
 	BACON_BUY_BUDDY = 2937
 	BACON_BUY_BUDDY_2 = 2938
 	BACON_SHOW_HEROPOWER_BUDDY_AS_EVOLVING_BIG_CARD = 2943
 	HIDDEN_CHOICE_OVERRIDE = 2946
 	FORGED = 3011
 	BUILDING_UP = 3016
@@ -810,14 +813,15 @@
 	CTHUN_HEALTH_BUFF = 3053
 	CTHUN_ATTACK_BUFF = 3054
 	FORGE_REVEALED = 3070
 	FORGES_INTO = 3074
 	FX_DATANUM_2 = 3077
 	RITUALIST_MINION = 3078
 	FX_DATANUM_3 = 3109
+	ALLOW_MOVE_BACON_SPELL = 3111
 	EXCAVATE = 3114
 	SUMMONED_WHEN_DRAWN = 3128
 	IS_ALTERNATE_HEROPOWER = 3130
 	TITAN_ABILITY_USED_1 = 3140
 	TITAN_ABILITY_USED_2 = 3141
 	TITAN_ABILITY_USED_3 = 3142
 	ANOMALY1 = 3182
@@ -827,15 +831,37 @@
 	TUTORIAL_PLAY_MINION_ANIM = 3195
 	TUTORIAL_HERO_POWER_TARGET_MINION_ANIM = 3196
 	TUTORIAL_HERO_POWER_TARGET_OPPONENT_ANIM = 3197
 	SUPPRESS_EVIL_TWIN_MUSTACHE_SOUND = 3198
 	HERO_DOESNT_MOVE_ON_ATTACK = 3211
 	CURRENT_EXCAVATE_TIER = 3249
 	ALONE_RANGER = 3258
+	CUTSCENE_CARD_TYPE = 3265
+	MINIATURIZE = 3318
+	MINI = 3319
 	MAX_EXCAVATE_TIER = 3326
+	PALADIN_AURA = 3374
+	ZILLIAX_CUSTOMIZABLE_COSMETICMODULE = 3376
+	ZILLIAX_CUSTOMIZABLE_FUNCTIONALMODULE = 3377
+	SIDEBOARD_TYPE = 3427
+	CREATED_BY_TWINSPELL = 3432
+	CREATED_BY_MINIATURIZE = 3433
+	SUPPRESS_HERO_STANDARD_SUMMON_FX = 3438
+	ZILLIAX_CUSTOMIZABLE_LINKED_COSMETICMOUDLE = 3450
+	MIN_SIDEBOARD_CARDS = 3459
+	FORGETFUL_ATTACK_VISUAL = 3460
+	SHUDDERWOCKHIGHLIGHTHINT = 3463
+	NUM_TURNS_LAST_AFFECTED_BY = 3464
+	EXTRA_TURNS_SPELL_OVERRIDE = 3465
+	ZILLIAX_CUSTOMIZABLE_LINKED_FUNCTIONALMOUDLE = 3470
+	HIDE_HEALTH_NUMBER = 3471
+	HIDE_ATTACK_NUMBER = 3472
+	ZILLIAX_CUSTOMIZABLE_SAVED_VERSION = 3477
+	SUPPRESS_MILL_ANIMATION = 3481
+	IGNORE_SUPPRESS_MILL_ANIMATION = 3482
 
 	InvisibleDeathrattle = 335
 	ImmuneToSpellpower = 349
 	AttackVisualType = 251
 	DevState = 268
 	GrantCharge = 355
 	HealTarget = 361
@@ -854,14 +880,16 @@
 	# Renamed
 	BACON_FREEZE = BACON_FREEZE_TOOLTIP
 	BACON_HIGHLIGHT_ATTACKING_MINION_DURING_COMBAT = HIGHLIGHT_ATTACKING_MINION_DURING_COMBAT
 	BACON_USE_FAST_ANIMATIONS = USE_FAST_ACTOR_TRANSITION_ANIMATIONS
 	CANT_BE_DAMAGED = IMMUNE
 	CANT_BE_DISPELLED = CANT_BE_SILENCED
 	CANT_BE_TARGETED_BY_ABILITIES = CANT_BE_TARGETED_BY_SPELLS
+	CURRENT_SPELLPOWER_BASE = CURRENT_SPELLPOWER
+	CURRENT_TEMP_SPELLPOWER_BASE = CURRENT_TEMP_SPELLPOWER
 	DEATH_RATTLE = DEATHRATTLE
 	DEATHRATTLE_SENDS_BACK_TO_DECK = DEATHRATTLE_RETURN_ZONE
 	DISABLE_GOLDEN_ANIMATIONS = DISABLE_NONHERO_GOLDEN_ANIMATIONS
 	EXTRA_DEATHRATTLES = EXTRA_MINION_DEATHRATTLES_BASE
 	HAND_REVEALED = ZONES_REVEALED
 	HEALING_DOUBLE = SPELL_HEALING_DOUBLE
 	# HIDE_COST = HIDE_STATS  # Added back
@@ -874,14 +902,50 @@
 	RED_MANA_CRYSTALS = RED_MANA_GEM
 	TAG_HERO_POWER_DOUBLE = HERO_POWER_DOUBLE
 	TAG_AI_MUST_PLAY = AI_MUST_PLAY
 	# TREASURE = DISCOVER  # Added back
 	SHOWN_HERO_POWER = HERO_POWER
 	EVILZUG = MARK_OF_EVIL
 	TRADE_COST = DECK_ACTION_COST
+	START_OF_GAME = START_OF_GAME_KEYWORD
+	SPELLRESISTANCE_ARCANE = SPELL_RESISTANCE_ARCANE
+	SPELLRESISTANCE_FIRE = SPELL_RESISTANCE_FIRE
+	SPELLRESISTANCE_FROST = SPELL_RESISTANCE_FROST
+	SPELLRESISTANCE_NATURE = SPELL_RESISTANCE_NATURE
+	SPELLRESISTANCE_HOLY = SPELL_RESISTANCE_HOLY
+	SPELLRESISTANCE_SHADOW = SPELL_RESISTANCE_SHADOW
+	SPELLRESISTANCE_FEL = SPELL_RESISTANCE_FEL
+	SPELLWEAKNESS_ARCANE = SPELL_WEAKNESS_ARCANE
+	SPELLWEAKNESS_FIRE = SPELL_WEAKNESS_FIRE
+	SPELLWEAKNESS_FROST = SPELL_WEAKNESS_FROST
+	SPELLWEAKNESS_NATURE = SPELL_WEAKNESS_NATURE
+	SPELLWEAKNESS_HOLY = SPELL_WEAKNESS_HOLY
+	SPELLWEAKNESS_SHADOW = SPELL_WEAKNESS_SHADOW
+	SPELLWEAKNESS_FEL = SPELL_WEAKNESS_FEL
+	LETTUCE_ATTACK = LETTUCE_KEYWORD_ATTACK
+	LETTUCE_SPELLCOMBO = LETTUCE_KEYWORD_SPELL_COMBO
+	BLEED = LETTUCE_BLEED
+	CRITICALDAMAGE = LETTUCE_KEYWORD_CRITICAL_DAMAGE
+	ROOT = LETTUCE_KEYWORD_ROOT
+	LETTUCE_HEALINGPOWER = LETTUCE_KEYWORD_HEALING_POWER
+	MERCS_SPELLWEAKNESS = MERCENARIES_SPELL_WEAKNESS
+	MERCS_SPELLRESISTANCE = MERCENARIES_SPELL_RESISTANCE
+	LETTUCE_SILENCE = LETTUCE_KEYWORD_SILENCE
+	ENRAGED_TOOLTIP = ENRAGE_TOOLTIP
+	SIDEQUEST = SIDE_QUEST
+	AUTOATTACK = AUTO_ATTACK
+	CASTSWHENDRAWN = CASTS_WHEN_DRAWN
+	FATIGUEREFERENCE = FATIGUE_REFERENCE
+	CORRUPTEDCARD = CORRUPTED_CARD
+	HONORABLEKILL = HONORABLE_KILL
+	BONUSEFFECTS = BONUS_EFFECTS
+	BLOOD_GEM = BACON_BLOOD_GEM_TOOLTIP
+	REFRESH = BACON_REFRESH_TOOLTIP
+	SPELLCRAFT = BACON_SPELLCRAFT_ID
+	BACON_PUTRICIDESCREATION_TOOLTIP = BACON_PUTRICIDES_CREATION_TOOLTIP
 
 	# Deleted
 	IGNORE_DAMAGE = 1
 	GOLD_REWARD_STATE = 13
 	COPY_DEATHRATTLE = 55
 	COPY_DEATHRATTLE_INDEX = 56
 	CARD_ID = 186
@@ -908,15 +972,14 @@
 	OUTGOING_COMBAT_DAMAGE_MULTIPLIER = 287
 	OUTGOING_COMBAT_DAMAGE_CAP = 288
 	INCOMING_COMBAT_DAMAGE_MULTIPLIER = 289
 	INCOMING_COMBAT_DAMAGE_CAP = 290
 	DIVINE_SHIELD_READY = 314
 	IGNORE_DAMAGE_OFF = 354
 	NUM_OPTIONS = 359
-	OBFUSCATED = 391
 	LAST_CARD_PLAYED = 397
 	RITUAL = 424
 	PROXY_CTHUN = 434
 	PENDING_EVOLUTIONS = 461
 	WEATHER = 1002
 	WEATHERSNOWSTORM = 1012
 	WEATHERTHUNDERSTORM = 1013
@@ -1003,15 +1066,15 @@
 	GameTag.HOW_TO_EARN: "HowToGetThisCard",
 	GameTag.HOW_TO_EARN_GOLDEN: "HowToGetThisGoldCard",
 	GameTag.AI_MUST_PLAY: "AIMustPlay",
 	GameTag.AFFECTED_BY_SPELL_POWER: "AffectedBySpellPower",
 	GameTag.SPARE_PART: "SparePart",
 	GameTag.HIDE_STATS: "HideStats",
 	GameTag.DISCOVER: "Treasure",
-	GameTag.AUTOATTACK: "AutoAttack",
+	GameTag.AUTO_ATTACK: "AutoAttack",
 }
 
 
 ##
 # Card enums
 
 class CardClass(IntEnum):
@@ -1106,15 +1169,17 @@
 	MERCENARIES_DEV = 1705
 	RETURN_OF_THE_LICH_KING = 1776
 	BATTLE_OF_THE_BANDS = 1809
 	TITANS = 1858
 	PATH_OF_ARTHAS = 1869
 	WILD_WEST = 1892
 	WONDERS = 1898
+	WHIZBANGS_WORKSHOP = 1897
 	TUTORIAL = 1904
+	EVENT = 1941
 
 	# Not actually present...
 	TAVERNS_OF_TIME = 1143
 	PLACEHOLDER_202204 = 1810
 
 	# Aliased from the original enums
 	FP1 = 12
@@ -1155,14 +1220,15 @@
 			CardSet.THE_SUNKEN_CITY,
 			CardSet.RETURN_OF_THE_LICH_KING,
 			CardSet.PATH_OF_ARTHAS,
 			CardSet.BATTLE_OF_THE_BANDS,
 			CardSet.TITANS,
 			CardSet.WILD_WEST,
 			CardSet.WONDERS,
+			CardSet.WHIZBANGS_WORKSHOP
 		)
 
 	@property
 	def name_global(self):
 		# Newer sets use a 2-3 letter set code
 		from .utils import CARDSET_GLOBAL_STRING_MAP
 		custom = CARDSET_GLOBAL_STRING_MAP.get(self)
@@ -1174,15 +1240,15 @@
 
 	@property
 	def short_name_global(self):
 		return self.name_global + "_SHORT"
 
 	@property
 	def is_standard(self):
-		return self in ZodiacYear.WOLF.standard_card_sets
+		return self in ZodiacYear.PEGASUS.standard_card_sets
 
 
 class CardType(IntEnum):
 	"""TAG_CARDTYPE"""
 
 	INVALID = 0
 	GAME = 1
@@ -1198,14 +1264,15 @@
 	BLANK = 11
 	GAME_MODE_BUTTON = 12
 	MOVE_MINION_HOVER_TARGET = 22
 	LETTUCE_ABILITY = 23
 	BATTLEGROUND_HERO_BUDDY = 24
 	LOCATION = 39
 	BATTLEGROUND_QUEST_REWARD = 40
+	BATTLEGROUND_SPELL = 42
 	BATTLEGROUND_ANOMALY = 43
 
 	# Renamed
 	ABILITY = SPELL
 
 	@property
 	def playable(self):
@@ -1974,14 +2041,16 @@
 	FIRE = 2
 	FROST = 3
 	NATURE = 4
 	HOLY = 5
 	SHADOW = 6
 	FEL = 7
 	PHYSICAL_COMBAT = 8
+	TAVERN = 9
+	SPELLCRAFT = 10
 
 
 class OptionType(IntEnum):
 	"""PegasusGame.Option.Type"""
 
 	PASS = 1
 	END_TURN = 2
@@ -2205,14 +2274,15 @@
 	POWERED_UP = 27
 	MULTIPLE_ALT_TEXT_SCRIPT_DATA_NUMS = 28
 	REFERENCE_SCRIPT_DATA_NUM_1_ENTITY_POWER = 29
 	REFERENCE_SCRIPT_DATA_NUM_1_CARD_DBID = 30
 	REFERENCE_SCRIPT_DATA_NUM_CARD_RACE = 31
 	BG_QUEST = 32
 	MULTIPLE_ALT_TEXT_SCRIPT_DATA_NUMS_REF_SDN6_CARD_DBID = 33
+	ZILLIAX_DELUXE_3000 = 34
 
 	# Renamed
 	DEPRECATED_5 = PRIMORDIAL_WAND
 	DEPRECATED_6 = ALTERNATE_CARD_TEXT
 	DEPRECATED_8 = GALAKROND_COUNTER
 	DEPRECATED_10 = PLAYER_TAG_THRESHOLD
 	DEPRECATED_11 = ENTITY_TAG_THRESHOLD
@@ -2412,15 +2482,15 @@
 	GameTag.PLAYSTATE: PlayState,
 	GameTag.ZONE: Zone,
 	GameTag.FAKE_ZONE: Zone,
 	GameTag.STEP: Step,
 	GameTag.NEXT_STEP: Step,
 	GameTag.STATE: State,
 	GameTag.MULLIGAN_STATE: Mulligan,
-	GameTag.AUTOATTACK: Type.BOOL,
+	GameTag.AUTO_ATTACK: Type.BOOL,
 	GameTag.SPELL_SCHOOL: SpellSchool,
 	GameTag.LETTUCE_ROLE: Role,
 }
 
 
 LOCALIZED_TAGS = [k for k, v in TAG_TYPES.items() if v == Type.LOCSTRING]
 
@@ -2485,14 +2555,15 @@
 	MAMMOTH = 2
 	RAVEN = 3
 	DRAGON = 4
 	PHOENIX = 5
 	GRYPHON = 6
 	HYDRA = 7
 	WOLF = 8
+	PEGASUS = 9
 
 	@property
 	def standard_card_sets(self):
 		from .utils import STANDARD_SETS
 		return STANDARD_SETS.get(self, [])
 
 	@classmethod
```

### Comparing `hearthstone-7.9.0/hearthstone/mercenaryxml.py` & `hearthstone-8.0.0/hearthstone/mercenaryxml.py`

 * *Files identical despite different names*

### Comparing `hearthstone-7.9.0/hearthstone/stringsfile.py` & `hearthstone-8.0.0/hearthstone/stringsfile.py`

 * *Files identical despite different names*

### Comparing `hearthstone-7.9.0/hearthstone/utils/__init__.py` & `hearthstone-8.0.0/hearthstone/utils/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -175,16 +175,21 @@
 		CardSet.RETURN_OF_THE_LICH_KING, CardSet.PATH_OF_ARTHAS,
 		CardSet.BATTLE_OF_THE_BANDS,
 	],
 	ZodiacYear.WOLF: [
 		CardSet.CORE,
 		CardSet.THE_SUNKEN_CITY, CardSet.REVENDRETH, CardSet.RETURN_OF_THE_LICH_KING,
 		CardSet.PATH_OF_ARTHAS, CardSet.BATTLE_OF_THE_BANDS, CardSet.TITANS,
-		CardSet.WILD_WEST
-	]
+		CardSet.WILD_WEST, CardSet.WHIZBANGS_WORKSHOP, CardSet.EVENT,
+	],
+	ZodiacYear.PEGASUS: [
+		CardSet.CORE,
+		CardSet.BATTLE_OF_THE_BANDS, CardSet.TITANS, CardSet.WILD_WEST,
+		CardSet.EVENT, CardSet.WHIZBANGS_WORKSHOP,
+	],
 }
 
 
 try:
 	_EPOCH = datetime.fromtimestamp(0)
 except OSError:
 	# https://bugs.python.org/issue29097 (Windows-only)
@@ -197,14 +202,15 @@
 	ZodiacYear.MAMMOTH: datetime(2017, 4, 7),
 	ZodiacYear.RAVEN: datetime(2018, 4, 12),
 	ZodiacYear.DRAGON: datetime(2019, 4, 9),
 	ZodiacYear.PHOENIX: datetime(2020, 4, 7),
 	ZodiacYear.GRYPHON: datetime(2021, 3, 30),
 	ZodiacYear.HYDRA: datetime(2022, 4, 12),
 	ZodiacYear.WOLF: datetime(2023, 4, 11),
+	ZodiacYear.PEGASUS: datetime(2024, 3, 19),
 }
 
 
 # QuestController.cs
 QUEST_REWARDS = {
 	"UNG_940": "UNG_940t8",
 	"UNG_954": "UNG_954t1",
@@ -390,14 +396,32 @@
 	"JAM_018t3": "JAM_018",  # Emotional Rhapsody
 	"JAM_018t4": "JAM_018",  # Wailing Rhapsody
 	# Remixed Musician
 	"JAM_033t": "JAM_033",  # Cathedral Musician
 	"JAM_033t2": "JAM_033",  # Tropical Musician
 	"JAM_033t3": "JAM_033",  # Romantic Musician
 	"JAM_033t4": "JAM_033",  # Noise Musician
+	# Lesser Opal Spellstone
+	"TOY_645t": "TOY_645",
+	"TOY_645t1": "TOY_645",
+	# Lesser Spinel Spellstone
+	"TOY_825t": "TOY_825",
+	"TOY_825t2": "TOY_825",
+	# Blossoms
+	"TTN_950t3": "TTN_950",  # Forest Seedlings
+	"TTN_930t": "TTN_930",  # Frost Lotus Seedling
+	# Zilliax Deluxe 3000
+	"TOY_330t5": "TOY_330",
+	"TOY_330t6": "TOY_330",
+	"TOY_330t7": "TOY_330",
+	"TOY_330t8": "TOY_330",
+	"TOY_330t9": "TOY_330",
+	"TOY_330t10": "TOY_330",
+	"TOY_330t11": "TOY_330",
+	"TOY_330t12": "TOY_330",
 }
 
 
 def get_original_card_id(card_id):
 	# Transfer Student
 	if str(card_id).startswith("SCH_199t"):
 		return "SCH_199"
```

### Comparing `hearthstone-7.9.0/hearthstone/xmlutils.py` & `hearthstone-8.0.0/hearthstone/xmlutils.py`

 * *Files identical despite different names*

### Comparing `hearthstone-7.9.0/hearthstone.egg-info/PKG-INFO` & `hearthstone-8.0.0/hearthstone.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hearthstone
-Version: 7.9.0
+Version: 8.0.0
 Summary: CardDefs.xml parser and Hearthstone enums for Python
 Home-page: https://github.com/HearthSim/python-hearthstone/
 Download-URL: https://github.com/HearthSim/python-hearthstone/tarball/master
 Author: Jerome Leclanche
 Author-email: jerome@leclan.ch
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `hearthstone-7.9.0/hearthstone.egg-info/SOURCES.txt` & `hearthstone-8.0.0/hearthstone.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hearthstone-7.9.0/setup.cfg` & `hearthstone-8.0.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = hearthstone
-version = 7.9.0
+version = 8.0.0
 description = CardDefs.xml parser and Hearthstone enums for Python
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Jerome Leclanche
 author_email = jerome@leclan.ch
 url = https://github.com/HearthSim/python-hearthstone/
 download_url = https://github.com/HearthSim/python-hearthstone/tarball/master
```

