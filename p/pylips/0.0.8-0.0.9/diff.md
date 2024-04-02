# Comparing `tmp/pylips-0.0.8.tar.gz` & `tmp/pylips-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylips-0.0.8.tar", last modified: Mon Mar 25 17:29:24 2024, max compression
+gzip compressed data, was "pylips-0.0.9.tar", last modified: Wed Mar 27 07:37:55 2024, max compression
```

## Comparing `pylips-0.0.8.tar` & `pylips-0.0.9.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 ndennler   (501) staff       (20)        0 2024-03-25 17:29:24.713081 pylips-0.0.8/
--rw-r--r--   0 ndennler   (501) staff       (20)       49 2024-03-23 21:26:41.000000 pylips-0.0.8/HISTORY.md
--rw-r--r--   0 ndennler   (501) staff       (20)     1071 2024-03-08 22:56:44.000000 pylips-0.0.8/LICENSE
--rw-r--r--   0 ndennler   (501) staff       (20)      137 2024-03-25 04:15:56.000000 pylips-0.0.8/MANIFEST.in
--rw-r--r--   0 ndennler   (501) staff       (20)     3033 2024-03-25 17:29:24.713014 pylips-0.0.8/PKG-INFO
--rw-r--r--   0 ndennler   (501) staff       (20)       43 2024-03-22 03:23:03.000000 pylips-0.0.8/README.md
-drwxr-xr-x   0 ndennler   (501) staff       (20)        0 2024-03-25 17:29:24.703451 pylips-0.0.8/pylips/
--rw-r--r--   0 ndennler   (501) staff       (20)      217 2024-03-25 17:28:29.000000 pylips-0.0.8/pylips/__init__.py
-drwxr-xr-x   0 ndennler   (501) staff       (20)        0 2024-03-25 17:29:24.705052 pylips-0.0.8/pylips/face/
--rw-r--r--   0 ndennler   (501) staff       (20)        0 2024-03-22 03:40:37.000000 pylips-0.0.8/pylips/face/__init_.py
--rw-r--r--   0 ndennler   (501) staff       (20)      820 2024-03-24 04:52:37.000000 pylips-0.0.8/pylips/face/start.py
-drwxr-xr-x   0 ndennler   (501) staff       (20)        0 2024-03-25 17:29:24.701910 pylips-0.0.8/pylips/face/static/
-drwxr-xr-x   0 ndennler   (501) staff       (20)        0 2024-03-25 17:29:24.708362 pylips-0.0.8/pylips/face/static/js/
--rw-r--r--   0 ndennler   (501) staff       (20)    57342 2024-03-15 18:52:37.000000 pylips-0.0.8/pylips/face/static/js/dat.gui.min.js
--rw-r--r--   0 ndennler   (501) staff       (20)    10345 2024-03-15 19:00:12.000000 pylips-0.0.8/pylips/face/static/js/facecontrol.js
--rw-r--r--   0 ndennler   (501) staff       (20)    40915 2024-03-09 20:14:40.000000 pylips-0.0.8/pylips/face/static/js/socketio.min.js
--rw-r--r--   0 ndennler   (501) staff       (20)    35344 2024-03-24 18:28:00.000000 pylips-0.0.8/pylips/face/static/js/svgFace.js
--rw-r--r--   0 ndennler   (501) staff       (20)     5797 2024-03-09 20:44:38.000000 pylips-0.0.8/pylips/face/static/js/tween.min.js
--rw-r--r--   0 ndennler   (501) staff       (20)   122410 2024-03-09 20:42:45.000000 pylips-0.0.8/pylips/face/static/js/two.min.js
-drwxr-xr-x   0 ndennler   (501) staff       (20)        0 2024-03-25 17:29:24.709515 pylips-0.0.8/pylips/face/templates/
--rw-r--r--   0 ndennler   (501) staff       (20)     1370 2024-03-25 03:22:23.000000 pylips-0.0.8/pylips/face/templates/editor.html
--rw-r--r--   0 ndennler   (501) staff       (20)     5506 2024-03-24 18:29:19.000000 pylips-0.0.8/pylips/face/templates/index.html
-drwxr-xr-x   0 ndennler   (501) staff       (20)        0 2024-03-25 17:29:24.711105 pylips-0.0.8/pylips/speech/
--rw-r--r--   0 ndennler   (501) staff       (20)      203 2024-03-25 03:38:18.000000 pylips-0.0.8/pylips/speech/__init__.py
--rw-r--r--   0 ndennler   (501) staff       (20)      408 2024-03-25 02:08:29.000000 pylips-0.0.8/pylips/speech/client.py
--rw-r--r--   0 ndennler   (501) staff       (20)     3418 2024-03-25 01:21:35.000000 pylips-0.0.8/pylips/speech/polly_tts.py
--rw-r--r--   0 ndennler   (501) staff       (20)     4505 2024-03-25 03:40:00.000000 pylips-0.0.8/pylips/speech/robot_face.py
--rw-r--r--   0 ndennler   (501) staff       (20)     4347 2024-03-25 17:27:59.000000 pylips-0.0.8/pylips/speech/system_tts.py
-drwxr-xr-x   0 ndennler   (501) staff       (20)        0 2024-03-25 17:29:24.711566 pylips-0.0.8/pylips.egg-info/
--rw-r--r--   0 ndennler   (501) staff       (20)     3033 2024-03-25 17:29:24.000000 pylips-0.0.8/pylips.egg-info/PKG-INFO
--rw-r--r--   0 ndennler   (501) staff       (20)      713 2024-03-25 17:29:24.000000 pylips-0.0.8/pylips.egg-info/SOURCES.txt
--rw-r--r--   0 ndennler   (501) staff       (20)        1 2024-03-25 17:29:24.000000 pylips-0.0.8/pylips.egg-info/dependency_links.txt
--rw-r--r--   0 ndennler   (501) staff       (20)        1 2024-03-23 21:58:25.000000 pylips-0.0.8/pylips.egg-info/not-zip-safe
--rw-r--r--   0 ndennler   (501) staff       (20)      793 2024-03-25 17:29:24.000000 pylips-0.0.8/pylips.egg-info/requires.txt
--rw-r--r--   0 ndennler   (501) staff       (20)        7 2024-03-25 17:29:24.000000 pylips-0.0.8/pylips.egg-info/top_level.txt
--rw-r--r--   0 ndennler   (501) staff       (20)      619 2024-03-25 17:29:24.713406 pylips-0.0.8/setup.cfg
--rw-r--r--   0 ndennler   (501) staff       (20)     2999 2024-03-25 17:28:17.000000 pylips-0.0.8/setup.py
+drwxr-xr-x   0 ndennler   (501) staff       (20)        0 2024-03-27 07:37:55.586602 pylips-0.0.9/
+-rw-r--r--   0 ndennler   (501) staff       (20)       49 2024-03-23 21:26:41.000000 pylips-0.0.9/HISTORY.md
+-rw-r--r--   0 ndennler   (501) staff       (20)     1071 2024-03-08 22:56:44.000000 pylips-0.0.9/LICENSE
+-rw-r--r--   0 ndennler   (501) staff       (20)      137 2024-03-25 04:15:56.000000 pylips-0.0.9/MANIFEST.in
+-rw-r--r--   0 ndennler   (501) staff       (20)     3067 2024-03-27 07:37:55.586516 pylips-0.0.9/PKG-INFO
+-rw-r--r--   0 ndennler   (501) staff       (20)       45 2024-03-27 06:41:21.000000 pylips-0.0.9/README.md
+drwxr-xr-x   0 ndennler   (501) staff       (20)        0 2024-03-27 07:37:55.576444 pylips-0.0.9/pylips/
+-rw-r--r--   0 ndennler   (501) staff       (20)      217 2024-03-27 07:37:49.000000 pylips-0.0.9/pylips/__init__.py
+drwxr-xr-x   0 ndennler   (501) staff       (20)        0 2024-03-27 07:37:55.577516 pylips-0.0.9/pylips/face/
+-rw-r--r--   0 ndennler   (501) staff       (20)        0 2024-03-22 03:40:37.000000 pylips-0.0.9/pylips/face/__init_.py
+-rw-r--r--   0 ndennler   (501) staff       (20)      820 2024-03-24 04:52:37.000000 pylips-0.0.9/pylips/face/start.py
+drwxr-xr-x   0 ndennler   (501) staff       (20)        0 2024-03-27 07:37:55.575193 pylips-0.0.9/pylips/face/static/
+drwxr-xr-x   0 ndennler   (501) staff       (20)        0 2024-03-27 07:37:55.581622 pylips-0.0.9/pylips/face/static/js/
+-rw-r--r--   0 ndennler   (501) staff       (20)    57342 2024-03-15 18:52:37.000000 pylips-0.0.9/pylips/face/static/js/dat.gui.min.js
+-rw-r--r--   0 ndennler   (501) staff       (20)    10345 2024-03-15 19:00:12.000000 pylips-0.0.9/pylips/face/static/js/facecontrol.js
+-rw-r--r--   0 ndennler   (501) staff       (20)    40915 2024-03-09 20:14:40.000000 pylips-0.0.9/pylips/face/static/js/socketio.min.js
+-rw-r--r--   0 ndennler   (501) staff       (20)    38182 2024-03-26 20:30:24.000000 pylips-0.0.9/pylips/face/static/js/svgFace.js
+-rw-r--r--   0 ndennler   (501) staff       (20)     5797 2024-03-09 20:44:38.000000 pylips-0.0.9/pylips/face/static/js/tween.min.js
+-rw-r--r--   0 ndennler   (501) staff       (20)   122410 2024-03-09 20:42:45.000000 pylips-0.0.9/pylips/face/static/js/two.min.js
+drwxr-xr-x   0 ndennler   (501) staff       (20)        0 2024-03-27 07:37:55.582891 pylips-0.0.9/pylips/face/templates/
+-rw-r--r--   0 ndennler   (501) staff       (20)     4102 2024-03-26 03:58:43.000000 pylips-0.0.9/pylips/face/templates/editor.html
+-rw-r--r--   0 ndennler   (501) staff       (20)     5506 2024-03-24 18:29:19.000000 pylips-0.0.9/pylips/face/templates/index.html
+drwxr-xr-x   0 ndennler   (501) staff       (20)        0 2024-03-27 07:37:55.584639 pylips-0.0.9/pylips/speech/
+-rw-r--r--   0 ndennler   (501) staff       (20)      203 2024-03-25 03:38:18.000000 pylips-0.0.9/pylips/speech/__init__.py
+-rw-r--r--   0 ndennler   (501) staff       (20)     1172 2024-03-26 21:40:56.000000 pylips-0.0.9/pylips/speech/client.py
+-rw-r--r--   0 ndennler   (501) staff       (20)     3418 2024-03-25 01:21:35.000000 pylips-0.0.9/pylips/speech/polly_tts.py
+-rw-r--r--   0 ndennler   (501) staff       (20)     4808 2024-03-27 07:35:27.000000 pylips-0.0.9/pylips/speech/robot_face.py
+-rw-r--r--   0 ndennler   (501) staff       (20)     4420 2024-03-27 07:30:21.000000 pylips-0.0.9/pylips/speech/system_tts.py
+drwxr-xr-x   0 ndennler   (501) staff       (20)        0 2024-03-27 07:37:55.585111 pylips-0.0.9/pylips.egg-info/
+-rw-r--r--   0 ndennler   (501) staff       (20)     3067 2024-03-27 07:37:55.000000 pylips-0.0.9/pylips.egg-info/PKG-INFO
+-rw-r--r--   0 ndennler   (501) staff       (20)      713 2024-03-27 07:37:55.000000 pylips-0.0.9/pylips.egg-info/SOURCES.txt
+-rw-r--r--   0 ndennler   (501) staff       (20)        1 2024-03-27 07:37:55.000000 pylips-0.0.9/pylips.egg-info/dependency_links.txt
+-rw-r--r--   0 ndennler   (501) staff       (20)        1 2024-03-23 21:58:25.000000 pylips-0.0.9/pylips.egg-info/not-zip-safe
+-rw-r--r--   0 ndennler   (501) staff       (20)      810 2024-03-27 07:37:55.000000 pylips-0.0.9/pylips.egg-info/requires.txt
+-rw-r--r--   0 ndennler   (501) staff       (20)        7 2024-03-27 07:37:55.000000 pylips-0.0.9/pylips.egg-info/top_level.txt
+-rw-r--r--   0 ndennler   (501) staff       (20)      619 2024-03-27 07:37:55.586943 pylips-0.0.9/setup.cfg
+-rw-r--r--   0 ndennler   (501) staff       (20)     3023 2024-03-27 07:37:16.000000 pylips-0.0.9/setup.py
```

### Comparing `pylips-0.0.8/LICENSE` & `pylips-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pylips-0.0.8/PKG-INFO` & `pylips-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylips
-Version: 0.0.8
+Version: 0.0.9
 Summary: An interface for embodied conversational interaction.
 Home-page: https://github.com/interaction-lab/PyLips
 Author: Interaction Lab
 Author-email: dennler@usc.edu
 License: MIT license
 Keywords: lips
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -25,14 +25,15 @@
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: flask>=2.0.1
 Requires-Dist: flask-socketio>=5.1.1
 Requires-Dist: python-socketio>=5.11.1
 Requires-Dist: websocket-client>=1.7.0
