# Comparing `tmp/tklinenums-1.5.1.tar.gz` & `tmp/tklinenums-1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tklinenums-1.5.1.tar", last modified: Tue Jan 24 15:12:48 2023, max compression
+gzip compressed data, was "tklinenums-1.6.tar", last modified: Fri Apr  7 19:01:06 2023, max compression
```

## Comparing `tklinenums-1.5.1.tar` & `tklinenums-1.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 joshyacktman   (501) staff       (20)        0 2023-01-24 15:12:48.476641 tklinenums-1.5.1/
--rw-r--r--   0 joshyacktman   (501) staff       (20)      712 2023-01-24 15:12:48.476384 tklinenums-1.5.1/PKG-INFO
--rw-r--r--   0 joshyacktman   (501) staff       (20)      456 2022-09-29 22:15:36.000000 tklinenums-1.5.1/README.md
--rw-r--r--   0 joshyacktman   (501) staff       (20)       38 2023-01-24 15:12:48.476703 tklinenums-1.5.1/setup.cfg
--rw-r--r--   0 joshyacktman   (501) staff       (20)      461 2023-01-24 14:32:32.000000 tklinenums-1.5.1/setup.py
-drwxr-xr-x   0 joshyacktman   (501) staff       (20)        0 2023-01-24 15:12:48.474049 tklinenums-1.5.1/tklinenums/
--rw-r--r--   0 joshyacktman   (501) staff       (20)       37 2022-09-23 12:50:43.000000 tklinenums-1.5.1/tklinenums/__init__.py
--rw-r--r--   0 joshyacktman   (501) staff       (20)     9195 2023-01-24 15:11:25.000000 tklinenums-1.5.1/tklinenums/tklinenums.py
-drwxr-xr-x   0 joshyacktman   (501) staff       (20)        0 2023-01-24 15:12:48.476010 tklinenums-1.5.1/tklinenums.egg-info/
--rw-r--r--   0 joshyacktman   (501) staff       (20)      712 2023-01-24 15:12:48.000000 tklinenums-1.5.1/tklinenums.egg-info/PKG-INFO
--rw-r--r--   0 joshyacktman   (501) staff       (20)      202 2023-01-24 15:12:48.000000 tklinenums-1.5.1/tklinenums.egg-info/SOURCES.txt
--rw-r--r--   0 joshyacktman   (501) staff       (20)        1 2023-01-24 15:12:48.000000 tklinenums-1.5.1/tklinenums.egg-info/dependency_links.txt
--rw-r--r--   0 joshyacktman   (501) staff       (20)       11 2023-01-24 15:12:48.000000 tklinenums-1.5.1/tklinenums.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 19:01:06.550646 tklinenums-1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-04-07 19:01:06.550646 tklinenums-1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-07 19:00:50.000000 tklinenums-1.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-07 19:01:06.550646 tklinenums-1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-04-07 19:00:50.000000 tklinenums-1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 19:01:06.546646 tklinenums-1.6/tklinenums/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-07 19:00:50.000000 tklinenums-1.6/tklinenums/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10823 2023-04-07 19:00:50.000000 tklinenums-1.6/tklinenums/tklinenums.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 19:01:06.550646 tklinenums-1.6/tklinenums.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-04-07 19:01:06.000000 tklinenums-1.6/tklinenums.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-07 19:01:06.000000 tklinenums-1.6/tklinenums.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 19:01:06.000000 tklinenums-1.6/tklinenums.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-07 19:01:06.000000 tklinenums-1.6/tklinenums.egg-info/top_level.txt
```

### Comparing `tklinenums-1.5.1/PKG-INFO` & `tklinenums-1.6/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,14 @@
-Metadata-Version: 2.1
-Name: tklinenums
-Version: 1.5.1
-Summary: A simple Tkinter widget for displaying line numbers
-Home-page: https://github.com/Moosems/TkLineNums
-Author: Moosems
-Author-email: moosems.j@gmail.com
-Description-Content-Type: text/markdown
-
-# TkLineNums V.1.5
+# TkLineNums V.1.6
 
 TkLineNums is a simple line numbering widget for Tkinter. It supports ttk themes through the set_to_ttk_style method.
 
 ![img](https://github.com/Moosems/TkLineNums/raw/main/images/TkLineNumsPhoto.png)
 
 ## Features
 
 * Clicking on line numbers will set the insert to the beginning of the line.
+* Shift clicking will select all text from the end of the line clicked by cursor and the insert position.
+* Awful click-drag scrolling (Needs help)
 * Scrolling the linebar will scroll the text widget
 * Supports ttk themes
-* Supports left, right, and center alignment with the `justify` option
+* Supports left, right, and center alignment with the `justify` option
```

### Comparing `tklinenums-1.5.1/tklinenums/tklinenums.py` & `tklinenums-1.6/tklinenums/tklinenums.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+"""TkLineNumbers - A line number widget for tkinter Text widgets"""
 from __future__ import annotations
 
 import platform
 from tkinter import Canvas, Event, Misc, Text
 from tkinter.font import Font
 
 system: str = str(platform.system())
@@ -91,32 +92,38 @@
             )
 
     def mouse_scroll(self, event: Event) -> None:
         """Scrolls the text widget when the mouse wheel is scrolled -- Internal use only"""
         if system == "Darwin":
             self.textwidget.yview_scroll(scroll_inversion * event.delta, "units")
         else:
-            self.textwidget.yview_scroll(int(scroll_inversion * (event.delta / 120)), "units")
+            self.textwidget.yview_scroll(
+                int(scroll_inversion * (event.delta / 120)), "units"
+            )
         self.redraw()
 
     def click_see(self, event: Event) -> None:
