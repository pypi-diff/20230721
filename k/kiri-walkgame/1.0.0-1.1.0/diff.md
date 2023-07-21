# Comparing `tmp/kiri_walkgame-1.0.0.tar.gz` & `tmp/kiri_walkgame-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kiri_walkgame-1.0.0.tar", max compression
+gzip compressed data, was "kiri_walkgame-1.1.0.tar", max compression
```

## Comparing `kiri_walkgame-1.0.0.tar` & `kiri_walkgame-1.1.0.tar`

### file list

```diff
@@ -1,13 +1,17 @@
--rw-r--r--   0        0        0     1068 2023-07-21 06:23:27.980276 kiri_walkgame-1.0.0/LICENSE
--rw-r--r--   0        0        0      453 2023-07-21 06:23:27.980276 kiri_walkgame-1.0.0/README.md
--rw-r--r--   0        0        0     6610 2023-07-21 06:23:27.980276 kiri_walkgame-1.0.0/kiri_walkgame/__init__.py
--rw-r--r--   0        0        0      177 2023-07-21 06:23:27.980276 kiri_walkgame-1.0.0/kiri_walkgame/__main__.py
--rw-r--r--   0        0        0     3098 2023-07-21 06:23:27.980276 kiri_walkgame-1.0.0/kiri_walkgame/characters.py
--rw-r--r--   0        0        0      838 2023-07-21 06:23:27.980276 kiri_walkgame-1.0.0/kiri_walkgame/output.py
--rw-r--r--   0        0        0     1625 2023-07-21 06:23:27.980276 kiri_walkgame-1.0.0/kiri_walkgame/shortcuts.py
--rw-r--r--   0        0        0      337 2023-07-21 06:23:27.984277 kiri_walkgame-1.0.0/kiri_walkgame/sources/box.png
--rw-r--r--   0        0        0      703 2023-07-21 06:23:27.984277 kiri_walkgame-1.0.0/kiri_walkgame/sources/kiri/run.png
--rw-r--r--   0        0        0      647 2023-07-21 06:23:27.984277 kiri_walkgame-1.0.0/kiri_walkgame/sources/kiri/stand.png
--rw-r--r--   0        0        0    97861 2023-07-21 06:23:27.984277 kiri_walkgame-1.0.0/kiri_walkgame/sources/logo.png
--rw-r--r--   0        0        0      474 2023-07-21 06:23:28.460289 kiri_walkgame-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     1096 1970-01-01 00:00:00.000000 kiri_walkgame-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-07-21 08:54:12.937524 kiri_walkgame-1.1.0/LICENSE
+-rw-r--r--   0        0        0      563 2023-07-21 08:54:12.937524 kiri_walkgame-1.1.0/README.md
+-rw-r--r--   0        0        0     8818 2023-07-21 08:54:12.937524 kiri_walkgame-1.1.0/kiri_walkgame/__init__.py
+-rw-r--r--   0        0        0      177 2023-07-21 08:54:12.937524 kiri_walkgame-1.1.0/kiri_walkgame/__main__.py
+-rw-r--r--   0        0        0     5533 2023-07-21 08:54:12.937524 kiri_walkgame-1.1.0/kiri_walkgame/characters.py
+-rw-r--r--   0        0        0      838 2023-07-21 08:54:12.937524 kiri_walkgame-1.1.0/kiri_walkgame/output.py
+-rw-r--r--   0        0        0     1788 2023-07-21 08:54:12.937524 kiri_walkgame-1.1.0/kiri_walkgame/shortcuts.py
+-rw-r--r--   0        0        0  5256004 2023-07-21 08:54:12.969525 kiri_walkgame-1.1.0/kiri_walkgame/sources/audios/Fantasy_by_Pufino_on_freetouse_com.mp3
+-rw-r--r--   0        0        0      337 2023-07-21 08:54:12.969525 kiri_walkgame-1.1.0/kiri_walkgame/sources/box.png
+-rw-r--r--   0        0        0      898 2023-07-21 08:54:12.969525 kiri_walkgame-1.1.0/kiri_walkgame/sources/icons/refresh.png
+-rw-r--r--   0        0        0     1016 2023-07-21 08:54:12.969525 kiri_walkgame-1.1.0/kiri_walkgame/sources/icons/voice_off.png
+-rw-r--r--   0        0        0      899 2023-07-21 08:54:12.969525 kiri_walkgame-1.1.0/kiri_walkgame/sources/icons/voice_on.png
+-rw-r--r--   0        0        0      703 2023-07-21 08:54:12.969525 kiri_walkgame-1.1.0/kiri_walkgame/sources/kiri/run.png
+-rw-r--r--   0        0        0      647 2023-07-21 08:54:12.969525 kiri_walkgame-1.1.0/kiri_walkgame/sources/kiri/stand.png
+-rw-r--r--   0        0        0    97861 2023-07-21 08:54:12.969525 kiri_walkgame-1.1.0/kiri_walkgame/sources/logo.png
+-rw-r--r--   0        0        0      532 2023-07-21 08:54:13.393527 kiri_walkgame-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1328 1970-01-01 00:00:00.000000 kiri_walkgame-1.1.0/PKG-INFO
```

### Comparing `kiri_walkgame-1.0.0/LICENSE` & `kiri_walkgame-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kiri_walkgame-1.0.0/kiri_walkgame/__init__.py` & `kiri_walkgame-1.1.0/kiri_walkgame/characters.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,226 +1,197 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """
-Created on Tue Jul 18 11:23:42 2023
-
-@author: Anthony Chow
+Created on Thu Jul 20 11:38:00 2023
 
+@author: anthony
 """
