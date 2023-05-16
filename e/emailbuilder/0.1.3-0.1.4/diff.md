# Comparing `tmp/emailbuilder-0.1.3.tar.gz` & `tmp/emailbuilder-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emailbuilder-0.1.3.tar", last modified: Tue Feb  7 03:37:05 2023, max compression
+gzip compressed data, was "emailbuilder-0.1.4.tar", last modified: Tue May 16 20:13:52 2023, max compression
```

## Comparing `emailbuilder-0.1.3.tar` & `emailbuilder-0.1.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 03:37:05.783802 emailbuilder-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     5402 2023-02-07 03:37:05.783802 emailbuilder-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4909 2023-02-07 03:36:53.000000 emailbuilder-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 03:37:05.783802 emailbuilder-0.1.3/emailbuilder/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-02-07 03:36:53.000000 emailbuilder-0.1.3/emailbuilder/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 03:37:05.783802 emailbuilder-0.1.3/emailbuilder/components/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-02-07 03:36:53.000000 emailbuilder-0.1.3/emailbuilder/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-02-07 03:36:53.000000 emailbuilder-0.1.3/emailbuilder/components/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3729 2023-02-07 03:36:53.000000 emailbuilder-0.1.3/emailbuilder/components/containers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-02-07 03:36:53.000000 emailbuilder-0.1.3/emailbuilder/components/elements.py
--rw-r--r--   0 runner    (1001) docker     (123)     3302 2023-02-07 03:36:53.000000 emailbuilder-0.1.3/emailbuilder/components/embeddables.py
--rw-r--r--   0 runner    (1001) docker     (123)     4600 2023-02-07 03:36:53.000000 emailbuilder-0.1.3/emailbuilder/email.py
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-02-07 03:36:53.000000 emailbuilder-0.1.3/emailbuilder/experimental.py
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-02-07 03:36:53.000000 emailbuilder-0.1.3/emailbuilder/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 03:37:05.783802 emailbuilder-0.1.3/emailbuilder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5402 2023-02-07 03:37:05.000000 emailbuilder-0.1.3/emailbuilder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-02-07 03:37:05.000000 emailbuilder-0.1.3/emailbuilder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-07 03:37:05.000000 emailbuilder-0.1.3/emailbuilder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-02-07 03:37:05.000000 emailbuilder-0.1.3/emailbuilder.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-02-07 03:36:53.000000 emailbuilder-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-07 03:37:05.783802 emailbuilder-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-02-07 03:36:53.000000 emailbuilder-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:13:52.775050 emailbuilder-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     5485 2023-05-16 20:13:52.775050 emailbuilder-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4992 2023-05-16 20:13:38.000000 emailbuilder-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:13:52.775050 emailbuilder-0.1.4/emailbuilder/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-16 20:13:38.000000 emailbuilder-0.1.4/emailbuilder/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:13:52.775050 emailbuilder-0.1.4/emailbuilder/components/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-16 20:13:38.000000 emailbuilder-0.1.4/emailbuilder/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5291 2023-05-16 20:13:38.000000 emailbuilder-0.1.4/emailbuilder/components/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4044 2023-05-16 20:13:38.000000 emailbuilder-0.1.4/emailbuilder/components/containers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-05-16 20:13:38.000000 emailbuilder-0.1.4/emailbuilder/components/elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3460 2023-05-16 20:13:38.000000 emailbuilder-0.1.4/emailbuilder/components/embeddables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8034 2023-05-16 20:13:38.000000 emailbuilder-0.1.4/emailbuilder/email.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-05-16 20:13:38.000000 emailbuilder-0.1.4/emailbuilder/experimental.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-05-16 20:13:38.000000 emailbuilder-0.1.4/emailbuilder/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:13:52.775050 emailbuilder-0.1.4/emailbuilder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5485 2023-05-16 20:13:52.000000 emailbuilder-0.1.4/emailbuilder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-05-16 20:13:52.000000 emailbuilder-0.1.4/emailbuilder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 20:13:52.000000 emailbuilder-0.1.4/emailbuilder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-16 20:13:52.000000 emailbuilder-0.1.4/emailbuilder.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-05-16 20:13:38.000000 emailbuilder-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 20:13:52.775050 emailbuilder-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-05-16 20:13:38.000000 emailbuilder-0.1.4/setup.py
```

### Comparing `emailbuilder-0.1.3/PKG-INFO` & `emailbuilder-0.1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emailbuilder
-Version: 0.1.3
+Version: 0.1.4
 Summary: Simple HTML e-mail generator
 Home-page: https://github.com/coheleth/emailbuilder
 Author: Coheleth
 Author-email: Diogo Silva <diogopiccirillo@gmail.com>
 License: MIT
 Project-URL: homepage, https://github.com/coheleth/emailbuilder
 Project-URL: documentation, https://github.com/coheleth/emailbuilder
