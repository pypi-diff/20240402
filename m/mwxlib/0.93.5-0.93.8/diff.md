# Comparing `tmp/mwxlib-0.93.5-py3-none-any.whl.zip` & `tmp/mwxlib-0.93.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,25 +1,29 @@
-Zip file size: 163432 bytes, number of entries: 23
+Zip file size: 171873 bytes, number of entries: 27
 -rw-rw-rw-  2.0 fat     2398 b- defN 23-Nov-10 02:50 mwx/__init__.py
 -rw-rw-rw-  2.0 fat     6613 b- defN 23-Dec-31 14:58 mwx/bookshelf.py
 -rw-rw-rw-  2.0 fat    47173 b- defN 24-Feb-13 09:50 mwx/controls.py
--rw-rw-rw-  2.0 fat    73951 b- defN 24-Feb-20 17:19 mwx/framework.py
--rw-rw-rw-  2.0 fat    70267 b- defN 24-Mar-21 10:46 mwx/graphman.py
+-rw-rw-rw-  2.0 fat    73951 b- defN 24-Mar-27 17:24 mwx/framework.py
+-rw-rw-rw-  2.0 fat    70156 b- defN 24-Mar-27 17:24 mwx/graphman.py
 -rw-rw-rw-  2.0 fat    49957 b- defN 23-Oct-30 22:59 mwx/images.py
--rw-rw-rw-  2.0 fat    32761 b- defN 24-Feb-20 17:19 mwx/matplot2.py
--rw-rw-rw-  2.0 fat    65552 b- defN 24-Feb-20 17:19 mwx/matplot2g.py
--rw-rw-rw-  2.0 fat    26343 b- defN 24-Feb-20 17:19 mwx/matplot2lg.py
+-rw-rw-rw-  2.0 fat    32682 b- defN 24-Mar-26 09:41 mwx/matplot2.py
+-rw-rw-rw-  2.0 fat    65585 b- defN 24-Mar-26 09:41 mwx/matplot2g.py
+-rw-rw-rw-  2.0 fat    27653 b- defN 24-Mar-27 17:24 mwx/matplot2lg.py
 -rw-rw-rw-  2.0 fat     5671 b- defN 23-Dec-23 15:51 mwx/mgplt.py
 -rw-rw-rw-  2.0 fat   135816 b- defN 24-Feb-15 03:46 mwx/nutshell.py
--rw-rw-rw-  2.0 fat    37040 b- defN 24-Feb-15 03:46 mwx/utilus.py
+-rw-rw-rw-  2.0 fat    37040 b- defN 24-Mar-27 17:24 mwx/utilus.py
 -rw-rw-rw-  2.0 fat    12717 b- defN 24-Feb-16 07:48 mwx/wxmon.py
 -rw-rw-rw-  2.0 fat    19129 b- defN 24-Feb-13 10:31 mwx/wxpdb.py
 -rw-rw-rw-  2.0 fat     5578 b- defN 24-Feb-13 10:31 mwx/wxwil.py
 -rw-rw-rw-  2.0 fat     7557 b- defN 24-Feb-27 17:09 mwx/wxwit.py
--rw-rw-rw-  2.0 fat        0 b- defN 23-Jan-23 14:06 mwx/py/__init__.py
+-rw-rw-rw-  2.0 fat       39 b- defN 24-Mar-27 17:24 mwx/py/__init__.py
+-rw-rw-rw-  2.0 fat     9399 b- defN 24-Mar-27 17:24 mwx/py/ffmpeg_view.py
+-rw-rw-rw-  2.0 fat     2675 b- defN 24-Mar-27 17:24 mwx/py/fft_view.py
 -rw-rw-rw-  2.0 fat    16806 b- defN 23-Nov-10 02:50 mwx/py/filling.py
--rw-rw-rw-  2.0 fat     1091 b- defN 24-Mar-22 05:08 mwxlib-0.93.5.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1925 b- defN 24-Mar-22 05:08 mwxlib-0.93.5.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Mar-22 05:08 mwxlib-0.93.5.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        4 b- defN 24-Mar-22 05:08 mwxlib-0.93.5.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1682 b- defN 24-Mar-22 05:08 mwxlib-0.93.5.dist-info/RECORD
-23 files, 620123 bytes uncompressed, 160822 bytes compressed:  74.1%
+-rw-rw-rw-  2.0 fat    10110 b- defN 24-Mar-27 17:24 mwx/py/frame_listview.py
+-rw-rw-rw-  2.0 fat      816 b- defN 24-Mar-27 17:24 mwx/py/line_profile.py
+-rw-rw-rw-  2.0 fat     1091 b- defN 24-Apr-02 09:06 mwxlib-0.93.8.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     1925 b- defN 24-Apr-02 09:06 mwxlib-0.93.8.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-02 09:06 mwxlib-0.93.8.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        4 b- defN 24-Apr-02 09:06 mwxlib-0.93.8.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1996 b- defN 24-Apr-02 09:06 mwxlib-0.93.8.dist-info/RECORD
+27 files, 644629 bytes uncompressed, 168789 bytes compressed:  73.8%
```

## zipnote {}

```diff
@@ -45,26 +45,38 @@
 
 Filename: mwx/wxwit.py
 Comment: 
 
 Filename: mwx/py/__init__.py
 Comment: 
 
