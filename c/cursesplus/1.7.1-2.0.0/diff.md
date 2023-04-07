# Comparing `tmp/cursesplus-1.7.1.tar.gz` & `tmp/cursesplus-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cursesplus-1.7.1.tar", last modified: Tue Mar  7 20:59:19 2023, max compression
+gzip compressed data, was "cursesplus-2.0.0.tar", last modified: Fri Apr  7 16:57:03 2023, max compression
```

## Comparing `cursesplus-1.7.1.tar` & `cursesplus-2.0.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 enderbyte09  (1000) enderbyte09  (1000)        0 2023-03-07 20:59:19.831436 cursesplus-1.7.1/
--rw-rw-r--   0 enderbyte09  (1000) enderbyte09  (1000)     1089 2023-01-20 19:53:48.000000 cursesplus-1.7.1/LICENSE
--rw-rw-r--   0 enderbyte09  (1000) enderbyte09  (1000)     1500 2023-03-07 20:59:19.831436 cursesplus-1.7.1/PKG-INFO
--rw-rw-r--   0 enderbyte09  (1000) enderbyte09  (1000)      897 2023-03-07 20:59:09.000000 cursesplus-1.7.1/README.md
--rw-rw-r--   0 enderbyte09  (1000) enderbyte09  (1000)      659 2023-03-07 20:36:51.000000 cursesplus-1.7.1/pyproject.toml
--rw-rw-r--   0 enderbyte09  (1000) enderbyte09  (1000)       38 2023-03-07 20:59:19.831436 cursesplus-1.7.1/setup.cfg
-drwxrwxr-x   0 enderbyte09  (1000) enderbyte09  (1000)        0 2023-03-07 20:59:19.827436 cursesplus-1.7.1/src/
--rw-rw-r--   0 enderbyte09  (1000) enderbyte09  (1000)     1358 2023-03-07 20:29:38.000000 cursesplus-1.7.1/src/__cptest.py
-drwxrwxr-x   0 enderbyte09  (1000) enderbyte09  (1000)        0 2023-03-07 20:59:19.827436 cursesplus-1.7.1/src/cursesplus/
--rw-rw-r--   0 enderbyte09  (1000) enderbyte09  (1000)      997 2023-03-07 20:31:46.000000 cursesplus-1.7.1/src/cursesplus/__init__.py
--rw-rw-r--   0 enderbyte09  (1000) enderbyte09  (1000)    11672 2023-03-07 19:36:50.000000 cursesplus-1.7.1/src/cursesplus/cp.py
--rw-rw-r--   0 enderbyte09  (1000) enderbyte09  (1000)    10919 2023-03-07 20:25:11.000000 cursesplus-1.7.1/src/cursesplus/filedialog.py
--rw-rw-r--   0 enderbyte09  (1000) enderbyte09  (1000)     5498 2023-03-07 20:33:46.000000 cursesplus-1.7.1/src/cursesplus/messagebox.py
-drwxrwxr-x   0 enderbyte09  (1000) enderbyte09  (1000)        0 2023-03-07 20:59:19.831436 cursesplus-1.7.1/src/cursesplus.egg-info/
--rw-rw-r--   0 enderbyte09  (1000) enderbyte09  (1000)     1500 2023-03-07 20:59:19.000000 cursesplus-1.7.1/src/cursesplus.egg-info/PKG-INFO
--rw-rw-r--   0 enderbyte09  (1000) enderbyte09  (1000)      306 2023-03-07 20:59:19.000000 cursesplus-1.7.1/src/cursesplus.egg-info/SOURCES.txt
--rw-rw-r--   0 enderbyte09  (1000) enderbyte09  (1000)        1 2023-03-07 20:59:19.000000 cursesplus-1.7.1/src/cursesplus.egg-info/dependency_links.txt
--rw-rw-r--   0 enderbyte09  (1000) enderbyte09  (1000)       20 2023-03-07 20:59:19.000000 cursesplus-1.7.1/src/cursesplus.egg-info/top_level.txt
+drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-04-07 16:57:03.465613 cursesplus-2.0.0/
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)     1089 2023-04-07 16:31:31.000000 cursesplus-2.0.0/LICENSE
+-rw-r--r--   0 jordan    (1000) jordan    (1000)     1556 2023-04-07 16:57:03.465613 cursesplus-2.0.0/PKG-INFO
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)      953 2023-04-07 16:31:31.000000 cursesplus-2.0.0/README.md
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)      659 2023-04-07 16:31:31.000000 cursesplus-2.0.0/pyproject.toml
+-rw-r--r--   0 jordan    (1000) jordan    (1000)       38 2023-04-07 16:57:03.465613 cursesplus-2.0.0/setup.cfg
+drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-04-07 16:57:03.465613 cursesplus-2.0.0/src/
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)      555 2023-04-07 16:31:31.000000 cursesplus-2.0.0/src/__cptest.py
+drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-04-07 16:57:03.465613 cursesplus-2.0.0/src/cursesplus/
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)      892 2023-04-07 16:31:31.000000 cursesplus-2.0.0/src/cursesplus/__init__.py
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)    11516 2023-04-07 16:31:31.000000 cursesplus-2.0.0/src/cursesplus/cp.py
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)    11277 2023-04-07 16:45:57.000000 cursesplus-2.0.0/src/cursesplus/filedialog.py
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)     5666 2023-04-07 16:31:31.000000 cursesplus-2.0.0/src/cursesplus/messagebox.py
+drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-04-07 16:57:03.465613 cursesplus-2.0.0/src/cursesplus.egg-info/
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)     1556 2023-04-07 16:57:03.000000 cursesplus-2.0.0/src/cursesplus.egg-info/PKG-INFO
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)      306 2023-04-07 16:57:03.000000 cursesplus-2.0.0/src/cursesplus.egg-info/SOURCES.txt
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)        1 2023-04-07 16:57:03.000000 cursesplus-2.0.0/src/cursesplus.egg-info/dependency_links.txt
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)       20 2023-04-07 16:57:03.000000 cursesplus-2.0.0/src/cursesplus.egg-info/top_level.txt
```

### Comparing `cursesplus-1.7.1/LICENSE` & `cursesplus-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cursesplus-1.7.1/PKG-INFO` & `cursesplus-2.0.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cursesplus
-Version: 1.7.1
+Version: 2.0.0
 Summary: An extension program to curses that offers option menus, message boxes, file dialogs and more
 Author-email: Enderbyte Programs <enderbyte09@gmail.com>
 Project-URL: Homepage, https://github.com/Enderbyte-Programs/Curses-Plus
 Project-URL: Bug Tracker, https://github.com/Enderbyte-Programs/Curses-Plus/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -36,24 +36,16 @@
 Microsoft Windows 11
 Any modern distro of Linux that supports Python3
 
 **Python Version 3.6 or newer**
 
 ## What's New?
 
