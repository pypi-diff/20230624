# Comparing `tmp/miniosl-0.0.5-cp311-cp311-macosx_13_0_arm64.whl.zip` & `tmp/miniosl-0.0.6-cp310-cp310-manylinux_2_28_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,20 @@
-Zip file size: 489342 bytes, number of entries: 14
--rwxr-xr-x  2.0 unx   694897 b- defN 23-Jun-18 05:31 libminioslcc20.dylib
--rwxr-xr-x  2.0 unx   444992 b- defN 23-Jun-18 14:32 minioslcc.cpython-311-darwin.so
--rw-rw-r--  2.0 unx     1130 b- defN 23-Jun-18 14:32 miniosl-0.0.5.dist-info/RECORD
--rw-r--r--  2.0 unx      110 b- defN 23-Jun-18 05:31 miniosl-0.0.5.dist-info/WHEEL
--rw-r--r--  2.0 unx       18 b- defN 23-Jun-18 05:31 miniosl-0.0.5.dist-info/top_level.txt
--rw-r--r--  2.0 unx     3417 b- defN 23-Jun-18 05:31 miniosl-0.0.5.dist-info/LICENSE.osl
--rw-r--r--  2.0 unx      514 b- defN 23-Jun-18 05:31 miniosl-0.0.5.dist-info/AUTHORS.osl
--rw-r--r--  2.0 unx     1236 b- defN 23-Jun-18 05:31 miniosl-0.0.5.dist-info/METADATA
--rw-r--r--  2.0 unx     8250 b- defN 23-Jun-18 05:26 miniosl/ui.py
--rw-r--r--  2.0 unx    10288 b- defN 23-Jun-18 05:26 miniosl/drawing.py
--rw-r--r--  2.0 unx      591 b- defN 23-Jun-18 05:26 miniosl/__init__.py
--rw-r--r--  2.0 unx     1724 b- defN 23-Jun-10 09:48 miniosl/network.py
--rw-r--r--  2.0 unx     2579 b- defN 23-Jun-18 05:26 miniosl/record.py
--rwxr-xr-x  2.0 unx   713040 b- defN 23-Jun-18 14:32 miniosl/.dylibs/libminioslcc20.dylib
-14 files, 1882786 bytes uncompressed, 487516 bytes compressed:  74.1%
+Zip file size: 871524 bytes, number of entries: 18
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-24 08:49 miniosl.libs/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-24 08:49 miniosl/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-24 08:49 miniosl-0.0.6.dist-info/
+-rwxr-xr-x  2.0 unx   928312 b- defN 23-Jun-24 08:49 libminioslcc20.so
+-rwxr-xr-x  2.0 unx   601817 b- defN 23-Jun-24 08:49 minioslcc.cpython-310-x86_64-linux-gnu.so
+-rwxr-xr-x  2.0 unx   989097 b- defN 23-Jun-24 08:49 miniosl.libs/libminioslcc20-6d91b922.so
+-rw-r--r--  2.0 unx     1724 b- defN 23-Jun-24 08:49 miniosl/network.py
+-rw-r--r--  2.0 unx     5106 b- defN 23-Jun-24 08:49 miniosl/state.py
+-rw-r--r--  2.0 unx    11495 b- defN 23-Jun-24 08:49 miniosl/ui.py
+-rw-r--r--  2.0 unx    10380 b- defN 23-Jun-24 08:49 miniosl/drawing.py
+-rw-r--r--  2.0 unx      686 b- defN 23-Jun-24 08:49 miniosl/__init__.py
+-rw-r--r--  2.0 unx     5101 b- defN 23-Jun-24 08:49 miniosl/record.py
+-rw-r--r--  2.0 unx       18 b- defN 23-Jun-24 08:49 miniosl-0.0.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1215 b- defN 23-Jun-24 08:49 miniosl-0.0.6.dist-info/RECORD
+-rw-r--r--  2.0 unx      514 b- defN 23-Jun-24 08:49 miniosl-0.0.6.dist-info/AUTHORS.osl
+-rw-r--r--  2.0 unx     1240 b- defN 23-Jun-24 08:49 miniosl-0.0.6.dist-info/METADATA
+-rw-r--r--  2.0 unx      114 b- defN 23-Jun-24 08:49 miniosl-0.0.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx     3417 b- defN 23-Jun-24 08:49 miniosl-0.0.6.dist-info/LICENSE.osl
+18 files, 2560236 bytes uncompressed, 869252 bytes compressed:  66.1%
```

## zipnote {}

```diff
@@ -1,43 +1,55 @@
-Filename: libminioslcc20.dylib
+Filename: miniosl.libs/
 Comment: 
 
