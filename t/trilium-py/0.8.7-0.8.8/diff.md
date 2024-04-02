# Comparing `tmp/trilium_py-0.8.7-py3-none-any.whl.zip` & `tmp/trilium_py-0.8.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 33811 bytes, number of entries: 14
+Zip file size: 33876 bytes, number of entries: 14
 -rw-r--r--  2.0 unx      141 b- defN 23-Aug-25 07:17 trilium_py/__init__.py
--rw-r--r--  2.0 unx    42977 b- defN 24-Feb-20 03:04 trilium_py/client.py
+-rw-r--r--  2.0 unx    43377 b- defN 24-Apr-02 02:04 trilium_py/client.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Aug-25 07:17 trilium_py/utils/__init__.py
 -rw-r--r--  2.0 unx     2301 b- defN 23-Aug-25 07:17 trilium_py/utils/html_util.py
 -rw-r--r--  2.0 unx     9328 b- defN 23-Aug-25 07:17 trilium_py/utils/markdown_math.py
 -rw-r--r--  2.0 unx     3923 b- defN 23-Aug-25 07:17 trilium_py/utils/note_util.py
 -rw-r--r--  2.0 unx      681 b- defN 23-Aug-25 07:17 trilium_py/utils/param_util.py
 -rw-r--r--  2.0 unx      208 b- defN 23-Aug-25 07:17 trilium_py/utils/time_util.py
 -rw-r--r--  2.0 unx      486 b- defN 23-Aug-25 07:17 trilium_py/utils/url_util.py
--rwxrwx---  2.0 unx    35184 b- defN 24-Feb-20 03:16 trilium_py-0.8.7.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx    15151 b- defN 24-Feb-20 03:16 trilium_py-0.8.7.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Feb-20 03:16 trilium_py-0.8.7.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 24-Feb-20 03:16 trilium_py-0.8.7.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1162 b- defN 24-Feb-20 03:16 trilium_py-0.8.7.dist-info/RECORD
-14 files, 111645 bytes uncompressed, 31873 bytes compressed:  71.5%
+-rwxrwx---  2.0 unx    35184 b- defN 24-Apr-02 03:07 trilium_py-0.8.8.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx    15197 b- defN 24-Apr-02 03:07 trilium_py-0.8.8.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-02 03:07 trilium_py-0.8.8.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 24-Apr-02 03:07 trilium_py-0.8.8.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1162 b- defN 24-Apr-02 03:07 trilium_py-0.8.8.dist-info/RECORD
+14 files, 112091 bytes uncompressed, 31938 bytes compressed:  71.5%
```

## zipnote {}

```diff
@@ -21,23 +21,23 @@
 
 Filename: trilium_py/utils/time_util.py
 Comment: 
 
 Filename: trilium_py/utils/url_util.py
 Comment: 
 
-Filename: trilium_py-0.8.7.dist-info/LICENSE.txt
+Filename: trilium_py-0.8.8.dist-info/LICENSE.txt
 Comment: 
 
-Filename: trilium_py-0.8.7.dist-info/METADATA
+Filename: trilium_py-0.8.8.dist-info/METADATA
 Comment: 
 
-Filename: trilium_py-0.8.7.dist-info/WHEEL
+Filename: trilium_py-0.8.8.dist-info/WHEEL
 Comment: 
 
-Filename: trilium_py-0.8.7.dist-info/top_level.txt
+Filename: trilium_py-0.8.8.dist-info/top_level.txt
 Comment: 
 
-Filename: trilium_py-0.8.7.dist-info/RECORD
+Filename: trilium_py-0.8.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## trilium_py/client.py