-### Patch 1.7.1
+Version 2.0: Incompatible api changes
 
--Improve documentation
-
-### Version 1.7
-
--Add more messageboxes
-
--Messagebox.showinfo for info
-
--messagebox.showwarning for warning
-
--messagebox.showerror for errors
+-askyesno now MUST be messagebox.askyesno
+-Rewrite colour system. load_colours() is now nonexistent.
+-Now use set_colour(background,foreground). A set of colour constants are defined in the cp class.
 
 ## Uses
 
 curses-plus offers many utilities to make writing TUI applications easy. (TUI stands for Terminal User Interface)
```

### Comparing `cursesplus-1.7.1/pyproject.toml` & `cursesplus-2.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "cursesplus"
-version = "1.7.1"
+version = "2.0.0"
 authors = [{name="Enderbyte Programs",email="enderbyte09@gmail.com"},]
 description = "An extension program to curses that offers option menus, message boxes, file dialogs and more"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
 	"Programming Language :: Python :: 3",
 	"License :: OSI Approved :: MIT License",
```

### Comparing `cursesplus-1.7.1/src/cursesplus/cp.py` & `cursesplus-2.0.0/src/cursesplus/cp.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,25 @@
 import curses#Depends on windows-curses on win32
 from curses.textpad import rectangle, Textbox
 import os
 from time import sleep
 import random
 from datetime import datetime
-from .messagebox import askyesno
+
+#DEFINE SOME CONSTANTS
+BLACK = curses.COLOR_BLACK
+WHITE = curses.COLOR_WHITE
+RED = curses.COLOR_RED
+YELLOW = curses.COLOR_YELLOW
+GREEN = curses.COLOR_GREEN
+CYAN = curses.COLOR_CYAN
+BLUE = curses.COLOR_BLUE
+MAGENTA = curses.COLOR_MAGENTA
+
+_C_INIT = False
 
 def cursestransition(stdscr,func_to_call=None,args=(),type=0):
     """
     Generate a fancy transition with curses. Type 0 is a wipe transition with lines. Type 1 is a more powerful random block pixel transition.
     Calls func_to_call(args) after transition is finishd
     """
     block = "█"
