# Comparing `tmp/colored-2.1.1.tar.gz` & `tmp/colored-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "colored-2.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "colored-2.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `colored-2.1.1.tar` & `colored-2.2.0.tar`

### file list

```diff
@@ -1,11 +1,14 @@
--rw-r--r--   0        0        0     2349 2023-06-20 16:18:37.000000 colored-2.1.1/README.md
--rw-r--r--   0        0        0      337 2023-06-20 16:18:37.000000 colored-2.1.1/colored/__init__.py
--rw-r--r--   0        0        0      734 2023-06-20 16:18:37.000000 colored-2.1.1/colored/attributes.py
--rw-r--r--   0        0        0      756 2023-06-20 16:18:37.000000 colored-2.1.1/colored/background.py
--rw-r--r--   0        0        0     8747 2023-06-20 16:18:37.000000 colored-2.1.1/colored/colored.py
--rw-r--r--   0        0        0      844 2023-06-20 16:18:37.000000 colored-2.1.1/colored/exceptions.py
--rw-r--r--   0        0        0      756 2023-06-20 16:18:37.000000 colored-2.1.1/colored/foreground.py
--rw-r--r--   0        0        0     1797 2023-06-20 16:18:37.000000 colored-2.1.1/colored/hexadecimal.py
--rw-r--r--   0        0        0    14896 2023-06-20 16:18:37.000000 colored-2.1.1/colored/library.py
--rw-r--r--   0        0        0      991 2023-06-20 16:18:37.000000 colored-2.1.1/pyproject.toml
--rw-r--r--   0        0        0     3176 1970-01-01 00:00:00.000000 colored-2.1.1/PKG-INFO
+-rw-r--r--   0        0        0     2349 2023-06-24 14:33:49.000000 colored-2.2.0/README.md
+-rw-r--r--   0        0        0      374 2023-06-24 14:33:49.000000 colored-2.2.0/colored/__init__.py
+-rw-r--r--   0        0        0     2085 2023-06-24 14:33:49.000000 colored-2.2.0/colored/attributes.py
+-rw-r--r--   0        0        0     2137 2023-06-24 14:33:49.000000 colored-2.2.0/colored/background.py
+-rw-r--r--   0        0        0    10859 2023-06-24 14:33:49.000000 colored-2.2.0/colored/colored.py
+-rw-r--r--   0        0        0     1984 2023-06-24 14:33:49.000000 colored-2.2.0/colored/controls.py
+-rw-r--r--   0        0        0     1574 2023-06-24 14:33:49.000000 colored-2.2.0/colored/cprint.py
+-rw-r--r--   0        0        0     1089 2023-06-24 14:33:49.000000 colored-2.2.0/colored/exceptions.py
+-rw-r--r--   0        0        0     2105 2023-06-24 14:33:49.000000 colored-2.2.0/colored/foreground.py
+-rw-r--r--   0        0        0     1854 2023-06-24 14:33:49.000000 colored-2.2.0/colored/hexadecimal.py
+-rw-r--r--   0        0        0    15604 2023-06-24 14:33:49.000000 colored-2.2.0/colored/library.py
+-rw-r--r--   0        0        0     2628 2023-06-24 14:33:49.000000 colored-2.2.0/colored/utilities.py
+-rw-r--r--   0        0        0      991 2023-06-24 14:33:49.000000 colored-2.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3176 1970-01-01 00:00:00.000000 colored-2.2.0/PKG-INFO
```

### Comparing `colored-2.1.1/README.md` & `colored-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `colored-2.1.1/colored/colored.py` & `colored-2.2.0/colored/colored.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,109 +1,132 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
+from __future__ import annotations
+
 import os
 import sys
 import platform
 from typing import Any
 
 from .library import Library
 from .hexadecimal import Hex
-from .exceptions import InvalidColor, InvalidHexColor, InvalidStyle
-
+from .utilities import Utilities
 
 TTY_AWARE = True
 IS_TTY = sys.stdout.isatty() and sys.stderr.isatty()
 
 _win_vterm_mode = None
 
 
 class Colored:
 