+Filename: mwx/py/ffmpeg_view.py
+Comment: 
+
+Filename: mwx/py/fft_view.py
+Comment: 
+
 Filename: mwx/py/filling.py
 Comment: 
 
-Filename: mwxlib-0.93.5.dist-info/LICENSE
+Filename: mwx/py/frame_listview.py
+Comment: 
+
+Filename: mwx/py/line_profile.py
+Comment: 
+
+Filename: mwxlib-0.93.8.dist-info/LICENSE
 Comment: 
 
-Filename: mwxlib-0.93.5.dist-info/METADATA
+Filename: mwxlib-0.93.8.dist-info/METADATA
 Comment: 
 
-Filename: mwxlib-0.93.5.dist-info/WHEEL
+Filename: mwxlib-0.93.8.dist-info/WHEEL
 Comment: 
 
-Filename: mwxlib-0.93.5.dist-info/top_level.txt
+Filename: mwxlib-0.93.8.dist-info/top_level.txt
 Comment: 
 
-Filename: mwxlib-0.93.5.dist-info/RECORD
+Filename: mwxlib-0.93.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mwx/framework.py

```diff
@@ -1,11 +1,11 @@
 #! python3
 """mwxlib framework.
 """
-__version__ = "0.93.5"
+__version__ = "0.93.8"
 __author__ = "Kazuya O'moto <komoto@jeol.co.jp>"
 
 from functools import wraps, partial
 from importlib import reload
 from contextlib import contextmanager
 import traceback
 import warnings
```

## mwx/graphman.py

```diff
@@ -29,14 +29,27 @@
 from .utilus import funcall as _F
 from .controls import ControlPanel, Icon
 from .framework import CtrlInterface, AuiNotebook
 from .matplot2g import GraphPlot
 from .matplot2lg import Histogram
 
 
+def split_paths(obj):
+    """Split obj path into dirname and basename.
+    The object can be module name:str, module, or class.
+    """
+    if hasattr(obj, '__file__'): #<class 'module'>
+        obj = obj.__file__
+    elif isinstance(obj, type):  #<class 'type'>
+        obj = inspect.getsourcefile(obj)
+    if obj.endswith(".py"):
+        obj, _ = os.path.splitext(obj)
+    return os.path.split(obj)
+
+
 class Thread(object):
     """Thread manager for graphman.Layer
     
     The worker:thread runs the given target.
     
     Attributes:
         target  : A target method of the Layer.
@@ -1058,36 +1071,22 @@
         
         _Plugin.__module__ = cls.__module__ = module.__name__
         _Plugin.__name__ = cls.__name__ + str("~")
         _Plugin.__doc__ = cls.__doc__
         module.Plugin = _Plugin
         return _Plugin
     
-    @staticmethod
-    def _split_paths(root):
-        if hasattr(root, '__file__'): #<class 'module'>
-            name = root.__file__
-        elif isinstance(root, type):  #<class 'type'>
-            name = inspect.getsourcefile(root)
-        else:
-            name = root
-        dirname = os.path.dirname(name)
-        name = os.path.basename(name)
-        if name.endswith(".py"):
-            name, _ = os.path.splitext(name)
-        return dirname, name
-    
     def load_module(self, root):
         """Load module of plugin (internal use only).
         
         Note:
             This is called automatically from load_plug,
             and should not be called directly from user.
         """
-        dirname_, name = self._split_paths(root)
+        dirname_, name = split_paths(root)
         
         ## Update the include-path to load the module correctly.
         if os.path.isdir(dirname_):
             if dirname_ in sys.path:
                 sys.path.remove(dirname_)
             sys.path.insert(0, dirname_)
         elif dirname_:
@@ -1143,18 +1142,18 @@
         
         Note:
             The root module must have a class Plugin <Layer>
         """
         props = dict(show=show, dock=dock, layer=layer, pos=pos, row=row, prop=prop,
                      floating_pos=floating_pos, floating_size=floating_size)
         
-        _dirname, name = self._split_paths(root)
+        _dirname, name = split_paths(root)
         
         plug = self.get_plug(name)
-        if plug and not force: # <plug:name> is already registered.
+        if plug and not force:
             self.update_pane(name, **props)
             try:
                 if session:
                     plug.load_session(session)
             except Exception as e:
                 traceback.print_exc()
                 print("- Failed to load session of", plug)
```

