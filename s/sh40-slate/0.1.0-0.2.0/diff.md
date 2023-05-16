# Comparing `tmp/sh40_slate-0.1.0.tar.gz` & `tmp/sh40_slate-0.2.0.tar.gz`

## Comparing `sh40_slate-0.1.0.tar` & `sh40_slate-0.2.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 sh40_slate-0.1.0/slate/__about__.py
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 sh40_slate-0.1.0/slate/__init__.py
--rw-r--r--   0        0        0     8690 2020-02-02 00:00:00.000000 sh40_slate-0.1.0/slate/color.py
--rw-r--r--   0        0        0     9500 2020-02-02 00:00:00.000000 sh40_slate-0.1.0/slate/color_info.py
--rw-r--r--   0        0        0    11063 2020-02-02 00:00:00.000000 sh40_slate-0.1.0/slate/core.py
--rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 sh40_slate-0.1.0/slate/event.py
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 sh40_slate-0.1.0/slate/key_names.py
--rw-r--r--   0        0        0     8164 2020-02-02 00:00:00.000000 sh40_slate-0.1.0/slate/screen.py
--rw-r--r--   0        0        0    16901 2020-02-02 00:00:00.000000 sh40_slate-0.1.0/slate/span.py
--rw-r--r--   0        0        0    12046 2020-02-02 00:00:00.000000 sh40_slate-0.1.0/slate/terminal.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sh40_slate-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 sh40_slate-0.1.0/tests/test_color.py
--rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 sh40_slate-0.1.0/tests/test_core.py
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 sh40_slate-0.1.0/tests/test_event.py
--rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 sh40_slate-0.1.0/tests/test_screen.py
--rw-r--r--   0        0        0     4791 2020-02-02 00:00:00.000000 sh40_slate-0.1.0/tests/test_span.py
--rw-r--r--   0        0        0     2262 2020-02-02 00:00:00.000000 sh40_slate-0.1.0/tests/test_terminal.py
--rw-r--r--   0        0        0     2996 2020-02-02 00:00:00.000000 sh40_slate-0.1.0/.gitignore
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 sh40_slate-0.1.0/LICENSE
--rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 sh40_slate-0.1.0/README.md
--rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 sh40_slate-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 sh40_slate-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 sh40_slate-0.2.0/slate/__about__.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 sh40_slate-0.2.0/slate/__init__.py
+-rw-r--r--   0        0        0    11144 2020-02-02 00:00:00.000000 sh40_slate-0.2.0/slate/color.py
+-rw-r--r--   0        0        0     9500 2020-02-02 00:00:00.000000 sh40_slate-0.2.0/slate/color_info.py
+-rw-r--r--   0        0        0    11061 2020-02-02 00:00:00.000000 sh40_slate-0.2.0/slate/core.py
+-rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 sh40_slate-0.2.0/slate/event.py
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 sh40_slate-0.2.0/slate/key_names.py
+-rw-r--r--   0        0        0     8164 2020-02-02 00:00:00.000000 sh40_slate-0.2.0/slate/screen.py
+-rw-r--r--   0        0        0    16844 2020-02-02 00:00:00.000000 sh40_slate-0.2.0/slate/span.py
+-rw-r--r--   0        0        0    11962 2020-02-02 00:00:00.000000 sh40_slate-0.2.0/slate/terminal.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sh40_slate-0.2.0/tests/__init__.py
+-rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 sh40_slate-0.2.0/tests/test_color.py
+-rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 sh40_slate-0.2.0/tests/test_core.py
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 sh40_slate-0.2.0/tests/test_event.py
+-rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 sh40_slate-0.2.0/tests/test_screen.py
+-rw-r--r--   0        0        0     4791 2020-02-02 00:00:00.000000 sh40_slate-0.2.0/tests/test_span.py
+-rw-r--r--   0        0        0     2262 2020-02-02 00:00:00.000000 sh40_slate-0.2.0/tests/test_terminal.py
+-rw-r--r--   0        0        0     2996 2020-02-02 00:00:00.000000 sh40_slate-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 sh40_slate-0.2.0/LICENSE
+-rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 sh40_slate-0.2.0/README.md
+-rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 sh40_slate-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 sh40_slate-0.2.0/PKG-INFO
```

### Comparing `sh40_slate-0.1.0/slate/color.py` & `sh40_slate-0.2.0/slate/color.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,50 @@
 """The Color class, and some related utilities."""
 
 from __future__ import annotations
 
 from colorsys import hls_to_rgb, rgb_to_hls
 from dataclasses import dataclass, field
 from functools import cached_property, lru_cache
