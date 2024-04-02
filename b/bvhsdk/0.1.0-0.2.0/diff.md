# Comparing `tmp/bvhsdk-0.1.0.tar.gz` & `tmp/bvhsdk-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bvhsdk-0.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "bvhsdk-0.2.0.tar", last modified: Tue Apr  2 19:36:41 2024, max compression
```

## Comparing `bvhsdk-0.1.0.tar` & `bvhsdk-0.2.0.tar`

### file list

```diff
@@ -1,17 +1,28 @@
--rw-r--r--   0        0        0        8 2023-09-07 16:30:33.520451 bvhsdk-0.1.0/README.md
--rw-r--r--   0        0        0      179 2023-02-09 02:02:14.366033 bvhsdk-0.1.0/bvhsdk/__init__.py
--rw-r--r--   0        0        0    35822 2023-09-05 18:42:37.344180 bvhsdk-0.1.0/bvhsdk/anim.py
--rw-r--r--   0        0        0    13227 2023-05-29 22:01:08.894594 bvhsdk-0.1.0/bvhsdk/bvh.py
--rw-r--r--   0        0        0    95234 2023-02-09 01:26:56.048464 bvhsdk-0.1.0/bvhsdk/egocentriccoord.py
--rw-r--r--   0        0        0       21 2023-03-23 18:35:49.006196 bvhsdk-0.1.0/bvhsdk/gui/__init__.py
--rw-r--r--   0        0        0     8337 2023-05-29 22:01:08.907442 bvhsdk-0.1.0/bvhsdk/gui/main.py
--rw-r--r--   0        0        0     7159 2023-02-08 23:07:26.593954 bvhsdk-0.1.0/bvhsdk/ik.py
--rw-r--r--   0        0        0    35605 2021-06-22 18:29:19.083852 bvhsdk-0.1.0/bvhsdk/mathutils.py
--rw-r--r--   0        0        0    14856 2021-08-16 18:17:19.423956 bvhsdk-0.1.0/bvhsdk/mlutils.py
--rw-r--r--   0        0        0    52327 2023-01-19 16:57:57.654067 bvhsdk-0.1.0/bvhsdk/plotanimation.py
--rw-r--r--   0        0        0    15523 2023-03-29 22:28:59.468358 bvhsdk-0.1.0/bvhsdk/retarget.py
--rw-r--r--   0        0        0    25520 2023-02-08 20:29:26.990842 bvhsdk-0.1.0/bvhsdk/skeletonmap.py
--rw-r--r--   0        0        0    44222 2023-02-08 20:41:38.510776 bvhsdk-0.1.0/bvhsdk/surface.py
--rw-r--r--   0        0        0     3820 2023-02-08 16:25:27.738587 bvhsdk-0.1.0/bvhsdk/test_old.py
--rw-r--r--   0        0        0      830 2023-09-07 20:00:13.968759 bvhsdk-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      792 1970-01-01 00:00:00.000000 bvhsdk-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      492 2023-09-12 12:35:22.787035 bvhsdk-0.2.0/.readthedocs.yaml
+-rw-r--r--   0        0        0     1097 2022-07-05 20:10:39.520550 bvhsdk-0.2.0/LICENSE
+-rw-r--r--   0        0        0     4745 2023-12-20 13:24:34.021867 bvhsdk-0.2.0/README.md
+-rw-r--r--   0        0        0      179 2023-02-09 02:02:14.366033 bvhsdk-0.2.0/bvhsdk/__init__.py
+-rw-r--r--   0        0        0    51152 2024-04-02 18:05:17.974414 bvhsdk-0.2.0/bvhsdk/anim.py
+-rw-r--r--   0        0        0    16436 2024-01-03 13:55:53.506284 bvhsdk-0.2.0/bvhsdk/bvh.py
+-rw-r--r--   0        0        0    95234 2023-02-09 01:26:56.048464 bvhsdk-0.2.0/bvhsdk/egocentriccoord.py
+-rw-r--r--   0        0        0       21 2023-03-23 18:35:49.006196 bvhsdk-0.2.0/bvhsdk/gui/__init__.py
+-rw-r--r--   0        0        0     8337 2023-05-29 22:01:08.907442 bvhsdk-0.2.0/bvhsdk/gui/main.py
+-rw-r--r--   0        0        0     7159 2023-02-08 23:07:26.593954 bvhsdk-0.2.0/bvhsdk/ik.py
+-rw-r--r--   0        0        0    42949 2024-01-05 17:32:48.793547 bvhsdk-0.2.0/bvhsdk/mathutils.py
+-rw-r--r--   0        0        0    56597 2024-04-02 18:58:13.529198 bvhsdk-0.2.0/bvhsdk/plotanimation.py
+-rw-r--r--   0        0        0    15523 2023-03-29 22:28:59.468358 bvhsdk-0.2.0/bvhsdk/retarget.py
+-rw-r--r--   0        0        0    25520 2023-02-08 20:29:26.990842 bvhsdk-0.2.0/bvhsdk/skeletonmap.py
+-rw-r--r--   0        0        0    44222 2023-02-08 20:41:38.510776 bvhsdk-0.2.0/bvhsdk/surface.py
+-rw-r--r--   0        0        0      658 2023-09-07 18:38:39.854201 bvhsdk-0.2.0/docs/Makefile
+-rwxr-xr-x   0        0        0      804 2023-09-07 18:38:39.854201 bvhsdk-0.2.0/docs/make.bat
+-rw-r--r--   0        0        0      329 2023-09-12 22:10:19.674461 bvhsdk-0.2.0/docs/source/bvhsdk.gui.md
+-rw-r--r--   0        0        0     1465 2023-12-20 13:23:08.362197 bvhsdk-0.2.0/docs/source/bvhsdk.md
+-rw-r--r--   0        0        0     2090 2023-09-12 22:10:19.695708 bvhsdk-0.2.0/docs/source/conf.py
+-rw-r--r--   0        0        0     3612 2023-09-13 17:30:05.884600 bvhsdk-0.2.0/docs/source/example.md
+-rw-r--r--   0        0        0     5846 2023-12-19 12:57:48.112034 bvhsdk-0.2.0/docs/source/index.md
+-rw-r--r--   0        0        0    27620 2023-09-12 22:10:19.702281 bvhsdk-0.2.0/docs/source/logo.png
+-rw-r--r--   0        0        0       55 2023-09-12 22:10:19.702281 bvhsdk-0.2.0/docs/source/modules.md
+-rw-r--r--   0        0        0     2561 2023-09-13 17:41:40.979023 bvhsdk-0.2.0/docs/source/usage.md
+-rw-r--r--   0        0        0    27620 2023-09-12 12:35:22.828374 bvhsdk-0.2.0/logo.png
+-rw-r--r--   0        0        0      882 2024-04-02 18:59:24.785061 bvhsdk-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     5499 1970-01-01 00:00:00.000000 bvhsdk-0.2.0/PKG-INFO
```

### Comparing `bvhsdk-0.1.0/bvhsdk/bvh.py` & `bvhsdk-0.2.0/bvhsdk/bvh.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,53 +1,74 @@
 import numpy as np
 from . import plotanimation, mathutils, skeletonmap
 from .anim import *
 from os.path import basename as getfilename
 from os.path import join as pathjoin
 import time
 