## mwx/matplot2.py

```diff
@@ -293,16 +293,16 @@
         self.selected.set_data([], [])
         
         #<matplotlib.widgets.Cursor>
         self.cursor = Cursor(self.axes, useblit=True, color='grey', linewidth=1)
         self.cursor.visible = 1
     
     def draw(self, art=None):
-        """Draw the plot.
-        Called every time the drawing is updated.
+        """Draw plots.
+        Call each time the drawing should be updated.
         """
         if isinstance(art, matplotlib.artist.Artist):
             self.axes.draw_artist(art)
             self.canvas.blit(art.get_clip_box())
             ## self.canvas.draw_idle()
         else:
             self.handler('canvas_draw', self.frame)
@@ -399,24 +399,24 @@
     
     ## --------------------------------
     ## External I/O file and clipboard 
     ## --------------------------------
     
     def copy_to_clipboard(self):
         """Copy canvas image to clipboard."""
-        self.message("Copy image to clipboard.")
+        ## b = self.selected.get_visible()
+        c = self.cursor.visible
         try:
-            b = self.selected.get_visible()
-            c = self.cursor.visible
-            self.selected.set_visible(0)
+            ## self.selected.set_visible(0)
             self.cursor.visible = 0
             self.canvas.draw()
             self.canvas.Copy_to_Clipboard()
+            self.message("Copy image to clipboard.")
         finally:
-            self.selected.set_visible(b)
+            ## self.selected.set_visible(b)
             self.cursor.visible = c
             self.canvas.draw()
     
     ## --------------------------------
     ## Selector interface
     ## --------------------------------
     
@@ -600,18 +600,14 @@
     
     ## --------------------------------
     ## Pan/Zoom actions 
     ## --------------------------------
     
     ZOOM_RATIO = 10**0.2
     
-    def update_position(self):
-        self.toolbar.update()
-        self.toolbar.push_current()
-    
     def OnDraw(self, evt):
         """Called before canvas.draw."""
         pass
     
     def OnMotion(self, evt):
         """Called when mouse moves in axes."""
         if not self.Selector.size:
@@ -626,20 +622,22 @@
         """Go backward view position."""
         self.toolbar.back()
         self.draw()
     
     def OnHomePosition(self, evt):
         """Go back to home position."""
         self.toolbar.home()
-        self.update_position()
+        self.toolbar.update()
+        self.toolbar.push_current()
         self.draw()
     
     def OnEscapeSelection(self, evt):
         """Escape from selection."""
         del self.Selector
+        self.canvas.draw_idle()
     
     ## def OnShiftLimit(self, evt, r=0.1):
     ##     w = self.xlim[1] - self.xlim[0]
     ##     h = self.ylim[1] - self.ylim[0]
     ##     if 'up' in evt.key: self.ylim += h * r
     ##     elif 'down' in evt.key: self.ylim -= h * r
     ##     elif 'left' in evt.key: self.xlim -= w * r
@@ -682,30 +680,28 @@
         self.toolbar.pan()
         self.__prev = self.handler.previous_state # save previous state of PAN
     
     def OnPanEnd(self, evt):
         ## self.toolbar.set_cursor(1)
         self.set_wxcursor(wx.CURSOR_ARROW)
         self.toolbar.pan()
-        ## self.draw()
         self.handler.current_state = self.__prev  # --> previous state of PAN
         del self.__prev
     
     def OnZoomBegin(self, evt):
         """Toolbar zoom - While zooming, press x/y to constrain the direction."""
         ## self.toolbar.set_cursor(3)
         self.set_wxcursor(wx.CURSOR_CROSS)
         self.toolbar.zoom()
         self.__prev = self.handler.previous_state # save previous state of ZOOM
     
     def OnZoomEnd(self, evt):
         ## self.toolbar.set_cursor(1)
         self.set_wxcursor(wx.CURSOR_ARROW)
         self.toolbar.zoom()
-        ## self.draw()
         self.handler.current_state = self.__prev  # --> previous state of ZOOM
         del self.__prev
     
     ## def OnZoomMove(self, evt):
     ##     """Zoom."""
     ##     ## http://aspn.activestate.com/ASPN/Cookbook/Python/Recipe/189744
     ##     ## matplotlib.backends.backend_wx - NavigationToolbar2Wx.draw_rubberband
```

## mwx/matplot2g.py