@@ -137,15 +148,15 @@
         else:
             rectangle(stdscr,1,0,2+len(options),maxlen+2)
         oi = -1
         for o in options[offset:offset+(my-4)]:
             oi += 1
             try:
                 if oi == selected-offset:
-                    stdscr.addstr(oi+2,1,o,curses.color_pair(4))
+                    stdscr.addstr(oi+2,1,o,set_colour(WHITE,BLACK))
                 else:
                     stdscr.addstr(oi+2,1,o)
             except curses.error:
                 pass
         stdscr.addstr(my-1,0,"Please choose an option with the arrow keys then press enter."[0:mx-1])
         stdscr.refresh()
         _ch = stdscr.getch()
@@ -169,57 +180,52 @@
 def askyesno_old(stdscr,title: str) -> bool:
     """Ask a yes no question provided by title."""
     result = displayops(stdscr,["Yes","No"],title)
     if result == 0:
         return True
     else:
         return False
-def load_colours(grayscale=False):
-    """Initialize basic colours in the terminal. Use grayscale=True to set all colours to black on white with no colours.
-    Thsi function is required to call optionmenu and yesno
-    List of colours
-    1: Red
-    2: Blue
-    3: Green
-    4: Cyan
-    5: Magenta
-    6: White (normal)
-    7: Black (usually invisible)
-    8: Yellow
-    9: Inverted (black on white background)
-    """
-    if not grayscale:
-        curses.init_pair(7,curses.COLOR_BLACK,curses.COLOR_BLACK)
-        curses.init_pair(1,curses.COLOR_RED,curses.COLOR_BLACK)
-        curses.init_pair(2,curses.COLOR_BLUE,curses.COLOR_BLACK)
-        curses.init_pair(3,curses.COLOR_GREEN,curses.COLOR_BLACK)
-        curses.init_pair(4,curses.COLOR_CYAN,curses.COLOR_BLACK)
-        curses.init_pair(5,curses.COLOR_MAGENTA,curses.COLOR_BLACK)
-        curses.init_pair(8,curses.COLOR_YELLOW,curses.COLOR_BLACK)
-        curses.init_pair(6,curses.COLOR_WHITE,curses.COLOR_BLACK) 
-        curses.init_pair(9,curses.COLOR_BLACK,curses.COLOR_WHITE)
-        curses.init_pair(10,curses.COLOR_WHITE,curses.COLOR_BLUE)
-        curses.init_pair(11,curses.COLOR_WHITE,curses.COLOR_RED)
-        curses.init_pair(12,curses.COLOR_WHITE,curses.COLOR_GREEN)
-        curses.init_pair(13,curses.COLOR_WHITE,curses.COLOR_YELLOW)
-    else:
-        for i in range(1,13):
-            curses.init_pair(i,curses.COLOR_BLACK,curses.COLOR_WHITE)
+_AVAILABLE_COL = list(range(1,255,1))
+_COL_INDEX = {}
+def set_colour(background: int, foreground: int) -> int:
+    global _C_INIT
+    global _COL_INDEX
+    global _AVAILABLE_COL
+    """Set a colour object. Use the constants provided. z
+    For attributes use | [ATTR] for example set_colour(RED,GREEN) | sdf
+    """
+    if not _C_INIT:
+        curses.start_color()
+        curses.use_default_colors()
+        _C_INIT = True
+
+    if str(foreground) in _COL_INDEX.keys() and str(background) in _COL_INDEX[str(foreground)].keys():
+        return curses.color_pair(_COL_INDEX[str(foreground)][str(background)])
+    if len(_AVAILABLE_COL) == 0:
+        raise Warning("Out of colours!")
+        _AVAILABLE_COL = list(range(1,255,1))#Replenish list
+    i = _AVAILABLE_COL.pop(0)
+    curses.init_pair(i,foreground,background)
+    if not str(foreground) in _COL_INDEX.keys():
+        _COL_INDEX[str(foreground)] = {}
+    _COL_INDEX[str(foreground)][str(background)] = i
+    return curses.color_pair(i)
 
-def load_colors(grayscale=False):
-    load_colours(grayscale)
+def set_color(background: int,foreground: int) -> int:
+    return set_colour(background,foreground)
 
 def displayerror(stdscr,e,msg: str):
     """
     Display an error message
     """
     displaymsg(stdscr,["An error occured",msg,str(e)])
 
 def filline(stdscr,line: int,colour: int):