-def WriteBVH(animation, path, name='_export', frametime = 0.00833333, refTPose = True, writeTranslation=True):
+def ReadFile(path,
+             surfaceinfo=None,
+             skipmotion=False):
     """
-    Create a bvh file with the motion contained in the animation.
+    Read BVH file and returns an anim.Animation object. The anim.Animation holds the information about the animation file and contain reference to anim.Joint objects. The global position of each joint is **not** computed when calling bvh.ReadFile().
 
-    :type animation: pyanimation.Animation
-    :param animation: Animation containing the motion
+    :param surface.Surface surfaceinfo: Attach the surface information of the corresponding character to the anim.Animation object. The surface information is only required for computing the egocentric coordinates. Default set to None. (*)
 
-    :type path: str
-    :param path: Full path to save the file
+    :param bool skipmotion: If set to True, the motion of the BVH file will not be read (skip everything after "Frame Time"), only the skeleton specification is stored. Default set to False.
+    
+    :returns: Animation object containing the information from the bvh file.
+    :rtype: anim.Animation
+    """
+    animation = GetBVHDataFromFile(path, skipmotion=skipmotion)
+    animation.surfaceinfo = surfaceinfo
+
+    return animation
+
+def WriteBVH(animation, 
+             path, 
+             name = '_export', 
+             frametime = None, 
+             writeTranslation = True,
+             refTPose = True):
+    """
+    Create a bvh file with the motion contained in the anim.Animation object using the information contained in joint.rotation and joint.translation.
 
-    :type name: str
-    :param name: Filename
+    :param anim.Animation animation: anim.Animation containing the motion
 
-    :type frametime: float
-    :param frametime: 1/(Frame per second), the time duration of each frame
+    :param str path: Full path to save the file
 
-    :type refTPose: bool
-    :param refTPose: If True, the first frame of the animation is the input TPose reference
+    :param str name: Filename without the '.bvh' extension.
 
-    :type writeTranslation: bool
-    :param writeTranslation: If True, write translations for every joint. If False, only write translation for the root joint
+    :param float frametime: 1/(frame per second), the time duration of each frame. Default set to 120 fps.
+
+    :param bool writeTranslation: If set to True (default), translations (local positions) are written for every joint. Each joint will have six channels, with the first three representing X, Y, and Z translations. If set to False, only the translation (global position) for the root joint will be written.
+
+    :param bool refTPose: If set to True, the first frame of the BVH file will be the input TPose reference (default). Note that the TPose reference must be set manually for each joint and stored in joint.tposetrans and joint.tposerot as in retarget.MotionRetargeting().
     """
-    path = pathjoin(path, name)
+    if name:
+        path = pathjoin(path, name)
     endsiteflag = False
     depth = 0
+    if frametime is None:
+        frametime = animation.frametime
     with open(str.format("%s.bvh" % path), "w") as file:
         file.write('HIERARCHY\n')
         for section in ['header', 'content']:
             if section == 'header':
                 for joint in animation.getlistofjoints():
                     if joint==animation.root:
                         file.write(str.format('ROOT %s\n' % joint.name))
                         file.write('{\n')
                         file.write(str.format('\tOFFSET %.5f %.5f %.5f\n' % (joint.offset[0],joint.offset[1],joint.offset[2])))
                         if joint.order == 'XYZ':
                             file.write(str.format("\tCHANNELS 6 Xposition Yposition Zposition Xrotation Yrotation Zrotation\n"))
                         elif joint.order == 'ZXY':
                             file.write(str.format("\tCHANNELS 6 Xposition Yposition Zposition Zrotation Xrotation Yrotation\n"))
-
+                        elif joint.order == 'ZYX':
+                            file.write(str.format("\tCHANNELS 6 Xposition Yposition Zposition Zrotation Yrotation Xrotation\n"))
                     else:
                         if endsiteflag:
                             endsiteflag = False
                             next_depth = joint.getDepth()
                             while depth >= next_depth:
                                 file.write('%s}\n' % ((depth)*'\t'))
                                 depth = depth-1
@@ -59,16 +80,19 @@
                             aux_string = str.format("%sCHANNELS 6 Xposition Yposition Zposition " % ((depth+1)*"\t"))
                         else:
                             aux_string = str.format("%sCHANNELS 3 " % ((depth+1)*"\t"))
                         if joint.order == 'XYZ':
                             file.write(aux_string + "Xrotation Yrotation Zrotation\n")
                         elif joint.order == 'ZXY':
                             file.write(aux_string + "Zrotation Xrotation Yrotation\n")
+                        elif joint.order == 'ZYX':
+                            file.write(aux_string + "Zrotation Yrotation Xrotation\n")
                         else:
-                            print('Order is not implemented')
+                            print('Order not implemented')
+                            raise NotImplementedError
                         if len(joint.endsite) > 0:
                             endsiteflag = True
                             file.write(str.format('%sEnd Site\n' % ((depth+1)*'\t')))
                             file.write('%s{\n' % ((depth+1)*'\t'))
                             file.write(str.format('%sOFFSET %.5f %.5f %.5f\n' % ((depth+2)*'\t',joint.endsite[0],joint.endsite[1],joint.endsite[2])))
                             file.write('%s}\n' % ((depth+1)*'\t'))
             elif section == 'content':
@@ -94,46 +118,50 @@
                     for joint in animation.getlistofjoints():
                         if writeTranslation or joint==animation.root:
                             line = line + [joint.tposetrans[0], joint.tposetrans[1], joint.tposetrans[2]]
                         if joint.order=='XYZ':
                             line = line + [joint.tposerot[0], joint.tposerot[1], joint.tposerot[2]]
                         elif joint.order=='ZXY':
                             line = line + [joint.tposerot[2], joint.tposerot[0], joint.tposerot[1]]
+                        elif joint.order=='ZYX':
+                            line = line + [joint.tposerot[2], joint.tposerot[1], joint.tposerot[0]]
                     string = " ".join(str.format("%.2f"%number) for number in line)
                     file.write(string+'\n')
 
                 #Write the rest of the file
                 for frame in range(animation.frames):
                     line = []
                     for joint in animation.getlistofjoints():
                         if writeTranslation or joint==animation.root:
-                            line = line + [joint.translation[frame,0], joint.translation[frame,1], joint.translation[frame,2]]
+                            if joint.n_channels == 6:
+                                line = line + [joint.translation[frame,0], joint.translation[frame,1], joint.translation[frame,2]]
+                            else:
+                                line = line + [joint.offset[0], joint.offset[1], joint.offset[2]]
                         if joint.order=='XYZ':
                             line = line + [joint.rotation[frame,0], joint.rotation[frame,1], joint.rotation[frame,2]]
                         elif joint.order=='ZXY':
                             line = line + [joint.rotation[frame,2], joint.rotation[frame,0], joint.rotation[frame,1]]
+                        elif joint.order=='ZYX':
+                            line = line + [joint.rotation[frame,2], joint.rotation[frame,1], joint.rotation[frame,0]]
                     string = " ".join(str.format("%.2f"%number) for number in line)
                     file.write(string+'\n')
     print('File Saved: %s' % (path+'.bvh'))
 
 