-Filename: minioslcc.cpython-311-darwin.so
+Filename: miniosl/
 Comment: 
 
-Filename: miniosl-0.0.5.dist-info/RECORD
+Filename: miniosl-0.0.6.dist-info/
 Comment: 
 
-Filename: miniosl-0.0.5.dist-info/WHEEL
+Filename: libminioslcc20.so
 Comment: 
 
-Filename: miniosl-0.0.5.dist-info/top_level.txt
+Filename: minioslcc.cpython-310-x86_64-linux-gnu.so
 Comment: 
 
-Filename: miniosl-0.0.5.dist-info/LICENSE.osl
+Filename: miniosl.libs/libminioslcc20-6d91b922.so
 Comment: 
 
-Filename: miniosl-0.0.5.dist-info/AUTHORS.osl
+Filename: miniosl/network.py
 Comment: 
 
-Filename: miniosl-0.0.5.dist-info/METADATA
+Filename: miniosl/state.py
 Comment: 
 
 Filename: miniosl/ui.py
 Comment: 
 
 Filename: miniosl/drawing.py
 Comment: 
 
 Filename: miniosl/__init__.py
 Comment: 
 
-Filename: miniosl/network.py
+Filename: miniosl/record.py
 Comment: 
 
-Filename: miniosl/record.py
+Filename: miniosl-0.0.6.dist-info/top_level.txt
+Comment: 
+
+Filename: miniosl-0.0.6.dist-info/RECORD
+Comment: 
+
+Filename: miniosl-0.0.6.dist-info/AUTHORS.osl
+Comment: 
+
+Filename: miniosl-0.0.6.dist-info/METADATA
+Comment: 
+
+Filename: miniosl-0.0.6.dist-info/WHEEL
 Comment: 
 
-Filename: miniosl/.dylibs/libminioslcc20.dylib
+Filename: miniosl-0.0.6.dist-info/LICENSE.osl
 Comment: 
 
 Zip file comment:
```

## filetype from file(1)

```diff
@@ -1 +1 @@
-Zip archive data, at least v2.0 to extract, compression method=deflate
+Zip archive data, at least v2.0 to extract, compression method=store
```

## miniosl/ui.py

```diff
@@ -4,15 +4,15 @@
 import numpy as np
 import os.path
 import copy
 import urllib
 
 
 def is_in_notebook() -> bool:
-    """detect run in ipython notebook"""
+    """detect run inside ipython notebook"""
     # https://stackoverflow.com/questions/15411967/
     try:
         shell = get_ipython().__class__
         if 'google.colab' in str(shell):
             return True
         shell = shell.__name__
         if shell == 'ZMQInteractiveShell':
@@ -36,14 +36,15 @@
     def __init__(self, init: str | miniosl.BaseState | miniosl.MiniRecord = '',
                  *, prefer_png=False, prefer_svg=False, default_format='usi'):
         if not UI.prefer_svg:
             UI.prefer_svg = prefer_svg or is_in_notebook()
         if not UI.prefer_png:
             UI.prefer_png = prefer_png
         self.default_format = default_format
+        self.opening_tree = None
 
         if isinstance(init, UI):
             self._record = copy.copy(init._record)
             self.replay(init.cur)
             return
 
         if isinstance(init, miniosl.MiniRecord):