```diff
@@ -859,15 +859,16 @@
     def kill_buffer_all(self):
         del self[:]
     
     def update_axis(self):
         """Reset display range (xylim's), update home position."""
         if self.frame:
             self.axes.axis(self.frame.get_extent()) # reset xlim and ylim
-            self.update_position()
+            self.toolbar.update()
+            self.toolbar.push_current()
             self.draw()
     
     def fit_to_canvas(self):
         """fit display range (xylim's) to canvas."""
         x, y = self.xlim, self.ylim
         w, h = self.canvas.GetSize()
         r = h/w
@@ -976,46 +977,46 @@
     ## 外部入出力／複合インターフェース
     ## --------------------------------
     ## GraphPlot 間共有のグローバル変数
     clipboard_name = None
     clipboard_data = None
     
     def write_buffer_to_clipboard(self):
-        """Copy - Write buffer data to clipboard."""
+        """Write buffer data to clipboard."""
         if not self.frame:
             self.message("No frame")
             return
         try:
-            self.message("Write buffer to clipboard.")
             name = self.frame.name
             data = self.frame.roi
             GraphPlot.clipboard_name = name
             GraphPlot.clipboard_data = data
             bins, vlim, img = imconvert(data, self.frame.vlim)
             Clipboard.imwrite(img)
+            self.message("Write buffer to clipboard.")
         except Exception as e:
-            self.message("- Failure in clipboard:", e)
             traceback.print_exc()
+            self.message("- Failed to write to clipboard:", e)
     
     def read_buffer_from_clipboard(self):
-        """Paste - Read buffer data from clipboard."""
+        """Read buffer data from clipboard."""
         try:
             name = GraphPlot.clipboard_name
             data = GraphPlot.clipboard_data
             if name:
                 self.message("Read buffer from clipboard.")
                 self.load(data)
                 GraphPlot.clipboard_name = None
                 GraphPlot.clipboard_data = None
             else:
                 self.message("Read image from clipboard.")
                 self.load(Clipboard.imread())
         except Exception as e:
-            self.message("- No data in clipboard:", e)
             traceback.print_exc()
+            self.message("- No data in clipboard:", e)
     
     def destroy_colorbar(self):
         if self.cbar:
             self.cbar = None
             cax = self.figure.axes[1]
             self.figure.delaxes(cax)
             self.canvas.draw_idle()
```

## mwx/matplot2lg.py