```diff
@@ -551,14 +551,20 @@
         url = f'{self.server_url}/etapi/calendar/days/{date}'
         res = requests.get(url, headers=self.get_header())
         noteId = res.json()['noteId']
         content = self.get_note_content(noteId)
         return content
 
     def set_day_note(self, date, content):
+        """
+        set note content by date
+        :param date: date string in format of "%Y-%m-%d", e.g. "2022-02-25"
+        :param content: note content
+        :return:
+        """
         url = f'{self.server_url}/etapi/calendar/days/{date}'
         res = requests.get(url, headers=self.get_header())
         noteId = res.json()['noteId']
         return self.update_note_content(noteId, content)
 
     def get_todo(self) -> list[list[Union[bool, str]]]:
         """get today's todo list.
@@ -615,25 +621,30 @@
         """uncheck a todo item by index.
 
         :param todo_index: index starts from 0
         :return: True if success, False if failed
         """
         return self.todo_check(todo_index, check=False)
 
-    def add_todo(self, todo_description: str, todo_caption: str = r'<p>TODO:</p>') -> bool:
+    def add_todo(
+        self, todo_description: str, todo_caption: str = r'<p>TODO:</p>', date: str = None
+    ) -> bool:
         """append item to todo list.
 
         :param todo_description: todo item
         :param todo_caption: caption added to new todo lists, default to '<p>TODO:</p>'
+        :param date: date string in format of "%Y-%m-%d", e.g. "2022-02-25"
         :return: True if success, False if failed
         """
         todo_description = todo_description.strip()
         soup: Optional[BeautifulSoup] = None
         try:
-            content = self.get_today_note_content()
+            if not date:
+                date = get_today()
+            content = self.get_day_note(date)
             soup = BeautifulSoup(content, 'html.parser')
             todo_labels = soup.find_all("label", {"class": "todo-list__label"})
             # append todo item after last todo item
             # special case 1: no todo available, add it to the beginning of document
             # special case 2: if last todo item is empty, update it
 
             if "todo-list__label" in todo_description:
@@ -656,16 +667,15 @@
                     empty_li.replace_with(todo_item)
                 else:
                     # if todo item list exists, append to the end
                     todo_item = BeautifulSoup(todo_item_html, 'html.parser')
                     todo_list_label = soup.find_all("ul", {"class": "todo-list"})[0]
                     todo_list_label.append(todo_item)
             new_content = str(soup)
-
-            return self.set_today_note_content(new_content)
+            return self.set_day_note(date, new_content)
         except Exception as e:
             logger.info(e)
             return False
         finally:
             # free mem
             if soup:
                 soup.decompose()
@@ -830,15 +840,16 @@
                             lambda x: x.replace("<", " \lt ").replace(">", " \gt "), latex_code_part
                         )
                     ),
                 )
         note_id = ''
 
         # detect images
-        pat = '<img (.*?)/>'
+        # https://github.com/Nriver/trilium-py/issues/36
+        pat = '<img (.*?)>'
         images = re.findall(pat, html)
 
         res = self.create_note(
             parentNoteId=parentNoteId,
             title=md_name,
             type="text",
             content=html,
```

## Comparing `trilium_py-0.8.7.dist-info/LICENSE.txt` & `trilium_py-0.8.8.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `trilium_py-0.8.7.dist-info/METADATA` & `trilium_py-0.8.8.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trilium-py
-Version: 0.8.7
+Version: 0.8.8
 Summary: Python client for ETAPI of Trilium Note. With some extra features powered by Python :)
 Home-page: https://github.com/nriver/trilium-py
 Author: Nriver
 Author-email: 
 Project-URL: Bug Reports, https://github.com/nriver/trilium-py/issues
 Project-URL: Funding, https://github.com/nriver/trilium-py
 Project-URL: Say Thanks!, https://github.com/nriver/trilium-py
@@ -156,15 +156,15 @@
 
 for x in res['results']:
     print(x['noteId'], x['title'])
 ```
 
 Search with regular expression. For example, search and get all child notes under certain note:
 
-```
+```python
 res = ea.search_note(
     # regular expression search for note title
     search="note.title %= '.*'",
     ancestorNoteId="Parent Note ID",
     fastSearch=False,
     limit=1000,
 )
@@ -277,15 +277,15 @@
 ```python
 res = ea.backup("test")
 ```
 
 You can use the cron utility in Linux to schedule regular automatic backups. For example, to set up a daily backup at 3:
 00 AM, you would use the following cron expression:
 
-```
+```bash
 0 3 * * * python /path/to/backup-script.py
 ```
 
 ### 🏷 Create attribute
 
 You can create a tag for a note
 
@@ -303,51 +303,51 @@
 noteId = res['note']['noteId']
 ```
 
 ### Get attachment info
 
 Get image title and etc.
 
-```
+```python
 res = ea.get_attachment('Y5V6pYq6nwXo')
 ```
 
 ### Update attachment info
 
 Change image title and etc.
 
