# Comparing `tmp/mapdata-1.8.0.tar.gz` & `tmp/mapdata-1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mapdata-1.8.0.tar", last modified: Mon May 15 01:29:58 2023, max compression
+gzip compressed data, was "mapdata-1.8.1.tar", last modified: Tue May 16 16:26:31 2023, max compression
```

## Comparing `mapdata-1.8.0.tar` & `mapdata-1.8.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2023-05-15 01:29:58.169349 mapdata-1.8.0/
--rw-------   0 dreas     (1000) dreas     (1000)      614 2023-05-10 02:52:31.000000 mapdata-1.8.0/LICENSE.txt
--rw-------   0 dreas     (1000) dreas     (1000)       88 2022-01-15 18:16:09.000000 mapdata-1.8.0/MANIFEST.in
--rw-rw-r--   0 dreas     (1000) dreas     (1000)     3009 2023-05-15 01:29:58.169349 mapdata-1.8.0/PKG-INFO
--rw-r--r--   0 dreas     (1000) dreas     (1000)     1866 2023-05-15 01:02:57.000000 mapdata-1.8.0/README.md
-drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2023-05-15 01:29:58.169349 mapdata-1.8.0/mapdata/
--rwxr-xr-x   0 dreas     (1000) dreas     (1000)    84596 2023-05-15 00:27:28.000000 mapdata-1.8.0/mapdata/mapdata.py
-drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2023-05-15 01:29:58.169349 mapdata-1.8.0/mapdata.egg-info/
--rw-rw-r--   0 dreas     (1000) dreas     (1000)     3009 2023-05-15 01:29:58.000000 mapdata-1.8.0/mapdata.egg-info/PKG-INFO
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      185 2023-05-15 01:29:58.000000 mapdata-1.8.0/mapdata.egg-info/SOURCES.txt
--rw-rw-r--   0 dreas     (1000) dreas     (1000)        1 2023-05-15 01:29:58.000000 mapdata-1.8.0/mapdata.egg-info/dependency_links.txt
--rw-rw-r--   0 dreas     (1000) dreas     (1000)        1 2023-05-15 01:29:58.000000 mapdata-1.8.0/mapdata.egg-info/top_level.txt
--rw-rw-r--   0 dreas     (1000) dreas     (1000)       38 2023-05-15 01:29:58.169349 mapdata-1.8.0/setup.cfg
--rw-rw-r--   0 dreas     (1000) dreas     (1000)     1279 2023-05-15 00:34:38.000000 mapdata-1.8.0/setup.py
+drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2023-05-16 16:26:31.799225 mapdata-1.8.1/
+-rw-------   0 dreas     (1000) dreas     (1000)      614 2023-05-10 02:52:31.000000 mapdata-1.8.1/LICENSE.txt
+-rw-------   0 dreas     (1000) dreas     (1000)       88 2022-01-15 18:16:09.000000 mapdata-1.8.1/MANIFEST.in
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)     3009 2023-05-16 16:26:31.799225 mapdata-1.8.1/PKG-INFO
+-rw-r--r--   0 dreas     (1000) dreas     (1000)     1866 2023-05-15 01:02:57.000000 mapdata-1.8.1/README.md
+drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2023-05-16 16:26:31.799225 mapdata-1.8.1/mapdata/
+-rwxr-xr-x   0 dreas     (1000) dreas     (1000)    85218 2023-05-16 16:06:41.000000 mapdata-1.8.1/mapdata/mapdata.py
+drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2023-05-16 16:26:31.799225 mapdata-1.8.1/mapdata.egg-info/
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)     3009 2023-05-16 16:26:31.000000 mapdata-1.8.1/mapdata.egg-info/PKG-INFO
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      185 2023-05-16 16:26:31.000000 mapdata-1.8.1/mapdata.egg-info/SOURCES.txt
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)        1 2023-05-16 16:26:31.000000 mapdata-1.8.1/mapdata.egg-info/dependency_links.txt
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)        1 2023-05-16 16:26:31.000000 mapdata-1.8.1/mapdata.egg-info/top_level.txt
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)       38 2023-05-16 16:26:31.799225 mapdata-1.8.1/setup.cfg
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)     1279 2023-05-16 16:06:59.000000 mapdata-1.8.1/setup.py
```

### Comparing `mapdata-1.8.0/LICENSE.txt` & `mapdata-1.8.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mapdata-1.8.0/PKG-INFO` & `mapdata-1.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapdata
-Version: 1.8.0
+Version: 1.8.1
 Summary: An interactive map and table explorer for geographic coordinates in a CSV file
 Home-page: https://osdn.net/project/mapdata/
 Author: Dreas Nielsen
 Author-email: dreas.nielsen@gmail.com
 License: GPL
 Keywords: Map,Locations,CRS,CSV,PNG,JPG,Postscript
 Platform: UNKNOWN