@@ -90,76 +91,93 @@
 
     def __deepcopy__(self, dict):
         return UI(self)
 
     def __len__(self) -> int:
         return self._record.state_size()  # state-size, that is, move-size + 1
 
-    def hint(self):
+    def hint(self, *args, **kwargs):
         if UI.prefer_png:
-            return self.to_png()
-        return self.to_svg() if UI.prefer_svg else self.to_csa()
+            return self.to_png(*args, **kwargs)
+        return self.to_svg(*args, **kwargs) if UI.prefer_svg else self.to_csa()
 
     # delegation for self._record
     def to_usi_history(self) -> str:
+        """show the history in usi"""
         return self._record.to_usi()
 
     def previous_repeat_index(self) -> int:
+        """the latest repeating state the history"""
         return self._record.previous_repeat_index(self.cur) if self.cur > 0 else 0
 
     def repeat_count(self) -> int:
+        """number of occurrence of the state in the history"""
         return self._record.repeat_count(self.cur)
 
     def to_apng(self, *args, **kwargs):
+        """make animated png for the history"""
         return self._record.to_apng(*args, **kwargs)
 
     # delegation for self._state
-    def to_move(self, move_rep):
+    def to_move(self, move_rep: str) -> miniosl.Move:
+        """interpret string as a Move"""
         return self._state.to_move(move_rep)
 
+    def read_japanese_move(self, move_rep: str, last_to: miniosl.Square | None = None):
+        return self._state.read_japanese_move(move_rep, last_to or miniosl.Square())
+
     def genmove(self):
+        """generate legal moves in the state"""
         return self._state.genmove()
 
     def hash_code(self):
         return self._state.hash_code()
 
     def to_csa(self):
+        """show state in csa"""
         return self._state.to_csa()
 
     def to_usi(self):
+        """show state in usi"""
         return self._state.to_usi()
 
     def _add_drawing_properties(self, dict):
         dict['last_to'] = self.last_to()
         dict['last_move_ja'] = self.last_move_ja
         dict['move_number'] = self.cur + 1
         dict['repeat_distance'] = self.cur - self.previous_repeat_index()
         dict['repeat_count'] = self.repeat_count()
 
     def to_svg(self, *args, **kwargs):
+        """show state in svg"""
         self._add_drawing_properties(kwargs)
         return miniosl.drawing.state_to_svg(self._state, *args, **kwargs)
 
     def to_png(self, *args, **kwargs):
+        """show state in png"""
         self._add_drawing_properties(kwargs)
         return miniosl.drawing.state_to_png(self._state, *args, **kwargs)
 
     # original / modified methods
     def first(self):
+        """go to the first state in the history"""
         return self.replay(0)
 
     def last(self):
+        """go to the last state in the history"""
         return self.replay(len(self._record))
 
     def go(self, step):
+        """make moves (step > 0) or unmake moves (step < 0)"""
         if not (0 <= self.cur + step <= len(self._record)):
             raise ValueError(f'step out of range {self.cur} + {step} max {len(self._record)}')
         return self.replay(self.cur+step)
 
     def make_move(self, move):
+        """make a move in the current state"""
         if isinstance(move, str):
             copy = move
             move = self._state.to_move(move)
             if not move.is_normal():
                 raise ValueError('please check syntax '+copy)
         if not self._state.is_legal(move):
             raise ValueError('illegal move '+str(move))
@@ -193,34 +211,35 @@
 
     def count_hand(self, color: miniosl.Player, ptype: miniosl.Ptype) -> int:
         return self._state.count_hand(color, ptype)
 
     def turn(self):
         return self._state.turn()
 
-    def copy(self) -> UI:
-        copy = UI()
-        copy._record = self._record.copy()
-        copy._state = self._state.copy()
-        copy.cur = self.cur()
-        return copy
-
     def to_np(self) -> np.array:
