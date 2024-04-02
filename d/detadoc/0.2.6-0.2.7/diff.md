# Comparing `tmp/detadoc-0.2.6.tar.gz` & `tmp/detadoc-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "detadoc-0.2.6.tar", max compression
+gzip compressed data, was "detadoc-0.2.7.tar", max compression
```

## Comparing `detadoc-0.2.6.tar` & `detadoc-0.2.7.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0        0 2023-12-30 15:32:37.773402 detadoc-0.2.6/detadoc/__init__.py
--rw-r--r--   0        0        0     1871 2024-02-04 21:38:04.629317 detadoc-0.2.6/detadoc/annotations.py
--rw-r--r--   0        0        0     4721 2024-03-26 21:37:58.470242 detadoc-0.2.6/detadoc/bases.py
--rw-r--r--   0        0        0     8987 2024-03-05 12:36:04.895830 detadoc-0.2.6/detadoc/enum.py
--rw-r--r--   0        0        0     2336 2024-03-04 23:54:12.920957 detadoc-0.2.6/detadoc/helper.py
--rw-r--r--   0        0        0    44512 2024-03-26 02:55:05.791108 detadoc-0.2.6/detadoc/models.py
--rw-r--r--   0        0        0     4988 2024-03-24 19:05:37.271242 detadoc-0.2.6/detadoc/regex.py
--rw-r--r--   0        0        0      519 2024-03-26 21:37:58.475002 detadoc-0.2.6/pyproject.toml
--rw-r--r--   0        0        0      760 2024-03-26 21:38:56.788820 detadoc-0.2.6/setup.py
--rw-r--r--   0        0        0      593 2024-03-26 21:38:56.789189 detadoc-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-12-30 15:32:37.773402 detadoc-0.2.7/detadoc/__init__.py
+-rw-r--r--   0        0        0     1871 2024-02-04 21:38:04.629317 detadoc-0.2.7/detadoc/annotations.py
+-rw-r--r--   0        0        0     3745 2024-03-27 03:28:40.331199 detadoc-0.2.7/detadoc/bases.py
+-rw-r--r--   0        0        0     9746 2024-04-01 19:44:24.905798 detadoc-0.2.7/detadoc/enum.py
+-rw-r--r--   0        0        0     2336 2024-03-04 23:54:12.920957 detadoc-0.2.7/detadoc/helper.py
+-rw-r--r--   0        0        0    46634 2024-04-02 00:56:53.301351 detadoc-0.2.7/detadoc/models.py
+-rw-r--r--   0        0        0     4988 2024-03-24 19:05:37.271242 detadoc-0.2.7/detadoc/regex.py
+-rw-r--r--   0        0        0      519 2024-04-02 14:18:14.244967 detadoc-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0      760 2024-04-02 14:18:53.755564 detadoc-0.2.7/setup.py
+-rw-r--r--   0        0        0      593 2024-04-02 14:18:53.755780 detadoc-0.2.7/PKG-INFO
```

### Comparing `detadoc-0.2.6/detadoc/annotations.py` & `detadoc-0.2.7/detadoc/annotations.py`

 * *Files identical despite different names*

### Comparing `detadoc-0.2.6/detadoc/bases.py` & `detadoc-0.2.7/detadoc/bases.py`

 * *Files 23% similar despite different names*

```diff
@@ -138,47 +138,7 @@
             return self.amount < other.amount
         return self.date < other.date
         
     
     def __str__(self):
         return f' R$ {self.amount} {self.flow} {self.date} {self.description}'
 
-
-# class Entry(SpaceModel):
-#     transaction: Transaction
-#     description: str = ''
-#
-#     def __lt__(self, other):
-#         assert isinstance(other, type(self))
-#         return self.transaction.accounting_date < other.transaction.accounting_date
-#
-#     def __str__(self):
-#         return f'{self.transaction.display} {self.description}'
-#
-#     @property
-#     def value(self) -> Decimal:
-#         if self.account.type == self.transaction_type:
-#             return self.amount
-#         return Decimal('0') - self.amount
-#
-#     @property
-#     def account(self):
-#         return self.transaction.account
-#
-#     @property
-#     def amount(self):
-#         return self.transaction.amount
-#
-#     @property
-#     def account_subtype(self):
-#         return self.account.subtype
-#
-#     @property
-#     def account_type(self):
-#         return self.account.subtype.type
-#
-#     @property
-#     def transaction_type(self):
-#         return self.transaction.type
-#
-#
-
```

### Comparing `detadoc-0.2.6/detadoc/enum.py` & `detadoc-0.2.7/detadoc/enum.py`

 * *Files 5% similar despite different names*

```diff
@@ -64,15 +64,37 @@
     def __int__(self):
         return self.minutes
     
     def __lt__(self, other):
         return self.minutes < other.minutes
 
 
