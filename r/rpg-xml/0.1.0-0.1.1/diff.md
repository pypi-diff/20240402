# Comparing `tmp/rpg_xml-0.1.0-py3-none-any.whl.zip` & `tmp/rpg_xml-0.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 9043 bytes, number of entries: 15
+Zip file size: 9107 bytes, number of entries: 15
 -rw-------  2.0 unx      134 b- defN 24-Mar-31 17:07 rpg_xml/__init__.py
--rw-------  2.0 unx     1332 b- defN 24-Mar-31 17:16 rpg_xml/engine.py
+-rw-------  2.0 unx     1270 b- defN 24-Apr-02 00:35 rpg_xml/engine.py
 -rw-------  2.0 unx     1116 b- defN 24-Mar-31 17:02 rpg_xml/music_controller.py
 -rw-------  2.0 unx     1174 b- defN 24-Mar-31 09:48 rpg_xml/music_player.py
--rw-------  2.0 unx     2069 b- defN 24-Mar-31 17:16 rpg_xml/scene_controller.py
+-rw-------  2.0 unx     2218 b- defN 24-Apr-01 02:31 rpg_xml/scene_controller.py
 -rw-------  2.0 unx     2068 b- defN 24-Mar-31 17:07 rpg_xml/scene_processor.py
 -rw-------  2.0 unx     2313 b- defN 24-Mar-31 16:23 rpg_xml/scene_processor_old.py
--rw-------  2.0 unx     2287 b- defN 24-Mar-31 07:09 rpg_xml/util.py
+-rw-------  2.0 unx     2662 b- defN 24-Apr-02 00:35 rpg_xml/util.py
 -rw-------  2.0 unx     2857 b- defN 24-Mar-31 06:37 rpg_xml/util_old.py
 -rw-------  2.0 unx     1007 b- defN 24-Mar-31 17:17 rpg_xml/xmlparser.py
--rw-------  2.0 unx     1070 b- defN 24-Mar-31 18:12 rpg_xml-0.1.0.dist-info/LICENSE
--rw-------  2.0 unx      135 b- defN 24-Mar-31 18:12 rpg_xml-0.1.0.dist-info/METADATA
--rw-------  2.0 unx       92 b- defN 24-Mar-31 18:12 rpg_xml-0.1.0.dist-info/WHEEL
--rw-------  2.0 unx        8 b- defN 24-Mar-31 18:12 rpg_xml-0.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1176 b- defN 24-Mar-31 18:12 rpg_xml-0.1.0.dist-info/RECORD
-15 files, 18838 bytes uncompressed, 7117 bytes compressed:  62.2%
+-rw-------  2.0 unx     1070 b- defN 24-Apr-02 00:51 rpg_xml-0.1.1.dist-info/LICENSE
+-rw-------  2.0 unx      135 b- defN 24-Apr-02 00:51 rpg_xml-0.1.1.dist-info/METADATA
+-rw-------  2.0 unx       92 b- defN 24-Apr-02 00:51 rpg_xml-0.1.1.dist-info/WHEEL
+-rw-------  2.0 unx        8 b- defN 24-Apr-02 00:51 rpg_xml-0.1.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1176 b- defN 24-Apr-02 00:51 rpg_xml-0.1.1.dist-info/RECORD
+15 files, 19300 bytes uncompressed, 7181 bytes compressed:  62.8%
```

## zipnote {}

```diff
@@ -24,23 +24,23 @@
 
 Filename: rpg_xml/util_old.py
 Comment: 
 
 Filename: rpg_xml/xmlparser.py
 Comment: 
 
-Filename: rpg_xml-0.1.0.dist-info/LICENSE
+Filename: rpg_xml-0.1.1.dist-info/LICENSE
 Comment: 
 
-Filename: rpg_xml-0.1.0.dist-info/METADATA
+Filename: rpg_xml-0.1.1.dist-info/METADATA
 Comment: 
 
-Filename: rpg_xml-0.1.0.dist-info/WHEEL
+Filename: rpg_xml-0.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: rpg_xml-0.1.0.dist-info/top_level.txt
+Filename: rpg_xml-0.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: rpg_xml-0.1.0.dist-info/RECORD
+Filename: rpg_xml-0.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## rpg_xml/engine.py