```

### Comparing `mapdata-1.8.0/README.md` & `mapdata-1.8.1/README.md`

 * *Files identical despite different names*

### Comparing `mapdata-1.8.0/mapdata/mapdata.py` & `mapdata-1.8.1/mapdata/mapdata.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,35 +1,32 @@
 #!/usr/bin/python
 #
-# mapdata_3.py
+# mapdata.py
 #
 # PURPOSE
 #	Create a simple interactive map of data points in Tkinter.
 #
 # COPYRIGHT AND LICENSE
-#	Copyright (c) 2022, R. Dreas Nielsen
+#	Copyright (c) 2023, R. Dreas Nielsen
 # 	This program is free software: you can redistribute it and/or modify
 # 	it under the terms of the GNU General Public License as published by
 # 	the Free Software Foundation, either version 3 of the License, or
 # 	(at your option) any later version.
 # 	This program is distributed in the hope that it will be useful,
 # 	but WITHOUT ANY WARRANTY; without even the implied warranty of
 # 	MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # 	GNU General Public License for more details.
 # 	The GNU General Public License is available at <http://www.gnu.org/licenses/>
-##
+#
 # NOTES
-#	1. This uses the "tkintermapview" library.
+#	1.
 #
 # AUTHOR
 #	Dreas Nielsen (RDN)
 #
-# TODO
-#	1. Enable export of selected table rows and map image.
-#
 # HISTORY
 #	 Date		 Remarks
 #	----------	-----------------------------------------------------
 #	2023-03-27	Created.  RDN.
 #	2023-04-16	Added CsvFile() and treeview_table(), and began
 #				MapUI().  RDN.
 #	2023-04-24	Completed MapUI() and tested to success.
@@ -59,18 +56,21 @@
 #	2023-05-08	Added conversion of other coordinate reference systems to 4326.  RDN.
 #	2023-05-09	Added ability to switch CRSs for the same data.  RDN.
 #	2023-05-11	Fixed map controls when resizing.  Added command-line arguments
 #				to export the map and quit.  RDN.
 #	2023-05-12	Added export of configuration settings.  Cleaned up help
 #				dialogs.  RDN.
 #	2023-05-14	Put the map and table in a PanedWindow.  RDN.
+#	2023-05-16	Fixed label wrapping in Windows on the CSV open dialog.  Corrected
+#				binding of Return and Escape keys to dialog button actions.  Adujsted
+#				button position in MsgDialog.  RDN.
 # ==================================================================
 
-version = "1.8.0"
-vdate = "2023-05-14"
+version = "1.8.1"
+vdate = "2023-05-16"
 
 copyright = "2023"
 
 
 import sys
 import os.path
 import io
@@ -96,15 +96,15 @@
 config_files = []
 # Configuration file read post-startup
 config_files_user = []
 
 
 # Default options
 multiselect = "0"
-#-- Default location marker.  This may be overridden by data columns in the input file.
+#-- Default location marker.  This may be overridden
 location_marker = "triangle_open"
 location_color = "black"
 #-- Selected item marker
 select_symbol = "wedge"
 select_color = "red"
 #-- Label appearance
 label_color = "black"
@@ -377,15 +377,15 @@
 		"steelblue", "tan", "teal", "thistle", "tomato", "turquoise", "violet", "wheat", "white", "whitesmoke", "yellow",
 		"yellowgreen")
 
 # A shorter list for interactive selection of the marker color
 select_colors = ('aqua', 'black', 'blue', 'blueviolet', 'brown', 'chartreuse', 'cornflowerblue', 'crimson',
 		'cyan', 'darkblue', 'darkgreen', 'darkmagenta', 'darkorange', 'darkred', 'darkslategray', 'deeppink',
 		'forestgreen', 'fuschia', 'green', 'greenyellow', 'magenta', 'maroon', 'navy', 'orange', 'orangered',
-		'purple', 'red', 'violet', 'yellow', 'yellowgreen')
+		'purple', 'red', 'violet', 'white', 'yellow', 'yellowgreen')
 
 
 # List of imported symbol names and paths
 imported_symbols = []
 
 # Keys for custom symbols are made up of the color name and the icon name, separated with a space.
 custom_icons = {}
@@ -652,17 +652,18 @@
 			wht = int(m.group(2))
 			swd = self.win.winfo_screenwidth()
 			sht = self.win.winfo_screenheight()
 			xpos = (swd/2) - (wwd/2)
 			ypos = (sht/2) - (wht/2)
 			self.win.geometry("%dx%d+%d+%d" % (wwd, wht, xpos, ypos))
 		# Limit resizing