+from math import sqrt
 
 from .color_info import COLOR_TABLE
 
 __all__ = ["Color"]
 
 OFF_WHITE = (245, 245, 245)
 OFF_BLACK = (35, 35, 35)
 
 
+def geometric_difference(
+    first: tuple[int, int, int], second: tuple[int, int, int]
+) -> float:
+    """Gets the geometric difference of 2 RGB triplets.
+
+    See https://en.wikipedia.org/wiki/Color_difference's Euclidian section.
+    """
+
+    red1, green1, blue1 = first
+    red2, green2, blue2 = second
+
+    redmean = (red1 + red2) // 2
+
+    delta_red = red1 - red2
+    delta_green = green1 - green2
+    delta_blue = blue1 - blue2
+
+    return sqrt(
+        (2 + (redmean / 256)) * (delta_red ** 2)
+        + 4 * (delta_green ** 2)
+        + (2 + (255 - redmean) / 256) * (delta_blue ** 2)
+    )
+
+
 def calculate_luminance(base: Color) -> float:
-    """Calculates the given color's perceived luminance (brightness).
+    """Calculates the given color's luminance (objective brightness).
 
     Source: https://stackoverflow.com/a/596243.
     """
 
     def _linearize(color: float) -> float:
         """Converts sRGB color to linear value."""
 
@@ -31,14 +56,29 @@
     red = _linearize(base.rgb[0] / 255)
     green = _linearize(base.rgb[1] / 255)
     blue = _linearize(base.rgb[2] / 255)
 
     return 0.2126 * red + 0.7152 * green + 0.0722 * blue
 
 
+def calculate_brightness(base: Color) -> float:
+    """Returns the given color's brightness (perceived luminance)..
+
+    From https://stackoverflow.com/a/56678483
+    """
+
+    if base.luminance <= (216 / 24389):
+        brightness = base.luminance * (24389 / 27)
+
+    else:
+        brightness = base.luminance ** (1 / 3) * 116 - 16
+
+    return brightness / 100
+
+
 def calculate_contrast(
     base: Color,
     white: Color | None = None,
     black: Color | None = None,
 ) -> Color:
     """Calculates the given color's black/white contrast.
 
@@ -79,14 +119,15 @@
 class Color:
     """A class that represents an RGB value."""
 
     rgb: tuple[int, int, int]
     is_background: bool = False
 
     luminance: float = field(init=False)
+    brightness: float = field(init=False)
     hls: tuple[float, float, float] = field(init=False)
     hex: str = field(init=False)
 
     def __post_init__(self) -> None:
         def _set_field(
             key: str, value: float | str | tuple[float, float, float]
         ) -> None:
@@ -94,14 +135,15 @@
 
         if any(not 0 <= val < 256 for val in self.rgb):
             raise ValueError(
                 f"Color RGB values must be between 0 and 256, got {self.rgb!r}."
             )
 
         _set_field("luminance", calculate_luminance(self))
+        _set_field("brightness", calculate_brightness(self))
         _set_field("hls", rgb_to_hls(*(val / 256 for val in self.rgb)))
         _set_field("hex", "#" + "".join(f"{i:02X}" for i in self.rgb))
 
     @classmethod
     def from_ansi(cls, ansi: str) -> Color:
         """Creates a color instance from an ANSI sequence's body."""
 
@@ -171,18 +213,61 @@
     @classmethod
     def white(cls) -> Color:
         """Returns a 100% white."""
 
         return WHITE
 
     @cached_property
-    def ansi(self) -> str:
-        """Returns the ANSI code that represents this color."""
+    def ansi(self, localize: bool = True) -> str:
+        """Returns the ANSI code that represents this color.
+
+        Args:
+            localize: If set, the color will be transformed to a format supported
+                by the terminal. This means terminals with worse color support can
+                always gracefully degrade to a format they support.
+        """
+        from .terminal import terminal
+        from .core import ColorSpace
+
+        lead = 38 + 10 * self.is_background
+
+        if terminal.color_space is ColorSpace.TRUE_COLOR:
+            return f"{lead};2;{';'.join(map(str, self.rgb))}"
+
+        if terminal.color_space is ColorSpace.NO_COLOR:
+            return f"{lead};5;{min(232 + self.brightness*23, 255):.0f}"
+
+        if terminal.color_space is ColorSpace.EIGHT_BIT:
+            # Normalize the color values
+            red, green, blue = (x / 255 for x in self.rgb)
+
+            # Calculate the eight-bit color index
+            index = 16
+            index += 36 * round(red * 5)
+            index += 6 * round(green * 5)
+            index += round(blue * 5)
+
+            return f"{lead};5;{index}"
+
+        if terminal.color_space is ColorSpace.STANDARD:
+            rgb = self.rgb
+
+            index = min(
+                range(16), key=lambda i: geometric_difference(rgb, COLOR_TABLE[i])
+            )
+
+            if index > 7:
+                index += 82
+            else:
+                index += 30
+
+            if self.is_background:
+                index += 10
 