```diff
@@ -3,35 +3,33 @@
 from .scene_controller import SceneController
 
 
 class Engine:
     def __init__(self, path) -> None:
         self.parser = XmlParser(path)
         self.ui = TerminalUI()
-        self.scene_processor = SceneController(self.ui, self.parser)
+        self.scene_controller = SceneController(self.ui, self.parser)
         self.scenes = self.parser.get_nodes("scene")
         self.current_scene_index = 0
 
     def start_game(self):
         self.ui.clear_screen()
         self.process_scene(self.current_scene_index)
-        self.ui.run_forever()
 
     def process_scene(self, scene_index):
         scene = self.scenes[scene_index]
-        next_scene_id = self.scene_processor.process(scene)
+        next_scene_id = self.scene_controller.process(scene)
         if next_scene_id is not None:
             next_scene_index = self.get_scene_index_by_id(next_scene_id)
             if next_scene_index is not None:
                 self.current_scene_index = next_scene_index
                 self.process_scene(self.current_scene_index)
             else:
                 self.ui.type_message("Cena não encontrada", color="red")
         else:
-            self.ui.type_message("Fim do jogo", color="red")
-            self.ui.close()
+            self.ui.run_forever(self.scene_controller)
 
     def get_scene_index_by_id(self, scene_id):
         for i, scene in enumerate(self.scenes):
             if scene.get("id") == scene_id:
                 return i
         return None
```

## rpg_xml/scene_controller.py

```diff
@@ -9,32 +9,39 @@
         self.parser = parser
         self.music_controller = MusicController()
 
     def process(self, scene):
         self._proc_messages(scene)
         return self._proc_option(scene)
 
+    def stop_music(self):
+        self.music_controller.stop_music()
+
     def _proc_messages(self, scene):
         for item in scene:
             if item.tag == "music":
                 if item.get("play"):
                     self.music_controller.play_music(item.get("play"))
                 elif item.get("stop"):
                     self.music_controller.stop_music()
+
             elif item.tag == "msg":
                 attrs_found = self._get_attr(item, msg_attr)
                 wrap_line = attrs_found.get("wrap-line", "True").lower() == "true"
                 self.ui.type_message(
                     item.text,
                     delay_before=int(attrs_found.get("delay-before", 100)),
                     wrap_line=wrap_line,
                     type_vel=int(attrs_found.get("type-vel", 50)),
                     color=attrs_found.get("color", "default"),
                 )
 
+            elif item.tag == "clear":
+                self.ui.clear_screen()
+
     def _proc_option(self, scene):
         option = scene.find("option")
         if option is None:
             return None
 
         queries = option.findall("query")
         if not queries:
```

## rpg_xml/util.py

```diff
@@ -36,42 +36,53 @@
 
         if wrap_line:
             print(f"{self.COLORS['default']}")  # Retorna ao estilo de texto padrão
 
     def render_menu(self, menu_items):
         while True:
             for i, item in enumerate(menu_items):
-                self.type_message(f"{i+1}. ", color="green", wrap_line=False)
-                self.type_message(f"{item}")
-
-            self.type_message("Escolha um número: ", color="cyan", wrap_line=False)
+                self.type_message(
+                    f"{i+1}. ", color="green", wrap_line=False, type_vel=5
+                )
+                self.type_message(f"{item}", type_vel=5)
+
+            self.type_message(
+                "Escolha um número:", color="cyan", wrap_line=False, type_vel=5
+            )
+            self.type_message(" ", wrap_line=False)
 
             try:
                 user_choice = int(input())
                 if 1 <= user_choice <= len(menu_items):
                     return menu_items[user_choice - 1]
                 else:
-                    print("Opção inválida. Tente novamente.")
+                    self.type_message(
+                        "Opção inválida. Tente novamente.", color="red", type_vel=5
+                    )
             except ValueError:
-                print("Entrada inválida. Digite um número válido.")
+                self.type_message(
+                    "Entrada inválida. Digite um número válido.",
+                    color="red",
+                    type_vel=5,
+                )
 
-    def run_forever(self):
+    def run_forever(self, scene):
         while self.running:
             try:
                 # Atualização contínua da tela
                 time.sleep(1)
             except KeyboardInterrupt:
+                scene.stop_music()
                 self.close()
 
     def close(self):
         self.running = False
         sys.exit()  # Sai do programa
 
 
 # Exemplo de uso
 if __name__ == "__main__":
     ui = TerminalUI()
     ui.type_message("Hello world!", color="green")
     lost = ["Kaic", "Salomao"]
     selected = ui.render_menu(lost)
     ui.type_message(selected, color="blue")
-    ui.run_forever()
```

## Comparing `rpg_xml-0.1.0.dist-info/LICENSE` & `rpg_xml-0.1.1.dist-info/LICENSE`

 * *Files identical despite different names*