-		self.win.minsize(width=300, height=0)
+		self.win.minsize(width=400, height=400)
 		# Set table status message
 		self.set_status()
+		# Just export the map and quit?
 		if map_export_file is not None:
 			self.imageoutputfile = map_export_file
 			self.win.after(export_time_sec * 1000, self.export_map_and_quit)
 	def available_tile_servers(self):
 		# Return a list of those without API keys or for which API keys are provided
 		avail = []
 		for k in bm_servers:
@@ -1235,19 +1236,20 @@
 		color_opts.grid(row=1, column=1, sticky=tk.W, padx=(3,3))
 		# Buttons
 		self.canceled = False
 		cancel_btn = ttk.Button(btn_frame, text="Cancel", command=self.do_cancel)
 		cancel_btn.grid(row=0, column=1, sticky=tk.E, padx=(3,5))
 		ok_btn = ttk.Button(btn_frame, text="Ok", command=self.do_select)
 		ok_btn.grid(row=0, column=0, sticky=tk.E, padx=(60,2))
-		ok_btn.bind("<Return>", self.do_select)
-	def do_cancel(self):
+		self.dlg.bind("<Return>", self.do_select)
+		self.dlg.bind("<Escape>", self.do_cancel)
+	def do_cancel(self, *args):
 		self.canceled = True
 		self.dlg.destroy()
-	def do_select(self):
+	def do_select(self, *args):
 		self.canceled = False
 		self.dlg.destroy()
 	def get_marker(self):
 		self.dlg.grab_set()
 		self.symbol_opts.focus()
 		self.dlg.wait_window(self.dlg)
 		if not self.canceled:
@@ -1296,19 +1298,20 @@
 		# Buttons
 		self.canceled = False
 		cancel_btn = ttk.Button(btn_frame, text="Cancel", command=self.do_cancel)
 		cancel_btn.grid(row=0, column=1, sticky=tk.E, padx=(3,5))
 		ok_btn = ttk.Button(btn_frame, text="Ok", command=self.do_select)
 		ok_btn["state"] = tk.DISABLED
 		ok_btn.grid(row=0, column=0, sticky=tk.E, padx=(60,2))
-		ok_btn.bind("<Return>", self.do_select)
-	def do_cancel(self):
+		self.dlg.bind("<Return>", self.do_select)
+		self.dlg.bind("<Escape>", self.do_cancel)
+	def do_cancel(self, *args):
 		self.canceled = True
 		self.dlg.destroy()
-	def do_select(self):
+	def do_select(self, *args):
 		self.canceled = False
 		self.dlg.destroy()
 	def run(self):
 		self.dlg.grab_set()
 		self.symbol_entry.focus()
 		self.dlg.wait_window(self.dlg)
 		if not self.canceled:
@@ -1357,16 +1360,19 @@
 		btn_frame = tk.Frame(self.dlg, borderwidth=3, relief=tk.RIDGE)
 		btn_frame.grid(row=1, column=0, sticky=tk.EW, padx=(3,3), pady=(3,3))
 		btn_frame.columnconfigure(0, weight=1)
 		# Prompts
 		#-- Directions
 		dir_lbl = ttk.Label(dir_frame,
 				text="Select a CSV file with columns containing latitude and longitude values, and optionally other information.",
-				width=80, justify=tk.LEFT, wraplength=650)
+				width=80, justify=tk.LEFT, wraplength=600)
 		dir_lbl.grid(row=0, column=0, padx=(3,3), pady=(3,3))
+		def wrap_msg(event):
+			dir_lbl.configure(wraplength=event.width - 5)
+		dir_lbl.bind("<Configure>", wrap_msg)
 		#-- Filename
 		fn_frame = tk.Frame(req_frame)
 		fn_frame.grid(row=0, column=0, sticky=tk.EW, pady=(5,5))
 		fn_label = ttk.Label(fn_frame, text="File:")
 		fn_label.grid(row=0, column=0, sticky=tk.E, padx=(3,3))
 		self.fn_var = tk.StringVar(fn_frame, '')
 		self.fn_var.trace('w', new_fn)
@@ -1429,22 +1435,24 @@
 		# Buttons
 		self.canceled = False
 		cancel_btn = ttk.Button(btn_frame, text="Cancel", command=self.do_cancel)
 		cancel_btn.grid(row=0, column=2, sticky=tk.E, padx=3)
 		ok_btn = ttk.Button(btn_frame, text="Ok", command=self.do_select)
 		ok_btn.grid(row=0, column=1, sticky=tk.E, padx=3)
 		ok_btn["state"] = tk.DISABLED