-    def __init__(self, color: Any):
-        self.color: str = str(color).lower()
-        self.hex_color: str = ''
-        self.hex = Hex()
-        self.ESC: str = Library.ESC
-        self.END: str = Library.END
-        self.FOREGROUND: str = Library.FOREGROUND
-        self.BACKGROUND: str = Library.BACKGROUND
-        self.COLORS: dict = Library.COLORS
-        self.HEX_COLORS: dict = Library.HEX_COLORS
-        self.STYLES: dict = Library.STYLES
+    def __init__(self, name: Any):
+        """ name can be str or int instead.
+
+        Args:
+            name: name of color or number of color
+        """
+        self._name: str = str(name).lower()
+        self._hex_color: str = ''
+        self._hex = Hex()
+        self._utils = Utilities()
+
+        self._ESC: str = Library.ESC
+        self._END: str = Library.END
+
+        self.DEFAULT_STYLE: str = Library.DEFAULT_STYLE
+        self.DEFAULT_FOREGROUND_256: str = Library.DEFAULT_FOREGROUND_256
+        self.DEFAULT_BACKGROUND_256: str = Library.DEFAULT_BACKGROUND_256
+
+        self._STYLES: dict = Library.STYLES
+        self._FOREGROUND_256: str = Library.FOREGROUND_256
+        self._BACKGROUND_256: str = Library.BACKGROUND_256
+
+        self._COLORS: dict = Library.COLORS
+        self._HEX_COLORS: dict = Library.HEX_COLORS
+        self._UNDERLINE_COLOR: str = Library.UNDERLINE_COLOR
+
+        if self._name.startswith('#'):
+            self._hex_color: str = self._hex.find(self._name)
 
         self.enable_windows_terminal_mode()
 
-    def attribute(self) -> str:
-        """ Return an attribute. """
-        self._is_style_exist()
+    def attribute(self, line_color: str = '') -> str:
+        """ Returns stylize text.
+
+        Args:
+            line_color: Sets color of the underline.
+
+        Returns:
+            str: Style code.
+        """
+        if not self._name:
+            return self.DEFAULT_STYLE
+
+        self._utils.is_style_exist(self._name)
 
         if not self.enabled():
             return ''
 
-        if self.color.isdigit():
-            return f'{self.ESC}{self.color}{self.END}'
+        if self._name in ('underline', '4') and line_color:
+            line_color: str = str(line_color).lower()
+            self._utils.is_color_exist(line_color)
+            if not line_color.isdigit():
+                line_color: str = self._COLORS[line_color]
+            return f'{self._UNDERLINE_COLOR}{line_color}{self._END}'
+
+        if not self._name.isdigit():
+            self._name: str = self._STYLES[self._name]
 
-        return f'{self.ESC}{self.STYLES[self.color]}{self.END}'
+        return f'{self._ESC}{self._name}{self._END}'
 
     def foreground(self) -> str:
-        """ Returns a foreground color. """
-        self._is_color_exist()
+        """ Returns a foreground 256 color code. """
+        if not self._name:
+            return self.DEFAULT_FOREGROUND_256
+
+        self._utils.is_color_exist(self._name)
 
         if not self.enabled():
             return ''
 
-        if self.color.isdigit():
-            return f'{self.FOREGROUND}{self.color}{self.END}'
-        elif self.color.startswith('#'):
-            return f'{self.FOREGROUND}{self.hex_color}{self.END}'
+        if self._name.startswith('#'):
+            return f'{self._FOREGROUND_256}{self._hex_color}{self._END}'
+        elif not self._name.isdigit():
+            self._name: str = self._COLORS[self._name]
 
-        return f'{self.FOREGROUND}{self.COLORS[self.color]}{self.END}'
+        return f'{self._FOREGROUND_256}{self._name}{self._END}'
 
     def background(self) -> str:
-        """ Returns a background color. """
-        self._is_color_exist()
+        """ Returns a background 256 color code. """
+        if not self._name:
+            return self.DEFAULT_BACKGROUND_256
+
+        self._utils.is_color_exist(self._name)
 
         if not self.enabled():
             return ''
 