-def GetBVHDataFromFile(path, skipmotion=False):
+def GetBVHDataFromFile(path, 
+                       skipmotion=False):
     """
-    Read a bvh file.
+    Auxiliary function to bvh.ReadFile(), it is not intended to be used by the user. It is the parser of the bvh file.
 
-    :type path: string or path
-    :param path: Complete path to the bvh file
+    :param str path: Full path to the bvh file
 
-    :type skipmotion: bool
-    :param skipmotion: Whether to read the motion of the file (False) or to
-    read only the skeleton definition.
-
-    :rtype bvhfile: Animation
-    :rparam bvhfile: An Animation object containing the information from the
-    bvh file.
+    :param bool skipmotion: If set to True, skip everything after "Frame Time", only the skeleton specification is stored. Default set to False.
+
+    :returns: Animation object containing the information from the bvh file.
+    :rtype: anim.Animation
     """
     # TODO: Account for BVH files without translation
     frame = 0
     bvhfile = None
     with open(path) as file:
         flagEndSite = False
         flagMotionDataBegin = False
@@ -176,19 +204,24 @@
                     lastJoint.n_channels = int(aux[1])
                     lastJoint.channels = {key: value for key, value in zip(aux[2:], np.arange(lastJoint.n_channels))}
                     if lastJoint.n_channels != 3 and lastJoint.n_channels != 6:
                         print("Number of channels must be 3 or 6")
                         raise NotImplementedError
                     X, Y, Z = lastJoint.channels["Xrotation"], lastJoint.channels["Yrotation"], lastJoint.channels["Zrotation"]
                     if Z < X and X < Y: lastJoint.order = "ZXY"
-                    elif X < Y and Y < Z: lastJoint.order = "XYZ"
                     else:
-                        lastJoint.order("XYZ")
-                        print("Invalid Channels order. XYZ chosen.")
-                        raise NotImplementedError
+                        if X < Y and Y < Z: 
+                            lastJoint.order = "XYZ"
+                        elif Z < Y and Y < X:
+                            lastJoint.order = "ZYX"
+                        else:
+                            print("Invalid Channels order.")
+                            raise NotImplementedError
+                        print("WARNING: Channels order %s for Joint %s is not fully implemented yet." % (lastJoint.order, lastJoint.name))
+                        print("bvhsdk only fully supports ZXY order. Use it with caution.")
 
                 elif (line.find("Frames")) >= 0:
                     bvhfile.frames = int(line[8:])
                     for joint in bvhfile.getlistofjoints():
                         joint.translation = np.empty(shape=(bvhfile.frames, 3))
                         joint.rotation = np.empty(shape=(bvhfile.frames, 3))
                 elif (line.find("Frame Time")) >= 0:
@@ -210,58 +243,56 @@
                         joint.translation[frame] = np.array( [values[joint.channels['Xposition']], values[joint.channels['Yposition']], values[joint.channels['Zposition']]] )
                     i+=len(joint.channels)
                 frame += 1
 
 
     return bvhfile
 
-def GetPositions(joint, frame=0, parentTransform=[], surfaceinfo=None, calibrating=None):
-    # Recebe o frame e a junta root, recursivamente calcula a posição de todos
-    # os filhos para esse frame
-    # Salva a posição em cada frame dentro de cada instância junta
+def GetPositions(joint,
+                 frame = 0,
+                 parentTransform=[],
+                 surfaceinfo=None,
+                 calibrating=None):
+    """
+    Recursevely compute the global position of each joint for the given frame. The global position is stored in joint.position. This function is not used anymore and could be removed or moved to the anim.Animation class in the future.
+
+    :param anim.Joint joint: Joint to calculate the global position
+
+    :param int frame: Frame to calculate the global position, default set to 0.
 
-    # Caso precise recalcular as posições das juntas, os dados antigos precisam
-    # ser apagados
+    :param list parentTransform: Parameter not intended for user input, used in recursion. List of 4x4 matrices, each matrix is the local transformation of the parent joint.
 
-    #TODO: Orientation não significa nada, arrumar
+    :param surface.Surface surfaceinfo: Legacy parameter, not used anymore. Should be removed in the future.
 
+    :param bool calibrating: Legacy parameter, not used anymore. Should be removed in the future.
+    """
     rot = joint.rotation[frame]
     transform = joint.getLocalTransform(frame)
 
     if len(parentTransform) == 0:
-        #Se for root apenas calcula a posição
+        # If it is the root joint, the global position is the same as the local position
         positionfinal = np.dot(transform, [0,0,0,1])
         orientation = np.asarray([rot[0], rot[1], rot[2]])
     else:
-        #Nos outros casos, multiplica pela transformada da junta pai
+        # If it is not the root joint, the global position is the joint's local transformation matrix multiplied by the parent joint's global transformation matrx
         transform = np.dot(parentTransform,transform)
         positionfinal = np.dot(transform,[0,0,0,1])
         orientation = joint.parent.orientation[frame,:] + np.asarray([rot[0], rot[1], rot[2]])
 
     if not calibrating:
         joint.addPosition(np.asarray(positionfinal[:-1]), frame)
         joint.addOrientation(orientation, frame)
 
-    #Caso a junta tenha um endsite (é um end effector)
+    # If joint have an endsite (it is an end effector)
     if len(joint.endsite)>0:
         ee_transform = mathutils.matrixTranslation(joint.endsite[0], joint.endsite[1], joint.endsite[2])
         ee_transform = np.dot(transform,ee_transform)
         endsitepos = np.dot(ee_transform,[0,0,0,1])
         if not calibrating:
-            #Salva a posição do endsite da junta no frame atual
+            # Save endsite position in the current joint
             joint.addEndSitePosition(np.asarray(endsitepos[:-1]), frame)
 
 
     parentTransform = np.copy(transform)
     for child in joint.children:
         GetPositions(child, frame, parentTransform, surfaceinfo, calibrating)
-    parentTransform=[]
-
-
-def ReadFile(path, surfaceinfo=None, skipmotion=False):
-    """
-    Read BVH file, create animation a joints instances and compute joint positions
-    """
-    animation = GetBVHDataFromFile(path, skipmotion=skipmotion)
-    animation.surfaceinfo = surfaceinfo
-
-    return animation
+    parentTransform=[]
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `bvhsdk-0.1.0/bvhsdk/egocentriccoord.py` & `bvhsdk-0.2.0/bvhsdk/egocentriccoord.py`

 * *Files identical despite different names*

### Comparing `bvhsdk-0.1.0/bvhsdk/gui/main.py` & `bvhsdk-0.2.0/bvhsdk/gui/main.py`

 * *Files identical despite different names*

### Comparing `bvhsdk-0.1.0/bvhsdk/ik.py` & `bvhsdk-0.2.0/bvhsdk/ik.py`

 * *Files identical despite different names*

### Comparing `bvhsdk-0.1.0/bvhsdk/mathutils.py` & `bvhsdk-0.2.0/bvhsdk/mathutils.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,23 +7,43 @@
 
 import numpy as np
 import time
 
 
 
 def xaxis():
+    """
+    :return: Return a numpy array representing the x axis
+    :rtype: numpy.ndarray
+    """
     return np.asarray([1,0,0])
 
 def yaxis():