-from io import BytesIO
+from collections.abc import Callable
 import pygame
-import numpy as np
-from kiri_pathfinding.map_generator import generate_map
-from kiri_pathfinding import PathFinding
-from kiri_walkgame.characters import Kiri
-from kiri_walkgame.shortcuts import SOURCES, equal_pos
-from kiri_walkgame.output import map_to_png
+from pygame.sprite import Sprite
+from kiri_walkgame.shortcuts import SOURCES, equal_pos, in_rect
 
 
-RATIO = 20
-COST_RATIOS = [5, 15, 20, 1]
-FPS = 20
+class BaseSprite(Sprite):
+    "base module of sprites"
 
+    def get_size(self):
+        "get the image size"
+        return self.image.get_size()
 
-class Game:
-    """
-    the main class of the game
 
+class Kiri(BaseSprite):
     """
+    module of the character: Kiri
 
-    __panel_size = RATIO * 4
-
-    __margin = RATIO
+    params
+    ------
+    size : int,
+        the size of the image
 
-    __c_size = RATIO * 2  # character's size
+    """
 
-    def __init__(self, height=20, width=20, **kwargs):
-        self.height, self.width = height * RATIO, width * RATIO
-        self.__generate_map(height, width, **kwargs)
-        self.__stop = None
-        self.__queue = []
-        self.__init_character()
-        self.__init_target()
-        self._reset()
-
-        self._running = False
-        self._waiting = False
-        self.screen = None
+    def __init__(self, size=40, fps=10):
+        super().__init__()
+        self.__load_frames(size, fps)
+        self.rect = None
+        self._frame_ind = 0
+        self.__update_image()
+        self._queue = []
+        self._current_pos = None
+        self._to_flip = False
 
     @property
-    def _stopped(self):
-        "test if the game stopped"
-        return (any((x is None for x in (self.start, self.stop))) or
-                equal_pos(self.start, self.stop))
-
-    def __init_character(self):
-        character = Kiri(self.__c_size, FPS)
-        self.__kiri = character
-
-    def __init_target(self):
-        self.__target = pygame.transform.scale(
-            pygame.image.load(SOURCES.box), (self.__c_size, self.__c_size))
-
-    def __generate_map(self, height, width, **kwargs):
-        self.map = generate_map(height, width, **kwargs)
-        map_size = self.width, self.height
-        self.__window_size = (
-            map_size[0] + self.__margin * 2,
-            map_size[1] + self.__margin + self.__panel_size)
-
-        # get bg image
-        map_to_show = BytesIO()
-        map_to_png(self.map, map_to_show)
-        map_to_show.seek(0)
-        self.__img_bg = pygame.transform.scale(
-            pygame.image.load(map_to_show), map_size)
-
-    def _reset(self):
-        "reset the map and status"
-        # game status
-        self.start = None
-        self.stop = None
-        self.__queue.clear()
-        self.cost = 0
-        self.expected_cost = 0
+    def moving(self):
+        "the character is moving or not"
+        return len(self._queue) > 0
 
-    @property
     def stop(self):
-        "the target point"
-        return self.__stop
+        "stop the move and clean the queue"
+        self._queue.clear()
 
-    @stop.setter
-    def stop(self, val):
-        self.__stop = val
-        self.__set_queue()
-
-    def __draw_background(self, to_flip=True):
-        self.screen.fill((255, 255, 255))
-        map_position = (self.__margin, self.__margin)
-        self.screen.blit(self.__img_bg, map_position)
-        if to_flip:
-            pygame.display.flip()
-
-    def __draw_kiri(self):
-        return self.__kiri.draw(self.screen)
-
-    def __move_kiri(self):
-        # refuse to control kiri when it is moving
-        if self.start is None or self.__kiri.moving:
-            return
+    def reset(self):
+        "reset all property"
+        self.stop()
+        self._current_pos = None
+
+    def move(self, position, speed):
+        """
+        move the character to the position in the given speed
+
+        params
+        ------
+        position : (int, int)
+            The target position
+        speed : int,
+            The quantity of moving steps.
+            The larger the given number, the slower the character moves.
+
+        """
+        # cases do not need to move
+        if self._current_pos is None or equal_pos(self._current_pos, position):
+            self._current_pos = position
+            return
+
+        # divide the move into steps and put the halfway positions into queue
+        delta_x, delta_y = [(x - y) / speed for x,
+                            y in zip(position, self._current_pos)]
+        self._to_flip = delta_x < 0
+        pos_x, pos_y = self._current_pos
+        self._queue.extend(
+            [(pos_x + delta_x * i, pos_y + delta_y * i)
+             for i in range(speed, 0, -1)])
+
+    def __load_frames(self, size, fps):
+        ratio = fps // 10
+        images = [pygame.transform.scale(pygame.image.load(x), (size, size))
+                  for x in (SOURCES.kiri.stand, SOURCES.kiri.run)]
+        if ratio > 1:
+            images = sum([[i for _ in range(ratio)] for i in images], [])
+        self.frames = tuple(images)
+
+    def __update_image(self):
+        self.image = self.frames[self._frame_ind]
+        if self.rect is None:
+            self.rect = self.image.get_rect()
+        else:
+            self.rect = self.image.get_rect(center=self.rect.center)
 
-        # place kiri in a position
-        if self.__kiri._current_pos is None:
-            speed = 1
-        # move kiri to a new position
+    def update(self, *args, **kwargs):
+        "update the character image"
+        if self.moving:
+            self._frame_ind += 1
+            self._frame_ind %= len(self.frames)
         else:
-            speed = COST_RATIOS[self.map[tuple(self.start)]] * 3
+            self._frame_ind = 0
+        self.__update_image()
 
-        position = self.__c_pixel_to_position(self.__kiri, self.start)
-        self.__kiri.move(position, speed)
+    def draw(self, screen):
+        "draw the character on screen"
+        if self._current_pos is None:
+            return None
 
-    def __draw_target(self):
-        if self.stop is None:
-            return
-        position = self.__c_pixel_to_position(self.__target, self.stop)
-        return self.screen.blit(self.__target, position)
+        if self.moving:
+            self._current_pos = self._queue.pop()
 
-    def __c_pixel_to_position(self, character, pixel):
-        "return a adjust position for characters"
-        position = self.__pixel_to_position(pixel)
-        width, height = character.get_size()
-        position = (position[0] - (width + RATIO) / 2, position[1] - height)
-        return position
-
-    def __pixel_to_position(self, pixel):
-        "transform the pixel on the map to the position on the screen"
-        return [x * RATIO + self.__margin + RATIO for x in pixel][::-1]
-
-    def __position_to_pixel(self, position):
-        "transform the position on the screen to the pixel on the map"
-        return [(x - self.__margin) // RATIO for x in position][::-1]
-
-    def on_init(self):
-        "init the game"
-        pygame.init()
-        logo = pygame.image.load(SOURCES.logo)
-        pygame.display.set_icon(logo)
-        pygame.display.set_caption("kiri walk game")
-        self.screen = pygame.display.set_mode(self.__window_size)
-        self.__draw_background(True)
-        self._running = True
-
-    def __on_event(self, event):
-        if event.type == pygame.QUIT:
-            self._running = False
-            return
-        if self._waiting:
-            return
-        if event.type == pygame.MOUSEBUTTONUP:
-            self.__set_start_stop(event)
-            return
+        self.update()
+        image = self.image
+        if self._to_flip:
+            image = pygame.transform.flip(image, True, False)
+        return screen.blit(image, self._current_pos)
 
-    def __set_start_stop(self, event):
-        "set the start point and stop point"
-        if event.button != 1:
-            return
-        pixel = self.__position_to_pixel(event.pos)
-        if not self.__check_pixel(pixel):
-            return
-        if self.start is None:
-            self.start = pixel
-        # elif self.stop is None or self._stopped:
+
+class Button(BaseSprite):
+    """
+    module to describe a button
+
+    params
+    ------
+    path : str
+        path of the button icon
+    size : (int, int)
+        the size of the button
+    action : func
+        the action when the button is pressed
+
+    """
+
+    normal_color = (150, 150, 150)
+
+    pressed_color = (50, 50, 50)
+
+    def __init__(self, path, position, size=(80, 40), margin=5, action=None):
+        super().__init__()
+        self.size = size
+        self.margin = margin
+        self._current_pos = position
+        self.__current = 0
+        self.__load_frames(path)
+        if isinstance(action, Callable):
+            self.action = action
         else:
-            self.stop = pixel
+            self.action = lambda x: None
+        self._pressed = False
 
-    def __check_pixel(self, pixel):
-        "test if the pixel still in the map"
-        pixel = np.asarray(pixel)
-        return np.all((pixel >= 0) & (pixel < self.map.shape))
-
-    def __set_queue(self):
-        "set queue to move"
-        if self._stopped or self.stop is None:
-            return
-        self.__kiri.stop()
-        self.__queue = PathFinding(self.map).find(
-            tuple(self.start), tuple(self.stop))[:0:-1]
-
-    def __on_loop(self):
-        if not self.__kiri.moving and len(self.__queue) > 0:
-            self.start = self.__queue.pop()
-        self.__move_kiri()
-
-    def __on_render(self, pre_rects):
-        rects = []
-        self.__draw_background(False)
-        rects.append(self.__draw_target())
-        rects.append(self.__draw_kiri())
-
-        # kiri get into the box
-        if equal_pos(self.start, self.stop) and not self.__kiri.moving:
-            rects.append(self.__draw_target())
-
-        pygame.display.update(pre_rects + rects)
-        return rects
-
-    def __on_cleanup(self):
-        pygame.quit()
-
-    def on_run(self):
-        "run the game"
-        self.on_init()
-
-        clock = pygame.time.Clock()
-        pre_rects = []
-        while (self._running):
-            for event in pygame.event.get():
-                self.__on_event(event)
-            self.__on_loop()
-            pre_rects = self.__on_render(pre_rects)
-            clock.tick(FPS)
-        self.__on_cleanup()
-
-
-if __name__ == '__main__':
-    game = Game()
-    screen = game.on_run()
+    @property
+    def image(self):
+        "image to show"
+        return self.frames[self.__current]
+
+    def __load_frames(self, path):
+        if isinstance(path, str):
+            path = [path]
+        size = min(self.size) - self.margin * 2
+        self.frames = [pygame.transform.scale(pygame.image.load(p),
+                                              (size, size))
+                       for p in path]
+
+        self._img_pos = [x + (dx - size) / 2 for x, dx in zip(self._current_pos,
+                                                     self.size)]
+        self._img_pos[1] = self._current_pos[1] + self.margin
+        self.surface = pygame.Surface(self.size)
+        self.rect = self.surface.get_rect()
+
+    def update(self):
+        "update the shown color"
+        color = self.normal_color
+        if self._pressed:
+            color = self.pressed_color
+            self._pressed = False
+        self.surface.fill(color)
+
+    def draw(self, screen):
+        "draw the button on screen"
+        self.update()
+        self.rect = screen.blit(self.surface, self._current_pos)
+        screen.blit(self.image, self._img_pos)
+        return self.rect
+
+    def on_event(self, event):
+        "react if the event happens on the button"
+        if in_rect(event.pos, self.rect):
+            self._pressed = True
+            self.__current += 1
+            self.__current %= len(self.frames)
+            self.action(event)
+            return True
+        return False
```

### Comparing `kiri_walkgame-1.0.0/kiri_walkgame/output.py` & `kiri_walkgame-1.1.0/kiri_walkgame/output.py`

 * *Files identical despite different names*

### Comparing `kiri_walkgame-1.0.0/kiri_walkgame/shortcuts.py` & `kiri_walkgame-1.1.0/kiri_walkgame/shortcuts.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """
 Created on Tue Jul 18 17:14:13 2023
 
 @author: Anthony Chow
 