```diff
@@ -22,20 +22,24 @@
     
     region : selected range (l,r) on the plot
     """
     def __init__(self, *args, **kwargs):
         MatplotPanel.__init__(self, *args, **kwargs)
         
         self.handler.update({ # DNA<LinePlot>
+            None : {
+                   'region_set' : [ None ],
+                 'region_unset' : [ None ],
+            },
             NORMAL : {
                'escape pressed' : (NORMAL, self.OnEscapeSelection),
                'delete pressed' : (NORMAL, self.OnEscapeSelection),
                   'M-a pressed' : (NORMAL, self.OnHomePosition),
                   'C-a pressed' : (NORMAL, self.OnHomePosition),
-             'Lbutton dblclick' : (NORMAL, self.OnEscapeSelection),
+             'Lbutton dblclick' : (NORMAL, self.OnEscapeSelection, self.OnDragLock),
              '*Lbutton pressed' : (NORMAL, self.OnDragLock),
                  '*Ldrag begin' : (REGION, self.OnDragBegin),
             },
             REGION : {
                   '*Ldrag move' : (REGION, self.OnDragMove),
                    '*Ldrag end' : (NORMAL, self.OnDragEnd),
             },
@@ -74,18 +78,20 @@
                 if   a < l: a = l
                 elif a > r: a = r
                 if   b < l: b = l
                 elif b > r: b = r
             v = np.array((a, b))
             self.__vspan.set_visible(1)
             self.__vspan.set_xy(((a,0), (a,1), (b,1), (b,0)))
+            self.handler('region_set', self.frame)
         else:
             self.__vspan.set_visible(0)
+            self.handler('region_unset', self.frame)
         self.__region = v
-        
+    
     @region.deleter
     def region(self):
         self.region = None
     
     def annotate(self):
         for art in self.__annotations:
             art.remove()
@@ -162,40 +168,45 @@
     def OnDragMove(self, evt):
         x = evt.xdata
         if self.__selection != 1:
             l, r = self.xbound
             if   x < l: x = l
             elif x > r: x = r
             self.region = (self.__lastpoint, x)
-        else:
+        elif self.region is not None:
             a, b = self.region
             d = x - self.__lastpoint
             if self.boundary is not None:
                 l, r = self.boundary
                 if a+d < l:
                     self.region = (l, l+b-a)
                 elif b+d > r:
                     self.region = (r-b+a, r)
                 else:
                     self.region = (a+d, b+d)
                     self.__lastpoint = x
             else:
                 self.region = (a+d, b+d)
                 self.__lastpoint = x
+        else:
+            self.message("- No region.") #<FSM logic-error>
         self.draw()
+        ## self.handler('region_draw', self.frame)
     
     def OnDragEnd(self, evt):
         self.set_wxcursor(wx.CURSOR_ARROW)
+        ## self.handler('region_drawn', self.frame)
     
     def OnEscapeSelection(self, evt):
         MatplotPanel.OnEscapeSelection(self, evt)
         
         self.set_wxcursor(wx.CURSOR_ARROW)
         self.region = None
         self.draw()
+        ## self.handler('region_removed', self.frame)
 
 
 class Histogram(LinePlot):
     """LinePlot panel for histogram (Multi-graph : Single-frame)
     
     frame.image <uint8> (buffer ではない) を参照して，ヒストグラムをプロットする
     常に整数ビット画像となるので，高速なビンづめ法で計算する
@@ -278,15 +289,16 @@
         self.__frame = frame # update reference of the frame
         if frame:
             x, y = frame.__data = self.calc(frame) # histogram_data buffer
             self.__plot.set_data(x, y)
             self.xlim = x.min(), x.max()
             self.ylim = 0, y.max()
             self.region = None
-            self.update_position()
+            self.toolbar.update()
+            self.toolbar.push_current()
             self.draw()
     
     def hreplot(self, frame):
         self.__frame = frame # update reference of the frame
         if frame:
             try:
                 image = self.frmae.image
@@ -304,15 +316,16 @@
                 self.region = (a, b)
             else:
                 self.region = None
         else:
             self.__plot.set_data([], [])
             self.region = None
         
-        self.update_position()
+        self.toolbar.update()
+        self.toolbar.push_current()
         self.draw()
     
     def writeln(self):
         if not self.modeline.IsShown():
             return
         frame = self.__frame
         if frame:
@@ -388,17 +401,17 @@
             NORMAL : {
             'S-Lbutton pressed' : (LINE, self.OnDragLock, self.OnRegionLock),
             'M-Lbutton pressed' : (MARK, self.OnDragLock, self.OnMarkPeaks),
              '*Lbutton pressed' : (NORMAL, self.OnDragLock),
                  '*Ldrag begin' : (REGION, self.OnDragBegin),
             },
             REGION : {
-                 'S-Ldrag move' : (REGION+LINE, self.OnRegionLock),
+                 'S-Ldrag move' : (REGION+LINE, self.OnRegionLock, self.OnDragLineBegin),
                  'M-Ldrag move' : (REGION+MARK, self.OnMarkPeaks, self.OnMarkSelectionBegin),
-                  '*Ldrag move' : (REGION, self.OnDragMove),
+                  '*Ldrag move' : (REGION, self.OnDragMove, self.OnDragTrace),
                    '*Ldrag end' : (NORMAL, self.OnDragEnd),
             },
             LINE: {
                    '* released' : (NORMAL, ),
                 'S-Ldrag begin' : (REGION+LINE, self.OnDragLineBegin),
             },
             REGION+LINE : {
@@ -427,15 +440,15 @@
                'frame_selected' : [ None, _F(self.linplot, fit=0, force=0) ],
             }
         }
         self.modeline.Show(1)
         
         self.menu += [
             (mwx.ID_(510), "&Copy data", "Copy data to clipboard",
-                lambda v: self.copy_data_to_clipboard()),
+                lambda v: self.write_data_to_clipboard()),
             (),
             (mwx.ID_(511), "Logic length", "Set axis-unit in logic base", wx.ITEM_RADIO,
                 lambda v: self.set_logic(1),
                 lambda v: v.Check(self.__logicp)),
                 
             (mwx.ID_(512), "Pixel length", "Set axis-unit in pxiel base", wx.ITEM_RADIO,
                 lambda v: self.set_logic(0),
@@ -512,14 +525,22 @@
             return x[[0,-1]]
     
     @property
     def plotdata(self):
         """Plotted (xdata, ydata) in single plot."""
         return self.__plot.get_data(orig=0)
     
+    def calc_average(self):
+        X, Y = self.plotdata
+        if self.region is not None:
+            a, b = self.region
+            Y = Y[(a <= X) & (X <= b)]
+        if Y.size:
+            return Y.mean()
+    
     def linplot(self, frame, fit=True, force=True):
         if not force:
             if frame is self.__frame:
                 return
         self.__frame = frame # update reference of the frame
         if frame:
             sel = frame.selector
@@ -568,15 +589,16 @@
             self.__plot.set_visible(1)
             
             if fit and len(ls) > 1: # drawing area
                 ly = self.ylim
                 self.xlim = ls[0], ls[-1]
                 self.ylim = ly[0], max(ly[1], max(zs))
             
-        self.update_position()
+        self.toolbar.update()
+        self.toolbar.push_current()
         self.draw()
     
     def writeln(self):
         if not self.modeline.IsShown():
             return
         frame = self.__frame
         if frame:
@@ -590,22 +612,22 @@
               length = len(self.plotdata[0]),
                 unit = frame.unit if self.__logicp else 1,
                    x = '++' if self.__logicp else '--',
                    a = '%%' if not frame.buffer.flags.writeable else '--'))
         else:
             self.modeline.write("")
     
-    def copy_data_to_clipboard(self):
-        """Copy plotdata to clipboard."""
-        self.message("Copy data to clipboard.")
+    def write_data_to_clipboard(self):
+        """Write plot data to clipboard."""
         X, Y = self.plotdata
         with io.StringIO() as o:
             for x, y in zip(X, Y):
                 o.write("{:g}\t{:g}\n".format(x, y))
             Clipboard.write(o.getvalue(), verbose=0)
+            self.message("Write data to clipboard.")
     
     ## --------------------------------
     ## Motion/Drag actions (override)
     ## --------------------------------
     
     def OnHomeXPosition(self, evt):
         x = self.plotdata[0]
@@ -625,15 +647,15 @@
         """Called before canvas.draw."""
         LinePlot.OnDraw(self, evt)
         
         x, y = self.plotdata
         if x.size:
             self.__fil.set_xy(list(chain([(x[0],0)], zip(x,y), [(x[-1],0)])))
         self.writeln()
-        
+    
     def OnLineWidth(self, evt):
         n = -2 if evt.key[-1] == '-' else 2
         self.set_linewidth(self.__linewidth + n)
     
     def OnRegionShift(self, evt):
         if self.__frame and self.region is not None:
             u = self.__frame.unit
@@ -644,15 +666,25 @@
     def OnEscapeSelection(self, evt):
         self.__hline.set_visible(0)
         LinePlot.OnEscapeSelection(self, evt)
     
     def OnDragLineBegin(self, evt):
         self.set_wxcursor(wx.CURSOR_SIZENS)
     
+    def OnDragTrace(self, evt):
+        """Show average value."""
+        y = self.calc_average()
+        if y is not None:
+            ## self.__hline.set_ydata([y])
+            ## self.__hline.set_visible(1)
+            ## self.canvas.draw_idle()
+            self.message(f"ya = {y:g}")
+    
     def OnRegionLock(self, evt):
+        """Show FWHM region."""
         x, y = self.plotdata
         if x.size:
             xc, yc = evt.xdata, evt.ydata
             u = x[1] - x[0] # != frame.unit (斜め線の場合 dx=unit とは限らない)
             v = (y < yc)
             if v.all():
                 self.region = None # all y < yc
@@ -674,18 +706,19 @@
                 else:
                     self.region = None
             else:
                 self.region = x[[0,-1]] # all y > yc
             
             self.__hline.set_ydata([yc])
             self.__hline.set_visible(1)
-            self.message("y = {:g}, xr = {}".format(yc, self.region))
             self.draw()
+            self.message(f"yc = {yc:g}")
     
     def OnMarkPeaks(self, evt):
+        """Set markers on peaks."""
         x, y = self.plotdata
         if x.size:
             lw = 5
             window = np.hanning(lw)
             ys = np.convolve(window/window.sum(), y, mode='same')
             
             ## maxima = signal.find_peaks_cwt(ys, np.arange(lw,lw*2))
@@ -695,15 +728,17 @@
             minima,_ = signal.find_peaks(-ys, width=lw, prominence=20)
             
             peaks = np.sort(np.append(maxima, minima))
             if peaks.size:
                 self.Selector = x[peaks], y[peaks]
     
     def OnMarkErase(self, evt):
-        del self.Selector
+        """Erase markers on peaks."""
+        ## del self.Selector
+        self.OnEscapeSelection(evt)
     
     def OnMarkSelectionBegin(self, evt):
         org = self.p_event
         xs, ys = self.Selector
         xc, yc = org.xdata, org.ydata
         ## xc, yc = evt.xdata, evt.ydata
         if xs.size:
```