+    """
+    :return: Return a numpy array representing the y axis
+    :rtype: numpy.ndarray
+    """
     return np.asarray([0,1,0])
 
 def zaxis():
+    """
+    :return: Return a numpy array representing the z axis
+    :rtype: numpy.ndarray
+    """
     return np.asarray([0,0,1])
 
 def matrixIdentity(shape=3):
+    """
+    Return identity matrix of shape 3x3 or 4x4
+    
+    :param int shape: shape of the matrix. 3 for 3x3 and 4 for 4x4
+    
+    :return: identity matrix
+    :rtype: numpy.ndarray
+    """
     if shape==3:
         matrix = np.array([
                 [1, 0, 0],
                 [0, 1, 0],
                 [0, 0, 1]
                 ])
     elif shape==4:
@@ -35,26 +55,54 @@
                 ])
     else:
         print("Incompatible shape, please choose 3 or 4.")
         return None
     return matrix
 
 
-def matrixTranslation(tx,ty,tz):
-    #Return translation matrix
+def matrixTranslation(tx,
+                      ty,
+                      tz):
+    """
+    Construct a transformation matrix for translation of tx, ty and tz
+
+    :param float tx: translation in x axis
+    :param float ty: translation in y axis
+    :param float tz: translation in z axis
+
+    :return: translation matrix
+    :rtype: numpy.ndarray
+    """
     matrix = np.array([
             [1, 0, 0, tx],
             [0, 1, 0, ty],
             [0, 0, 1, tz],
             [0, 0, 0, 1]
             ])
     return matrix
 
-def matrixRotation(angle, x=0, y=0, z=0,shape=4):
-    #Return rotation matrix
+def matrixRotation(angle,
+                   x=0,
+                   y=0,
+                   z=0,
+                   shape=4):
+    """
+    Construct a transformation matrix for rotation of angle degrees around the axis defined by x, y and z.
+    If shape is 4 it will append create a 4x4 transformation matrix with translation equals to zero.
+
+    :param float angle: angle in degrees
+    :param float x: x axis
+    :param float y: y axis
+    :param float z: z axis
+    :param int shape: shape of the matrix. 3 for 3x3 and 4 for 4x4
+
+    :return: rotation matrix
+    :rtype: numpy.ndarray
+    """
+
     if x==0 and y==0 and z==0:
         print("No axis found. Values x, y and z can't be all zero.")
         return None
 
     if shape!=3 and shape!=4:
         print("Incompatible shape. Please choose 3 or 4")
         return None
@@ -86,25 +134,32 @@
 
     matrix[3,0] = 0
     matrix[3,1] = 0
     matrix[3,2] = 0
     matrix[3,3] = 1
 
     if shape==3:
-#        matrix = np.asarray([matrix[i,j] for i in range(3) for j in range(3)])
         matrix = shape4ToShape3(matrix)
 
     return matrix
 
 
 
-def matrixMultiply(m0, m1):
-    #Multiplication  of 3x3 by 3x3 matrices or 4x4 by 4x4 matrices
-#    teste0 = np.asarray(m0)
-#    teste1 = np.asarray(m1)
+def matrixMultiply(m0,
+                   m1):
+    """
+    Perform matrix multiplication between m0 and m1. m0 and m1 can be 3x3 or 4x4 matrices.
+    For performance reasons, use numpy.dot() instead.
+
+    :param numpy.ndarray m0: matrix 0
+    :param numpy.ndarray m1: matrix 1
+
+    :return: matrix resulting from the multiplication
+    :rtype: numpy.ndarray
+    """
     start=time.time()
 
     if type(m0)!=type(np.ndarray([])):
         try:
             m0 = np.asarray(m0)
         except:
             print("First argument could not be converted to a numpy array.")
@@ -180,29 +235,49 @@
 
     matrixMultiply.time += time.time()-start
     matrixMultiply.count += 1
     return matrix
 
 
 def inverseMatrix(m0):
+    """
+    Tries to invert matrix m0 using numpy.linalg.inv(). If it is not possible, returns None.
+
+    :param numpy.ndarray m0: matrix to be inverted
+
+    :return: inverted matrix
+    :rtype: numpy.ndarray
+    """
     try:
         matrix = np.linalg.inv(m0)
     except np.linalg.LinAlgError:
         # Not invertible. Skip this one.
         print('Matrix not invertible.')
         return None
     return matrix
 
 
-def projectedBarycentricCoord(p, p1, p2, p3):
+def projectedBarycentricCoord(p,
+                              p1,
+                              p2,
+                              p3):
+    """
+    Compute the baricentric coordinates of a point p projected onto a triangle defined by p1, p2 and p3.
+    Algorithm from "Computing the barycentric coordinates of a projected point." by Heidrich, Wolfgang, Journal of Graphics Tools 10, no. 3 (2005): 9-12.
+    
+    :param numpy.ndarray p: point to be projected
+    :param numpy.ndarray p1: first point of the triangle
+    :param numpy.ndarray p2: second point of the triangle
+    :param numpy.ndarray p3: third point of the triangle
+
+    :return: normal vector, baricentric coordinates, displacement vector, baricentric coordinates in cartesian space and a boolean indicating if the point is inside the triangle
+    :rtype: numpy.ndarray, numpy.ndarray, numpy.ndarray, numpy.ndarray, bool
+    """
     start = time.time()
-    #Algorithm from Heidrich, Wolfgang.
-    #"Computing the barycentric coordinates of a projected point."
-    #Journal of Graphics Tools 10, no. 3 (2005): 9-12.
-    # p: point. p1, p2 and p3: triangle's vertices points
+    
     if len(p)>3: p=p[:3]
     if len(p1)>3: p1=p1[:3]
     if len(p2)>3: p2=p2[:3]
     if len(p3)>3: p3=p3[:3]
     p1 = np.asarray(p1)
     p2 = np.asarray(p2)
     p3 = np.asarray(p3)
@@ -228,20 +303,32 @@
     dispvector = p-b_cartesian
     n = n/np.linalg.norm(n)
 
     projectedBarycentricCoord.count += 1
     projectedBarycentricCoord.time += time.time()-start
     return n, b, dispvector, b_cartesian, inside
 
-def clampedBarycentric(p,p1,p2,p3):
+def clampedBarycentric(p,
+                       p1,
+                       p2,
+                       p3):
+    """
+    Compute the baricentric coordinates of a point p projected onto a triangle defined by p1, p2 and p3.
+    Different from mathutils.projectedBarycentricCoord(), if p is outside the triangle, the baricentric coordinates are clamped to the triangle edges.
+    Algorithm from "Computing the barycentric coordinates of a projected point." by Heidrich, Wolfgang, Journal of Graphics Tools 10, no. 3 (2005): 9-12.
+    
+    :param numpy.ndarray p: point to be projected
+    :param numpy.ndarray p1: first point of the triangle
+    :param numpy.ndarray p2: second point of the triangle
+    :param numpy.ndarray p3: third point of the triangle
+
+    :return: normal vector, baricentric coordinates, displacement vector, baricentric coordinates in cartesian space and a boolean indicating if the point is inside the triangle
+    :rtype: numpy.ndarray, numpy.ndarray, numpy.ndarray, numpy.ndarray, bool
+    """
     start = time.time()