-```
+```python
 res = ea.update_attachment(
     attachmentId='2b7pPzqocS1s', title='hello etapi', role='image', mime='image/png'
 )
 ```
 
 ### Get attachment content
 
 Get the real image file
 
-```
+```python
 res = ea.get_attachment_content('icpDE4orQxlI')
 with open('1.png', 'wb') as f:
     f.write(res)
 ```
 
 ### Update attachment content
 
 Replace the image with new one
 
-```
+```python
 res = ea.update_attachment_content('icWqV6zFtE0V', '/home/nate/data/1.png')
 ```
 
 ### Create attachment
 
 Upload a image file as attachment of a note.
 
-```
+```python
 res = ea.create_attachment(
     ownerId='8m8luXym5LxT',
     file_path='/home/nate/data/ksnip_20230630-103509.png',
 )
 ```
 
 ## (Advanced Usage) ✅ TODO List
@@ -536,15 +536,15 @@
 
 Sort a note by the heading names. This feature could prove invaluable for notes containing extensive lists, such as book
 titles sorted into various genres. It's equally useful for managing browser bookmarks or collecting links.
 
 Additionally, you have the option to specify a language code for sorting based on your local language. This enhances the
 sorting process and tailors it to your linguistic preferences.
 
-```
+```python
 res = ea.sort_note_content('lPxtkknjR2bJ')
 res = ea.sort_note_content('y6hROhWjNmHQ', 'zh_CN.UTF-8')
 ```
 
 ## 🛠️ Develop
 
 Install with pip egg link to make package change without reinstall.
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: trilium-py Version: 0.8.7 Summary: Python client
+Metadata-Version: 2.1 Name: trilium-py Version: 0.8.8 Summary: Python client
 for ETAPI of Trilium Note. With some extra features powered by Python :) Home-
 page: https://github.com/nriver/trilium-py Author: Nriver Author-email:
 Project-URL: Bug Reports, https://github.com/nriver/trilium-py/issues Project-
 URL: Funding, https://github.com/nriver/trilium-py Project-URL: Say Thanks!,
 https://github.com/nriver/trilium-py Project-URL: Source, https://github.com/
 nriver/trilium-py/ Keywords: trilium,etapi,api client Classifier: Development
 Status :: 5 - Production/Stable Classifier: Intended Audience :: Developers
@@ -71,16 +71,16 @@
 initialization, you can use Trilium ETAPI with python now. The following are
 some examples. ### ð Application Information To start with, you can get the
 application information like this. ```python print(ea.app_info()) ``` It should
 give you the version of your server application and some extra information. ###
 ð Search note Search note with keyword. ```python res = ea.search_note
 ( search="python", ) for x in res['results']: print(x['noteId'], x['title'])
 ``` Search with regular expression. For example, search and get all child notes
-under certain note: ``` res = ea.search_note( # regular expression search for
-note title search="note.title %= '.*'", ancestorNoteId="Parent Note ID",
+under certain note: ```python res = ea.search_note( # regular expression search
+for note title search="note.title %= '.*'", ancestorNoteId="Parent Note ID",
 fastSearch=False, limit=1000, ) ``` ### ð­ Create Note You can create a
 simple note like this. ```python res = ea.create_note( parentNoteId="root",
 title="Simple note 1", type="text", content="Simple note example",
 noteId="note1" ) ``` The `noteId` is not mandatory, if not provided, Trilium
 will generate a random one. You can retrieve it in the return. ```python noteId
 = res['note']['noteId'] ``` #### ð¼ï¸ Create Image note Image note is a
 special kind of note. You can create an image note with minimal information
@@ -99,65 +99,66 @@
 a (html) string. ```python ea.set_day_note(date, new_content) ``` ### ð¤
 Export note Export note comes in two formats `html` or `markdown`/`md`.
 ```python res = ea.export_note( noteId='sK5fn4T6yZRI', format='md', savePath='/
 home/nate/data/1/test.zip', ) ``` ### ð¾ Create data backup This example will
 create a database backup file like this `trilium-data/backup/backup-test.db`.
 ```python res = ea.backup("test") ``` You can use the cron utility in Linux to
 schedule regular automatic backups. For example, to set up a daily backup at 3:
-00 AM, you would use the following cron expression: ``` 0 3 * * * python /path/
-to/backup-script.py ``` ### ð· Create attribute You can create a tag for a
-note ```python res = ea.create_attribute( noteId='noteid', type='label',
+00 AM, you would use the following cron expression: ```bash 0 3 * * * python /
+path/to/backup-script.py ``` ### ð· Create attribute You can create a tag for
+a note ```python res = ea.create_attribute( noteId='noteid', type='label',
 name='name_of_the_tag', value='value_of_the_tag', isInheritable=True ) ``` The
 `noteId` is not mandatory, if not provided, Trilium will generate a random one.
 You can retrieve it in the return. ```python noteId = res['note']['noteId'] ```
-### Get attachment info Get image title and etc. ``` res = ea.get_attachment
-('Y5V6pYq6nwXo') ``` ### Update attachment info Change image title and etc. ```
-res = ea.update_attachment( attachmentId='2b7pPzqocS1s', title='hello etapi',
-role='image', mime='image/png' ) ``` ### Get attachment content Get the real
-image file ``` res = ea.get_attachment_content('icpDE4orQxlI') with open
-('1.png', 'wb') as f: f.write(res) ``` ### Update attachment content Replace
-the image with new one ``` res = ea.update_attachment_content('icWqV6zFtE0V',
-'/home/nate/data/1.png') ``` ### Create attachment Upload a image file as
-attachment of a note. ``` res = ea.create_attachment( ownerId='8m8luXym5LxT',
-file_path='/home/nate/data/ksnip_20230630-103509.png', ) ``` ## (Advanced
-Usage) â TODO List With the power of Python, I have expanded the basic usage
-of ETAPI. You can do something with todo list now. ### Add TODO item You can
-use `add_todo` to add a TODO item, param is the TODO description ```python
-ea.add_todo("ä¹°æå®å®") ``` ### Check/Uncheck a TODO item param is the
-index of the TODO item ```python ea.todo_check(0) ea.todo_uncheck(1) ``` ###
-Update a TODO item Use `update_todo` to update a TODO item description at
-certain index. ```python ea.update_todo(0, "å»ç å¤´æ´ç¹è¯æ¡") ``` ###
-Delete a TODO item Remove a TODO item by its index. ```python ea.delete_todo(1)
-``` ### Move yesterday's unfinished todo to today As the title suggests, you
-can move yesterday's unfinished things to today. Unfinished todo's will be
-deleted from yesterday's note. ```python
-ea.move_yesterday_unfinished_todo_to_today() ``` ## (Advanced Usage) ð
-Upload Markdown files ### Upload single Markdown file with images You can
-import Markdown file with images into Trilium now! Trilium-py will help you to
-upload the images and fix the links for you! ```python res = ea.upload_md_file
-( parentNoteId="root", file="./md-demo/manjaro ä¿®æ¹caps lock.md", ) ``` ###
-Bulk upload Markdown files in a folder You can upload a folder with lots of
-Markdown files to Trilium and preserve the folder structure! #### Import from
-VNote Say, upload all the notes from [VNote](https://github.com/vnotex/vnote),
-simply do this: ```python res = ea.upload_md_folder( parentNoteId="root",
-mdFolder="~/data/vnotebook/", ignoreFolder=['vx_notebook', 'vx_recycle_bin',
-'vx_images', '_v_images'], ) ``` #### Import from Joplin Joplin can be imported
-effortlessly. ```python res = ea.upload_md_folder( parentNoteId="root",
-mdFolder="/home/nate/data/joplin_data/", ignoreFolder=['_resources', ], ) ```
-#### Import from Logseq ```python res = ea.upload_md_folder
-( parentNoteId="root", mdFolder="/home/nate/data/logseq_data/", ignoreFolder=
-['assets', 'logseq'], ) ``` #### Import from Obsidian Obsidian has a very
-unique linking system for files. You should use [obsidian-export ](https://
-github.com/zoni/obsidian-export) to convert a Obsidian vault to regular
-Markdown files. Then you should be able to import the note into Trilium with
-trilium-py. Convert it first. ```bash obsidian-export /path/to/your/vault /out
-``` Then import just like a normal markdown, trilium-py will handle the images
-for you. ```python res = ea.upload_md_folder( parentNoteId="root", mdFolder="E:
-/data/out", ) ``` #### Import from Youdao Note/æéäºç¬è®° Youdao does not
-provide an export feature anymore. Luckily, you can use
+### Get attachment info Get image title and etc. ```python res =
+ea.get_attachment('Y5V6pYq6nwXo') ``` ### Update attachment info Change image
+title and etc. ```python res = ea.update_attachment
+( attachmentId='2b7pPzqocS1s', title='hello etapi', role='image', mime='image/
+png' ) ``` ### Get attachment content Get the real image file ```python res =
+ea.get_attachment_content('icpDE4orQxlI') with open('1.png', 'wb') as f:
+f.write(res) ``` ### Update attachment content Replace the image with new one
+```python res = ea.update_attachment_content('icWqV6zFtE0V', '/home/nate/data/
+1.png') ``` ### Create attachment Upload a image file as attachment of a note.
+```python res = ea.create_attachment( ownerId='8m8luXym5LxT', file_path='/home/
+nate/data/ksnip_20230630-103509.png', ) ``` ## (Advanced Usage) â TODO List
+With the power of Python, I have expanded the basic usage of ETAPI. You can do
+something with todo list now. ### Add TODO item You can use `add_todo` to add a
+TODO item, param is the TODO description ```python ea.add_todo("ä¹°æå®å®")
+``` ### Check/Uncheck a TODO item param is the index of the TODO item ```python
+ea.todo_check(0) ea.todo_uncheck(1) ``` ### Update a TODO item Use
+`update_todo` to update a TODO item description at certain index. ```python
+ea.update_todo(0, "å»ç å¤´æ´ç¹è¯æ¡") ``` ### Delete a TODO item Remove a
+TODO item by its index. ```python ea.delete_todo(1) ``` ### Move yesterday's
+unfinished todo to today As the title suggests, you can move yesterday's
+unfinished things to today. Unfinished todo's will be deleted from yesterday's
+note. ```python ea.move_yesterday_unfinished_todo_to_today() ``` ## (Advanced
+Usage) ð Upload Markdown files ### Upload single Markdown file with images
+You can import Markdown file with images into Trilium now! Trilium-py will help
+you to upload the images and fix the links for you! ```python res =
+ea.upload_md_file( parentNoteId="root", file="./md-demo/manjaro ä¿®æ¹caps
+lock.md", ) ``` ### Bulk upload Markdown files in a folder You can upload a
+folder with lots of Markdown files to Trilium and preserve the folder
+structure! #### Import from VNote Say, upload all the notes from [VNote](https:
+//github.com/vnotex/vnote), simply do this: ```python res = ea.upload_md_folder
+( parentNoteId="root", mdFolder="~/data/vnotebook/", ignoreFolder=
+['vx_notebook', 'vx_recycle_bin', 'vx_images', '_v_images'], ) ``` #### Import
+from Joplin Joplin can be imported effortlessly. ```python res =
+ea.upload_md_folder( parentNoteId="root", mdFolder="/home/nate/data/
+joplin_data/", ignoreFolder=['_resources', ], ) ``` #### Import from Logseq
+```python res = ea.upload_md_folder( parentNoteId="root", mdFolder="/home/nate/
+data/logseq_data/", ignoreFolder=['assets', 'logseq'], ) ``` #### Import from
+Obsidian Obsidian has a very unique linking system for files. You should use
+[obsidian-export ](https://github.com/zoni/obsidian-export) to convert a
+Obsidian vault to regular Markdown files. Then you should be able to import the
+note into Trilium with trilium-py. Convert it first. ```bash obsidian-export /
+path/to/your/vault /out ``` Then import just like a normal markdown, trilium-py
+will handle the images for you. ```python res = ea.upload_md_folder
+( parentNoteId="root", mdFolder="E:/data/out", ) ``` #### Import from Youdao
+Note/æéäºç¬è®° Youdao does not provide an export feature anymore.
+Luckily, you can use
 github.com/DeppWang/youdaonote-pull> to download your notes and convert them
 into markdown files. After that, trilium-py should be able to help you import
 them. ```python res = ea.upload_md_folder( parentNoteId="root", mdFolder="/
 home/nate/gitRepo/youdaonote-pull/out/", ) ``` #### Import from Turtl You need
 to convert Turtl from json to markdown first. See [turtl-to-markdown](https://
 github.com/Nriver/trilium-py/tree/main/examples/turtl-to-markdown) for details.
 Then you can import with trilium-py like this: ```python res =
@@ -178,14 +179,14 @@
 Beautify a note and its child notes ```python ea.beautify_sub_notes
 ('tlPuzU2szLJh') ``` ## (Advanced Usage) ð§¹ Sort note content Sort a note by
 the heading names. This feature could prove invaluable for notes containing
 extensive lists, such as book titles sorted into various genres. It's equally
 useful for managing browser bookmarks or collecting links. Additionally, you
 have the option to specify a language code for sorting based on your local
 language. This enhances the sorting process and tailors it to your linguistic
-preferences. ``` res = ea.sort_note_content('lPxtkknjR2bJ') res =
+preferences. ```python res = ea.sort_note_content('lPxtkknjR2bJ') res =
 ea.sort_note_content('y6hROhWjNmHQ', 'zh_CN.UTF-8') ``` ## ð ï¸ Develop
 Install with pip egg link to make package change without reinstall. ```python
 python -m pip install --user -e . ``` ## ð Original OpenAPI Documentation
 The original OpenAPI document is [here](https://github.com/zadam/trilium/blob/
 master/src/etapi/etapi.openapi.yaml). You can open it with [swagger editor]
 (https://editor.swagger.io/).
```

## Comparing `trilium_py-0.8.7.dist-info/RECORD` & `trilium_py-0.8.8.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 trilium_py/__init__.py,sha256=uSMH49RW2MFU_LVKKKm6lt3xOBsDWo0cb8--nMcNlgY,141
-trilium_py/client.py,sha256=E_FyGJjDLLuojfRmNP16saEEl_4IbBnkDT-WWLuoG5o,42977
+trilium_py/client.py,sha256=g64hW5RRti0XM646N5IT9PG-1FwN6ZkmkPWYDSf8XlU,43377
 trilium_py/utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 trilium_py/utils/html_util.py,sha256=HWniQG6udrU6vcaJdCETA30DH_MSdLFDncUiooKYV7I,2301
 trilium_py/utils/markdown_math.py,sha256=sAiR_5YaCE_EOeQ4vZBjoc5t0Z1n_5EQ4JmJ1TAweCY,9328
 trilium_py/utils/note_util.py,sha256=tx2kD1g9X_jILntDKEoXzHPytRGxj85ebKO2D8Ef72M,3923
 trilium_py/utils/param_util.py,sha256=jlnKrCKBtaN1wfQgxDTvGmuMM0p7vk809vpaLgK0dXg,681
 trilium_py/utils/time_util.py,sha256=DIFQmCKZ_wL5lCdeTMJZAtFolZw_dic6NKZ8CCJTa1A,208
 trilium_py/utils/url_util.py,sha256=1eHmHlti4CwsN-hjqfennxiohkrUX0jtuX3UleTD120,486
-trilium_py-0.8.7.dist-info/LICENSE.txt,sha256=bx5iLIKjgAdYQ7sISn7DsfHRKkoCUm1154sJJKhgqnU,35184
-trilium_py-0.8.7.dist-info/METADATA,sha256=3KIHD9MYw1mvDG_wzxGlvAFdJly4z6JSC8HIsk_fl6I,15151
-trilium_py-0.8.7.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
-trilium_py-0.8.7.dist-info/top_level.txt,sha256=nm0WM9tsACU6iD5bbVQgo-LgS3xkDUFPK87VYZfaToo,11
-trilium_py-0.8.7.dist-info/RECORD,,
+trilium_py-0.8.8.dist-info/LICENSE.txt,sha256=bx5iLIKjgAdYQ7sISn7DsfHRKkoCUm1154sJJKhgqnU,35184
+trilium_py-0.8.8.dist-info/METADATA,sha256=hh4RsCfmsx8ep81mGQKXj-Rd2-n3wCavLFpmUAsJ54A,15197
+trilium_py-0.8.8.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+trilium_py-0.8.8.dist-info/top_level.txt,sha256=nm0WM9tsACU6iD5bbVQgo-LgS3xkDUFPK87VYZfaToo,11
+trilium_py-0.8.8.dist-info/RECORD,,
```