## mwx/utilus.py

```diff
@@ -566,15 +566,15 @@
             if self.default_state is None:
                 default = next((k for k in contexts if k is not None), None)
         self.default_state = default
         self.clear(default) # the first clear creates object localvars
         self.update(contexts)
     
     def __missing__(self, key):
-        raise Exception("FSM:logic-error: undefined state {!r}".format(key))
+        raise Exception("FSM logic-error: undefined state {!r}".format(key))
     
     def __repr__(self):
         return "<{} object at 0x{:X}>".format(self.__class__.__name__, id(self))
     
     def __str__(self):
         return '\n'.join("[ {!r} ]\n{!s}".format(k, v) for k, v in self.items())
     
@@ -658,15 +658,15 @@
                     self.__event = event
                 try:
                     ret = act(*args, **kwargs) # call actions after transition
                     retvals.append(ret)
                 except BdbQuit:
                     pass
                 except Exception as e:
-                    self.dump("- FSM:exception: {!r}".format(e),
+                    self.dump("- FSM exception: {!r}".format(e),
                               "  event  : {}".format(event),
                               "  from   : {}".format(self.__prev_state),
                               "  to     : {}".format(self.__state),
                               "  action : {}".format(typename(act)),
                               "  args   : {}".format(args),
                               "  kwargs : {}".format(kwargs))
                     traceback.print_exc()
@@ -795,45 +795,45 @@
         assert isinstance(event, str)
         assert callable(action) or action is None
         
         def warn(msg):
             warnings.warn(msg, stacklevel=3)
         
         if state not in self:
-            warn("- FSM:warning: [{!r}] context newly created.".format(state))
+            warn("- FSM warning: [{!r}] context newly created.".format(state))
             self[state] = SSM() # new context
         
         context = self[state]
         if state2 is None:
             state2 = state
         
         if event in context:
             if state2 != context[event][0]:
-                warn("- FSM:warning: transaction may conflict.\n"
+                warn("- FSM warning: transaction may conflict.\n"
                      "  The state {2!r} and the original state is not the same."
                      "  {0!r} : {1!r} --> {2!r}".format(event, state, state2))
                 pass
                 context[event][0] = state2 # update transition
         else:
             ## if state2 not in self:
-            ##     warn("- FSM:warning: transaction may contradict\n"
+            ##     warn("- FSM warning: transaction may contradict\n"
             ##          "  The state {2!r} is not found in the contexts."
             ##          "  {0!r} : {1!r} --> {2!r}".format(event, state, state2))
             ##     pass
             context[event] = [state2] # new event:transaction
         
         transaction = context[event]
         if action is None:
             return lambda f: self.bind(event, f, state, state2)
         
         if action not in transaction:
             try:
                 transaction.append(action)
             except AttributeError:
-                warn("- FSM:warning: cannot append new transaction ({!r} : {!r})\n"
+                warn("- FSM warning: cannot append new transaction ({!r} : {!r})\n"
                      "  The transaction must be a list, not a tuple".format(state, event))
         return action
     
     def unbind(self, event, action=None, state=None):
         """Remove a transaction from the context.
         
         equiv. self[state] -= {event : [?, action]}
@@ -843,34 +843,34 @@
         """
         assert callable(action) or action is None
         
         def warn(msg):
             warnings.warn(msg, stacklevel=3)
         
         if state not in self:
-            warn("- FSM:warning: [{!r}] context does not exist.".format(state))
+            warn("- FSM warning: [{!r}] context does not exist.".format(state))
             return
         
         context = self[state]
         if event not in context:
-            warn("- FSM:warning: No such transaction ({!r} : {!r})".format(state, event))
+            warn("- FSM warning: No such transaction ({!r} : {!r})".format(state, event))
             return
         
         transaction = context[event]
         if action is None:
             for act in transaction[1:]:
                 self.unbind(event, act, state)
             return True
         
         if action in transaction:
             try:
                 transaction.remove(action)
                 return True
             except AttributeError:
-                warn("- FSM:warning: removing action from context ({!r} : {!r})\n"
+                warn("- FSM warning: removing action from context ({!r} : {!r})\n"
                      "  The transaction must be a list, not a tuple".format(state, event))
         return False
 
 
 class TreeList(object):
     """Interface class for tree list control.
```