+@enummap
+class DayTime2(StrEnum):
+    _ignore_ = 'DayTime2 h m add_right_zero'
+    DayTime2 = vars()
+    for h in range(24):
+        for m in range(0, 60, 15):
+            DayTime2[f'T{add_right_zero(h)}_{add_right_zero(m)}'] = f'{add_right_zero(h)}:{add_right_zero(m)}'
+    
+    @property
+    def minutes(self):
+        numbers = [int(x) for x in self.value.split(":")]
+        return (numbers[0] * 60) + numbers[-1]
+    
+    @classmethod
+    def parse(cls, value: datetime.datetime = None):
+        value = value or datetime.datetime.now()
+        return DayTime[f'T{add_right_zero(value.hour)}_{add_right_zero(value.minute)}']
+    
+    def __int__(self):
+        return self.minutes
     
+    def __lt__(self, other):
+        return self.minutes < other.minutes
     
 @enummap
 class Month(StrEnum):
     JAN = "Janeiro"
     FEB = "Fevereiro"
     MAR = 'Março'
     APR = "Abril"
```

### Comparing `detadoc-0.2.6/detadoc/helper.py` & `detadoc-0.2.7/detadoc/helper.py`

 * *Files identical despite different names*

### Comparing `detadoc-0.2.6/detadoc/models.py` & `detadoc-0.2.7/detadoc/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -267,15 +267,14 @@
     specialties: ListOfStrings
     subspecialties: ListOfStrings
 
 
 @modelmap
 class Doctor(ProfessionalBase):
     MODEL_GROUPS = ['Profile', 'Staff']
-    EXIST_QUERY = 'key'
     crm: Optional[str] = None
 
     @classmethod
     async def admin_data(cls) -> dict:
         return await cls.fetch_one('admin')
     
     @classmethod
@@ -289,14 +288,16 @@
             return f'Dr. {self.name}'
         return f'Dra. {self.name}'
     
     
 @enummap
 class Admin(Doctor):
     TABLE_NAME = 'Doctor'
+    EXIST_QUERY = 'key'
+
     
     def model_post_init(self, __context: Any) -> None:
         super().model_post_init(__context)
         self.key = 'admin'
 
 
 @modelmap
@@ -394,15 +395,14 @@
     PAYABLE_ACCOUNT: ClassVar[Account] = Account.PLI
     RECEIVABLE_ACCOUNT: ClassVar[Account] = Account.RAT
     CASH_ACCOUNT: ClassVar[Account] = Account.CAT
     BANK_ACCOUNT: ClassVar[Account] = Account.BAT
     DIVIDEND_ACCOUNT: ClassVar[Account] = Account.WDI
     INVOICE_TYPE: ClassVar[InvoiceType] = InvoiceType.G
     
-    
     @computed_field
     @property
     def type(self) -> str:
         return self.INVOICE_TYPE.name
     
     def __str__(self):
         if self.flow == CashFlow.EX:
@@ -623,15 +623,15 @@
     def date(self):
         return self.start
     
     async def setup_instance(self):
         pass
     
     def __str__(self):
-        return f'{self.start} Diagnóstico: {self.title}'
+        return f'{self.start}: {self.title}'
 
     def __lt__(self, other):
         return self.start < other.start
     
     
     
 @modelmap
@@ -791,14 +791,26 @@
     def items_dict(self):
         result = {}
         for item in self.items_list():
             result[item.name] = (self.LabResultItem.parse_number(item.amount), item.unit)
         return result
     
 
+@modelmap
+class SubstanceAbuse(PatientKeyBase):
+    SINGULAR = 'Abuso de Substância'
+    PLURAL = 'Abuso de Substâncias'
+    EXIST_QUERY = 'patient_key substance date'
+    substance: str
+    dosage: Decimal = Field(Decimal('1'))
+    dosage_form: str = Field(default_factory=str)
+    period: Period = Period.D1
+    frequency: Frequency = Frequency.N1
+    notes: Optional[str] = None
+
     
 @modelmap
 class Prescription(PatientKeyBase):
     SINGULAR = 'Prescrição'
     PLURAL = 'Prescrições'
     EXIST_QUERY = 'medication_key patient_key start'
     FETCH_QUERY = {'end': None}
@@ -880,17 +892,59 @@
     TABLE_NAME = 'Prescription'
     FETCH_QUERY = {'end?ne': None}
     
     
 @modelmap
 class Sleep(PatientKeyBase):
     SINGULAR = 'Sono'