-        """When clicking on a line number it scrolls to that line -- Internal use only"""
-        # Add shift click
+        """When clicking on a line number it scrolls to that line if not shifting -- Internal use only"""
+        if event.state == 1:
+            self.shift_click(event)
+            return
         self.textwidget.tag_remove("sel", "1.0", "end")
         self.textwidget.mark_set(
             "insert",
             f"{self.textwidget.index(f'@{event.x},{event.y}').split('.')[0]}.0",
         )
         self.textwidget.see("insert")
         first_visible_line, last_visible_line = int(
             self.textwidget.index("@0,0").split(".")[0]
         ), int(
             self.textwidget.index(f"@0,{self.textwidget.winfo_height()}").split(".")[0]
         )
-        if (insert := int(self.textwidget.index("insert").split(".")[0])) == first_visible_line:
+        if (
+            insert := int(self.textwidget.index("insert").split(".")[0])
+        ) == first_visible_line:
             self.textwidget.yview_scroll(-1, "units")
         elif insert == last_visible_line:
             self.textwidget.yview_scroll(1, "units")
         self.click_pos = self.textwidget.index("insert")
 
     def unclick(self, event: Event) -> None:
         """When the mouse button is released it removes the selection -- Internal use only"""
@@ -125,35 +132,69 @@
     def double_click(self, event: Event) -> None:
         """Selects the line when double clicked -- Internal use only"""
         self.textwidget.tag_remove("sel", "1.0", "end")
         self.textwidget.tag_add("sel", "insert", "insert + 1 line")
 
     def drag(self, event: Event) -> None:
         """When click dragging it selects the text -- Internal use only"""
+
+        """
+        Issues:
+         - Once it starts going it's hard to stop drag clicking (because most people pull back up when done but this is still
+           considered dragging and it remembers the direction meaning it will continue to drag in that direction)
+         - When you reach your end point for scroll clicking you can't go back unless you go completely the opposite way which 
+           then means you can't go back the original way
+         - When you go down and then try to go back up you can't
+         - Must continue to drag cursor for it to select more even if cursor is off-screen or trying to slowly select more (Means
+           it might need to become recursive)
+        """ #TODO: Fix issues
         if self.click_pos is None:
             return
         start, end = self.textwidget.index("insert"), self.click_pos
         if self.textwidget.compare("insert", ">", self.click_pos):
             start, end = end, start
         self.textwidget.mark_set("insert", f"@0,{event.y}")
         self.textwidget.tag_remove("sel", "1.0", "end")
         self.textwidget.tag_add("sel", start, end)
-        first_line, last_line = self.textwidget.index("@0,0").split(".")[0], self.textwidget.index(f"@0,{self.textwidget.winfo_height()}").split(".")[0]
+        first_line, last_line = (
+            self.textwidget.index("@0,0").split(".")[0],
+            self.textwidget.index(f"@0,{self.textwidget.winfo_height()}").split(".")[0],
+        )
         if end.split(".")[0] == last_line and event.y > self.winfo_y():
-            self.textwidget.yview_scroll(1, "units") if system == "Darwin" else self.textwidget.yview_scroll((1 / 120), "units")
-            self.textwidget.tag_add("sel", start, str(float(end)+1))
-            self.textwidget.mark_set("insert", str(float(end)+1))
+            self.textwidget.yview_scroll(
+                1, "units"
+            ) if system == "Darwin" else self.textwidget.yview_scroll(
+                (1 / 120), "units"
+            )
+            self.textwidget.tag_add("sel", start, str(float(end) + 1))
+            self.textwidget.mark_set("insert", str(float(end) + 1))
             return None
-        elif start.split(".")[0] == first_line and event.y < self.winfo_y() + self.winfo_height():
-            self.textwidget.yview_scroll(-1, "units") if system == "Darwin" else self.textwidget.yview_scroll((-1 / 120), "units")
-            self.textwidget.tag_add("sel", str(float(start)-1), end)
-            self.textwidget.mark_set("insert", str(float(start)-1))
+        elif (
+            start.split(".")[0] == first_line
+            and event.y < self.winfo_y() + self.winfo_height()
+        ):
+            self.textwidget.yview_scroll(
+                -1, "units"
+            ) if system == "Darwin" else self.textwidget.yview_scroll(
+                (-1 / 120), "units"
+            )
+            self.textwidget.tag_add("sel", str(float(start) - 1), end)
+            self.textwidget.mark_set("insert", str(float(start) - 1))
             return None
         self.redraw()
 
+    def shift_click(self, event: Event) -> None:
+        """When shift clicking it selects the text between the click and the cursor -- Internal use only"""
+        start_pos, end_pos = self.textwidget.index("insert"), self.textwidget.index(
+            f"@0,{event.y}"
+        )
+        self.textwidget.tag_remove("sel", "1.0", "end")
+        if self.textwidget.compare(start_pos, ">", end_pos):
+            start_pos, end_pos = end_pos, start_pos
+        self.textwidget.tag_add("sel", start_pos, end_pos)
 
     def resize(self) -> None:
         """Resizes the widget to fit the text widget"""
         end = self.textwidget.index("end").split(".")[0]
         self.config(width=self.font.measure(" 1234 ")) if int(
             end
         ) <= 1000 else self.config(width=self.font.measure(f" {end} "))
@@ -188,16 +229,16 @@
                     )[:-1]
                 ),
                 size=font[-1],
             )
 
 
 if __name__ == "__main__":
-    from tkinter import Text, Tk
     import platform
+    from tkinter import Text, Tk
     from tkinter.font import Font
     from tkinter.ttk import Style
 
     system = str(platform.system())
 
     if system == "Darwin":
         contmand = "Command"
```