-    # Algorithm from Heidrich, Wolfgang.
-    # "Computing the barycentric coordinates of a projected point."
-    # Journal of Graphics Tools 10, no. 3 (2005): 9-12.
-    # p: point. p1, p2 and p3: triangle's vertices points
     if len(p)>3: p=p[:3]
     if len(p1)>3: p1=p1[:3]
     if len(p2)>3: p2=p2[:3]
     if len(p3)>3: p3=p3[:3]
     p1 = np.asarray(p1)
     p2 = np.asarray(p2)
     p3 = np.asarray(p3)
@@ -268,47 +355,95 @@
     dispvector = p-b_cartesian
     n = n/np.linalg.norm(n)
 
     clampedBarycentric.count += 1
     clampedBarycentric.time += time.time()-start
     return n, b, dispvector, b_cartesian, inside
 
-def barycentric2cartesian(bary, v1, v2, v3):
+def barycentric2cartesian(bary,
+                          v1,
+                          v2,
+                          v3):
+    """
+    Convert baricentric coordinates to cartesian coordinates
+
+    :param numpy.ndarray bary: baricentric coordinates
+    :param numpy.ndarray v1: first point of the triangle
+    :param numpy.ndarray v2: second point of the triangle
+    :param numpy.ndarray v3: third point of the triangle
+
+    :return: cartesian coordinates, normal vector
+    :rtype: numpy.ndarray, numpy.ndarray
+    """
     if len(bary)>3: bary=bary[:3]
     if len(v1)>3: v1=v1[:3]
     if len(v2)>3: v2=v2[:3]
     if len(v3)>3: v3=v3[:3]
     u = v2-v1
     v = v3-v1
     n = np.cross( u, v )
     cart = np.zeros(3)
     cart = bary[0]*v1 + bary[1]*v2 + bary[2]*v3
     return cart, n
 
-def getCentroid(p1,p2,p3):
+def getCentroid(p1,
+                p2,
+                p3):
+    """
+    Compute the centroid of a triangle defined by p1, p2 and p3.
+
+    :param numpy.ndarray p1: first point of the triangle
+    :param numpy.ndarray p2: second point of the triangle
+    :param numpy.ndarray p3: third point of the triangle
+
+    :return: centroid, normal vector
+    :rtype: numpy.ndarray, numpy.ndarray
+    """
     if len(p1)>3: p1=p1[:3]
     if len(p2)>3: p2=p2[:3]
     if len(p3)>3: p3=p3[:3]
     p1 = np.asarray(p1)
     p2 = np.asarray(p2)
     p3 = np.asarray(p3)
     u = p2-p1
     v = p3-p1
     n = unitVector(np.cross( u, v ))
     return np.mean([p1,p2,p3], axis=0), n
 
-def distFromCentroid(p, p1, p2, p3):
+def distFromCentroid(p,
+                     p1,
+                     p2,
+                     p3):
+    """
+    Compute the distance from a point p to the centroid of a triangle defined by p1, p2 and p3.
+
+    :param numpy.ndarray p: point of interest
+    :param numpy.ndarray p1: first point of the triangle
+    :param numpy.ndarray p2: second point of the triangle
+    :param numpy.ndarray p3: third point of the triangle
+    
+    :return: centroid, distance vector, normal vector
+    :rtype: numpy.ndarray, numpy.ndarray, numpy.ndarray
+    """
     if len(p)>3: p=p[:3]
     centroid, n = getCentroid(p1,p2,p3)
     distance = p-centroid
     return centroid, distance ,n
 
 
 
 def matrixSkew(vec):
+    """
+    Construct a skew-symmetric matrix from a vector. If the vector is 3D, the matrix will be 3x3. If the vector is 4D, the matrix will be 4x4.
+
+    :param numpy.ndarray vec: vector to be converted to skew-symmetric matrix
+
+    :return: skew-symmetric matrix
+    :rtype: numpy.ndarray
+    """
     if vec.shape[0] == 4:
         matrix = np.array([
                 [0,       -vec[2], vec[1],  0],
                 [vec[2],  0,       -vec[0], 0],
                 [-vec[1], vec[0],  0,       0],
                 [0,       0,       0,       1]
                 ])
@@ -319,22 +454,30 @@
             [-vec[1], vec[0],  0]
             ])
     else:
         print('Wrong vector shape, expected 3.')
         return None
     return matrix
 
-def alignVectors(a,b,shape=3):
-    """
-    Returns a rotation matrix to align vector a onto vector b
-    #https://math.stackexchange.com/questions/180418/calculate-rotation-matrix-to-align-vector-a-to-vector-b-in-3d
+def alignVectors(a,
+                 b,
+                 shape=3):
+    """
+    Returns a rotation matrix to align vector a onto vector b.
+    This matrix is not constructed as RxRyRz, but from an axis-angle representation.
+    
+    Based on the algorithm available at https://math.stackexchange.com/questions/180418/calculate-rotation-matrix-to-align-vector-a-to-vector-b-in-3d
 
+    :param numpy.ndarray a: vector to be aligned
+    :param numpy.ndarray b: vector to be aligned to
 
-    ESSA MATRIZ NÃO É CONSTRUIDA RxRyRz, MAS A PARTIR DE UM EIXO
+    :return: rotation matrix
+    :rtype: numpy.ndarray
     """
+
     start=time.time()
     if (shape != 3) and (shape != 4):
         print('Shape %i not supported to represent a rotation matrix at mathutils.alignVectores(). Please choose 3 or 4.' % shape)
         return matrixIdentity(3)
     a_norm = np.asarray(a / np.linalg.norm(a))
     b_norm = np.asarray(b / np.linalg.norm(b))
     aux_vector = np.cross(a_norm, b_norm)
@@ -360,39 +503,59 @@
         return matrixIdentity(shape)
     rotationMatrix = matrixIdentity(3)
     skew = matrixSkew(aux_vector)
     matrix = rotationMatrix + skew + np.dot(skew,skew)*(1/(1+cos))
     if shape==4:
         matrix = shape3ToShape4(matrix)
 
-
     alignVectors.time += time.time()-start
     alignVectors.count += 1
     return matrix
 
-def angleBetween(a,b):
+def angleBetween(a,
+                 b):
     """
-    Returns the euler angle between the vectors (from a to b)
+    Returns the euler angle between the vectors (from a to b) and the rotation axis
     https://stackoverflow.com/questions/15101103/euler-angles-between-two-3d-vectors
     http://www.euclideanspace.com/maths/geometry/rotations/conversions/angleToEuler/index.htm
     https://en.wikipedia.org/wiki/Rotation_formalisms_in_three_dimensions