-        return f"{38 + 10*self.is_background};2;{';'.join(map(str, self.rgb))}"
+            return f"{index}"
 
     @cached_property
     def contrast(self) -> Color:
         """Returns this given color's black/white contrast color."""
 
         return calculate_contrast(self)
```

### Comparing `sh40_slate-0.1.0/slate/color_info.py` & `sh40_slate-0.2.0/slate/color_info.py`

 * *Files identical despite different names*

### Comparing `sh40_slate-0.1.0/slate/core.py` & `sh40_slate-0.2.0/slate/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -127,22 +127,22 @@
         A hexadecimal triplet with the format `rrggbb`. Note that it doesn't include
         a leading hash.
     """
 
     if not stream.isatty():
         return DEFAULT_COLOR_DEFAULTS[layer]
 
+    stream.flush()
     stream.write(f"\x1b]{layer};?\007")
     stream.flush()
 
     reply = getch()
 
     mtch = RE_PALETTE_REPLY.match(reply)
     if mtch is None:
-        print(layer)
         return DEFAULT_COLOR_DEFAULTS[layer]
 
     _, red, green, blue = mtch.groups()
 
     rgb: list[str] = []
     for part in (red, green, blue):
         rgb.append(part[:2])
```

### Comparing `sh40_slate-0.1.0/slate/event.py` & `sh40_slate-0.2.0/slate/event.py`

 * *Files 10% similar despite different names*

```diff
@@ -53,7 +53,12 @@
                 else:
                     callback(data)
 
             except Exception as exc:
                 raise CallbackError(f"Error executing callback {callback!r}.") from exc
 
         return len(self._listeners)
+
+    def clear(self) -> None:
+        """Removes all listeners from th event."""
+
+        self._listeners.clear()
```

### Comparing `sh40_slate-0.1.0/slate/key_names.py` & `sh40_slate-0.2.0/slate/key_names.py`

 * *Files identical despite different names*

### Comparing `sh40_slate-0.1.0/slate/screen.py` & `sh40_slate-0.2.0/slate/screen.py`

 * *Files identical despite different names*

### Comparing `sh40_slate-0.1.0/slate/span.py` & `sh40_slate-0.2.0/slate/span.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import re
 from dataclasses import dataclass, field, fields
 from itertools import chain
 from typing import Any, Generator, Iterable
 from html import escape
 
-from .color import Color
+from .color import Color, BLACK, WHITE
 
 SETTERS = {
     "bold": "1",
     "dim": "2",
     "italic": "3",
     "underline": "4",
     "blink": "5",
@@ -148,15 +148,15 @@
             color_buffer += part
 
             if _is_valid_color(color_buffer):
                 key = (
                     "back" if _is_background_color(color_buffer) else "fore"
                 ) + "ground"
 
-                options[key] = color_buffer
+                options[key] = Color.from_ansi(color_buffer)
 
                 color_buffer = ""
                 in_color = False
 
             else:
                 color_buffer += ";"
 
@@ -166,15 +166,15 @@
             options[SETTERS_TO_STYLES[part]] = True
             continue
 
         if part in UNSETTERS_TO_STYLES:
             key = UNSETTERS_TO_STYLES[part]
 
             if key in ["foreground", "background"]:
-                options[key] = ""
+                options[key] = None
 
             else:
                 options[key] = False
 
                 # Not sure why this is said to not be covered.
                 if key == "bold":  # no-cov
                     options["dim"] = False
@@ -192,16 +192,16 @@
 
     Note that spans are immutable, so to get new versions of an existing span you can
     use one of the `as_{style_name}` methods, or the more raw `mutate`.
     """
 
     text: str
 