-    stdscr.addstr(line,0," "*(os.get_terminal_size()[0]-1),curses.color_pair(colour))
+    """Fill a line, colour is the result of set_colour(fg,bg)"""
+    stdscr.addstr(line,0," "*(os.get_terminal_size()[0]-1),colour)
 
 def hidecursor():
     """Hide Cursor. Can only be called in an active curses window"""
     curses.curs_set(0)
 
 def showcursor():
     """Show cursor. Can only be called in an active curses window"""
@@ -241,31 +247,29 @@
         self.submsg = ""
         self.mx, self.my = os.get_terminal_size()
         self.wfkp = waitforkeypress
     def update(self):
         lheight = self.my - 7
         """Redraws progress bar"""
         self.screen.erase()
-        self.screen.addstr(0,0," "*(self.mx-1),curses.color_pair(10))
-        self.screen.addstr(0,0,self.msg[0:self.mx-1],curses.color_pair(10))
-        filline(self.screen,1,11)
-        filline(self.screen,2,11)
-        filline(self.screen,3,11)
-        #self.screen.addstr(2,0," "*(os.get_terminal_size()[0]-1),curses.color_pair(11))
-        #self.screen.addstr()
-        self.screen.addstr(1,0,"-"*(self.mx-1),curses.color_pair(11))
-        self.screen.addstr(3,0,"-"*(self.mx-1),curses.color_pair(11))
+        self.screen.addstr(0,0," "*(self.mx-1),set_colour(BLUE,WHITE))
+        self.screen.addstr(0,0,self.msg[0:self.mx-1],set_colour(BLUE,WHITE))
+        #filline(self.screen,1,set_colour(GREEN,WHITE))
+        filline(self.screen,2,set_colour(RED,WHITE))
+        #filline(self.screen,3,set_colour(GREEN,WHITE))
+        self.screen.addstr(1,0,"-"*(self.mx-1),set_colour(RED,WHITE))
+        self.screen.addstr(3,0,"-"*(self.mx-1),set_colour(RED,WHITE))
         barfill = round((self.value/self.max)*self.mx-1)
         if not self.value > self.max:
-            self.screen.addstr(2,0," "*barfill,curses.color_pair(12))
+            self.screen.addstr(2,0," "*barfill,set_colour(GREEN,WHITE))
         else:
-            self.screen.addstr(2,0," "*self.mx-1,curses.color_pair(12))
-        self.screen.addstr(3,0,self.submsg[0:self.mx-1],curses.color_pair(11))
+            self.screen.addstr(2,0," "*self.mx-1,set_colour(GREEN,WHITE))
+        self.screen.addstr(3,0,self.submsg[0:self.mx-1],set_colour(RED,WHITE))
         if self.sp:
-            self.screen.addstr(3,self.mx-7,f"{round(self.value/self.max*100,1)} %",curses.color_pair(11))
+            self.screen.addstr(3,self.mx-7,f"{round(self.value/self.max*100,1)} %",set_colour(RED,WHITE))
         if self.sl:
             rectangle(self.screen,4,0,self.my-2,self.mx-1)
             if len(self.loglist) > lheight:
                 lx = 0
                 for val in self.loglist[len(self.loglist)-lheight:]:
                     self.screen.addstr(lx+5,1,val[0:self.mx-2],self.lclist[len(self.loglist)-lheight+lx])
                     lx += 1
```

### Comparing `cursesplus-1.7.1/src/cursesplus/filedialog.py` & `cursesplus-2.0.0/src/cursesplus/filedialog.py`

 * *Files 16% similar despite different names*

```diff
@@ -57,50 +57,50 @@
     selected: int = 0
     while True:
         masterlist: list = list[Fileobj]
         mx,my = os.get_terminal_size()
         MAXNL = mx - 33
         stdscr.clear()
         cp.rectangle(stdscr,2,0,my-2,mx-1)
-        cp.filline(stdscr,0,10)
-        cp.filline(stdscr,1,12)
-        cp.filline(stdscr,my-2,9)
-        cp.filline(stdscr,my-1,11)
+        cp.filline(stdscr,0,cp.set_color(cp.BLUE,cp.WHITE))
+        cp.filline(stdscr,1,cp.set_color(cp.GREEN,cp.WHITE))
+        cp.filline(stdscr,my-2,cp.set_color(cp.WHITE,cp.BLACK))
+        cp.filline(stdscr,my-1,cp.set_color(cp.RED,cp.WHITE))
         topline = "Name"+" "*(MAXNL-4)+"|"+"Size     "+"|Date Modified"
         topline = topline+(mx-2-len(topline))*" "
         directories = [directory+"/"+l for l in os.listdir(directory) if os.path.isdir(directory+"/"+l)]
         if filter[activefilter][0].strip() == "*":
             files = [directory+"/"+l for l in os.listdir(directory) if os.path.isfile(directory+"/"+l)]
         else:
             files = glob.glob(directory+"/"+filter[activefilter][0])
         directories.sort()
         files.sort()
         #displaymsg(stdscr,directories+files)
         masterlist = [Fileobj(f) for f in (directories+files)]