+
+    :param numpy.ndarray a: vector to be aligned
+    :param numpy.ndarray b: vector to be aligned to
+
+    :return: angle between the vectors, axis of rotation
+    :rtype: float, numpy.ndarray
     """
     start = time.time()
     a_norm = a / np.linalg.norm(a)
     b_norm = b / np.linalg.norm(b)
     axis = np.cross(a_norm, b_norm)
     axis_norm = axis/np.linalg.norm(axis)
     angle = np.arccos(np.dot(a_norm, b_norm))
     angleBetween.time += time.time() - start
     angleBetween.count += 1
     return angle, axis_norm
     #axisAngleToEuler(aux_vector_norm,angle)
 
 #def axisAngleToEuler(axis,angle):
 
+def multiInterp(x,
+                xp,
+                arr):
+    """
+    Performs a linear interpolation like numpy.interp() but for multidimensional arrays. Interpolation is performed independently for each dimension.
+    
+    :param numpy.ndarray x: The x-coordinates at which to evaluate the interpolated values (same for all dimensions)
+    :param numpy.ndarray xp: The x-coordinates of the data points (same for all dimensions)
+    :param numpy.ndarray arr: Multi-dimensional array of data with the same length as xp along the interpolation axis.
+
+    :return: interpolated array
+    :rtype: numpy.ndarray
+    """
+    return np.array([np.interp(x, xp, arr[:,i]) for i in range(arr.shape[1])]).T
 
 def isnear(x,y, epsilon = 1e-4):
     if abs(x-y) < epsilon:
         return True
     else:
         return False
 
@@ -493,14 +656,20 @@
             matrix[0,0] = cy*cz-sy*sz = cos(y+z)
             matrix[1,0] = cy*sz+sy*cz = sen(y+z)
             matrix[0,2] = sy*cz+sz*cy = sen(y+z) = matrix[1,0]
             matrix[1,2] = sy*sz-cy*cz = -cos(y+z) = -matrix[0,0]
             z + y = atan2(matrix[1,0], -matrix[0,0])
             z = -y + atan2(matrix[1,0], -matrix[0,0])
 
+    order = 'ZYX'
+    ((RzRx)Ry) =
+        cos(y)cos(z)    sin(x)sin(y)cos(z)-cos(x)sen(z)   cos(x)sin(y)cos(z)+sen(x)sen(z)
+        cos(y)sin(z)    sin(x)sin(y)sin(z)+cos(x)cos(z)   cos(x)sin(y)sin(z)-sen(x)cos(z)
+        -sin(y)         sin(x)cos(y)                      cos(x)cos(y)
+
     :type matrix: numpy.ndarray
     :param matrix: 3x3 rotation matrix or 4x4 transform matrix
 
     :type order: string
     :param order: order of rotation (working only for ZXY)
     """
     start= time.time()
@@ -539,23 +708,42 @@
             elif isNear(matrix[2,1],1):
                 x1 = np.pi/2
                 y1 = 0
                 z1 = np.arctan2(matrix[1,0], -matrix[0,0]) #(-y)
             else:
                 x1,y1,z1=0,0,0
 
+    elif order == 'ZYX':
+        if not isNear(matrix[2,0],1) and not isNear(matrix[2,0], -1):
+            y1 = -np.arcsin(matrix[2,0])
+            #sin(pi-theta) = sin(theta)
+            #y2 = np.pi - y1
+            x1 = np.arctan2(matrix[2,1]/np.cos(y1),matrix[2,2]/np.cos(y1))
+            #x2 = np.arctan2(matrix[2,1]/np.cos(y2),matrix[2,2]/np.cos(y2))
+            z1 = np.arctan2(matrix[1,0]/np.cos(y1),matrix[0,0]/np.cos(y1))
+            #z2 = np.arctan2(matrix[1,0]/np.cos(y2),matrix[0,0]/np.cos(y2))
+        else:
+            warning = True
+            z1 = 0
+            if isNear(matrix[2,0],-1):
+                y1 = np.pi/2
+                x1 = np.arctan2(matrix[0,1], matrix[0,2])
+            elif isNear(matrix[2,0],1):
+                y1 = -np.pi/2
+                x1 = np.arctan2(-matrix[0,1], -matrix[0,2])
 
     #TODO: Corrigir
     elif order == 'XYZ':
         y1 = np.arccos(matrix[0,0])
         x1 = np.arccos(matrix[2,2]/matrix[0,0])
         z1 = np.arcsin(-matrix[1,0]/matrix[0,0])
         x2,y2,z2 =0,0,0
         if matrix[0,0] < 0.01:
             warning = True
+        raise ValueError('Order %s not implemented yet.' % order)
 
 #    return np.asarray([x1,y1,z1])*180/np.pi, np.asarray([x2,y2,z2])*180/np.pi, warning
 
     eulerFromMatrix.count+=1
     eulerFromMatrix.time+=time.time()-start
     return np.asarray([x1,y1,z1])*180/np.pi, warning
 
@@ -624,14 +812,17 @@
     rotz = matrixRotation(R[2],0,0,1)
     if order == "ZXY":
         matrix = np.dot(rotz, rotx)
         matrix = np.dot(matrix, roty)
     elif order == "XYZ":
         matrix = np.dot(rotx, roty)
         matrix = np.dot(matrix, rotz)
+    elif order == "ZYX":
+        matrix = np.dot(rotz, roty)
+        matrix = np.dot(matrix, rotx)
     else:
         print('mathutils.matrixR does not accept rotation order %s' %order)
     if shape == 3:
         matrix = shape4ToShape3(matrix)
     return matrix
 
 