+        """make tensor of piece placement in the board.
+           each 9x9 channel is responsible for a specific piece type and color,
+           where each element is 1 (0) for existence (absent) of the piece
+        """
         return self._state.to_np().reshape(9, 9)
 
     def to_np_hand(self) -> np.array:
+        """make tensor of pieces in hand for both player"""
         return self._state.to_np_hand().reshape(2, 7)
 
     def to_np_cover(self) -> np.array:
+        """make planes to show a square is covered (1) or not (0)"""
         return self._state.to_np_cover().reshape(2, 9, 9)
 
     def to_np_pack(self) -> np.array:
+        """compress state information"""
         return self._state.to_np_pack()
 
     def replay(self, idx: int):
+        """move to idx-th state in the history"""
         self._state = miniosl.State(self._record.initial_state)
         self.cur = idx
         self.last_move_ja = None
         if idx == 0:
             return self.hint()
         if idx > len(self._record):
             raise ValueError(f'index too large {idx} > {len(self._record)}')
@@ -231,10 +250,58 @@
             self._do_make_move(move, last_to)
             if i+1 >= idx:
                 break
         return self.hint()
 
     def _do_make_move(self, move: miniosl.Move,
                       last_to: miniosl.Square | None = None):
+        self._features = None
         if last_to is not None:
             self.last_move_ja = miniosl.to_ja(move, self._state, last_to)
         self._state.make_move(move)
+
+    def load_opening_tree(self, filename):
+        """load opening db"""
+        self.opening_tree = miniosl.load_opening_tree(filename)
+
+    def opening_moves(self):
+        """retrieve or show opening moves"""
+        if self.opening_tree is None:
+            raise RuntimeError("opening_tree not loaded")
+        all = self.opening_tree[self._state.hash_code()].count()
+        children = self.opening_tree.retrieve_children(self._state)
+        if not is_in_notebook():
+            for c in children:
+                print(c[1], f'{c[0].count()/all*100:5.2f}% {c[0].count():5}'
+                      + f'({c[0].black_advantage()*100:5.2f}%)', )
+        else:
+            plane = np.zeros((9, 9))
+            for c in children:
+                x, y = c[1].dst().to_xy()
+                plane[y-1][x-1] = c[0].count()/all
+            return self.hint(plane=plane)
+
+    def follow_opening(self, nth: int = 0):
+        """make a move following the opening db"""
+        if self.opening_tree is None:
+            raise RuntimeError("opening_tree not loaded")
+        children = self.opening_tree.retrieve_children(self._state)
+        if nth >= len(children):
+            raise IndexError(f"opening {nth} >= {len(children)}")
+        self.make_move(children[nth][1])
+        return self.opening_moves()
+
+    def make_opening_db_from_sfen(self, filename: str, threshold: int = 100):
+        """make opening tree from sfen records, and save in npz"""
+        set = miniosl.RecordSet.from_usi_file(filename)
+        if not filename.endswith('.npz'):
+            set.save_npz("sfen.npz")
+        tree = miniosl.OpeningTree.from_record_set(set, threshold)
+        self.opening_tree = tree
+        tree.save_npz('opening.npz')
+
+    def show_features(self, plane_id: int, *args, **kwargs):
+        if self._features is None:
+            self._features = self._state.to_np_stdch().reshape((-1, 9, 9))
+        if not is_in_notebook():
+            print(self._features[plane_id])
+        return self.hint(plane=self._features[plane_id], *args, **kwargs)
```

## miniosl/drawing.py

```diff
@@ -93,14 +93,17 @@
         self.draw_plane(plane_c, 'purple')
         self.draw_plane(plane_b, 'orange')
         self.draw_plane(plane_w, 'blue')
 
     def draw_plane(self, plane: np.ndarray, color: str, stroke: int = 0) -> None:
         if plane.shape != (9, 9):
             raise ValueError(f'unexpected shape of plane {plane.shape}')