-    foreground: str = ""
-    background: str = ""
+    foreground: Color | None = None
+    background: Color | None = None
     hyperlink: str = ""
 
     bold: bool = False
     dim: bool = False
     italic: bool = False
     underline: bool = False
     blink: bool = False
@@ -243,31 +243,38 @@
 
         attributes = f"{self.text!r}, "
         truthy_fields = (
             field.name for field in fields(self) if getattr(self, field.name) is True
         )
         attributes += ", ".join(f"{name}=True" for name in truthy_fields)
 
-        if self.foreground != "":
+        if self.foreground is not None:
             attributes += f", foreground={self.foreground!r}"
 
-        if self.background != "":
+        if self.background is not None:
             attributes += f", background={self.background!r}"
 
         if self.hyperlink != "":
             attributes += f", hyperlink={self.hyperlink!r}"
 
         return f"{name}({attributes})"
 
     def _generate_sequences(self) -> str:
         """Generates the sequences represented by this Span."""
 
-        sequences = ";".join([self.foreground, self.background])
+        colors = []
+        if self.foreground is not None:
+            colors.append(self.foreground.ansi)
 
-        if sequences != "" and not sequences.endswith(";"):
+        if self.background is not None:
+            colors.append(self.background.ansi)
+
+        sequences = ";".join(colors)
+
+        if len(sequences) > 0:
             sequences += ";"
 
         for fld in fields(self):
             if not (fld.name in SETTERS and getattr(self, fld.name)):
                 continue
 
             sequences += SETTERS[fld.name] + ";"
@@ -301,15 +308,15 @@
     def yield_from(cls, line: str) -> Generator[Span, None, None]:
         """Generates Span objects from the given line."""
 
         # Add trailing ESC char to allow detection by regex
         if not line.endswith("\x1b"):
             line += "\x1b"
 
-        options: dict[str, bool | str] = {}
+        options: dict[str, bool | Color | None] = {}
 
         index = 0
         for mtch in RE_ANSI_STYLES.finditer(line):
             index = mtch.end()
             sequence, plain = mtch.groups()
 
             if (error_part := _parse_sequence(sequence, options)) is not None:
@@ -405,27 +412,19 @@
 
         css = {}
 
         for key, value in self.attrs.items():
             if key == "text":
                 continue
 
-            if not self.invert and key == "foreground" and value != "":
-                assert isinstance(
-                    value, str
-                ), f"invalid type for foreground: {value!r}."
-
-                css["fill"] = Color.from_ansi(value).hex
-
-            if self.invert and key == "background" and value != "":
-                assert isinstance(
-                    value, str
-                ), f"invalid type for background: {value!r}."
+            if not self.invert and key == "foreground" and value is not None:
+                css["fill"] = value.hex
 
-                css["fill"] = Color.from_ansi(value).hex
+            if self.invert and key == "background" and value is not None:
+                css["fill"] = value.hex
 
             elif key in STYLE_TO_CSS and value:
                 key, value = STYLE_TO_CSS[key]
                 css[key] = value
 
         return css
 