## mwx/py/__init__.py

```diff
@@ -0,0 +1,3 @@
+00000000: 2321 2070 7974 686f 6e33 0d0a 2222 2250  #! python3.."""P
+00000010: 6c75 672d 696e 7320 2f20 4164 642d 696e  lug-ins / Add-in
+00000020: 732e 2222 220d 0a                        s."""..
```

## Comparing `mwxlib-0.93.5.dist-info/LICENSE` & `mwxlib-0.93.8.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mwxlib-0.93.5.dist-info/METADATA` & `mwxlib-0.93.8.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mwxlib
-Version: 0.93.5
+Version: 0.93.8
 Summary: A wrapper of matplotlib and wxPython (phoenix)
 Home-page: https://github.com/komoto48g/mwxlib
 Author: Kazuya O'moto
 Author-email: komoto@jeol.co.jp
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

## Comparing `mwxlib-0.93.5.dist-info/RECORD` & `mwxlib-0.93.8.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 mwx/__init__.py,sha256=5B4YSOuijG1Uo5-FLtLHGB52Cp_F4vnN--4wGPBx7do,2398
 mwx/bookshelf.py,sha256=FrissUYdGXLABOzJmMaQU6GXvu6n_9DVW3d5wGwQzjM,6613
 mwx/controls.py,sha256=9C1sXBwQl-oZtCb3rXoT-doW48Sv1J359toNq9ScF9M,47173