+        maximum = np.max(plane)
+        if maximum > 5:
+            plane /= maximum
         weight = 1 if plane.max() > 2 or plane.max() == 0 else 4/plane.max()
         p = {'fill': color,  'fill_opacity': 0.2, 'stroke_width': stroke,
              'stroke': color}
         for y in range(1, 10):
             for x in range(1, 10):
                 self.add(dw.Circle(gx(x-.5), gy(y-.5),
                                    radius(weight*plane[y-1][x-1]), **p))
@@ -192,15 +195,15 @@
             self.add(dw.Text(hand_w[i], x=gx(10.2)+scale*.5, y=gy(8.4-(i-2)*0.8),
                              rotate=180, **prop))
         if len(hand_w) >= 14:
             self.add(dw.Text(hand_others, x=gx(9.9), y=gy(5*0.8), **prop))
 
 
 def state_to_svg(state: miniosl.BaseState, id: int = 0, *,
-                 decorate: bool = False, plane: np.ndarray = None,
+                 decorate: bool = False, plane: np.ndarray | None = None,
                  plane_color: str = 'orange',
                  last_move_ja: str = '',
                  last_to: miniosl.Square | None = None,
                  move_number: int = 0, repeat_distance: int = 0,
                  repeat_count: int = 0,
                  ) -> dw.drawing.Drawing:
     """make a picture of state as svg"""
```

## miniosl/__init__.py

```diff
@@ -1,14 +1,18 @@
 from miniosl.ui import UI
 from minioslcc import *
-import miniosl.record
-from miniosl.record import np_array_to_sfen_file, sfen_file_to_np_array, \
-    sfen_file_to_training_np_array
+from .record import np_array_to_sfen_file, sfen_file_to_np_array, \
+    sfen_file_to_training_np_array, load_record_set, load_opening_tree
 
-setattr(miniosl.MiniRecord, 'replay', miniosl.record.minirecord_replay)
-setattr(miniosl.MiniRecord, 'to_apng', miniosl.record.minirecord_to_apng)
+setattr(MiniRecord, 'replay', record.minirecord_replay)
+setattr(MiniRecord, 'to_apng', record.minirecord_to_apng)
 
-setattr(miniosl.BaseState, 'to_svg', miniosl.drawing.state_to_svg)
-setattr(miniosl.BaseState, 'to_png', miniosl.drawing.state_to_png)
+setattr(BaseState, 'to_svg', drawing.state_to_svg)
+setattr(BaseState, 'to_png', drawing.state_to_png)
 
-setattr(miniosl.State, 'to_svg', miniosl.drawing.state_to_svg)
-setattr(miniosl.State, 'to_png', miniosl.drawing.state_to_png)
+setattr(State, 'to_svg', drawing.state_to_svg)
+setattr(State, 'to_png', drawing.state_to_png)
+
+setattr(RecordSet, 'save_npz', record.save_record_set)
+
+setattr(OpeningTree, 'save_npz', record.save_opening_tree)
+setattr(OpeningTree, 'retrieve_children', record.retrieve_children)
```

## miniosl/record.py

```diff
@@ -73,7 +73,75 @@
             record, n = miniosl.unpack_record(data[code_count:])
             f.write(record.to_usi()+'\n')
             code_count += n
             record_count += 1
             if code_count >= len(data) or n == 0:
                 break
     return record_count