-        if self.color.isdigit():
-            return f'{self.BACKGROUND}{self.color}{self.END}'
-        elif self.color.startswith('#'):
-            return f'{self.BACKGROUND}{self.hex_color}{self.END}'
-
-        return f'{self.BACKGROUND}{self.COLORS[self.color]}{self.END}'
-
-    def _is_color_exist(self) -> None:
-        """ Checks for valid color by name or by hex style name or number,
-            and raise a InvalidColor or InvalidHexColor exception if it doesn't exist. """
-        if self.color.startswith('#'):
-            if self.color not in self.HEX_COLORS.values():
-                raise InvalidColor(f'{InvalidHexColor.__name__}: {self.color}')
-            self.hex_color: str = self.hex.find(self.color)
-
-        elif self.color not in self.COLORS.keys() and self.color not in self.COLORS.values():
-            raise InvalidColor(f'{InvalidColor.__name__}: {self.color}')
-
-    def _is_style_exist(self) -> None:
-        """ Checks for valid style and raise a InvalidStyle exception
-            if it doesn't exist. """
-        if self.color not in self.STYLES.keys() and self.color not in self.STYLES.values():
-            raise InvalidStyle(f'{InvalidStyle.__name__}: {self.color}')
+        if self._name.startswith('#'):
+            return f'{self._BACKGROUND_256}{self._hex_color}{self._END}'
+        elif not self._name.isdigit():
+            self._name: str = self._COLORS[self._name]
+
+        return f'{self._BACKGROUND_256}{self._name}{self._END}'
 
     @staticmethod
     def enable_windows_terminal_mode() -> Any:
-        """ Contribution by:
-            Andreas Fredrik Klasson
-            Magnus Heskestad
-            Dimitris Papadopoulos
+        """ Contribution by: Andreas Fredrik Klasson, Magnus Heskestad,
+        Dimitris Papadopoulos.
 
         Enable virtual terminal processing in Windows terminal. Does
         nothing if not on Windows. This is based on the rejected
-        enhancement <https://bugs.python.org/issue29059>. """
+        enhancement <https://bugs.python.org/issue29059>.
+        """
         global _win_vterm_mode
         if _win_vterm_mode is not None:
             return _win_vterm_mode
 
         # Note: Cygwin should return something like 'CYGWIN_NT...'
         _win_vterm_mode = platform.system().lower() == 'windows'
         if _win_vterm_mode is False:
@@ -122,32 +145,33 @@
         mode = wintypes.DWORD(0)
         ok = windll.kernel32.GetConsoleMode(wintypes.HANDLE(hStdout), byref(mode))
         if not ok:
             _win_vterm_mode = False
             return
 
         mode = wintypes.DWORD(mode.value | ENABLE_VIRTUAL_TERMINAL_PROCESSING)
-        ok = windll.kernel32.SetConsoleMode(wintypes.HANDLE(hStdout), mode)
+        ok = windll.kernel32.SetsConsoleMode(wintypes.HANDLE(hStdout), mode)
         if not ok:
             # Something went wrong, probably a version too old
             # to support the VT100 mode.
             # To be more certain we could check kernel32.GetLastError
             # for STATUS_INVALID_PARAMETER, but since we only enable
             # one flag we can be certain enough.
             _win_vterm_mode = False
             return
 
     @staticmethod
     def enabled() -> bool:
-        """ Contribution by Andreas Motl. """
-        # https://github.com/chalk/supports-color#info
-        # Use the environment variable FORCE_COLOR=1 (level 1), FORCE_COLOR=2
-        # (level 2), or FORCE_COLOR=3 (level 3) to forcefully enable color, or
-        # FORCE_COLOR=0 to forcefully disable. The use of FORCE_COLOR overrides
-        # all other color support checks.
+        """ Contribution by Andreas Motl.
+        https://github.com/chalk/supports-color#info
+        Use the environment variable FORCE_COLOR=1 (level 1), FORCE_COLOR=2
+        (level 2), or FORCE_COLOR=3 (level 3) to forcefully enable color, or
+        FORCE_COLOR=0 to forcefully disable. The use of FORCE_COLOR overrides
+        all other color support checks.
+        """
         if 'FORCE_COLOR' in os.environ:
             if int(os.environ['FORCE_COLOR']) == 0:
                 return False
             return True
 
         # https://no-color.org/
         # Check for the presence of a NO_COLOR environment variable that, when
@@ -160,88 +184,184 @@
         if TTY_AWARE and not IS_TTY:
             return False
 
         # In all other cases, enable coloring.
         return True
 
 
-def style(color: Any) -> str:
-    """ Alias for Colored().attribute() """
-    return Colored(color).attribute()
+def style(name: int | str, color: str | int = '') -> str:
+    """ Alias for Colored(name).attribute()
+
+    Args:
+        name: Sets the name of the color.
+        color: Sets the underline color.
+
+    Returns:
+        str: Style code.
+    """
+    return Colored(name).attribute(color)
+
+
+def fore(name: int | str) -> str:
+    """ Combination with text returns color text.
+
+    Args:
+        name: Sets the name of the color.
+
+    Returns:
+        str: Foreground code.
+    """
+    return Colored(name).foreground()
+
+
+def back(name: int | str) -> str:
+    """ Combination with text returns color background with text.
+
+    Args:
+        name: Sets the name of the color.
 