@@ -755,15 +946,14 @@
 def capsuleCollision(point, p0, p1, capradius):
     """
     Creates a capsule (extruded sphere): a cylinder with radius capradius and two half spheres (top and bottom) with radius capradius
     Returns the normalized intersection LOCAL cylindric coordinates and the intersection GLOBAL euclidean coordinates
 
     Surface: x^2+y^2+(1/4)*(|z-caplength|+|z+caplength| - 2*caplength)^2 - capradius^2 = 0
 
-
     Example:
     caplength = 10
     capradius = 2
     if z=5:
         x^2+y^2+(1/4)*(|5-10|+|5+10| - 2*10)^2 - 2^2 = 0
         x^2+y^2+(1/4)*(20 - 20)^2 - 2^2 = 0
         x^2+y^2 - 4 = 0
@@ -781,15 +971,14 @@
         (Outside cylinder)
     if z=11:
         x^2+y^2+(1/4)*(|11-10|+|11+10| - 2*10)^2 - 2^2 = 0
         x^2+y^2+(1/4)*(22 - 20)^2 - 2^2 = 0
         x^2+y^2+ 1 - 4 = 0
         x^2+y^2 - 3 = 0
         (Analogous to z=5)
-
     Finding surface starting from [0,0,0] and moving along direction=[a,b,c] with step=t
     (a*t)^2+(b*t)^2+(1/4)*(|(z*t)-caplength|+|(z*t)+caplength| - 2*caplength)^2 - capradius^2 = 0
 
     :type point: numpy.ndarray
     :param point: Point outside the capsule to give the direction of the collinsion vector (from the origin to the point)
 
     :type p0: numpy.ndarray
```

### Comparing `bvhsdk-0.1.0/bvhsdk/plotanimation.py` & `bvhsdk-0.2.0/bvhsdk/plotanimation.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,14 +5,177 @@
 from matplotlib.animation import FuncAnimation
 from mpl_toolkits.mplot3d import Axes3D
 
 plt.rcParams['font.family'] = 'serif'
 plt.rcParams["font.serif"] = "Times New Roman"
 plt.rcParams["font.size"] = 20.0
 
+def plot3d(animation,
+           mode = 'bones',
+           frameDelay = 0,
+           viewPlane = 0,
+           floorPlane = True,
+           skiproot = 0,
+           dist = 7,
+           figsize = (12,8),
+           color = 'black',
+           marker='o', 
+           linestyle='-', 
+           markersize=2,
+           ):
+    """
+    Plot BVH animation joints. Currently assumes Y-up character.
+    Supports 3D scatter plot and bones plot ('scatter' and 'bones' modes, respectively).
+
+    Ipython Jupyter Notebook-friendly function.
+    Make sure to include the following line in your notebook:
+    %matplotlib notebook
+    import matplotlib
+    matplotlib.rc('animation', html='html5')
+    These lines may also be necessary:
+    from ipywidgets import interact, interactive, widgets
+    from IPython.display import display
+    
+    :param anim.Animation animation: Animation object to be draw
+    :param str mode: Choose between 'bones' or 'scatter' modes. 'bones' will draw the bones of the skeleton, 'scatter' will draw the joints as points.
+    :param int frameDelay: Interval or delay between frames of matplotlib's FuncAnimation function in miliseconds. If 0, use animation's frametime to match intended fps from BVH file.
+    :param int viewPlane: Primary view plane option (choose between 1 and )
+    :param bool floorPlane: If True, draw a XZ plane with Y = 0 as reference.
+    :param int skiproot: Skip the first skiproot joints in the hierarchy. Useful when the skeleton has a body world reference or an origin joint.
+    :param float dist: Distance from the camera to the plot. Matplotlib default is 10.
+    :param tuple figsize: Figure size in inches.
+    :param str color: Color of the plot elements.
+    :param str marker: Marker style for scatter plot.
+    :param str linestyle: Line style for bones plot.
+    :param int markersize: Marker size for scatter plot.
+
+    :return: Return a matplotlib.animation object containing the animation.
+    :rtype: matplotlib.animation
+    """
+    fig = plt.figure(figsize=figsize)
+    ax = fig.add_subplot(111, projection='3d')
+
+    print('Precomputing positions...')
+    precomp_positions = [joint.getPosition(frame) for frame in range(animation.frames) for joint in animation.getlistofjoints()]
+    precomp_positions = np.reshape(np.asarray(precomp_positions), newshape = (animation.frames, len(animation.getlistofjoints()), 3))
+    # precomp_positions shape: (frames, joints, xyz)
+
+    frameDelay = int(animation.frametime * 1000) if frameDelay == 0 else frameDelay
+
+    mindata = np.min(precomp_positions)
+    maxdata = np.max(precomp_positions)
+
+    if mode == 'bones':
+        ani = plot3DBones(animation, fig, ax, precomp_positions, frameDelay, color, skiproot, marker, linestyle, markersize)
+    elif mode == 'scatter':
+        ani = plot3DJoints(animation, fig, ax, precomp_positions, frameDelay, color, marker, markersize)
+    else:
+        print('Invalid mode. Choose between "bones" or "scatter".')
+        return None
+
+    mindata = np.min(precomp_positions)
+    maxdata = np.max(precomp_positions)
+    ax.set_xlim(mindata,maxdata)
+    ax.set_ylim(mindata,maxdata)
+    ax.set_zlim(mindata,maxdata)
+
+    # Draw floor plane
+    if floorPlane:
+        sx, sz = np.meshgrid(range(-int(maxdata), int(maxdata)), range(-int(maxdata), int(maxdata)))
+        sy = np.zeros(shape=sx.shape)
+        ax.plot_surface(sx, sy, sz, alpha=0.2)
+    
+    # Set initial view direction
+    if viewPlane:
+        # (plane, (elev, azim, roll))
+        views = [('XY',   (90, -90, 0)),
+                ('XZ',    (0, -90, 0)),
+                ('YZ',    (0,   0, 0)),
+                ('-XY', (-90,  90, 0)),
+                ('-XZ',   (0,  90, 0)),
+                ('-YZ',   (0, 180, 0))]
+        angles = views[viewPlane - 1][1]
+        ax.view_init(elev=angles[0], azim=angles[1])
+    else:
+        ax.view_init(elev=100, azim=-90)
+        
+    if dist:
+        ax.dist=dist
+        
+    ax.grid(False)
+    ax.axis('off')
+
+    return ani
+    
+def plot3DJoints(animation, 
+            fig,
+            ax,
+            precomp_positions,
+            frameDelay,
+            color,
+            marker,
+            markersize,
+            ):
+    def update(frame, scatters, precomp_positions):
+        for scat, joint, i in zip(scatters, animation.getlistofjoints(), range(len(animation.getlistofjoints()))):
+            if precompute:
+                position = precomp_positions[frame, i]
+            else:
+                position = joint.getPosition(frame)
+            scat.set_data([position[0]],[position[1]])
+            scat.set_3d_properties([position[2]])
+
+        return scatters
+        
+    scatters = []
+    for i, _ in enumerate(animation.getlistofjoints()):
+        position = precomp_positions[0, i]
+        scatters.append(ax.plot([position[0]],[position[1]],[position[2]], marker=marker, color=color, markersize=markersize)[0])
+    
+    ani = FuncAnimation(fig, update, frames=np.arange(animation.frames), fargs=([scatters, precomp_positions]) ,interval=frameDelay, blit=True)
+    plt.show()
+    return ani
+
+def plot3DBones(animation,
+                  fig,
+                  ax,
+                  precomp_positions,
+                  frameDelay,
+                  color,
+                  skiproot,
+                  marker,
+                  linestyle,
+                  markersize,
+                  ):
+
+    def update(frame, lines, precomp_positions, parents):
+        for line, i in zip(lines, range(len(parents)-len(lines), len(parents))): # This range is to account for skiproot
+            x = [precomp_positions[frame, parents[i], 0], precomp_positions[frame, i, 0]]
+            y = [precomp_positions[frame, parents[i], 1], precomp_positions[frame, i, 1]]
+            z = [precomp_positions[frame, parents[i], 2], precomp_positions[frame, i, 2]]
+            line.set_data(x,y)
+            line.set_3d_properties(z)
+        return lines
+            
+    parents = animation.arrayParent()
+    
+    lines = []
+    for i in range(skiproot, len(parents)):
+        x = [precomp_positions[0, parents[i], 0], precomp_positions[0 , i, 0]]
+        y = [precomp_positions[0, parents[i], 1], precomp_positions[0 , i, 1]]
+        z = [precomp_positions[0, parents[i], 2], precomp_positions[0 , i, 2]]
+        lines.append(ax.plot(x, y, z, marker=marker, linestyle=linestyle, markersize=markersize, c=color)[0])  
+    
+    ani = FuncAnimation(fig, update, frames=np.arange(animation.frames), fargs=([lines, precomp_positions, parents]),
+                        interval=frameDelay, blit=True)
+
+    
+    plt.show()
+    return ani
+
 def AnimPlot(data):
 
     def update(frame):
         xdata, ydata, zdata = [], [], []
         #print("-------------------Frame: %f"%(frame))
         #xdata.append(data[frame,0,:])
         #ydata.append(data[frame,1,:])
@@ -41,47 +204,14 @@
 
     fig = plt.figure(figsize=(12,8))
     ax = fig.add_subplot(111, projection='3d')
     xdata, ydata, zdata = [], [], []
     ln, = plt.plot([], [], 'ro', animated=True)
     animate()
 
-def AnimPlotBones(data):
-
-    def update(frame, lines, data):
-        print(frame)
-        for line, dataBone in zip(lines, data):
-            x = np.asarray([dataBone[0,frame], dataBone[4,frame]])
-            y = np.asarray([dataBone[1,frame], dataBone[5,frame]])
-            z = np.asarray([dataBone[2,frame], dataBone[6,frame]])
-            line.set_data(x,y)
-            line.set_3d_properties(z)
-        return lines
-
-    fig = plt.figure(figsize=(12,8))
-    ax = fig.add_subplot(111, projection='3d')
-
-    lines = []
-    for i in range(len(data)):
-        lines.append(ax.plot([data[i,0,0], data[i,4,0]], [data[i,1,0], data[i,5,0]], [data[i,2,0], data[i,6,0]],'-o', c='black')[0])
-
-
-    ax.set_xlabel('X Label')
-    ax.set_ylabel('Y Label')
-    ax.set_zlabel('Z Label')
-    mini,maxi = np.min(data), np.max(data)
-    ax.set_xlim(mini,maxi)
-    ax.set_ylim(mini,maxi)
-    ax.set_zlim(mini,maxi)
-    ani = FuncAnimation(fig, update, frames=np.arange(len(data[0,0,:])), fargs=(lines, data),interval=2,
-                             blit=True)
-
-    plt.show()
-
-
 def AnimPlotBones2D(data, plotax='xy'):
 
     def update(frame, lines, data, ax1, ax2):
         for line, dataBone in zip(lines, data):
             x = np.asarray([dataBone[ax1[0],frame], dataBone[ax1[1],frame]])
             y = np.asarray([dataBone[ax2[0],frame], dataBone[ax2[1],frame]])
             line.set_data(x,y)
@@ -512,57 +642,14 @@
         ax.plot([Upspine[0],LArm[0]],[Upspine[1],LArm[1]], '-o',color='yellow')
         ax.plot([RArm[0],RFore[0]],[RArm[1],RFore[1]], '-o',color='red')
         ax.plot([LArm[0],LFore[0]],[LArm[1],LFore[1]], '-o',color='red')
         ax.plot([RFore[0],RHand[0]],[RFore[1],RHand[1]], '-o',color='blue')
         ax.plot([LFore[0],LHand[0]],[LFore[1],LHand[1]], '-o',color='blue')
         plt.show()
 
-def PlotBVH(animation):
-    """
-    Plot animation as BVH, calculate the position inside this funtion
-
-    :type animation: Animation class object
-    :param animation: Animation to be draw
-    """
-    def update(frame, scatters):
-        print(frame)
-        for scat, joint in zip(scatters,animation.getlistofjoints()):
-            position = joint.getPosition(frame)
-            scat.set_data([position[0]],[position[1]])
-            scat.set_3d_properties([position[2]])
-
-        return scatters
-
-    fig = plt.figure(figsize=(12,8))
-    ax = fig.add_subplot(111, projection='3d')
-
-    scatters = []
-    maxdata = -np.inf
-    mindata = np.inf
-    for joint in animation.getlistofjoints():
-        position = joint.getPosition(frame = 0)
-        scatters.append(ax.plot([position[0]],[position[1]],[position[2]],'o', color='red', markersize=1)[0])
-        if np.min(position)<mindata:
-            mindata = np.min(position)
-        if np.max(position)>maxdata:
-            maxdata = np.max(position)
-
-    ax.set_xlabel('X Label')
-    ax.set_ylabel('Y Label')
-    ax.set_zlabel('Z Label')
-    ax.set_xlim(mindata,maxdata)
-    ax.set_ylim(mindata,maxdata)
-    ax.set_zlim(mindata,maxdata)
-
-    ani = FuncAnimation(fig, update, frames=np.arange(animation.frames), fargs=([scatters]) ,interval=1, blit=True)
-
-    plt.show()
-    return ani
-
-
 def PlotBVHSurface(animation, surface):
     def update(frame, surf, lines):
         for triangle_plot, i in zip(surf, range(len(surface.headmesh)+len(surface.bodymesh))):
             if i< len(surface.headmesh):
                 vertices = [[vert.getPosition(animation,frame)[0],vert.getPosition(animation,frame)[1],vert.getPosition(animation,frame)[2]] for vert in surface.headmesh[i]]
                 vertices.append([surface.headmesh[i][0].getPosition(animation,frame)[0],surface.headmesh[i][0].getPosition(animation,frame)[1],surface.headmesh[i][0].getPosition(animation,frame)[2]])
                 vertices = np.asarray(vertices)
```

### Comparing `bvhsdk-0.1.0/bvhsdk/retarget.py` & `bvhsdk-0.2.0/bvhsdk/retarget.py`

 * *Files identical despite different names*

### Comparing `bvhsdk-0.1.0/bvhsdk/skeletonmap.py` & `bvhsdk-0.2.0/bvhsdk/skeletonmap.py`

 * *Files identical despite different names*

### Comparing `bvhsdk-0.1.0/bvhsdk/surface.py` & `bvhsdk-0.2.0/bvhsdk/surface.py`

 * *Files identical despite different names*

### Comparing `bvhsdk-0.1.0/pyproject.toml` & `bvhsdk-0.2.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,34 @@
-[build-system]
-requires = ["flit_core >= 3.8, <4"]
-build-backend = "flit_core.buildapi"
-
-[project]
-name = "bvhsdk"
-version = "0.1.0"
-authors = [
-  { name="Rodolfo Luis Tonoli", email="rltonoli@gmail.com" },
-]
-description = "A package that handles bvh files in python. You can read, write, and modify your bvh files among other useful tools."
-readme = "README.md"
-requires-python = ">=3.7"
-classifiers = [
-    "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: MIT License",
-    "Operating System :: OS Independent",
-]
-dependencies = [
-    "matplotlib >= 3.5.3",
-    "numpy >= 1.21.6",
-]
-
-[project.optional-dependencies]
-doc = [
-    "sphinx >= 7",
-    "furo",
-    "sphinx-rtd-theme",
-]
-
-[project.urls]
-"Homepage" = "https://github.com/rltonoli/bvhsdk"
+[build-system]
+requires = ["flit_core >= 3.8, <4"]
+build-backend = "flit_core.buildapi"
+
+[project]
+name = "bvhsdk"
+version = "0.2.0"
+authors = [
+  { name="Rodolfo Luis Tonoli", email="rltonoli@gmail.com" },
+]
+description = "A package that handles bvh files in python. You can read, write, and modify your bvh files among other useful tools."
+readme = "README.md"
+requires-python = ">=3.7"
+classifiers = [
+    "Programming Language :: Python :: 3",
+    "License :: OSI Approved :: MIT License",
+    "Operating System :: OS Independent",
+]
+dependencies = [
+    "matplotlib >= 3.5.3",
+    "numpy >= 1.21.6",
+]
+
+[project.optional-dependencies]
+doc = [
+    "sphinx >= 7",
+    "furo",
+    "sphinx-rtd-theme",
+    "myst-parser",
+]
+
+[project.urls]
+"Homepage" = "https://github.com/rltonoli/bvhsdk"
 "Bug Tracker" = "https://github.com/rltonoli/bvhsdk/issues"
```