+
+
+def save_record_set(records: miniosl.RecordSet, filename: str,
+                    name: str = '') -> (np.ndarray):
+    """save recordset to npz"""
+    filename = filename if filename.endswith('.npz') else filename+'.npz'
+    if name == '':
+        name = 'record_set'
+    data = []
+    count = 0
+    for r in records.records:
+        data += r.pack_record()
+        count += 1
+    dict = {}
+    dict[name] = np.array(data, dtype=np.uint64)
+    dict[name+'_record_count'] = count
+    np.savez_compressed(filename, **dict)
+
+
+def load_record_set(filename: str, name: str = ''):
+    """load RecordSet from npz file"""
+    filename = filename if filename.endswith('.npz') else filename+'.npz'
+    dict = np.load(filename)
+    for key in dict.keys():
+        data = dict[key]
+        if data.ndim != 1 or not (name == '' or name == key):
+            continue
+        code_count = 0
+        record_set = []
+        while code_count < len(data):
+            record, n = miniosl.unpack_record(data[code_count:])
+            record_set.append(record)
+            code_count += n
+            if n == 0:
+                raise ValueError("malformed data")
+        return miniosl.RecordSet(record_set)
+    raise ValueError("data not found")
+
+
+def save_opening_tree(tree: miniosl.OpeningTree,
+                      filename: str) -> (np.ndarray):
+    """save OpeningTree to npz"""
+    filename = filename if filename.endswith('.npz') else filename+'.npz'
+    key_board, key_stand, node = tree.export_all()
+    dict = {}
+    dict['board'] = np.array(key_board, dtype=np.uint64)
+    dict['stand'] = np.array(key_stand, dtype=np.uint64)
+    dict['node'] = np.array(node, dtype=np.uint64)
+    np.savez_compressed(filename, **dict)
+
+
+def load_opening_tree(filename: str) -> miniosl.OpeningTree:
+    """load OpeningTree from npz file"""
+    filename = filename if filename.endswith('.npz') else filename+'.npz'
+    dict = np.load(filename)
+    return miniosl.OpeningTree.restore_from(dict['board'], dict['stand'],
+                                            dict['node'])
+
+
+def retrieve_children(tree: miniosl.OpeningTree, state: miniosl.BaseState
+                      ) -> list[(miniosl.OpeningTree.Node, miniosl.Move)]:
+    code = state.hash_code()
+    code_list = [(miniosl.hash_after_move(code, move), move)
+                 for move in state.genmove()]
+    children = [(tree[new_code], move)
+                for new_code, move in code_list if new_code in tree]
+    children.sort(key=lambda node: -node[0].count())
+    return children
```

## Comparing `miniosl-0.0.5.dist-info/RECORD` & `miniosl-0.0.6.dist-info/RECORD`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,15 @@
-libminioslcc20.dylib,sha256=KCl3M57QG2Rgqzl0RZv9EsebuVnjPgepypg_p7AMe08,694897
-minioslcc.cpython-311-darwin.so,sha256=kaMZdPzYpbp8BlB_xEb0lqkk-WnKEbPeAbd74gYUpY8,444992
-miniosl-0.0.5.dist-info/RECORD,,
-miniosl-0.0.5.dist-info/WHEEL,sha256=9u5azgharjYBfdIrZMb7YtYWGPqS21BRmRBngkXCmzk,110
-miniosl-0.0.5.dist-info/top_level.txt,sha256=CL6BH9dvcGWX2Cj9E925TVZFSHixVc7wMjoVay8eySU,18
-miniosl-0.0.5.dist-info/LICENSE.osl,sha256=kQEi5lWHwshUUBeva0d4R2VmtHdpBu3C-J3S6qEZFKE,3417
-miniosl-0.0.5.dist-info/AUTHORS.osl,sha256=DeZsMUL4-Ef2jj6q7ku9Tp1xzGl0kLCsgosCwz8Mb4c,514
-miniosl-0.0.5.dist-info/METADATA,sha256=pfpZP_r42Lf8RQ0FFMsnkI8sZMRvTG-VWXWBeEpv9Ng,1236
-miniosl/ui.py,sha256=YUWoxuGmQ4hy4hJXBwx4WNfzGRSxULLuZpdA-NVRqGM,8250
-miniosl/drawing.py,sha256=TgtymxmGMppG5cy5cFEaFnEorzCXhwCFLdfbcuqmnF0,10288
-miniosl/__init__.py,sha256=J7xgrlNMnTD4TSl6fCrBUm_upUbt9b92oHXfXiDVzMM,591
+libminioslcc20.so,sha256=bZG5Ip9uFaE9jg5H9yQiRXlXBtC1b6icP927T2U4mmk,928312
+minioslcc.cpython-310-x86_64-linux-gnu.so,sha256=aWvwckmU2xhm-dxeWfTyDAU6pj2wKBZg_wz3TUFWgyg,601817
+miniosl.libs/libminioslcc20-6d91b922.so,sha256=TtpJ9pGccI6R2Lim54E75KcrtLPKtsC_1SOSfz2XCnY,989097
 miniosl/network.py,sha256=JRk0H0YQTAdbppcTyVkdKEh-wIt7HRvhtyFjC2FxFPM,1724
-miniosl/record.py,sha256=wyNl0aLqAJpxaq0W-C3N6PBe3qKUfRkOw_lgR6cR66c,2579
-miniosl/.dylibs/libminioslcc20.dylib,sha256=4byRgI3XUgxY9jvK0tMPa_tD4GPkAQ2xuLfcJf92r94,713040
+miniosl/state.py,sha256=JZisTZ2ZKw-O7Nj0YhbMMcm4y4K0d-dhUPcPyEGEg40,5106
+miniosl/ui.py,sha256=qECdsZizI9GCrc8MKb8Dzfm0DMI4kjeF2Hj8Tcr2YCY,11495
+miniosl/drawing.py,sha256=1QTOdekq7dMBxFW0ozN6Sg07HS3eBGNcxRd1Vt1gF3s,10380
+miniosl/__init__.py,sha256=BD9i-hkg3erAoL6ci3h-qP5tNfsK1WxWRPi0HTkgQgE,686
+miniosl/record.py,sha256=y0A4utxGWV8npbLfY3hk8KuSuFK4x8BelhTbACqiNwQ,5101
+miniosl-0.0.6.dist-info/top_level.txt,sha256=CL6BH9dvcGWX2Cj9E925TVZFSHixVc7wMjoVay8eySU,18
+miniosl-0.0.6.dist-info/RECORD,,
+miniosl-0.0.6.dist-info/AUTHORS.osl,sha256=DeZsMUL4-Ef2jj6q7ku9Tp1xzGl0kLCsgosCwz8Mb4c,514
+miniosl-0.0.6.dist-info/METADATA,sha256=JcxGFeDN3Qfeg7wxlkcNdWvWNR0XPjZtf8LORpd1-cY,1240
+miniosl-0.0.6.dist-info/WHEEL,sha256=9rnmjtxhPKPVe0Tp4jfKCIcCRc7MAyKmWpLWATLJWWk,114
+miniosl-0.0.6.dist-info/LICENSE.osl,sha256=kQEi5lWHwshUUBeva0d4R2VmtHdpBu3C-J3S6qEZFKE,3417
```