-        stdscr.addstr(0,0,title+"|H for Help|Press Shift-Left Arrow to move up directory"[0:mx],cp.curses.color_pair(10))
-        stdscr.addstr(1,0,directory[xoffset:xoffset+mx],cp.curses.color_pair(12))
-        stdscr.addstr(my-2,0,f"{filter[activefilter][1]} ({filter[activefilter][0]}) [{len(masterlist)} objects found]"[0:mx],cp.curses.color_pair(9))
+        stdscr.addstr(0,0,title+"|H for Help|Press Shift-Left Arrow to move up directory"[0:mx],cp.set_colour(cp.BLUE,cp.WHITE))
+        stdscr.addstr(1,0,directory[xoffset:xoffset+mx],cp.set_colour(cp.GREEN,cp.WHITE))
+        stdscr.addstr(my-2,0,f"{filter[activefilter][1]} ({filter[activefilter][0]}) [{len(masterlist)} objects found]"[0:mx],cp.set_colour(cp.WHITE,cp.BLACK))
         stdscr.addstr(2,1,topline[0:mx-1])
         
         try:
-            stdscr.addstr(my-1,0,masterlist[selected].path[xoffset:xoffset+mx],cp.curses.color_pair(11))
+            stdscr.addstr(my-1,0,masterlist[selected].path[xoffset:xoffset+mx],cp.set_colour(cp.RED,cp.WHITE))
         except:
             pass
         ind = yoffset#Track position in list
         indx = 0#track position in iter
         for fileobjects in masterlist[yoffset:yoffset+my-5]:
             wstr = fileobjects.strippedpath[xoffset:xoffset+MAXNL]
             wstr += " "*(MAXNL-len(wstr)+1)
             wstr += fileobjects.sizestr
             wstr += " "*(10-len(fileobjects.sizestr))
             wstr += fileobjects.date
             if selected == ind:
-                stdscr.addstr(3+indx,1,wstr,cp.curses.color_pair(5))
+                stdscr.addstr(3+indx,1,wstr,cp.set_colour(cp.BLACK,cp.MAGENTA))
             elif fileobjects.isdir:
-                stdscr.addstr(3+indx,1,wstr,cp.curses.color_pair(2))
+                stdscr.addstr(3+indx,1,wstr,cp.set_colour(cp.BLACK,cp.BLUE))
             else:
                 stdscr.addstr(3+indx,1,wstr)
             ind += 1
             indx += 1#Inc both
 
         
         stdscr.refresh()
@@ -125,15 +125,15 @@
         elif ch == cp.curses.KEY_ENTER or ch == 10 or ch == 13:
             if masterlist[selected].isdir:
                 directory = masterlist[selected].path
                 selected = 0
                 yoffset = 0
             else:
                 return masterlist[selected].path
-        elif ch == cp.curses.KEY_SLEFT:
+        elif ch == cp.curses.KEY_SLEFT or ch == 98:
             directory = "/".join(directory.split("/")[0:-1])
             selected = 0
             yoffset = 0
             if directory == "":
                 directory = "/"
         elif ch == 104:
             cp.displaymsg(stdscr,["List of Keybinds","Down Arrow: Scroll down","Up Arrow: Scroll up","Left Arrow: Scroll left","Right Arrow: Scroll right","Shift-left arrow: Move up to parent Directory","Enter: Open/select","F: Change filter"])
@@ -161,52 +161,52 @@
     chosen.clear()
     while True:
         masterlist: list = list[Fileobj]
         mx,my = os.get_terminal_size()
         MAXNL = mx - 33
         stdscr.clear()
         cp.rectangle(stdscr,2,0,my-2,mx-1)