-		ok_btn.bind("<Return>", self.do_select)
-		cancel_btn.bind("<Escape>", self.do_cancel)
-	def do_cancel(self):
+		self.dlg.bind("<Return>", self.do_select)
+		self.dlg.bind("<Escape>", self.do_cancel)
+		self.dlg.resizable(False, False)
+	def do_cancel(self, *args):
 		self.canceled = True
 		self.dlg.destroy()
-	def do_select(self):
-		self.canceled = False
-		self.dlg.destroy()
+	def do_select(self, *args):
+		if self.fn_var.get() != '' and self.lat_var.get() != '' and self.lon_var.get() != '':
+			self.canceled = False
+			self.dlg.destroy()
 	def get_datafile(self):
 		self.dlg.grab_set()
 		self.dlg.wait_window(self.dlg)
 		self.dlg = None
 		if not self.canceled:
 			return (self.fn_var.get(), self.id_var.get(), self.lat_var.get(), self.lon_var.get(),
 					self.crs_var.get(), self.sym_var.get(), self.col_var.get(), self.title_var.get())
@@ -1468,19 +1476,20 @@
 		self.crs_entry.grid(row=0, column=1, sticky=tk.W, padx=(3,3))
 		# Buttons
 		self.canceled = False
 		cancel_btn = ttk.Button(btn_frame, text="Cancel", command=self.do_cancel)
 		cancel_btn.grid(row=0, column=1, sticky=tk.E, padx=(3,5))
 		ok_btn = ttk.Button(btn_frame, text="Ok", command=self.do_select)
 		ok_btn.grid(row=0, column=0, sticky=tk.E, padx=(3,3))
-		ok_btn.bind("<Return>", self.do_select)
-	def do_cancel(self):
+		self.dlg.bind("<Return>", self.do_select)
+		self.dlg.bind("<Escape>", self.do_cancel)
+	def do_cancel(self, *args):
 		self.canceled = True
 		self.dlg.destroy()
-	def do_select(self):
+	def do_select(self, *args):
 		self.canceled = False
 		self.dlg.destroy()
 	def get_crs(self):
 		self.dlg.grab_set()
 		self.crs_entry.focus()
 		self.dlg.wait_window(self.dlg)
 		if not self.canceled:
@@ -1500,21 +1509,23 @@
 		#center_y = int(scr_height/2 - height / 2)
 		#self.dlg.geometry(f'{width}x{height}+{center_x}+{center_y}')
 		prompt_frame = tk.Frame(self.dlg)
 		prompt_frame.grid(row=0, column=0, sticky=tk.NSEW, pady=(3,3))
 		msg_lbl = ttk.Label(prompt_frame, text=message)
 		msg_lbl.grid(row=0, column=0, padx=(6,6), pady=(3,3))
 		btn_frame = tk.Frame(self.dlg, borderwidth=3, relief=tk.RIDGE)
+		btn_frame.columnconfigure(0, weight=1)
 		btn_frame.grid(row=1, column=0, sticky=tk.EW, pady=(3,3))
 		# Buttons
 		self.canceled = False
 		ok_btn = ttk.Button(btn_frame, text="Close", command=self.do_select)
 		ok_btn.grid(row=0, column=0, sticky=tk.E, padx=(6,6))
-		ok_btn.bind("<Return>", self.do_select)
-	def do_select(self):
+		self.dlg.bind("<Return>", self.do_select)
+		self.dlg.bind("<Escape>", self.do_select)
+	def do_select(self, *args):
 		self.dlg.destroy()
 	def show(self):
 		self.dlg.grab_set()
 		self.dlg.wait_window(self.dlg)
```

### Comparing `mapdata-1.8.0/mapdata.egg-info/PKG-INFO` & `mapdata-1.8.1/mapdata.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapdata
-Version: 1.8.0
+Version: 1.8.1
 Summary: An interactive map and table explorer for geographic coordinates in a CSV file
 Home-page: https://osdn.net/project/mapdata/
 Author: Dreas Nielsen
 Author-email: dreas.nielsen@gmail.com
 License: GPL
 Keywords: Map,Locations,CRS,CSV,PNG,JPG,Postscript
 Platform: UNKNOWN
```

### Comparing `mapdata-1.8.0/setup.py` & `mapdata-1.8.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 import io
 
 with io.open('README.md', encoding='utf-8') as f:
 	long_description = f.read()
 
 setuptools.setup(name='mapdata',
-	version='1.8.0',
+	version='1.8.1',
 	description="An interactive map and table explorer for geographic coordinates in a CSV file",
 	author='Dreas Nielsen',
 	author_email='dreas.nielsen@gmail.com',
     url='https://osdn.net/project/mapdata/',
 	scripts=['mapdata/mapdata.py'],
     license='GPL',
 	requires=['tkintermapview', 'pyproj', 'odfpy'],
```