@@ -453,23 +452,23 @@
             cls: The classname inserted into the `class` attribute of the text tag.
         """
 
         char_width = round(font_size * SVG_CHAR_WIDTH, 4)
         rect_height = round(font_size * SVG_RECT_HEIGHT, 4)
 
         foreground = (
-            Color.from_ansi(self.foreground).hex
-            if self.foreground != ""
-            else default_foreground
+            self.foreground
+            if self.foreground is not None
+            else Color.from_hex(default_foreground)
         )
 
         background = (
-            Color.from_ansi(self.background).hex
-            if self.background != ""
-            else default_background
+            self.background
+            if self.background is not None
+            else Color.from_hex(default_background)
         )
 
         if self.invert:
             foreground, background = background, foreground
 
         length = len(self.text)
 
@@ -481,15 +480,15 @@
         x = round(x, 2)
         y = round(y, 2)
 
         svg = (
             "<rect"
             + f" x='{x}'"
             + f" y='{y - baseline_offset}'"
-            + f" fill='{background}'"
+            + f" fill='{background.hex}'"
             + f" width='{round(char_width * length + 0.5, 2):.4f}'"
             + f" height='{rect_height}'"
             + "></rect>"
         )
 
         if inline_styles:
             styles = "; ".join(
```

### Comparing `sh40_slate-0.1.0/slate/terminal.py` & `sh40_slate-0.2.0/slate/terminal.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,14 +27,19 @@
     getch_timeout,
     set_echo,
 )
 from .event import Event
 from .screen import Screen
 from .span import Span, SVG_CHAR_WIDTH, SVG_CHAR_HEIGHT
 
+__all__ = [
+    "Terminal",
+    "terminal",
+]
+
 RE_PIXEL_SIZE = re.compile(r"\x1b\[4;([\d]+);([\d]+)t")
 
 SVG_TEMPLATE = """
 <svg width="{total_width}" height="{total_height}"
     viewBox="0 0 {total_width} {total_height}" xmlns="http://www.w3.org/2000/svg">
     <style type="text/css">
         text {{
@@ -69,14 +74,17 @@
 
     def __post_init__(self) -> None:
         self._screen = Screen(*self.size)
 
         self.on_resize = Event("Terminal Resized")
         self.on_resize += self._screen.resize
 
+        self.foreground_color = get_default_color("10", stream=self.stream)
+        self.background_color = get_default_color("11", stream=self.stream)
+
     @property
     def color_space(self) -> ColorSpace:
         """Returns the best color space available on the system.
 
         If `NO_COLOR` is set, ColorSpace.NO_COLOR is returned.
         """
 
@@ -253,24 +261,14 @@
 
         if self._custom_title:
             self.write_control(STORE_TITLE)
 
         self.write_control(SET_TITLE.format(title=new))
         self._custom_title = new
 
-    def get_fg_color(self) -> str:
-        """Returns the foreground color of the terminal."""
-
-        return get_default_color("10", stream=self.stream)
-
-    def get_bg_color(self) -> str:
-        """Returns the background color of the terminal."""
-
-        return get_default_color("11", stream=self.stream)
-
     def show_cursor(self, value: bool = True) -> None:  # no-cov
         """Shows or hides the terminal's cursor."""
 
         if value:
             self.write_control(SHOW_CURSOR)
 
         else:
@@ -369,20 +367,20 @@
             font_size: The font size used for the screen's content.
             default_foreground: For each character on the screen, this color is used
                 when it doesn't have a foreground color.
             default_background: For each character on the screen, this color is used
                 when it doesn't have a background color.
         """
 
-        background_color = default_background or self.get_bg_color()
+        background_color = default_background or self.background_color
 
         screen, screen_stylesheet = self._screen.export_svg_with_styles(
             origin=(0, 0),
             font_size=font_size,
-            default_foreground=default_foreground or self.get_fg_color(),
+            default_foreground=default_foreground or self.foreground_color,
             default_background=background_color,
         )
 
         margin_x = 16
         margin_y = 16
 
         total_width = self.width * SVG_CHAR_WIDTH * font_size + 2 * margin_x
@@ -400,7 +398,10 @@
             total_width=total_width,
             total_height=total_height,
             stylesheet=screen_stylesheet,
             background=background,
             chrome="",
             screen=screen,
         )
+
+
+terminal = Terminal()
```

### Comparing `sh40_slate-0.1.0/tests/test_color.py` & `sh40_slate-0.2.0/tests/test_color.py`

 * *Files identical despite different names*

### Comparing `sh40_slate-0.1.0/tests/test_core.py` & `sh40_slate-0.2.0/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `sh40_slate-0.1.0/tests/test_event.py` & `sh40_slate-0.2.0/tests/test_event.py`

 * *Files identical despite different names*

### Comparing `sh40_slate-0.1.0/tests/test_screen.py` & `sh40_slate-0.2.0/tests/test_screen.py`

 * *Files identical despite different names*

### Comparing `sh40_slate-0.1.0/tests/test_span.py` & `sh40_slate-0.2.0/tests/test_span.py`

 * *Files identical despite different names*

### Comparing `sh40_slate-0.1.0/tests/test_terminal.py` & `sh40_slate-0.2.0/tests/test_terminal.py`

 * *Files identical despite different names*

### Comparing `sh40_slate-0.1.0/.gitignore` & `sh40_slate-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `sh40_slate-0.1.0/LICENSE` & `sh40_slate-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sh40_slate-0.1.0/pyproject.toml` & `sh40_slate-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sh40_slate-0.1.0/PKG-INFO` & `sh40_slate-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sh40-slate
-Version: 0.1.0
+Version: 0.2.0
 Summary: A lightweight set of tools for interfacing with the terminal.
 Project-URL: Documentation, https://github.com/shade40/slate#readme
 Project-URL: Issues, https://github.com/shade40/slate/issues
 Project-URL: Source, https://github.com/shade40/slate
 Author-email: bczsalba <bczsalba@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
```