-        cp.filline(stdscr,0,10)
-        cp.filline(stdscr,1,12)
-        cp.filline(stdscr,my-2,9)
-        cp.filline(stdscr,my-1,11)
+        cp.filline(stdscr,0,cp.set_color(cp.BLUE,cp.WHITE))
+        cp.filline(stdscr,1,cp.set_color(cp.GREEN,cp.WHITE))
+        cp.filline(stdscr,my-2,cp.set_color(cp.WHITE,cp.BLACK))
+        cp.filline(stdscr,my-1,cp.set_color(cp.RED,cp.WHITE))
         topline = "Name"+" "*(MAXNL-4)+"|"+"Size     "+"|Date Modified"
         topline = topline+(mx-2-len(topline))*" "
         directories = [directory+"/"+l for l in os.listdir(directory) if os.path.isdir(directory+"/"+l)]
         if filter[activefilter][0] == "*":
             files = [directory+"/"+l for l in os.listdir(directory) if os.path.isfile(directory+"/"+l)]
         else:
             files = glob.glob(directory+"/"+filter[activefilter][0])
         directories.sort()
         files.sort()
         #displaymsg(stdscr,directories+files)
         masterlist = [Fileobj(f) for f in (directories+files)]
-        stdscr.addstr(0,0,title+"|H for Help|Press Shift-Left Arrow to move up directory"[0:mx],cp.curses.color_pair(10))
-        stdscr.addstr(1,0,directory[xoffset:xoffset+mx],cp.curses.color_pair(12))
-        stdscr.addstr(my-2,0,f"{filter[activefilter][1]} ({filter[activefilter][0]}) [{len(masterlist)} objects found]"[0:mx],cp.curses.color_pair(9))
+        stdscr.addstr(0,0,title+"|H for Help|Press Shift-Left Arrow to move up directory"[0:mx],cp.set_colour(cp.BLUE,cp.WHITE))
+        stdscr.addstr(1,0,directory[xoffset:xoffset+mx],cp.set_colour(cp.GREEN,cp.WHITE))
+        stdscr.addstr(my-2,0,f"{filter[activefilter][1]} ({filter[activefilter][0]}) [{len(masterlist)} objects found]"[0:mx],cp.set_colour(cp.WHITE,cp.BLACK))
         stdscr.addstr(2,1,topline[0:mx-1])
         
         try:
-            stdscr.addstr(my-1,0,str(chosen)[xoffset:xoffset+mx],cp.curses.color_pair(11))
+            stdscr.addstr(my-1,0,str(chosen)[xoffset:xoffset+mx],cp.set_colour(cp.RED,cp.WHITE))
         except:
             pass
         ind = yoffset#Track position in list
         indx = 0#track position in iter
         for fileobjects in masterlist[yoffset:yoffset+my-5]:
             wstr = fileobjects.strippedpath[xoffset:xoffset+MAXNL]
             wstr += " "*(MAXNL-len(wstr)+1)
             wstr += fileobjects.sizestr
             wstr += " "*(10-len(fileobjects.sizestr))
             wstr += fileobjects.date
             if selected == ind:
-                stdscr.addstr(3+indx,1,wstr,cp.curses.color_pair(5))
+                stdscr.addstr(3+indx,1,wstr,cp.set_colour(cp.BLACK,cp.MAGENTA))
             elif fileobjects.isdir:
-                stdscr.addstr(3+indx,1,wstr,cp.curses.color_pair(2))
+                stdscr.addstr(3+indx,1,wstr,cp.set_colour(cp.BLACK,cp.BLUE))
             elif fileobjects.path in chosen:
-                stdscr.addstr(3+indx,1,wstr,cp.curses.color_pair(4))
+                stdscr.addstr(3+indx,1,wstr,cp.set_colour(cp.BLACK,cp.CYAN))
             else:
                 stdscr.addstr(3+indx,1,wstr)
             ind += 1
             indx += 1#Inc both
 
         
         stdscr.refresh()
@@ -239,15 +239,15 @@
         elif ch == 115:
             #s for add to selection
             if not masterlist[selected].isdir:
                 if masterlist[selected].path in chosen:
                     chosen.remove(masterlist[selected].path)
                 else:
                     chosen.append(masterlist[selected].path)
-        elif ch == cp.curses.KEY_SLEFT:
+        elif ch == cp.curses.KEY_SLEFT or ch == 98:
             directory = "/".join(directory.split("/")[0:-1])
             selected = 0
             yoffset = 0
             if directory == "":
                 directory = "/"
         elif ch == 100 or cp.curses.keyname(ch).decode() == "^X":
             return [c for c in chosen if os.path.isfile(c) and c.replace(" ","") != ""]#Only return files that still exist