## Comparing `miniosl-0.0.5.dist-info/LICENSE.osl` & `miniosl-0.0.6.dist-info/LICENSE.osl`

 * *Files identical despite different names*

## Comparing `miniosl-0.0.5.dist-info/AUTHORS.osl` & `miniosl-0.0.6.dist-info/AUTHORS.osl`

 * *Files identical despite different names*

## Comparing `miniosl-0.0.5.dist-info/METADATA` & `miniosl-0.0.6.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: miniosl
-Version: 0.0.5
+Version: 0.0.6
 Summary: A python interface to miniosl (shogi library)
 Author: Tomoyuki Kaneko
 Author-email: kaneko@graco.c.u-tokyo.ac.jp
 Project-URL: Source, https://github.com/tkaneko/miniosl
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.osl
@@ -22,15 +22,15 @@
 
 ![](https://github.com/tkaneko/miniosl/raw/main/doc/policy-sample.png)
 
 ## pip wheel
 
 - [https://pypi.org/project/miniosl/](https://pypi.org/project/miniosl/)
 
-## build from source
+## work with source code
 
 - C++20 (tested with g++ 12.2.1 in `manylinux_2_28`, Apple clang 14.0.3)
 - Python 3.10+
 - cmake 3.22+
 
 typical commands
 - `git clone --recursive https://github.com/tkaneko/miniosl.git`
```