-Shortcuts to access sources
+Shortcuts to access sources or some useful functions
 
 """
 
 import os
 from collections.abc import Iterable
 
 
@@ -55,7 +55,11 @@
 
 
 def equal_pos(pos1, pos2):
     "test if the pos1 == pos2"
     if not all((isinstance(x, Iterable) for x in (pos1, pos2))):
         return False
     return all((x == y for x, y in zip(pos1, pos2)))
+
+def in_rect(pos, rect):
+    "test if the pos in rect"
+    return all((a < x < a + b for x, (a, b) in zip(pos, zip(rect[:2], rect[2:]))))
```

### Comparing `kiri_walkgame-1.0.0/kiri_walkgame/sources/kiri/run.png` & `kiri_walkgame-1.1.0/kiri_walkgame/sources/kiri/run.png`

 * *Files identical despite different names*

### Comparing `kiri_walkgame-1.0.0/kiri_walkgame/sources/kiri/stand.png` & `kiri_walkgame-1.1.0/kiri_walkgame/sources/kiri/stand.png`

 * *Files identical despite different names*

### Comparing `kiri_walkgame-1.0.0/kiri_walkgame/sources/logo.png` & `kiri_walkgame-1.1.0/kiri_walkgame/sources/logo.png`

 * *Files identical despite different names*

### Comparing `kiri_walkgame-1.0.0/PKG-INFO` & `kiri_walkgame-1.1.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: kiri-walkgame
-Version: 1.0.0
+Version: 1.1.0
 Summary: a mini game to visualize the path-finding algorithm
+Home-page: https://github.com/kiri-chow/kiri-walkgame
 License: MIT
 Author: anthony
 Author-email: mrchowpoor@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: kiri-pathfinding (>=1.2.0,<2.0.0)
 Requires-Dist: pygame (>=2.5.0,<3.0.0)
 Requires-Dist: pypng (>=0.20220715.0,<0.20220716.0)
+Project-URL: Repository, https://github.com/kiri-chow/kiri-walkgame
 Description-Content-Type: text/markdown
 
 # kiri-walkgame
 
 ![PythonVersion](https://img.shields.io/badge/python-3.*-blue)
 ![PyPi](https://img.shields.io/pypi/v/kiri-walkgame)
 
@@ -27,7 +29,12 @@
 
 ## Usage
 
 ```shell
 python kiri_walkgame
 ```
 
+## Credits
+Music track: Fantasy by Pufino
+Source: https://freetouse.com/music
+Copyright Free Music for Video
+
```