+    Returns:
+        str: Background code.
+    """
+    return Colored(name).background()
 
-def fore(color: Any) -> str:
-    """ Alias for Colored().foreground() """
-    return Colored(color).foreground()
 
+def fore_rgb(r: int | str, g: int | str, b: int | str) -> str:
+    """ Combination with text returns color text.
 
-def back(color: Any) -> str:
-    """ Alias for Colored().background() """
-    return Colored(color).background()
+    Args:
+        r: Red color.
+        g: Green color.
+        b: Blue color.
 
+    Returns:
+        str: Foreground RGB code.
+    """
+    utils = Utilities()
+    r, g, b = utils.is_percentages((r, g, b))
 
-def attr(color: Any) -> str:
-    """ This will be deprecated in the future, do not use this for version >= 2.0.0,
-        instead please use style() function (See issue #28). """
-    return Colored(color).attribute()
+    pattern: str = f'{Library.FOREGROUND_RGB}{r};{g};{b}{Library.END}'
+    if not any((r, g, b)):
+        pattern: str = Library.DEFAULT_FOREGROUND_RGB
 
+    return pattern
 
-def fg(color: Any) -> str:
-    """ This will be deprecated in the future, do not use this for version >= 2.0.0,
-        instead please use fore() function (See issue #28). """
-    return Colored(color).foreground()
 
+def back_rgb(r: int | str, g: int | str, b: int | str) -> str:
+    """ Combination with text returns color background with text.
 
-def bg(color: Any) -> str:
-    """ This will be deprecated in the future, do not use this for version >= 2.0.0,
-        instead please use style() function (See issue #28). """
-    return Colored(color).background()
+    Args:
+        r: Red color.
+        g: Green color.
+        b: Blue color.
 
+    Returns:
+        str: Background RGB code.
+    """
+    utils = Utilities()
+    r, g, b = utils.is_percentages((r, g, b))
 
-def cprint(text: str, foreground='', background='', formatting='', reset=True, **kwargs) -> None:
-    """ Looks like a patch to a built-in python print() function that allows
-    to pass colored text and style, to this function. """
-    styling: str = Colored(formatting).attribute()
-    back_color: str = Colored(background).background()
-    fore_color: str = Colored(foreground).foreground()
-    terminator: str = Colored('reset').attribute() if reset else ''
-    print(f'{styling}{back_color}{fore_color}{text}{terminator}',  **kwargs)
+    pattern: str = f'{Library.BACKGROUND_RGB}{r};{g};{b}{Library.END}'
+    if not any((r, g, b)):
+        pattern: str = Library.DEFAULT_BACKGROUND_RGB
 
+    return pattern
 
-def stylize(text: str, formatting: str, reset=True) -> str:
-    """ Conveniently styles your text as and resets ANSI codes at its end. """
+
+def attr(name: int | str) -> str:
+    """ This will be deprecated in the future, do not use with version >= 2.0.0,
+    instead please use style() function (See issue #28).
+
+    Args:
+        name: Sets the name of the color.
+
+    Returns:
+        str: Style code.
+    """
+    return Colored(name).attribute()
+
+
+def fg(name: int | str) -> str:
+    """ This will be deprecated in the future, do not use with version >= 2.0.0,
+    instead please use style() function (See issue #28).
+
+    Args:
+        name: Sets the name of the color.
+
+    Returns:
+        str: Foreground code.
+    """
+    return Colored(name).foreground()
+
+
+def bg(name: int | str) -> str:
+    """ This will be deprecated in the future, do not use with version >= 2.0.0,
+    instead please use style() function (See issue #28).
+
+    Args:
+        name: Sets the name of the color.
+
+    Returns:
+        str: Background code.
+    """
+    return Colored(name).background()
+
+
+def stylize(text: str, formatting: int | str, reset=True) -> str:
+    """ Conveniently styles your text as and resets ANSI codes at its end.
+
+    Args:
+        text: String type text.
+        formatting: Sets the formatting (color or style) of the text.
+        reset: Reset the formatting style at its end, default is True.
+
+    Returns:
+        str: Formatting string text.
+    """
     terminator: str = style('reset') if reset else ''
     return f'{"".join(formatting)}{text}{terminator}'
 
 
 def _c0wrap(formatting: str) -> str:
     """ Contribution by brrzap.
-    Wrap a set of ANSI styles in C0 control codes for readline safety. """
-    C0_SOH: str = '\x01'   # mark the beginning of nonprinting characters
-    C0_STX: str = '\x02'   # mark the end of nonprinting characters
+    Wrap a set of ANSI styles in C0 control codes for readline safety.
+
+    Args:
+        formatting: Sets the formatting (color or style) of the text.
+    """
+    C0_SOH: str = '\x01'  # mark the beginning of nonprinting characters
+    C0_STX: str = '\x02'  # mark the end of nonprinting characters
     return f'{C0_SOH}{"".join(formatting)}{C0_STX}'
 
 
 def stylize_interactive(text: str, formatting: str, reset=True) -> str:
-    """ Contribution by:
-        Jay Deiman
-        brrzap
-
+    """ Contribution by: Jay Deiman, brrzap
     stylize() variant that adds C0 control codes (SOH/STX) for readline
-    safety. """
+    safety.
+
+    Args:
+        text: String type text.
+        formatting: Sets the formatting (color or style) of the text.
+        reset: Reset the formatting style at its end, default is True.
+
+    Returns:
+        str: Formatting string text.
+    """
     # problem: readline includes bare ANSI codes in width calculations.
     # solution: wrap nonprinting codes in SOH/STX when necessary.
     # see: https://gitlab.com/dslackw/colored/issues/5
     terminator: str = _c0wrap(style('reset')) if reset else ''
     return f'{_c0wrap(formatting)}{text}{terminator}'
 
 
 def set_tty_aware(awareness=True) -> None:
-    """ Contribution by:
-        Andreas Motl
-        Jay Deiman
+    """ Contribution by: Andreas Motl, Jay Deiman
 
     Makes all interactions here tty aware. This means that if either
     stdout or stderr are directed to something other than a tty,
-    colorization will not be added. """
+    colorization will not be added.
+
+    Args:
+        awareness: Default is True.
+    """
     global TTY_AWARE
     TTY_AWARE = awareness
```

### Comparing `colored-2.1.1/colored/exceptions.py` & `colored-2.2.0/colored/exceptions.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,29 +4,39 @@
 
 class InvalidColor(Exception):
     """ Custom Exception for invalid colors. """
     def __init__(self, message: str):
         super(Exception, self).__init__(message)
         self.message: str = message
 
-    def __str__(self) -> str:
+    def __str__(self):
         return self.message
 
 
 class InvalidHexColor(Exception):
     """ Custom Exception for invalid hex colors. """
     def __init__(self, message: str):
         super(Exception, self).__init__(message)
         self.message: str = message
 
-    def __str__(self) -> str:
+    def __str__(self):
         return self.message
 
 
 class InvalidStyle(Exception):
     """ Custom Exception for invalid style. """
     def __init__(self, message: str):
         super(Exception, self).__init__(message)
         self.message: str = message
 
-    def __str__(self) -> str:
+    def __str__(self):
+        return self.message
+
+
+class InvalidNavigation(Exception):
+    """ Custom Exception for invalid navigation. """
+    def __init__(self, message: str):
+        super(Exception, self).__init__(message)
+        self.message: str = message
+
+    def __str__(self):
         return self.message
```

### Comparing `colored-2.1.1/colored/hexadecimal.py` & `colored-2.2.0/colored/hexadecimal.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
+from __future__ import annotations
+
 from .library import Library
 
 
 class Hex:
 
-    def find(self, color: str) -> str:
+    def find(self, color: str | int) -> str:
         """ Contribution by Fredrik Klasson """
 
         # Extend shorthand #ABC -> #AABBCC, like in CSS
 
         if len(color) == 4:
             color: str = '#' + color[1] * 2 + color[2] * 2 + color[3] * 2
 
@@ -37,16 +39,16 @@
             if cube_d < min_cube_d:
                 min_cube_d: int = cube_d
                 nearest: int = code
 
         return nearest
 
     @staticmethod
-    def cube(x) -> int:
+    def cube(x: int) -> int:
         # Do not assign a lambda expression, use a def (E731)
         # cube = lambda x: x * x
         return x * x
 
-    def fit(self, hex_val, ref) -> int:
+    def fit(self, hex_val: str, ref: int) -> int:
         # Do not assign a lambda expression, use a def (E731)
         # f = lambda hex_val, ref: cube(int(hex_val, 16) - ref)
         return self.cube(int(hex_val, 16) - ref)
```

### Comparing `colored-2.1.1/colored/library.py` & `colored-2.2.0/colored/library.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,39 +4,62 @@
 from dataclasses import dataclass
 
 
 @dataclass
 class Library:
 
     ESC: str = '\x1b['
-    FOREGROUND: str = f'{ESC}38;5;'
-    BACKGROUND: str = f'{ESC}48;5;'
     END: str = 'm'
+    FOREGROUND_256: str = f'{ESC}38;5;'
+    BACKGROUND_256: str = f'{ESC}48;5;'
+    FOREGROUND_RGB: str = f'{ESC}38;2;'
+    BACKGROUND_RGB: str = f'{ESC}48;2;'
+    UNDERLINE_COLOR: str = f'{ESC}4;58;5;'
+
+    DEFAULT_STYLE: str = f'{ESC}{END}'
+    DEFAULT_FOREGROUND_256: str = f'{FOREGROUND_256}{END}'
+    DEFAULT_BACKGROUND_256: str = f'{BACKGROUND_256}{END}'
+    DEFAULT_FOREGROUND_RGB: str = f'{FOREGROUND_RGB}{END}'
+    DEFAULT_BACKGROUND_RGB: str = f'{BACKGROUND_RGB}{END}'
+
+    CONTROLS = {
+        'up': 'A',
+        'down': 'B',
+        'right': 'C',
+        'left': 'D',
+        'next': 'E',
+        'previous': 'F',
+        'horizontal': 'G',
+        'position': 'H',
+        'erase_display': 'J',
+        'erase_line': 'K',
+        'scroll_up': 'S',
+        'scroll_down': 'T'
+    }
 
     STYLES = {
-        '': '',
         'bold': '1',
         'dim': '2',
         'italic': '3',
-        'underlined': '4',
+        'underline': '4',
         'blink': '5',
         'reverse': '7',
         'hidden': '8',
         'strikeout': '9',
         'reset': '0',
         'res_bold': '21',
         'res_dim': '22',
-        'res_underlined': '24',
+        'res_underline': '24',
         'res_blink': '25',
         'res_reverse': '27',
         'res_hidden': '28',
+        'res_underline_color': '59'
     }
 
     COLORS = {
-        '': '',
         'black': '0',
         'red': '1',
         'green': '2',
         'yellow': '3',
         'blue': '4',
         'magenta': '5',
         'cyan': '6',
@@ -288,15 +311,14 @@
         'grey_82': '252',
         'grey_85': '253',
         'grey_89': '254',
         'grey_93': '255',
     }
 
     HEX_COLORS = {
-        '': '',
         '0': '#000000',
         '1': '#800000',
         '2': '#008000',
         '3': '#808000',
         '4': '#000080',
         '5': '#800080',
         '6': '#008080',
```

### Comparing `colored-2.1.1/pyproject.toml` & `colored-2.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core>=3.2.0,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "colored"
-version = "2.1.1"
+version = "2.2.0"
 authors = [
     {name = "Dimitris Zlatanidis", email = "dslackw@gmail.com"},
 ]
 description = "Simple python library for color and formatting to terminal"
 readme = "README.md"
 requires-python = ">=3.9"
 keywords = ['xterm', 'color', 'vt100', 'ansi', 'terminal', 'python']
```

### Comparing `colored-2.1.1/PKG-INFO` & `colored-2.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: colored
-Version: 2.1.1
+Version: 2.2.0
 Summary: Simple python library for color and formatting to terminal
 Keywords: xterm,color,vt100,ansi,terminal,python
 Author-email: Dimitris Zlatanidis <dslackw@gmail.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: colored Version: 2.1.1 Summary: Simple python
+Metadata-Version: 2.1 Name: colored Version: 2.2.0 Summary: Simple python
 library for color and formatting to terminal Keywords:
 xterm,color,vt100,ansi,terminal,python Author-email: Dimitris Zlatanidis
 gmail.com> Requires-Python: >=3.9 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable Classifier: Environment
 :: Console Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: POSIX :: Other Classifier: Operating System :: POSIX ::
 Linux Classifier: Operating System :: Microsoft :: Windows Classifier:
```