+Requires-Dist: requests>=2.31.0
 Requires-Dist: boto3>=1.18.67
 Requires-Dist: pygame>=2.1.1
 Requires-Dist: py3-tts>=3.5
 Requires-Dist: allosaurus>=1.0.2
 Requires-Dist: soundfile>=0.12.1
 Provides-Extra: dev
 Requires-Dist: pip>=20.3; extra == "dev"
@@ -65,12 +66,14 @@
 Requires-Dist: twine==4.0.2; extra == "dev"
 Requires-Dist: check-wheel-contents==0.4.0; extra == "dev"
 
 # PyLips
 Web-Enabled Facial Text-to-Speech
 
 
+
+
 # History
 
 ## 0.0.0 (2024-03-24)
 
 - pylips begins
```

### Comparing `pylips-0.0.8/pylips/face/start.py` & `pylips-0.0.9/pylips/face/start.py`

 * *Files identical despite different names*

### Comparing `pylips-0.0.8/pylips/face/static/js/dat.gui.min.js` & `pylips-0.0.9/pylips/face/static/js/dat.gui.min.js`

 * *Files identical despite different names*

### Comparing `pylips-0.0.8/pylips/face/static/js/facecontrol.js` & `pylips-0.0.9/pylips/face/static/js/facecontrol.js`

 * *Files identical despite different names*

### Comparing `pylips-0.0.8/pylips/face/static/js/socketio.min.js` & `pylips-0.0.9/pylips/face/static/js/socketio.min.js`

 * *Files identical despite different names*

### Comparing `pylips-0.0.8/pylips/face/static/js/svgFace.js` & `pylips-0.0.9/pylips/face/static/js/svgFace.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -927,14 +927,32 @@
     function makeBrowGroup(side) {
         var sign = side == 'left' ? 1 : -1
         var browCurve = two.makeCurve(sign * width, 0, sign * width / 8, -0.75 * thickness, -sign * width, thickness, true)
         browCurve.fill = 'None'
         browCurve.linewidth = thickness
         browCurve.stroke = color
         browCurve.cap = 'round'
+
+        // var keypoint_color = '#e8cd25'
+        // kp1 = two.makeCircle(sign*width,0, 30);
+        // kp1.fill = 'transparent'; // Set fill to transparent
+        // kp1.stroke = keypoint_color; // Set stroke color (you can change it to any color you prefer)
+        // kp1.linewidth = 10; 
+
+        // kp2 = two.makeCircle(sign*width/8,-0.75*thickness, 30);
+        // kp2.fill = 'transparent'; // Set fill to transparent
+        // kp2.stroke = keypoint_color; // Set stroke color (you can change it to any color you prefer)
+        // kp2.linewidth = 10; 
+
+        // kp3 = two.makeCircle(-sign*width, thickness, 30);
+        // kp3.fill = 'transparent'; // Set fill to transparent
+        // kp3.stroke = keypoint_color; // Set stroke color (you can change it to any color you prefer)
+        // kp3.linewidth = 10; 
+
+        // return two.makeGroup(browCurve, kp1,kp2,kp3)
         return two.makeGroup(browCurve)
     }
 
     function getIdleCoords(side) {
         var sign = side == 'left' ? 1 : -1
         return {
             x0: -sign * width,
@@ -951,24 +969,36 @@
         var goal = goal;
         var target = this.currentControlPoint;
         var tween = new TWEEN.Tween(target, {
             override: true
         }).to(goal, t);
         tween.easing(TWEEN.Easing.Quadratic.InOut);
         var browInfo = this.group.children[0]
+        // var kp1 = this.group.children[1]
+        // var kp2 = this.group.children[2]
+        // var kp3 = this.group.children[3]
         tween.onUpdate(function() {
 
             browInfo.vertices[0].x = this.x0
             browInfo.vertices[0].y = this.y0
 
             browInfo.vertices[1].x = this.x1
             browInfo.vertices[1].y = this.y1
 
             browInfo.vertices[2].x = this.x2
             browInfo.vertices[2].y = this.y2
+
+            // kp1.translation.x = this.x0
+            // kp1.translation.y = this.y0
+
+            // kp2.translation.x = this.x1
+            // kp2.translation.y = this.y1
+
+            // kp3.translation.x = this.x2
+            // kp3.translation.y = this.y2
         });
         tween.start();
     }
 
     var leye = getPart("leye");
     var reye = getPart("reye");
 
@@ -997,39 +1027,80 @@
 
     function makeLipGroup() {
         var lipCurve = two.makeCurve(width / 2, 0, width / 8, height, -width / 8, height, -width / 2, 0, true)
         lipCurve.fill = 'None'
         lipCurve.linewidth = thickness
         lipCurve.stroke = color
         lipCurve.cap = 'round'
+
+        // var keypoint_color = '#e8cd25'
+        // kp1 = two.makeCircle(width/2,0, 30);
+        // kp1.fill = 'transparent'; // Set fill to transparent
+        // kp1.stroke = keypoint_color; // Set stroke color (you can change it to any color you prefer)
+        // kp1.linewidth = 10; 
+
+        // kp2 = two.makeCircle(width/8,height, 30);
+        // kp2.fill = 'transparent'; // Set fill to transparent
+        // kp2.stroke = keypoint_color; // Set stroke color (you can change it to any color you prefer)
+        // kp2.linewidth = 10; 
+
+        // kp3 = two.makeCircle(-width/8,height, 30);
+        // kp3.fill = 'transparent'; // Set fill to transparent
+        // kp3.stroke = keypoint_color; // Set stroke color (you can change it to any color you prefer)
+        // kp3.linewidth = 10; 
+
+        // kp4 = two.makeCircle(-width/2,0, 30);
+        // kp4.fill = 'transparent'; // Set fill to transparent
+        // kp4.stroke = keypoint_color; // Set stroke color (you can change it to any color you prefer)
+        // kp4.linewidth = 10; 
+
+        // return two.makeGroup(lipCurve, kp1,kp2,kp3,kp4)
         return two.makeGroup(lipCurve)
     }
 
     function interpolateLips(goal, t) {
         TWEEN.remove(this.currentControlPoint);
 
         var goal = goal;
         var target = this.currentControlPoint;
         var tween = new TWEEN.Tween(target, {
             override: true
         }).to(goal, t);
         tween.easing(TWEEN.Easing.Quadratic.InOut);
         var mouthInfo = this.group.children[0]
+
+        // var kp1 = this.group.children[1]
+        // var kp2 = this.group.children[2]
+        // var kp3 = this.group.children[3]
+        // var kp4 = this.group.children[4]
+
         tween.onUpdate(function() {
             mouthInfo.vertices[0].x = this.x0
             mouthInfo.vertices[0].y = this.y0
 
             mouthInfo.vertices[1].x = this.x1
             mouthInfo.vertices[1].y = this.y1
 
             mouthInfo.vertices[2].x = this.x2
             mouthInfo.vertices[2].y = this.y2
 
             mouthInfo.vertices[3].x = this.x3
             mouthInfo.vertices[3].y = this.y3
+
+            // kp1.translation.x = this.x0
+            // kp1.translation.y = this.y0
+
+            // kp2.translation.x = this.x1
+            // kp2.translation.y = this.y1
+
+            // kp3.translation.x = this.x2
+            // kp3.translation.y = this.y2
+
+            // kp4.translation.x = this.x3
+            // kp4.translation.y = this.y3
         });
         tween.start();
     }
 
     llip = new facePart('llip', makeLipGroup(), windowHalfX + x, windowHalfY - y)
     llip.idleControlPoint = {
         x0: width / 2,
```

### Comparing `pylips-0.0.8/pylips/face/static/js/tween.min.js` & `pylips-0.0.9/pylips/face/static/js/tween.min.js`

 * *Files identical despite different names*

### Comparing `pylips-0.0.8/pylips/face/static/js/two.min.js` & `pylips-0.0.9/pylips/face/static/js/two.min.js`

 * *Files identical despite different names*

### Comparing `pylips-0.0.8/pylips/face/templates/index.html` & `pylips-0.0.9/pylips/face/templates/index.html`

 * *Files identical despite different names*

### Comparing `pylips-0.0.8/pylips/speech/polly_tts.py` & `pylips-0.0.9/pylips/speech/polly_tts.py`

 * *Files identical despite different names*

### Comparing `pylips-0.0.8/pylips/speech/robot_face.py` & `pylips-0.0.9/pylips/speech/robot_face.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,31 +24,34 @@
 
         if os.path.exists('pylips_phrases') == False:
             os.mkdir('pylips_phrases')
 
         self.name = robot_name
         self.voice_id = voice_id
 
-        self.io = socketio.Client()
-        self.io.connect(server_ip)
+        try:
+            self.io = socketio.Client()
+            self.io.connect(server_ip)
+        except socketio.exceptions.ConnectionError as e:
+            print(f'Error connecting to server at {server_ip}. Try running:\npython3 -m pylips.face.start')
 
         pygame.mixer.init()
         self.channel = 0
 
         tts_methods = ['polly']
         if tts_method not in tts_method:
             raise Exception(f'parameter tts_method must be one of {tts_methods}')
         
         # TODO: implement other TTS things, but for now we will use polly
         if tts_method == 'system':
             self.tts = SystemTTS()
         if tts_method == 'polly':
             self.tts = PollyTTS()
 
-    def say(self, content):
+    def say(self, content, wait=False):
         '''
             The main method for the RobotFace class. This method will take in a string of text and
             convert it to speech using the AWS Polly service.
             :param: content - the text that the robot should speak
         '''
 
         fname, times, visemes = self.tts.gen_audio_and_visemes(content, self.voice_id)
@@ -67,14 +70,17 @@
              
         sound = pygame.mixer.Sound(fname)
 
         #play sound and face
         self.io.emit('face_control', request)
         pygame.mixer.Channel(self.channel).play(sound)
 
+        while wait and pygame.mixer.Channel(self.channel).get_busy():
+            pygame.time.wait(100)
+
     def save_file(self, content, filename):
         '''
             The main method for the RobotFace class. This method will take in a string of text and
             convert it to speech.
             :param: content - the text that the robot should speak
         '''
         self.tts.gen_audio_and_visemes(content, self.voice_id, filename)
```

### Comparing `pylips-0.0.8/pylips/speech/system_tts.py` & `pylips-0.0.9/pylips/speech/system_tts.py`

 * *Files 6% similar despite different names*

```diff
@@ -80,32 +80,32 @@
 }
 
 class SystemTTS:
     def __init__(self):
         self.engine = pyttsx3.init()
         self.engine.setProperty('rate', 120)
         self.model = read_recognizer()
+        self.voices = self.engine.getProperty('voices')
 
     def list_voices(self):
-        voices = self.engine.getProperty('voices')
-        for voice in voices:
+        for voice in self.voices:
             print(voice.id)
 
     def gen_audio_and_visemes(self, text, voice_id=None, fname=None):
         '''
         generates an audio file that says the text of _text_ in the voice of _voice_id_
 
         :param: text - the text that the robot should speak
         :param: voice_id - the voice that the robot should speak in
         :param: fname - the name of the file that the audio should be saved to
         '''
         if voice_id is None:
-            voices = self.engine.getProperty('voices')
-            voice_id = 'default'
-            # self.engine.setProperty('voice', voices[0].id)
+            voice_id = 'en' if platform == "linux" or platform == "linux2" else 'default'
+        elif voice_id not in self.voices:
+            raise Exception(f'voice "{voice_id}" does not exist')
         else:
             self.engine.setProperty('voice', voice_id)
 
         if fname is None:   
             fname = f"pylips_phrases/{voice_id}_output.wav"
         else:
             #if it was already cached, return it, otherwise, generate it and return it
@@ -113,15 +113,15 @@
             if os.path.exists(fname):
                 times, visemes = pickle.load(open(f'{fname[:-4]}.pkl', 'rb'))
                 return fname, times, visemes
 
         # Synthesize speech
         if platform == "linux" or platform == "linux2":
             # linux has issues with saving multiple files...
-            os.system(f"espeak-ng -s 100 '{text}' -w {fname}")
+            os.system(f"espeak-ng -v {voice_id} -s 100 '{text}' -w {fname}")
         else:
             self.engine.save_to_file(text, fname)
             self.engine.runAndWait()
 
         data, samplerate = sf.read(fname)
         sf.write(fname, data, samplerate)
```

### Comparing `pylips-0.0.8/pylips.egg-info/PKG-INFO` & `pylips-0.0.9/pylips.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylips
-Version: 0.0.8
+Version: 0.0.9
 Summary: An interface for embodied conversational interaction.
 Home-page: https://github.com/interaction-lab/PyLips
 Author: Interaction Lab
 Author-email: dennler@usc.edu
 License: MIT license
 Keywords: lips
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -25,14 +25,15 @@
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: flask>=2.0.1
 Requires-Dist: flask-socketio>=5.1.1
 Requires-Dist: python-socketio>=5.11.1
 Requires-Dist: websocket-client>=1.7.0
+Requires-Dist: requests>=2.31.0
 Requires-Dist: boto3>=1.18.67
 Requires-Dist: pygame>=2.1.1
 Requires-Dist: py3-tts>=3.5
 Requires-Dist: allosaurus>=1.0.2
 Requires-Dist: soundfile>=0.12.1
 Provides-Extra: dev
 Requires-Dist: pip>=20.3; extra == "dev"
@@ -65,12 +66,14 @@
 Requires-Dist: twine==4.0.2; extra == "dev"
 Requires-Dist: check-wheel-contents==0.4.0; extra == "dev"
 
 # PyLips
 Web-Enabled Facial Text-to-Speech
 
 
+
+
 # History
 
 ## 0.0.0 (2024-03-24)
 
 - pylips begins
```

### Comparing `pylips-0.0.8/pylips.egg-info/SOURCES.txt` & `pylips-0.0.9/pylips.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pylips-0.0.8/pylips.egg-info/requires.txt` & `pylips-0.0.9/pylips.egg-info/requires.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 flask>=2.0.1
 flask-socketio>=5.1.1
 python-socketio>=5.11.1
 websocket-client>=1.7.0
+requests>=2.31.0
 boto3>=1.18.67
 pygame>=2.1.1
 py3-tts>=3.5
 allosaurus>=1.0.2
 soundfile>=0.12.1
 
 [dev]
```

### Comparing `pylips-0.0.8/setup.cfg` & `pylips-0.0.9/setup.cfg`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.0.8
+current_version = 0.0.9
 commit = True
 tag = False
 
 [bumpversion:file:setup.py]
 search = version="{current_version}"
 replace = version="{new_version}"
```

### Comparing `pylips-0.0.8/setup.py` & `pylips-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 
 install_requires = [
     #web server
     "flask>=2.0.1",
     "flask-socketio>=5.1.1",
     "python-socketio>=5.11.1",
     "websocket-client>=1.7.0",
+    "requests>=2.31.0",
     #TTS
     "boto3>=1.18.67",
     "pygame>=2.1.1",
     "py3-tts>=3.5",
     "allosaurus>=1.0.2",
     "soundfile>=0.12.1",
 ]
@@ -93,10 +94,10 @@
     include_package_data=True,
     keywords="lips",
     name="pylips",
     packages=find_packages(include=["pylips", "pylips.*"]),
     python_requires=">=3.8.0",
     test_suite="tests",
     url="https://github.com/interaction-lab/PyLips",
-    version="0.0.8",
+    version="0.0.9",
     zip_safe=False,
 )
```