-    bed_hours: float
-    sleep_hours: float
-
+    bed_time: DayTime
+    sleep_time: DayTime
+    awake_time: DayTime
+    rise_time: DayTime
+    quality: Quality
+    awakes: PositiveIntegerField = 0
+    notes: str = Field(default_factory=str)
+    
+    @staticmethod
+    def subtracted(value: DayTime):
+        return int(DayTime.T23_59) - int(value)
+    
+    @property
+    def bed_to_sleep_minutes(self):
+        if self.sleep_time < self.bed_time:
+            return int(self.sleep_time) + self.subtracted(self.bed_time)
+        return int(self.sleep_time) - int(self.bed_time)
+    
+    @property
+    def sleep_to_awake_minutes(self):
+        if self.awake_time < self.sleep_time:
+            return int(self.awake_time) + self.subtracted(self.sleep_time)
+        return int(self.awake_time) - int(self.sleep_time)
+    
+    @property
+    def awake_to_rise_minutes(self):
+        if self.rise_time < self.awake_time:
+            return int(self.rise_time) + self.subtracted(self.awake_time)
+        return int(self.rise_time) - int(self.awake_time)
+    
+    @property
+    def bed_to_rise_minutes(self):
+        if self.rise_time < self.bed_time:
+            return int(self.rise_time) + self.subtracted(self.bed_time)
+        return int(self.rise_time) - int(self.bed_time)
+    
+    @property
+    def sleep_hours(self):
+        return(self.sleep_to_awake_minutes / 60).__round__(2)
+    
+    @property
+    def bed_hours(self):
+        return(self.bed_to_rise_minutes / 60).__round__(2)
+        
+    
     
 @modelmap
 class Task(CreatedBase):
     TABLE_NAME = 'Task'
     creator: str 
     title: str
     description: str
@@ -1378,11 +1432,22 @@
     def __str__(self):
         return f'{self.created.date()}: {self.complaints}'
         
     
 
 
 if __name__ == '__main__':
-    x = ProfileMessage('2024-04-08T22:30:09 Doctor.admin Boa noite.')
-    print(x.value)
-    print(x.text)
-    print(x)
+    now = datetime.datetime.now()
+    x = Sleep(
+            patient_key='teste',
+            bed_time=now,
+            sleep_time=now + datetime.timedelta(minutes=60),
+            awake_time=now + datetime.timedelta(minutes=60*6),
+            rise_time=now + datetime.timedelta(minutes=60*7),
+            quality='I',
+            awakes=1
+    )
+    print(x)
+    print(x.sleep_minutes)
+    print(x.sleep_hours)
+    print(x.bed_hours)
+    print(x.bed_to_sleep_minutes)
```

### Comparing `detadoc-0.2.6/detadoc/regex.py` & `detadoc-0.2.7/detadoc/regex.py`

 * *Files identical despite different names*

### Comparing `detadoc-0.2.6/pyproject.toml` & `detadoc-0.2.7/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "detadoc"
-version = "0.2.6"
+version = "0.2.7"
 description = ""
 authors = ["Daniel Arantes <arantesdv@me.com>"]
 exclude = ['src', '.space', 'Spacefile', '.env', 'dev.py']
 
 [tool.poetry.dependencies]
 python = "^3.9"
 bcrypt = "^4.1.1"
 email-validator = "^2.1.0"
 httpx = {extras = ["http2"], version = "^0.26.0"}
 requests = "^2.31.0"
 Markdown = "^3.5.2"
-spacestar = "^0.3.0"
+spacestar = "^0.3.1"
 hx-markup = "^0.2.2"
 
 [tool.poetry.dev-dependencies]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `detadoc-0.2.6/setup.py` & `detadoc-0.2.7/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,19 +10,19 @@
 install_requires = \
 ['Markdown>=3.5.2,<4.0.0',
  'bcrypt>=4.1.1,<5.0.0',
  'email-validator>=2.1.0,<3.0.0',
  'httpx[http2]>=0.26.0,<0.27.0',
  'hx-markup>=0.2.2,<0.3.0',
  'requests>=2.31.0,<3.0.0',
- 'spacestar>=0.3.0,<0.4.0']
+ 'spacestar>=0.3.1,<0.4.0']
 
 setup_kwargs = {
     'name': 'detadoc',
-    'version': '0.2.6',
+    'version': '0.2.7',
     'description': '',
     'long_description': None,
     'author': 'Daniel Arantes',
     'author_email': 'arantesdv@me.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `detadoc-0.2.6/PKG-INFO` & `detadoc-0.2.7/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: detadoc
-Version: 0.2.6
+Version: 0.2.7
 Summary: 
 Author: Daniel Arantes
 Author-email: arantesdv@me.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: Markdown (>=3.5.2,<4.0.0)
 Requires-Dist: bcrypt (>=4.1.1,<5.0.0)
 Requires-Dist: email-validator (>=2.1.0,<3.0.0)
 Requires-Dist: httpx[http2] (>=0.26.0,<0.27.0)
 Requires-Dist: hx-markup (>=0.2.2,<0.3.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
-Requires-Dist: spacestar (>=0.3.0,<0.4.0)
+Requires-Dist: spacestar (>=0.3.1,<0.4.0)
```