-mwx/framework.py,sha256=SeFOWD9YzxgP5WlkYFeONWj9EoToH7IQ5LmyJbECqMw,73951
-mwx/graphman.py,sha256=0ppruAsbvUK6vUKnRc3-6gNW83V8XVp9Xr8mQrAaLTI,70267
+mwx/framework.py,sha256=ZwsNOIUpR8Xpilvc_ndcdhKIgoDoJ0whMTKweAwSzlI,73951
+mwx/graphman.py,sha256=SKYJFxi-TqWOALRczYz-M-2ZYEbqiZuAuKCfEIedctY,70156
 mwx/images.py,sha256=mrnUYH12I3XLVSZcEXlpVltX0XMxufbl2yRvDIQJZqc,49957
-mwx/matplot2.py,sha256=g902yipGCiO5SARTSafbE3c6-ZkQ-JbOkXSo7iltnDQ,32761
-mwx/matplot2g.py,sha256=d0g48JhBWvqqmHQKvuwEAQqa8ol9MX8UvEHU__hQiz4,65552
-mwx/matplot2lg.py,sha256=mCeT_OBwsq7OamW56WRg9YqyXe6WPJrjCfCVAzDvSlw,26343
+mwx/matplot2.py,sha256=qaF_gvLoLn-TimLbRR59KUavNr1ZpZQdSMqjzJk47rk,32682
+mwx/matplot2g.py,sha256=Txcz3yusiFF0j1QnAS0dCGTbGrkx4VC6BZbWbjIRZnw,65585
+mwx/matplot2lg.py,sha256=IfTZSJaKtiw7SWM3lDNBO6qz5AOTJ6UmPVoMzXZoR8I,27653
 mwx/mgplt.py,sha256=ITzxA97yDwr_35BUk5OqnyskSuKVDbpf2AQCKY1jHTI,5671
 mwx/nutshell.py,sha256=5HErOObnOprMc6gYnXV7wY-ALnlwNpmhV8f0EyipYA4,135816
-mwx/utilus.py,sha256=IaB9RYPatprJXsulyrM2kEcVr-3ji0M88PUYBr9Nx6k,37040
+mwx/utilus.py,sha256=THDxQ-QqbHYVc8iX8qN9yxvfcf7Pvpm7sfTP9ipYvzs,37040
 mwx/wxmon.py,sha256=Qk86VbuuW2rR46pqEYLur13G_aloWz5SVv6sib30YY0,12717
 mwx/wxpdb.py,sha256=2z3ZD9Oo1H-ONBHlaprkB9hrTmAI7o03sqO46ppEFE4,19129
 mwx/wxwil.py,sha256=JK1du4i1RVMbDLqN8jLRDSu_JhKEp4mhHVMElzo4yoE,5578
 mwx/wxwit.py,sha256=2gFHi-8nwWRh26RdvZ_AUP--8PDjJB8TUU72y2fBUWM,7557
-mwx/py/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+mwx/py/__init__.py,sha256=NzBazvjN9KMFoylsHsLiNOHbcDrNflgSwEFlkT12Rnw,39
+mwx/py/ffmpeg_view.py,sha256=vUYNybIJsF1JGkDzjBgDyBQvDh8e1oKHlEMY5Fwc8L4,9399
+mwx/py/fft_view.py,sha256=evj2kCe6N10JQczW8IajgLVrUWOihQaHQ2xiBzAsAl4,2675
 mwx/py/filling.py,sha256=KaHooM32hrGGgqw75Cbt8lAvACwC6RXadob9LGgNnEc,16806
-mwxlib-0.93.5.dist-info/LICENSE,sha256=PGtRKCaTkmUDlBQwpptJAxJtdqxIUtAmdBsaT9nUVkA,1091
-mwxlib-0.93.5.dist-info/METADATA,sha256=-z6_xKYj1N7D9gfLX6jJ6Yn1fPXwjnMvJO1utGox9Cc,1925
-mwxlib-0.93.5.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-mwxlib-0.93.5.dist-info/top_level.txt,sha256=SI1Mh118AstnUFGPNq5aMNKiAnVNmZk1S9Ij-OwAEpY,4
-mwxlib-0.93.5.dist-info/RECORD,,
+mwx/py/frame_listview.py,sha256=T-2xSv_D2bk9fJ64aiSEe1rJRTeqaIpLVAYEUXW5vz8,10110
+mwx/py/line_profile.py,sha256=WJB5z7F53yg4dII2R36IFZvtkSOGWT669b1HmAAXSnQ,816
+mwxlib-0.93.8.dist-info/LICENSE,sha256=PGtRKCaTkmUDlBQwpptJAxJtdqxIUtAmdBsaT9nUVkA,1091
+mwxlib-0.93.8.dist-info/METADATA,sha256=zJOmDRH4dCa-5QzpMr-hCP-ZhYBPlwZ2AlNzSn_q9Nw,1925
+mwxlib-0.93.8.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+mwxlib-0.93.8.dist-info/top_level.txt,sha256=SI1Mh118AstnUFGPNq5aMNKiAnVNmZk1S9Ij-OwAEpY,4
+mwxlib-0.93.8.dist-info/RECORD,,
```