```

### Comparing `cursesplus-1.7.1/src/cursesplus/messagebox.py` & `cursesplus-2.0.0/src/cursesplus/messagebox.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,23 +13,23 @@
         if "\n" in o:
             message.insert(ox,o.split("\n")[1])
     message = [m[0:x-5].split("\n")[0] for m in message[0:y-5]]#Limiting characters
     maxs = max([len(s) for s in message])
     while True:
         for by in range(y//2-(len(message)//2)-1,y//2+(len(message)//2)+4):
             for bx in range(x//2-(maxs//2)-1,x//2+(maxs//2+1)+1):
-                stdscr.addstr(by,bx," ",curses.color_pair(12))
+                stdscr.addstr(by,bx," ",cp.set_colour(cp.GREEN,cp.WHITE))
         rectangle(stdscr,y//2-(len(message)//2)-1, x//2-(maxs//2)-1, y//2+(len(message)//2)+4, x//2+(maxs//2+1)+1)
         stdscr.addstr(y//2+(len(message)//2)+4,x//2-(maxs//2),"Y: Yes | N: No")
         mi = -(len(message)/2)
-        stdscr.addstr(y//2+(len(message)//2)+3,x//2-(maxs//2),"[Yes]",[curses.color_pair(9) if selected else curses.color_pair(6)][0])
-        stdscr.addstr(y//2+(len(message)//2)+3,x//2-(maxs//2)+10,"[No]",[curses.color_pair(6) if selected else curses.color_pair(9)][0])   
+        stdscr.addstr(y//2+(len(message)//2)+3,x//2-(maxs//2),"[Yes]",[cp.set_colour(cp.WHITE,cp.BLACK) if selected else cp.set_colour(cp.BLACK,cp.WHITE)][0])
+        stdscr.addstr(y//2+(len(message)//2)+3,x//2-(maxs//2)+10,"[No]",[cp.set_colour(cp.BLACK,cp.WHITE) if selected else cp.set_colour(cp.WHITE,cp.BLACK)][0])   
         for msgl in message:
             mi += 1
-            stdscr.addstr(int(y//2+mi),int(x//2-len(msgl)//2),msgl,curses.color_pair(12))
+            stdscr.addstr(int(y//2+mi),int(x//2-len(msgl)//2),msgl,cp.set_colour(cp.GREEN,cp.WHITE))
     
         stdscr.refresh()
         
         ch = stdscr.getch()
         if ch == curses.KEY_RIGHT or ch == curses.KEY_LEFT:
             selected = not selected
         elif ch == 121 or ch == 110:
@@ -47,22 +47,22 @@
         if "\n" in o:
             message.insert(ox,o.split("\n")[1])
     message = [m[0:x-5].split("\n")[0] for m in message[0:y-5]]#Limiting characters
     maxs = max([len(s) for s in message])
     while True:
         for by in range(y//2-(len(message)//2)-1,y//2+(len(message)//2)+4):
             for bx in range(x//2-(maxs//2)-1,x//2+(maxs//2+1)+1):
-                stdscr.addstr(by,bx," ",curses.color_pair(10))
+                stdscr.addstr(by,bx," ",cp.set_colour(cp.BLUE,cp.WHITE))
         rectangle(stdscr,y//2-(len(message)//2)-1, x//2-(maxs//2)-1, y//2+(len(message)//2)+4, x//2+(maxs//2+1)+1)
         stdscr.addstr(y//2-(len(message)//2)-1, x//2-(maxs//2)-1,title)
         mi = -(len(message)/2)
-        stdscr.addstr(y//2+(len(message)//2)+3,x//2-(maxs//2),"[OK]",curses.color_pair(9)) 
+        stdscr.addstr(y//2+(len(message)//2)+3,x//2-(maxs//2),"[OK]",cp.set_colour(cp.WHITE,cp.BLACK)) 
         for msgl in message:
             mi += 1
-            stdscr.addstr(int(y//2+mi),int(x//2-len(msgl)//2),msgl,curses.color_pair(10))
+            stdscr.addstr(int(y//2+mi),int(x//2-len(msgl)//2),msgl,cp.set_colour(cp.BLUE,cp.WHITE))
     
         stdscr.refresh()
         
         ch = stdscr.getch()
         if ch == 10 or ch == 13 or ch == curses.KEY_ENTER:
             return
 
@@ -76,22 +76,22 @@
         if "\n" in o:
             message.insert(ox,o.split("\n")[1])
     message = [m[0:x-5].split("\n")[0] for m in message[0:y-5]]#Limiting characters
     maxs = max([len(s) for s in message])
     while True:
         for by in range(y//2-(len(message)//2)-1,y//2+(len(message)//2)+4):
             for bx in range(x//2-(maxs//2)-1,x//2+(maxs//2+1)+1):
-                stdscr.addstr(by,bx," ",curses.color_pair(13))
+                stdscr.addstr(by,bx," ",cp.set_colour(cp.YELLOW,cp.WHITE))
         rectangle(stdscr,y//2-(len(message)//2)-1, x//2-(maxs//2)-1, y//2+(len(message)//2)+4, x//2+(maxs//2+1)+1)
         stdscr.addstr(y//2-(len(message)//2)-1, x//2-(maxs//2)-1,title)
         mi = -(len(message)/2)
-        stdscr.addstr(y//2+(len(message)//2)+3,x//2-(maxs//2),"[OK]",curses.color_pair(9)) 
+        stdscr.addstr(y//2+(len(message)//2)+3,x//2-(maxs//2),"[OK]",cp.set_colour(cp.WHITE,cp.BLACK)) 
         for msgl in message:
             mi += 1
-            stdscr.addstr(int(y//2+mi),int(x//2-len(msgl)//2),msgl,curses.color_pair(13))
+            stdscr.addstr(int(y//2+mi),int(x//2-len(msgl)//2),msgl,cp.set_colour(cp.YELLOW,cp.WHITE))
     
         stdscr.refresh()
         
         ch = stdscr.getch()
         if ch == 10 or ch == 13 or ch == curses.KEY_ENTER:
             return
 
@@ -105,21 +105,21 @@
         if "\n" in o:
             message.insert(ox,o.split("\n")[1])
     message = [m[0:x-5].split("\n")[0] for m in message[0:y-5]]#Limiting characters
     maxs = max([len(s) for s in message])
     while True:
         for by in range(y//2-(len(message)//2)-1,y//2+(len(message)//2)+4):
             for bx in range(x//2-(maxs//2)-1,x//2+(maxs//2+1)+1):
-                stdscr.addstr(by,bx," ",curses.color_pair(11))
+                stdscr.addstr(by,bx," ",cp.set_colour(cp.RED,cp.WHITE))
         rectangle(stdscr,y//2-(len(message)//2)-1, x//2-(maxs//2)-1, y//2+(len(message)//2)+4, x//2+(maxs//2+1)+1)
         stdscr.addstr(y//2-(len(message)//2)-1, x//2-(maxs//2)-1,title)
         mi = -(len(message)/2)
-        stdscr.addstr(y//2+(len(message)//2)+3,x//2-(maxs//2),"[OK]",curses.color_pair(9)) 
+        stdscr.addstr(y//2+(len(message)//2)+3,x//2-(maxs//2),"[OK]",cp.set_colour(cp.WHITE,cp.BLACK)) 
         for msgl in message:
             mi += 1
-            stdscr.addstr(int(y//2+mi),int(x//2-len(msgl)//2),msgl,curses.color_pair(11))
+            stdscr.addstr(int(y//2+mi),int(x//2-len(msgl)//2),msgl,cp.set_colour(cp.RED,cp.WHITE))
     
         stdscr.refresh()
         
         ch = stdscr.getch()
         if ch == 10 or ch == 13 or ch == curses.KEY_ENTER:
             return
```

### Comparing `cursesplus-1.7.1/src/cursesplus.egg-info/PKG-INFO` & `cursesplus-2.0.0/src/cursesplus.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cursesplus
-Version: 1.7.1
+Version: 2.0.0
 Summary: An extension program to curses that offers option menus, message boxes, file dialogs and more
 Author-email: Enderbyte Programs <enderbyte09@gmail.com>
 Project-URL: Homepage, https://github.com/Enderbyte-Programs/Curses-Plus
 Project-URL: Bug Tracker, https://github.com/Enderbyte-Programs/Curses-Plus/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -36,24 +36,16 @@
 Microsoft Windows 11
 Any modern distro of Linux that supports Python3
 
 **Python Version 3.6 or newer**
 
 ## What's New?
 
-### Patch 1.7.1
+Version 2.0: Incompatible api changes
 
--Improve documentation
-
-### Version 1.7
-
--Add more messageboxes
-
--Messagebox.showinfo for info
-
--messagebox.showwarning for warning
-
--messagebox.showerror for errors
+-askyesno now MUST be messagebox.askyesno
+-Rewrite colour system. load_colours() is now nonexistent.
+-Now use set_colour(background,foreground). A set of colour constants are defined in the cp class.
 
 ## Uses
 
 curses-plus offers many utilities to make writing TUI applications easy. (TUI stands for Terminal User Interface)
```