@@ -22,15 +22,15 @@
   - [Table of Contents](#table-of-contents)
   - [Installation](#installation)
   - [Usage](#usage)
   - [The EMail Class/Object](#the-email-classobject)
     - [Attributes](#attributes)
       - [Subject](#subject)
       - [Sender](#sender)
-      - [Receiver](#receiver)
+      - [Receiver, Copy and Blind Copy](#receiver-copy-and-blind-copy)
       - [Style](#style)
     - [Methods](#methods)
       - [email.append()](#emailappend)
       - [email.attach()](#emailattach)
       - [email.html()](#emailhtml)
       - [email.plain() (W.I.P.)](#emailplain-wip)
       - [email.message()](#emailmessage)
@@ -123,15 +123,15 @@
 
 The e-mail's subject, as a string
 
 #### Sender
 
 The sender's e-mail, as a string
 
-#### Receiver
+#### Receiver, Copy and Blind Copy
 
 The receiver(s)'s e-mail(s), as either a string or a list
 
 #### Style
 
 A dictionary containing the basic style rules for the e-mail.
 (More information concerning styling to be added)
@@ -272,10 +272,11 @@
 ---
 
 ## To-Do
 
 - [x] Write basic usage guide
 - [x] Add win32com.client outlook support
 - [x] Improve classes and functions documentation
+- [x] Add CC and BCC
 - [ ] Add table component
 - [ ] Document `style` argument
 - [ ] Improve plain text function
```

### Comparing `emailbuilder-0.1.3/README.md` & `emailbuilder-0.1.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
   - [Table of Contents](#table-of-contents)
   - [Installation](#installation)
   - [Usage](#usage)
   - [The EMail Class/Object](#the-email-classobject)
     - [Attributes](#attributes)
       - [Subject](#subject)
       - [Sender](#sender)
-      - [Receiver](#receiver)
+      - [Receiver, Copy and Blind Copy](#receiver-copy-and-blind-copy)
       - [Style](#style)
     - [Methods](#methods)
       - [email.append()](#emailappend)
       - [email.attach()](#emailattach)
       - [email.html()](#emailhtml)
       - [email.plain() (W.I.P.)](#emailplain-wip)
       - [email.message()](#emailmessage)
@@ -109,15 +109,15 @@
 
 The e-mail's subject, as a string
 
 #### Sender
 
 The sender's e-mail, as a string
 
-#### Receiver
+#### Receiver, Copy and Blind Copy
 
 The receiver(s)'s e-mail(s), as either a string or a list
 
 #### Style
 
 A dictionary containing the basic style rules for the e-mail.
 (More information concerning styling to be added)
@@ -258,10 +258,11 @@
 ---
 
 ## To-Do
 
 - [x] Write basic usage guide
 - [x] Add win32com.client outlook support
 - [x] Improve classes and functions documentation
+- [x] Add CC and BCC
 - [ ] Add table component
 - [ ] Document `style` argument
 - [ ] Improve plain text function
```

### Comparing `emailbuilder-0.1.3/emailbuilder/components/base.py` & `emailbuilder-0.1.4/emailbuilder/components/containers.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,132 +1,123 @@
-from ..utils import const, parse_style
+from .base import Component, Container
+from ..utils import const, parse_style, parse_properties
 from typing import Any, Optional
 
 
-class Component:
+class OrderedList(Container):
   """
-  Base component class
+  An ordered list element
+  <OL />
 
   :param style: Custom style rules
   """
 
-  def __init__(self, style: Optional[dict] = None) -> None:
-    if style is None:
-      style = {}
-    self.style = style
-    self.keys = ["global"]
-    self.email = None
-
-  def apply_style(self, style: dict) -> dict:
-    """
-    Concatenates the component's inherited
-    style rules with its custom ones
-    """
-    _applied_style = {}
-
-    for key, value in style.items():
-      if key in self.keys and type(value) is dict:
-        for attr, value in value.items():
-          _applied_style[attr] = value
-
-    return _applied_style
-
-  def html(self, style) -> str:
-    """
-    Renders the HTML code for the component
-
-    :param style : The component's inherited style rules
-
-    :return: The HTML code for the component
-    """
-    _style = style
-    return ""
+  def __init__(self, style: Optional[dict] = None, properties: Optional[dict] = None, kwargs: Optional[dict] = None) -> None:
+    super().__init__(style, properties)
+    self.order_prefix = ""
+
+  def render_child(self, child: Any, style: dict) -> str:
+    if issubclass(type(child), Component):
+      return f"<li>{child.html(style)}</li>"
+    else:
+      return f"<li>{str(child)}</li>"
+
+  def html(self, style: dict) -> str:
+    _style = {**self.apply_style(style), **self.style}
+    return f"<ol style=\"{parse_style(_style)}\" {parse_properties(self.properties)}>{self.render_children(style)}</ol>"
 
   def plain(self) -> str:
-    """
-    Gets the component as plain text
+    _tab = self.indent + ' ' * const["tab_size"]
+    _plain = ""
+    for i, child in enumerate(self.children):
+      _prefix = f"{self.order_prefix}{i+1}."
+      if issubclass(type(child), OrderedList):
+        child.indent = _tab
+        child.order_prefix = _prefix
+        _plain += f"{child.plain()}"
+      elif issubclass(type(child), Container):
+        child.indent = _tab + (" " * (len(_prefix) + 1))
+        _plain += f"{_tab}{_prefix} {child.plain()[(len(_tab + _prefix) + 1):]}"
+      elif issubclass(type(child), Component):
+        _plain += f"{_tab}{_prefix} {child.plain()}\n"
+      else:
+        _plain += f"{_tab}{_prefix} {str(child)}\n"
+    return _plain
 
-    :return: The component as plain text
-    """
-    return ""
 
+class UnorderedList(Container):
 
-class Container(Component):
   """
-  Base container component class
+  An unordered list element
+  <UL />
 
   :param style: Custom style rules
   """
 
-  def __init__(self, style=None) -> None:
-    super().__init__(style)
-    self.children = []
-    self.before = "<div style={style}>"
-    self.after = "</div>"
-    self.keys.extend(["container"])
-    self.indent = ""
-
-  def append(self, item: str | Component) -> None:
-    """
-    Appends a child component to the container
-
-    :param item: Component or text to append
-    """
-    self.children.append(item)
-
-  def render_child(self, child: Any, style: dict) -> str:
-    """
-    Renders a child component to HTML
+  def __init__(self, decorator: str = "*", style: Optional[dict] = None, properties: Optional[dict] = None, kwargs: Optional[dict] = None) -> None:
+    super().__init__(style, properties)
+    self.decorator = decorator + " "
 
-    :param child: Component to render
-    :param style: The style rules the child will inherit
 
-    :return: The rendered HTML
-    """
+  def render_child(self, child: Any, style: dict) -> str:
     if issubclass(type(child), Component):
-      child.email = self.email
-      return child.html(style)
+      return f"<li>{child.html(style)}</li>"
     else:
-      return f"{str(child)}<br/>"
-
-  def render_children(self, style: dict) -> str:
-    """
-    Renders the container's children to HTML
-
-    :param style: The style rules the child components will inherit
+      return f"<li>{str(child)}</li>"
 
-    :return: The rendered HTML
-    """
+  def html(self, style: dict) -> str:
     _style = {**self.apply_style(style), **self.style}
-    _append_style = {}
-    for key in self.keys:
-      if key != "global":
-        _append_style[key] = self.style
-    _combined_style = {**style, **_append_style}
-
-    _passable_attrs = ["color", "font-family", "font-size", "font-weight"]
-    for attr in _passable_attrs:
-      # print(f"{attr}: {attr in self.apply_style(style).keys()}")
-      if attr in _style.keys():
-        _combined_style["global"][attr] = _style[attr]
+    return f"<ul style=\"{parse_style(_style)}\" {parse_properties(self.properties)}>{self.render_children(style)}</ul>"
 
-    _html = ""
+  def plain(self) -> str:
+    _tab = self.indent + ' ' * const["tab_size"]
+    _plain = ""
     for i, child in enumerate(self.children):
-      _html += self.render_child(child, _combined_style)
-    return _html
+      if issubclass(type(child), UnorderedList):
+        child.indent = _tab
+        _plain += child.plain()
+      elif issubclass(type(child), Container):
+        child.indent = _tab + (" " * len(self.decorator))
+        _plain += _tab + self.decorator + \
+            child.plain()[len(_tab + self.decorator):]
+      elif issubclass(type(child), Component):
+        _plain += _tab + self.decorator + child.plain() + "\n"
+      else:
+        _plain += _tab + self.decorator + str(child) + "\n"
+    return _plain
+
+
+class Table(Container):
+
+  """
+  A table element (W.I.P.)
+  <TABLE />
 
-  def html(self, style) -> str:
+  :param style: Custom style rules
+  """
+
+  def render_child(self, child: Any, style: dict,  kwargs: Optional[dict] = None) -> str:
+    if issubclass(type(child), Component):
+      return child.html(style)
+    else:
+      return str(child)
+
+  def html(self, style: dict) -> str:
     _style = {**self.apply_style(style), **self.style}
-    return f"<div style=\"{parse_style(_style)}\">{self.render_children(style)}</div>"
+    return f"<table style=\"{parse_style(_style)}\" {parse_properties(self.properties)}>{self.render_children(style)}</table>"
 
   def plain(self) -> str:
-    _tab = self.indent
+    _tab = self.indent + ' ' * const["tab_size"]
     _plain = ""
-    for child in self.children:
-      if issubclass(type(child), Container):
-        child.indent = self.indent
-        _plain += f"{child.plain()}"
+    for i, child in enumerate(self.children):
+      if issubclass(type(child), UnorderedList):
+        child.indent = _tab
+        _plain += child.plain()
+      elif issubclass(type(child), Container):
+        child.indent = _tab
+        _plain += _tab + \
+            child.plain()[len(_tab):]
       elif issubclass(type(child), Component):
-        _plain += f"{_tab}{child.plain()}\n"
+        _plain += _tab + child.plain() + "\n"
       else:
-        _plain += f"{_tab}{str(child)}\n"
+        _plain += _tab + str(child) + "\n"
     return _plain
```

### Comparing `emailbuilder-0.1.3/emailbuilder/components/elements.py` & `emailbuilder-0.1.4/emailbuilder/components/elements.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,47 +1,47 @@
 from .base import Component
-from ..utils import const, parse_style, parse_text
+from ..utils import const, parse_style, parse_text, parse_properties
 from typing import Optional
 
 
 class Header(Component):
   """
   A level 1 header element
   <h1 />
 
   :param content: Text content
   :param style: Custom style rules
   """
 
-  def __init__(self, content: str, style: Optional[dict] = None) -> None:
-    super().__init__(style)
+  def __init__(self, content: str, style: Optional[dict] = None, properties: Optional[dict] = None) -> None:
+    super().__init__(style, properties)
     self.content = content
     self.keys.extend(["header"])
 
   def html(self, style) -> str:
     _style = {**self.apply_style(style), **self.style}
-    return f"<h1 style=\"{parse_style(_style)}\">{self.content}</h1>"
+    return f"<h1 style=\"{parse_style(_style)}\" {parse_properties(self.properties)}>{self.content}</h1>"
 
   def plain(self) -> str:
     return f"# {self.content} #\n\n"
 
 
 class Paragraph(Component):
   """
   A paragraph element
   <p />
 
   :param content: Text content
   :param style: Custom style rules
   """
 
-  def __init__(self, content: str, style: Optional[dict] = None) -> None:
-    super().__init__(style)
+  def __init__(self, content: str, style: Optional[dict] = None, properties: Optional[dict] = None) -> None:
+    super().__init__(style, properties)
     self.content = content
     self.keys.extend(["paragraph"])
 
   def html(self, style) -> str:
     _style = {**self.apply_style(style), **self.style}
-    return f"<p style=\"{parse_style(_style)}\">{parse_text(self.content)}</p>"
+    return f"<p style=\"{parse_style(_style)}\" {parse_properties(self.properties)}>{parse_text(self.content)}</p>"
 
   def plain(self) -> str:
     return f"{self.content}\n"
```

### Comparing `emailbuilder-0.1.3/emailbuilder/components/embeddables.py` & `emailbuilder-0.1.4/emailbuilder/components/embeddables.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 
   :param src: Source image file
   :param alt: Alternative text
   :param cid: Custom content ID
   :param style: Custom style rules
   """
 
-  def __init__(self, src: str, alt: str = "", cid: Optional[str] = None, style: Optional[dict] = None) -> None:
-    super().__init__(style)
+  def __init__(self, src: str, alt: str = "", cid: Optional[str] = None, style: Optional[dict] = None, properties: Optional[dict] = None) -> None:
+    super().__init__(style, properties)
     self.alt = alt
     self.src = src
     if cid is None:
       cid = src.split("\\")[-1].split("/")[-1]
     self.cid = cid
     self.keys.extend(["image"])
 
@@ -49,16 +49,16 @@
   :param image: Image as bytes
   :param extension: The image's file format
   :param alt: Alternative text
   :param cid: Custom content ID
   :param style: Custom style rules
   """
 
-  def __init__(self, image: Any, extension: str, alt: str = "", cid: Optional[str] = None, style: Optional[dict] = None) -> None:
-    super().__init__(style)
+  def __init__(self, image: Any, extension: str, alt: str = "", cid: Optional[str] = None, style: Optional[dict] = None,properties: Optional[dict] = None) -> None:
+    super().__init__(style, properties)
     self.alt = alt
     self.image = image
     self.type = extension
     if cid is None:
       cid = str(hash(image))
     self.cid = cid
     self.keys.extend(["image"])
@@ -87,16 +87,16 @@
 
   :param figure: The figure object
   :param alt: Alternative text
   :param style: Custom style rules
   :param kwargs: Custom kwargs
   """
 
-  def __init__(self, figure: Any, alt: Optional[str] = None, style: Optional[dict] = None, kwargs: Any = None) -> None:
-    super().__init__(style)
+  def __init__(self, figure: Any, alt: Optional[str] = None, style: Optional[dict] = None, properties: Optional[dict] = None, kwargs: Any = None) -> None:
+    super().__init__(style, properties)
     if alt is None:
       alt = str(hash(figure))
     if kwargs is None:
       kwargs = {}
     self.figure = figure
     self.alt = alt
     self.kwargs = kwargs
@@ -109,14 +109,14 @@
 
     if self.email:
       self.email.attach(
           item=_image,
           mime=_mime_image,
           type="image",
           extension="png",
-          cid=self.alt
+          cid=str(hash(_image))
       )
 
-    return f"<img src=\"cid:{self.alt}\" style=\"{parse_style(_style)}\" alt=\"{self.alt}\" />"
+    return f"<img src=\"cid:{str(hash(_image))}\" style=\"{parse_style(_style)}\" alt=\"{self.alt}\" />"
 
   def plain(self) -> str:
     return self.alt + "\n"
```

### Comparing `emailbuilder-0.1.3/emailbuilder/experimental.py` & `emailbuilder-0.1.4/emailbuilder/experimental.py`

 * *Files identical despite different names*

### Comparing `emailbuilder-0.1.3/emailbuilder.egg-info/PKG-INFO` & `emailbuilder-0.1.4/emailbuilder.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emailbuilder
-Version: 0.1.3
+Version: 0.1.4
 Summary: Simple HTML e-mail generator
 Home-page: https://github.com/coheleth/emailbuilder
 Author: Coheleth
 Author-email: Diogo Silva <diogopiccirillo@gmail.com>
 License: MIT
 Project-URL: homepage, https://github.com/coheleth/emailbuilder
 Project-URL: documentation, https://github.com/coheleth/emailbuilder
@@ -22,15 +22,15 @@
   - [Table of Contents](#table-of-contents)
   - [Installation](#installation)
   - [Usage](#usage)
   - [The EMail Class/Object](#the-email-classobject)
     - [Attributes](#attributes)
       - [Subject](#subject)
       - [Sender](#sender)
-      - [Receiver](#receiver)
+      - [Receiver, Copy and Blind Copy](#receiver-copy-and-blind-copy)
       - [Style](#style)
     - [Methods](#methods)
       - [email.append()](#emailappend)
       - [email.attach()](#emailattach)
       - [email.html()](#emailhtml)
       - [email.plain() (W.I.P.)](#emailplain-wip)
       - [email.message()](#emailmessage)
@@ -123,15 +123,15 @@
 
 The e-mail's subject, as a string
 
 #### Sender
 
 The sender's e-mail, as a string
 
-#### Receiver
+#### Receiver, Copy and Blind Copy
 
 The receiver(s)'s e-mail(s), as either a string or a list
 
 #### Style
 
 A dictionary containing the basic style rules for the e-mail.
 (More information concerning styling to be added)
@@ -272,10 +272,11 @@
 ---
 
 ## To-Do
 
 - [x] Write basic usage guide
 - [x] Add win32com.client outlook support
 - [x] Improve classes and functions documentation
+- [x] Add CC and BCC
 - [ ] Add table component
 - [ ] Document `style` argument
 - [ ] Improve plain text function
```

### Comparing `emailbuilder-0.1.3/setup.py` & `emailbuilder-0.1.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 README = open('README.md').read()
 
 setup(
     name='emailbuilder',
     packages=find_packages(exclude=['test']),
     python_requires='>=3.7',
-    version='0.1.3',
+    version='0.1.4',
     description='Simple HTML e-mail generator',
     long_description_content_type="text/markdown",
     long_description=README,
     author='Coheleth',
     license='MIT',
     url='https://github.com/coheleth/emailbuilder',
     install_requires=[],
```

