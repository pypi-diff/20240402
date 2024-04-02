# Comparing `tmp/BMPboot-3.3.tar.gz` & `tmp/BMPboot-3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BMPboot-3.3.tar", last modified: Tue Apr  2 15:56:35 2024, max compression
+gzip compressed data, was "BMPboot-3.4.tar", last modified: Tue Apr  2 16:58:43 2024, max compression
```

## Comparing `BMPboot-3.3.tar` & `BMPboot-3.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-02 15:56:35.527268 BMPboot-3.3/
-drwxrwxrwx   0        0        0        0 2024-04-02 15:56:35.510268 BMPboot-3.3/BMPboot/
--rw-rw-rw-   0        0        0       96 2024-04-02 10:53:12.000000 BMPboot-3.3/BMPboot/__init__.py
--rw-rw-rw-   0        0        0     2184 2024-04-02 10:53:12.000000 BMPboot-3.3/BMPboot/address_book.py
--rw-rw-rw-   0        0        0    18251 2024-04-02 10:53:12.000000 BMPboot-3.3/BMPboot/main.py
-drwxrwxrwx   0        0        0        0 2024-04-02 15:56:35.524268 BMPboot-3.3/BMPboot.egg-info/
--rw-rw-rw-   0        0        0      309 2024-04-02 15:56:35.000000 BMPboot-3.3/BMPboot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      275 2024-04-02 15:56:35.000000 BMPboot-3.3/BMPboot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-02 15:56:35.000000 BMPboot-3.3/BMPboot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2024-04-02 15:56:35.000000 BMPboot-3.3/BMPboot.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        8 2024-04-02 15:56:35.000000 BMPboot-3.3/BMPboot.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2024-04-02 15:56:35.000000 BMPboot-3.3/BMPboot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      309 2024-04-02 15:56:35.525269 BMPboot-3.3/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-04-02 15:56:35.527268 BMPboot-3.3/setup.cfg
--rw-rw-rw-   0        0        0      746 2024-04-02 15:56:32.000000 BMPboot-3.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-02 15:56:35.521268 BMPboot-3.3/test/
--rw-rw-rw-   0        0        0      201 2024-04-02 10:53:12.000000 BMPboot-3.3/test/testowanie.py
+drwxrwxrwx   0        0        0        0 2024-04-02 16:58:43.018157 BMPboot-3.4/
+drwxrwxrwx   0        0        0        0 2024-04-02 16:58:42.997158 BMPboot-3.4/BMPboot/
+-rw-rw-rw-   0        0        0       96 2024-04-02 10:53:12.000000 BMPboot-3.4/BMPboot/__init__.py
+-rw-rw-rw-   0        0        0     2184 2024-04-02 10:53:12.000000 BMPboot-3.4/BMPboot/address_book.py
+-rw-rw-rw-   0        0        0    18589 2024-04-02 16:57:24.000000 BMPboot-3.4/BMPboot/main.py
+drwxrwxrwx   0        0        0        0 2024-04-02 16:58:43.014160 BMPboot-3.4/BMPboot.egg-info/
+-rw-rw-rw-   0        0        0      309 2024-04-02 16:58:42.000000 BMPboot-3.4/BMPboot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      275 2024-04-02 16:58:42.000000 BMPboot-3.4/BMPboot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 16:58:42.000000 BMPboot-3.4/BMPboot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2024-04-02 16:58:42.000000 BMPboot-3.4/BMPboot.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        8 2024-04-02 16:58:42.000000 BMPboot-3.4/BMPboot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2024-04-02 16:58:42.000000 BMPboot-3.4/BMPboot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      309 2024-04-02 16:58:43.016157 BMPboot-3.4/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-04-02 16:58:43.018157 BMPboot-3.4/setup.cfg
+-rw-rw-rw-   0        0        0      746 2024-04-02 16:57:40.000000 BMPboot-3.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-02 16:58:43.011158 BMPboot-3.4/test/
+-rw-rw-rw-   0        0        0      201 2024-04-02 10:53:12.000000 BMPboot-3.4/test/testowanie.py
```

### Comparing `BMPboot-3.3/BMPboot/address_book.py` & `BMPboot-3.4/BMPboot/address_book.py`

 * *Files identical despite different names*

### Comparing `BMPboot-3.3/BMPboot/main.py` & `BMPboot-3.4/BMPboot/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -348,17 +348,22 @@
                     alphabetical = not alphabetical
 
         return "Done"
     
 
 def change_fields(user, contacts, option='remove'):
     while True:
+        note_text = ''
+        if len(contacts[user].notes) > 0:
+            note_text += '| 6: Note'
+
+            
         operation = input(f'What field do you want to {option}?\n'
         '0: Exit | 1: Name | 2: Address | 3: Phone | '
-        '4: Email | 5: Birthday | 6: Note\n')
+        f'4: Email | 5: Birthday {note_text}\n')
         
         if int(operation) in list(range(7)):
             break
         else:
             print('You have chosen wrong number!')
     
     operation_number = int(operation)
@@ -376,25 +381,28 @@
                 question = input(f'Provide a new value for the {fields[operation_number]}: ')
             
             if operation_number == 1:
                 setattr(contacts[user], fields[operation_number], dispatch_dict[fields[operation_number]](question))
                 break
             else:
                 func_name = 'add_' + fields[operation_number]
-                func = getattr(contacts[user], func_name)
 
                 try:
-                    func(question)
+                    if option == 'change':
+                        func = getattr(contacts[user], func_name)
+                        func(question)
+                    else:
+                        setattr(contacts[user], fields[operation_number], '')                  
                 except PhoneFormatException:
                     print('Number should contain 10 digits!')
                 except EmailFormatException:
                     print('Wrong email address format!')
                 else:
                     break 
-    elif operation == '6':
+    elif operation == '6' and len(contacts[user].notes) > 0:
         notes_dict = {}
         found_notes = contacts[user].notes
         note_text = ''
         count = len(found_notes)
 
         for count, key in enumerate(found_notes, 1):
             notes_dict[count] = key
```

### Comparing `BMPboot-3.3/setup.py` & `BMPboot-3.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # with open("README.md", "r", encoding="utf-8") as fh:
     #long_description = fh.read()
 long_description = "The Best of Boots: 'BMP' - an address book application"
 
 setup(
     name='BMPboot',
-    version='3.3',
+    version='3.4',
     install_requires=[
         'thefuzz',
     ],
     entry_points={
         'console_scripts': [
             'start = BMPboot.main:main',
         ],
```

