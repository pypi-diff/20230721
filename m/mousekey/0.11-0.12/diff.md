# Comparing `tmp/mousekey-0.11.tar.gz` & `tmp/mousekey-0.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mousekey-0.11.tar", last modified: Tue Dec 27 12:24:20 2022, max compression
+gzip compressed data, was "mousekey-0.12.tar", last modified: Fri Jul 21 01:19:08 2023, max compression
```

## Comparing `mousekey-0.11.tar` & `mousekey-0.12.tar`

### file list

```diff
@@ -1,19 +1,18 @@
-drwxrwxrwx   0        0        0        0 2022-12-27 12:24:20.741280 mousekey-0.11/
--rw-rw-rw-   0        0        0     1148 2022-12-27 12:24:09.000000 mousekey-0.11/LICENSE.rst
--rw-rw-rw-   0        0        0      121 2022-12-27 12:24:09.000000 mousekey-0.11/MANIFEST.in
--rw-rw-rw-   0        0        0    16686 2022-12-27 12:24:20.741280 mousekey-0.11/PKG-INFO
--rw-rw-rw-   0        0        0    15355 2022-12-27 12:21:55.000000 mousekey-0.11/README.md
-drwxrwxrwx   0        0        0        0 2022-12-27 12:24:20.738353 mousekey-0.11/mousekey/
--rw-rw-rw-   0        0        0     1069 2022-10-02 04:27:48.000000 mousekey-0.11/mousekey/LICENSE
--rw-rw-rw-   0        0        0    15355 2022-12-27 12:21:55.000000 mousekey-0.11/mousekey/README.MD
--rw-rw-rw-   0        0        0    74278 2022-12-27 12:01:17.000000 mousekey-0.11/mousekey/__init__.py
--rw-rw-rw-   0        0        0       88 2022-12-27 12:24:19.000000 mousekey-0.11/mousekey/requirements.txt
--rw-rw-rw-   0        0        0        2 2022-12-27 12:24:19.000000 mousekey-0.11/mousekey/thirdparty.json
-drwxrwxrwx   0        0        0        0 2022-12-27 12:24:20.741280 mousekey-0.11/mousekey.egg-info/
--rw-rw-rw-   0        0        0    16686 2022-12-27 12:24:20.000000 mousekey-0.11/mousekey.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      319 2022-12-27 12:24:20.000000 mousekey-0.11/mousekey.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-27 12:24:20.000000 mousekey-0.11/mousekey.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       83 2022-12-27 12:24:20.000000 mousekey-0.11/mousekey.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2022-12-27 12:24:20.000000 mousekey-0.11/mousekey.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      115 2022-12-27 12:24:20.742257 mousekey-0.11/setup.cfg
--rw-rw-rw-   0        0        0     1599 2022-12-27 12:24:19.000000 mousekey-0.11/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-21 01:19:08.541926 mousekey-0.12/
+-rw-rw-rw-   0        0        0     1148 2023-07-21 01:18:53.000000 mousekey-0.12/LICENSE.rst
+-rw-rw-rw-   0        0        0       95 2023-07-21 01:18:50.000000 mousekey-0.12/MANIFEST.in
+-rw-rw-rw-   0        0        0    16003 2023-07-21 01:19:08.542924 mousekey-0.12/PKG-INFO
+-rw-rw-rw-   0        0        0    15355 2023-04-15 00:18:26.000000 mousekey-0.12/README.md
+drwxrwxrwx   0        0        0        0 2023-07-21 01:19:08.538935 mousekey-0.12/mousekey/
+-rw-rw-rw-   0        0        0    15355 2023-04-15 00:18:26.000000 mousekey-0.12/mousekey/README.MD
+-rw-rw-rw-   0        0        0    75182 2023-07-21 01:16:48.000000 mousekey-0.12/mousekey/__init__.py
+-rw-rw-rw-   0        0        0       88 2023-07-21 01:19:07.000000 mousekey-0.12/mousekey/requirements.txt
+-rw-rw-rw-   0        0        0    56390 2023-07-21 01:19:07.000000 mousekey-0.12/mousekey/thirdparty.json
+drwxrwxrwx   0        0        0        0 2023-07-21 01:19:08.541926 mousekey-0.12/mousekey.egg-info/
+-rw-rw-rw-   0        0        0    16003 2023-07-21 01:19:08.000000 mousekey-0.12/mousekey.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      302 2023-07-21 01:19:08.000000 mousekey-0.12/mousekey.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-21 01:19:08.000000 mousekey-0.12/mousekey.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       83 2023-07-21 01:19:08.000000 mousekey-0.12/mousekey.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-21 01:19:08.000000 mousekey-0.12/mousekey.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       85 2023-07-21 01:19:08.543921 mousekey-0.12/setup.cfg
+-rw-rw-rw-   0        0        0     1499 2023-07-21 01:19:07.000000 mousekey-0.12/setup.py
```

### Comparing `mousekey-0.11/LICENSE.rst` & `mousekey-0.12/LICENSE.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
  The MIT License (MIT)
- Copyright (c) 2022 Johannes Fischer
+ Copyright (c) 2023 Johannes Fischer
  
  Permission is hereby granted, free of charge, to any person obtaining a copy
  of this software and associated documentation files (the "Software"), to deal
  in the Software without restriction, including without limitation the rights
  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
  copies of the Software, and to permit persons to whom the Software is
  furnished to do so, subject to the following conditions:
```

### Comparing `mousekey-0.11/PKG-INFO` & `mousekey-0.12/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,441 +1,418 @@
-Metadata-Version: 2.1
-Name: mousekey
-Version: 0.11
-Summary: Automates mouse/keyboard, works with games like Roblox!
-Home-page: https://github.com/hansalemaos/mousekey
-Author: Johannes Fischer
-Author-email: <aulasparticularesdealemaosp@gmail.com>
-License: MIT
-Keywords: automate,keystroke,mouse,games,pyautogui
-Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Topic :: Scientific/Engineering :: Visualization
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Text Editors :: Text Processing
-Classifier: Topic :: Text Processing :: General
-Classifier: Topic :: Text Processing :: Indexing
-Classifier: Topic :: Text Processing :: Filters
-Classifier: Topic :: Utilities
-Description-Content-Type: text/markdown
-License-File: LICENSE.rst
-
-
-<h2>mousekey</h2>
-
-
-
-
-* Works with multi screens
-* Keyboard and mouse can be used in Games like Roblox 
-* Has only a few dependencies (all of them pure python except NumPy)
-* Can simulate human-like mouse movement 
-* Facilitates multi key presses 
-
-
-<h2>Check out the videos</h2>
-<h3>Some methods</h3>
-
-
-<div align="left">
-      <a href="https://www.youtube.com/watch?v=1YugTBZBiyE">
-         <img src="https://img.youtube.com/vi/1YugTBZBiyE/0.jpg" style="width:100%;">
-      </a>
-</div>
-
-<h3>25 minutes of Roblox botting - 900x clicks / 900x keystrokes   </h3>
-
-<div align="left">
-      <a href="https://www.youtube.com/watch?v=OGPoiBnsy1M">
-         <img src="https://img.youtube.com/vi/OGPoiBnsy1M/0.jpg" style="width:100%;">
-      </a>
-</div>
-
-
-
-<h2>Installation</h2>
-
-
-
-```python
-$pip install mousekey
-from mousekey import MouseKey
-mkey = MouseKey()
-
-
-```
-
-
-<h2>Before you start, enable your guardian angel :)   </h2>
-
-
-
-```python
-# Kills the whole process, does always work (even with pure except)
-mkey.enable_failsafekill('ctrl+e')
-
-try:
-    while True:
-        try:
-            print('baba')
-            time.sleep(1)
-        except:
-            pass
-except:
-    pass
-baba
-baba
-baba
-baba
-
-# After pressing ctrl+e:
-Process finished with exit code 1
-```
-
-
-<h2>How to click and move </h2>
-
-
-The click methods should be able to handle any Game
-
-I have tested it with Roblox, which is known for blocking almost everything.
-
-As far as I know, there is no Python module that can handle Roblox [(https://pypi.org/project/ahk/](https://pypi.org/project/ahk/) works, but you need to download ahk.exe) 
-
-<h2>Absolute coordinates</h2>
-
-
-
-```python
-mkey.left_click_xy_natural(
-    200,
-    200,
-    delay=.3, # duration of the mouse click (down - up)
-    min_variation=-3, #  a random value will be added to each pixel  - define the minimum here 
-    max_variation=3,  # a random value will be added to each pixel  - define the maximum here 
-    use_every=4, # use every nth pixel 
-    sleeptime=(0.005, 0.009), # delay between each coordinate
-    print_coords=True, # console output 
-    percent=90, # the lower, the straighter the mouse movement
-) # A logarithm calculation lowers the speed when the cursor is getting close to the destination, like you do it in real life.
-```
-
-
-
-```python
-# Also available: 
-mkey.middle_click_xy_natural
-mkey.right_click_xy_natural
-```
-
-
-
-```python
-# if you don't want to click, only move, use:
-mkey.move_to_natural(100,100) # natural mouse movement
-mkey.move_to(3100,100) = move # no delay 
-```
-
-
-
-```python
-# Moving without delay and clicking:
-mkey.left_click_xy(10,10)
-mkey.right_click_xy(10,10)
-mkey.middle_click_xy(10,10)
-
-#Only clicking:
-mkey.left_click()
-mkey.middle_click()
-mkey.right_click()
-```
-
-
-<h2>Relative coordinates</h2>
-
-
-
-```python
-# For relative coordinates, use: 
-mkey.left_click_xy_natural_relative(
-    50,
-    50,
-    delay=0.1,
-    sleeptime=(0.00005, 0.00009),
-    print_coords=True,
-)
-
-mkey.right_click_xy_natural_relative(
-    x=500,
-    y=500,
-    delay=0.1,
-    sleeptime=(0.00005, 0.00009),
-    print_coords=True,
-)
-```
-
-
-
-```python
-# move and click relatively
-mkey.move_relative
-mkey.middle_click_xy_relative(-100,-100)
-mkey.move_to_natural_relative(300,-400)
-```
-
-
-<h2>Pressing keys</h2>
-
-
-
-```python
-# press a single key
-mkey.force_activate_window(10290540)
-mkey.press_key('f', delay=1) # delay in seconds
-```
-
-
-
-```python
-# You can press as many keys simultaneously as you want. 
-# The first value in each tuple indicates the sleep time before the next key is pressed, and presstime is the delay of the whole action.
-mkey.force_activate_window(10290540)
-mkey.press_keys_simultaneously_own_interval(
-    keystopress=[(0.1, "ctrl"), (0.1, "v")], presstime=.5
-)
-```
-
-
-
-```python
-# This method will calculate the sleep time between each key presses, so you don't have to worry about it. 
-mkey.force_activate_window(10290540)
-mkey.press_keys_simultaneously(
-    keystopress=["alt", "f4", "enter", "enter"],  
-    presstime=1.1,
-    percentofregularpresstime=100,
-)
-```
-
-
-
-```python
-# You can get a list with all available keys here: mkey.show_all_keys
-# I covered different writing styles ('volume_mute', 'VOLUME_MUTE', 'VOLUME MUTE', 'volume mute'), 
-{'control-break processing': 3,
- 'backspace': 8,
- 'tab': 9,
- 'clear': 254,
- 'enter': 13,
- 'shift': 16,
- 'ctrl': 17,
- 'alt': 18,
- 'pause': 19,
- 'caps lock': 20,
- 'ime hangul mode': 21,
- 'ime junja mode': 23,
- 'ime final mode': 24,
- 'ime kanji mode': 25,
- 'esc': 27,
- 'ime convert': 28,
- 'ime nonconvert': 29,
- 'ime accept': 30,
- 'ime mode change request': 31,
- 'spacebar': 32,
- 'page up': 33,
- ...}
-```
-
-
-
-```python
-# You can block the mouse/keyboard input while executing actions.
-# That way, the user can't mess it up. 
-# If something goes wrong, press ctrl+alt+del 
-# This will automatically unlock the mouse/keyboard
-
-# Here is one example. Always use mkey.block_user_input() / mkey.unblock_user_input()
-if mkey.block_user_input():
-    try:
-        for k in range(3):
-            mkey.right_click()
-            sleep(1)
-            mkey.left_click_xy_natural(10, 10)
-            sleep(1)
-    finally:
-        mkey.unblock_user_input()
-```
-
-
-
-
-```python
-# You can send Unicode strings as well
-mkey.force_activate_window(10290540)
-mkey.send_unicode('bababöä')
-```
-
-
-
-```python
-# I have slightly modified 2 methods from pywinauto 
-# Most of the code is from pywinauto, I only changed the way the window gets activated
-mkey.send_keys_to_hwnd(handle=7539468, keys='babadu')
-mkey.send_keystrokes_to_hwnd(handle=7539468, '%{F4}')  # alt+f4
-
-# Here are all keystrokes for those 2 methods:
-https://pywinauto.readthedocs.io/en/latest/code/pywinauto.keyboard.html?highlight=VK_SPACE#pywinauto-keyboard
-
-{SCROLLLOCK}, {VK_SPACE}, {VK_LSHIFT}, {VK_PAUSE}, {VK_MODECHANGE},
-{BACK}, {VK_HOME}, {F23}, {F22}, {F21}, {F20}, {VK_HANGEUL}, {VK_KANJI},
-{VK_RIGHT}, {BS}, {HOME}, {VK_F4}, {VK_ACCEPT}, {VK_F18}, {VK_SNAPSHOT},
-{VK_PA1}, {VK_NONAME}, {VK_LCONTROL}, {ZOOM}, {VK_ATTN}, {VK_F10}, {VK_F22},
-{VK_F23}, {VK_F20}, {VK_F21}, {VK_SCROLL}, {TAB}, {VK_F11}, {VK_END},
-{LEFT}, {VK_UP}, {NUMLOCK}, {VK_APPS}, {PGUP}, {VK_F8}, {VK_CONTROL},
-{VK_LEFT}, {PRTSC}, {VK_NUMPAD4}, {CAPSLOCK}, {VK_CONVERT}, {VK_PROCESSKEY},
-{ENTER}, {VK_SEPARATOR}, {VK_RWIN}, {VK_LMENU}, {VK_NEXT}, {F1}, {F2},
-{F3}, {F4}, {F5}, {F6}, {F7}, {F8}, {F9}, {VK_ADD}, {VK_RCONTROL},
-{VK_RETURN}, {BREAK}, {VK_NUMPAD9}, {VK_NUMPAD8}, {RWIN}, {VK_KANA},
-{PGDN}, {VK_NUMPAD3}, {DEL}, {VK_NUMPAD1}, {VK_NUMPAD0}, {VK_NUMPAD7},
-{VK_NUMPAD6}, {VK_NUMPAD5}, {DELETE}, {VK_PRIOR}, {VK_SUBTRACT}, {HELP},
-{VK_PRINT}, {VK_BACK}, {CAP}, {VK_RBUTTON}, {VK_RSHIFT}, {VK_LWIN}, {DOWN},
-{VK_HELP}, {VK_NONCONVERT}, {BACKSPACE}, {VK_SELECT}, {VK_TAB}, {VK_HANJA},
-{VK_NUMPAD2}, {INSERT}, {VK_F9}, {VK_DECIMAL}, {VK_FINAL}, {VK_EXSEL},
-{RMENU}, {VK_F3}, {VK_F2}, {VK_F1}, {VK_F7}, {VK_F6}, {VK_F5}, {VK_CRSEL},
-{VK_SHIFT}, {VK_EREOF}, {VK_CANCEL}, {VK_DELETE}, {VK_HANGUL}, {VK_MBUTTON},
-{VK_NUMLOCK}, {VK_CLEAR}, {END}, {VK_MENU}, {SPACE}, {BKSP}, {VK_INSERT},
-{F18}, {F19}, {ESC}, {VK_MULTIPLY}, {F12}, {F13}, {F10}, {F11}, {F16},
-{F17}, {F14}, {F15}, {F24}, {RIGHT}, {VK_F24}, {VK_CAPITAL}, {VK_LBUTTON},
-{VK_OEM_CLEAR}, {VK_ESCAPE}, {UP}, {VK_DIVIDE}, {INS}, {VK_JUNJA},
-{VK_F19}, {VK_EXECUTE}, {VK_PLAY}, {VK_RMENU}, {VK_F13}, {VK_F12}, {LWIN},
-{VK_DOWN}, {VK_F17}, {VK_F16}, {VK_F15}, {VK_F14}
-
-'+': {VK_SHIFT}
-'^': {VK_CONTROL}
-'%': {VK_MENU} a.k.a. Alt key
-```
-
-
-<h2>Activating windows </h2>
-
-
-
-<table>
-  <tr>
-  </tr>
-</table>
-
-
-
-```python
-# lists all current windows and their hwnds, pid ...
-mkey.get_all_windows()
-
- WindowInfo(pid=24880, title='tooltips_class32', windowtext='', hwnd=38931464, length=1, tid=14156, status='invisible', coords_client=(0, 0, 0, 0), dim_client=(0, 0), coords_win=(0, 0, 0, 0), dim_win=(0, 0), class_name='tooltips_class32', path='C:\\Windows\\explorer.exe'),
- WindowInfo(pid=24916, title='IME', windowtext='Default IME', hwnd=333592, length=12, tid=6716, status='invisible', coords_client=(0, 0, 0, 0), dim_client=(0, 0), coords_win=(0, 0, 0, 0), dim_win=(0, 0), class_name='IME', path='C:\\Windows\\System32\\notepad.exe'),
- WindowInfo(pid=24916, title='IME', windowtext='Default IME', hwnd=1706956, length=12, tid=20004, status='invisible', coords_client=(0, 0, 0, 0), dim_client=(0, 0), coords_win=(0, 0, 0, 0), dim_win=(0, 0), class_name='IME', path='C:\\Windows\\System32\\notepad.exe'),
- WindowInfo(pid=24916, title='MSCTFIME UI', windowtext='MSCTFIME UI', hwnd=35652702, length=12, tid=20004, status='invisible', coords_client=(0, 0, 0, 0), dim_client=(0, 0), coords_win=(0, 0, 0, 0), dim_win=(0, 0), class_name='MSCTFIME UI', path='C:\\Windows\\System32\\notepad.exe'),
- WindowInfo(pid=24916, title='Notepad', windowtext='*Untitled - Notepad', hwnd=10290540, length=20, tid=20004, status='visible', coords_client=(0, 840, 0, 519), dim_client=(840, 519), coords_win=(714, 1570, 196, 774), dim_win=(856, 578), class_name='Notepad', path='C:\\Windows\\System32\\notepad.exe'),
- WindowInfo(pid=24916, title='WorkerW', windowtext='', hwnd=984520, length=1, tid=6716, status='invisible', coords_client=(0, 120, 0, 0), dim_client=(120, 0), coords_win=(0, 136, 0, 39), dim_win=(136, 39), class_name='WorkerW', path='C:\\Windows\\System32\\notepad.exe')]
-
-```
-
-
-
-```python
-# pass and hwnd (code above) as argument.
-mkey.activate_window(10290540) # usually this is enough to activate a window 
-
-#if not, use this method 
-# Activating a window is sometimes tricky. This method forces the activation of the window and works quite often when other methods don't 
-mkey.force_activate_window(17630556) 
-```
-
-
-
-```python
-# Pins a window on top of all others. 
-mkey.activate_topmost(17630556)
-
-# Restore the normal hierarchy. 
-# This method is helpful when one of your windows gets stuck during the automation in the topmost position
-mkey.deactivate_topmost(17630556)
-
-
-```
-
-
-
-```python
-# Some apps hide the cursor, here can you check it 
-mkey.is_cursor_shown ()
-True
-```
-
-
-
-```python
-# Shows you the coordinates of the current cursor position. Press ctrl+l when you have found the right coordinates.
-mkey.start_showing_cursor_position(exit_keys='ctrl+l')
-```
-
-
-
-```python
-mkey.get_single_element_from_coords(200,200)
-
-WindowInfo(parent=-1, pid=20440, title='Edit', windowtext='', hwnd=592576, length=1, tid=17252, status='visible', coords_client=(0, 1903, 0, 1007), dim_client=(1903, 1007), coords_win=(0, 1920, 43, 1050), dim_win=(1920, 1007), class_name='Edit', path='C:\\Windows\\System32\\notepad.exe')
-
-
-
-mkey.get_elements_from_coords(200,200)
-
-{'element': WindowInfo(parent=-1, pid=20440, title='Edit', windowtext='', hwnd=592576, length=1, tid=17252, status='visible', coords_client=(0, 1903, 0, 1007), dim_client=(1903, 1007), coords_win=(0, 1920, 43, 1050), dim_win=(1920, 1007), class_name='Edit', path='C:\\Windows\\System32\\notepad.exe'),
- 'family': [WindowInfo(parent=-1, pid=20440, title='Edit', windowtext='', hwnd=592576, length=1, tid=17252, status='visible', coords_client=(0, 1903, 0, 1007), dim_client=(1903, 1007), coords_win=(0, 1920, 43, 1050), dim_win=(1920, 1007), class_name='Edit', path='C:\\Windows\\System32\\notepad.exe'),
-  WindowInfo(parent=-1, pid=20440, title='Notepad', windowtext='*Untitled - Notepad', hwnd=1051364, length=20, tid=17252, status='visible', coords_client=(0, 1920, 0, 1007), dim_client=(1920, 1007), coords_win=(-8, 1928, -8, 1058), dim_win=(1936, 1066), class_name='Notepad', path='C:\\Windows\\System32\\notepad.exe'),
-  WindowInfo(parent=-1, pid=20440, title='msctls_statusbar32', windowtext='', hwnd=2886324, length=1, tid=17252, status='invisible', coords_client=(0, 484, 0, 23), dim_client=(484, 23), coords_win=(0, 484, 461, 484), dim_win=(484, 23), class_name='msctls_statusbar32', path='C:\\Windows\\System32\\notepad.exe'),
-  WindowInfo(parent=-1, pid=784, title='#32769', windowtext='', hwnd=65552, length=1, tid=984, status='visible', coords_client=(0, 1920, 0, 1080), dim_client=(1920, 1080), coords_win=(0, 1920, 0, 1080), dim_win=(1920, 1080), class_name='#32769', path='')]}
-  
-  
-mkey.get_elements_from_hwnd(2886324)
-
-{'element': WindowInfo(parent=-1, pid=20440, title='msctls_statusbar32', windowtext='', hwnd=2886324, length=1, tid=17252, status='invisible', coords_client=(0, 484, 0, 23), dim_client=(484, 23), coords_win=(0, 484, 461, 484), dim_win=(484, 23), class_name='msctls_statusbar32', path='C:\\Windows\\System32\\notepad.exe'),
- 'family': [WindowInfo(parent=-1, pid=20440, title='Edit', windowtext='', hwnd=592576, length=1, tid=17252, status='visible', coords_client=(0, 1903, 0, 1007), dim_client=(1903, 1007), coords_win=(0, 1920, 43, 1050), dim_win=(1920, 1007), class_name='Edit', path='C:\\Windows\\System32\\notepad.exe'),
-  WindowInfo(parent=-1, pid=20440, title='Notepad', windowtext='*Untitled - Notepad', hwnd=1051364, length=20, tid=17252, status='visible', coords_client=(0, 1920, 0, 1007), dim_client=(1920, 1007), coords_win=(-8, 1928, -8, 1058), dim_win=(1936, 1066), class_name='Notepad', path='C:\\Windows\\System32\\notepad.exe'),
-  WindowInfo(parent=-1, pid=20440, title='msctls_statusbar32', windowtext='', hwnd=2886324, length=1, tid=17252, status='invisible', coords_client=(0, 484, 0, 23), dim_client=(484, 23), coords_win=(0, 484, 461, 484), dim_win=(484, 23), class_name='msctls_statusbar32', path='C:\\Windows\\System32\\notepad.exe'),
-  WindowInfo(parent=-1, pid=784, title='#32769', windowtext='', hwnd=65552, length=1, tid=984, status='visible', coords_client=(0, 1920, 0, 1080), dim_client=(1920, 1080), coords_win=(0, 1920, 0, 1080), dim_win=(1920, 1080), class_name='#32769', path='')]}
-
-
-mkey.get_single_element_from_hwnd(10290540)
-
-Out[18]: WindowInfo(parent=-1, pid=24916, title='Notepad', windowtext='*Untitled - Notepad', hwnd=10290540, length=20, tid=20004, status='visible', coords_client=(0, 840, 0, 519), dim_client=(840, 519), coords_win=(714, 1570, 196, 774), dim_win=(856, 578), class_name='Notepad', path='C:\\Windows\\System32\\notepad.exe')
-```
-
-
-
-```python
-# Gets the rgb values from coordinates and shows the values simultaneously, press ctrl+c when you are done, the method will return a list with all coordinates and colors. 
-rgblist = mkey.show_rgb_values_at_mouse_position(        
-        sleeptime=0.01,
-        on_left_click=False,
-        on_right_click=False,
-        rgb_values=True,
-        rgba_values=True,
-        coords=True,
-        time_value=True,) 
-```
-
-
-
-```python
-# Getting the screen resolution
-mkey.get_screen_resolution()
-(1920, 1080)
-
-mkey.get_active_window()
-WindowInfo(pid=11144, title='SunAwtFrame', windowtext='Python Console - dfdir', hwnd=30283760, length=23, tid=6976, status='visible', coords_client=(0, 1921, 0, 996), dim_client=(1921, 996), coords_win=(2039, 3976, 54, 1058), dim_win=(1937, 1004), class_name='SunAwtFrame', path='C:\\Program Files\\JetBrains\\PyCharm Community Edition 2020.3\\bin\\pycharm64.exe')
-
-mkey.get_cursor_position() # executed only once
-(2436, 994)
-```
-
+<h2>mousekey</h2>
+
+
+
+
+* Works with multi screens
+* Keyboard and mouse can be used in Games like Roblox 
+* Has only a few dependencies (all of them pure python except NumPy)
+* Can simulate human-like mouse movement 
+* Facilitates multi key presses 
+
+
+<h2>Check out the videos</h2>
+<h3>Some methods</h3>
+
+
+<div align="left">
+      <a href="https://www.youtube.com/watch?v=1YugTBZBiyE">
+         <img src="https://img.youtube.com/vi/1YugTBZBiyE/0.jpg" style="width:100%;">
+      </a>
+</div>
+
+<h3>25 minutes of Roblox botting - 900x clicks / 900x keystrokes   </h3>
+
+<div align="left">
+      <a href="https://www.youtube.com/watch?v=OGPoiBnsy1M">
+         <img src="https://img.youtube.com/vi/OGPoiBnsy1M/0.jpg" style="width:100%;">
+      </a>
+</div>
+
+
+
+<h2>Installation</h2>
+
+
+
+```python
+$pip install mousekey
+from mousekey import MouseKey
+mkey = MouseKey()
+
+
+```
+
+
+<h2>Before you start, enable your guardian angel :)   </h2>
+
+
+
+```python
+# Kills the whole process, does always work (even with pure except)
+mkey.enable_failsafekill('ctrl+e')
+
+try:
+    while True:
+        try:
+            print('baba')
+            time.sleep(1)
+        except:
+            pass
+except:
+    pass
+baba
+baba
+baba
+baba
+
+# After pressing ctrl+e:
+Process finished with exit code 1
+```
+
+
+<h2>How to click and move </h2>
+
+
+The click methods should be able to handle any Game
+
+I have tested it with Roblox, which is known for blocking almost everything.
+
+As far as I know, there is no Python module that can handle Roblox [(https://pypi.org/project/ahk/](https://pypi.org/project/ahk/) works, but you need to download ahk.exe) 
+
+<h2>Absolute coordinates</h2>
+
+
+
+```python
+mkey.left_click_xy_natural(
+    200,
+    200,
+    delay=.3, # duration of the mouse click (down - up)
+    min_variation=-3, #  a random value will be added to each pixel  - define the minimum here 
+    max_variation=3,  # a random value will be added to each pixel  - define the maximum here 
+    use_every=4, # use every nth pixel 
+    sleeptime=(0.005, 0.009), # delay between each coordinate
+    print_coords=True, # console output 
+    percent=90, # the lower, the straighter the mouse movement
+) # A logarithm calculation lowers the speed when the cursor is getting close to the destination, like you do it in real life.
+```
+
+
+
+```python
+# Also available: 
+mkey.middle_click_xy_natural
+mkey.right_click_xy_natural
+```
+
+
+
+```python
+# if you don't want to click, only move, use:
+mkey.move_to_natural(100,100) # natural mouse movement
+mkey.move_to(3100,100) = move # no delay 
+```
+
+
+
+```python
+# Moving without delay and clicking:
+mkey.left_click_xy(10,10)
+mkey.right_click_xy(10,10)
+mkey.middle_click_xy(10,10)
+
+#Only clicking:
+mkey.left_click()
+mkey.middle_click()
+mkey.right_click()
+```
+
+
+<h2>Relative coordinates</h2>
+
+
+
+```python
+# For relative coordinates, use: 
+mkey.left_click_xy_natural_relative(
+    50,
+    50,
+    delay=0.1,
+    sleeptime=(0.00005, 0.00009),
+    print_coords=True,
+)
+
+mkey.right_click_xy_natural_relative(
+    x=500,
+    y=500,
+    delay=0.1,
+    sleeptime=(0.00005, 0.00009),
+    print_coords=True,
+)
+```
+
+
+
+```python
+# move and click relatively
+mkey.move_relative
+mkey.middle_click_xy_relative(-100,-100)
+mkey.move_to_natural_relative(300,-400)
+```
+
+
+<h2>Pressing keys</h2>
+
+
+
+```python
+# press a single key
+mkey.force_activate_window(10290540)
+mkey.press_key('f', delay=1) # delay in seconds
+```
+
+
+
+```python
+# You can press as many keys simultaneously as you want. 
+# The first value in each tuple indicates the sleep time before the next key is pressed, and presstime is the delay of the whole action.
+mkey.force_activate_window(10290540)
+mkey.press_keys_simultaneously_own_interval(
+    keystopress=[(0.1, "ctrl"), (0.1, "v")], presstime=.5
+)
+```
+
+
+
+```python
+# This method will calculate the sleep time between each key presses, so you don't have to worry about it. 
+mkey.force_activate_window(10290540)
+mkey.press_keys_simultaneously(
+    keystopress=["alt", "f4", "enter", "enter"],  
+    presstime=1.1,
+    percentofregularpresstime=100,
+)
+```
+
+
+
+```python
+# You can get a list with all available keys here: mkey.show_all_keys
+# I covered different writing styles ('volume_mute', 'VOLUME_MUTE', 'VOLUME MUTE', 'volume mute'), 
+{'control-break processing': 3,
+ 'backspace': 8,
+ 'tab': 9,
+ 'clear': 254,
+ 'enter': 13,
+ 'shift': 16,
+ 'ctrl': 17,
+ 'alt': 18,
+ 'pause': 19,
+ 'caps lock': 20,
+ 'ime hangul mode': 21,
+ 'ime junja mode': 23,
+ 'ime final mode': 24,
+ 'ime kanji mode': 25,
+ 'esc': 27,
+ 'ime convert': 28,
+ 'ime nonconvert': 29,
+ 'ime accept': 30,
+ 'ime mode change request': 31,
+ 'spacebar': 32,
+ 'page up': 33,
+ ...}
+```
+
+
+
+```python
+# You can block the mouse/keyboard input while executing actions.
+# That way, the user can't mess it up. 
+# If something goes wrong, press ctrl+alt+del 
+# This will automatically unlock the mouse/keyboard
+
+# Here is one example. Always use mkey.block_user_input() / mkey.unblock_user_input()
+if mkey.block_user_input():
+    try:
+        for k in range(3):
+            mkey.right_click()
+            sleep(1)
+            mkey.left_click_xy_natural(10, 10)
+            sleep(1)
+    finally:
+        mkey.unblock_user_input()
+```
+
+
+
+
+```python
+# You can send Unicode strings as well
+mkey.force_activate_window(10290540)
+mkey.send_unicode('bababöä')
+```
+
+
+
+```python
+# I have slightly modified 2 methods from pywinauto 
+# Most of the code is from pywinauto, I only changed the way the window gets activated
+mkey.send_keys_to_hwnd(handle=7539468, keys='babadu')
+mkey.send_keystrokes_to_hwnd(handle=7539468, '%{F4}')  # alt+f4
+
+# Here are all keystrokes for those 2 methods:
+https://pywinauto.readthedocs.io/en/latest/code/pywinauto.keyboard.html?highlight=VK_SPACE#pywinauto-keyboard
+
+{SCROLLLOCK}, {VK_SPACE}, {VK_LSHIFT}, {VK_PAUSE}, {VK_MODECHANGE},
+{BACK}, {VK_HOME}, {F23}, {F22}, {F21}, {F20}, {VK_HANGEUL}, {VK_KANJI},
+{VK_RIGHT}, {BS}, {HOME}, {VK_F4}, {VK_ACCEPT}, {VK_F18}, {VK_SNAPSHOT},
+{VK_PA1}, {VK_NONAME}, {VK_LCONTROL}, {ZOOM}, {VK_ATTN}, {VK_F10}, {VK_F22},
+{VK_F23}, {VK_F20}, {VK_F21}, {VK_SCROLL}, {TAB}, {VK_F11}, {VK_END},
+{LEFT}, {VK_UP}, {NUMLOCK}, {VK_APPS}, {PGUP}, {VK_F8}, {VK_CONTROL},
+{VK_LEFT}, {PRTSC}, {VK_NUMPAD4}, {CAPSLOCK}, {VK_CONVERT}, {VK_PROCESSKEY},
+{ENTER}, {VK_SEPARATOR}, {VK_RWIN}, {VK_LMENU}, {VK_NEXT}, {F1}, {F2},
+{F3}, {F4}, {F5}, {F6}, {F7}, {F8}, {F9}, {VK_ADD}, {VK_RCONTROL},
+{VK_RETURN}, {BREAK}, {VK_NUMPAD9}, {VK_NUMPAD8}, {RWIN}, {VK_KANA},
+{PGDN}, {VK_NUMPAD3}, {DEL}, {VK_NUMPAD1}, {VK_NUMPAD0}, {VK_NUMPAD7},
+{VK_NUMPAD6}, {VK_NUMPAD5}, {DELETE}, {VK_PRIOR}, {VK_SUBTRACT}, {HELP},
+{VK_PRINT}, {VK_BACK}, {CAP}, {VK_RBUTTON}, {VK_RSHIFT}, {VK_LWIN}, {DOWN},
+{VK_HELP}, {VK_NONCONVERT}, {BACKSPACE}, {VK_SELECT}, {VK_TAB}, {VK_HANJA},
+{VK_NUMPAD2}, {INSERT}, {VK_F9}, {VK_DECIMAL}, {VK_FINAL}, {VK_EXSEL},
+{RMENU}, {VK_F3}, {VK_F2}, {VK_F1}, {VK_F7}, {VK_F6}, {VK_F5}, {VK_CRSEL},
+{VK_SHIFT}, {VK_EREOF}, {VK_CANCEL}, {VK_DELETE}, {VK_HANGUL}, {VK_MBUTTON},
+{VK_NUMLOCK}, {VK_CLEAR}, {END}, {VK_MENU}, {SPACE}, {BKSP}, {VK_INSERT},
+{F18}, {F19}, {ESC}, {VK_MULTIPLY}, {F12}, {F13}, {F10}, {F11}, {F16},
+{F17}, {F14}, {F15}, {F24}, {RIGHT}, {VK_F24}, {VK_CAPITAL}, {VK_LBUTTON},
+{VK_OEM_CLEAR}, {VK_ESCAPE}, {UP}, {VK_DIVIDE}, {INS}, {VK_JUNJA},
+{VK_F19}, {VK_EXECUTE}, {VK_PLAY}, {VK_RMENU}, {VK_F13}, {VK_F12}, {LWIN},
+{VK_DOWN}, {VK_F17}, {VK_F16}, {VK_F15}, {VK_F14}
+
+'+': {VK_SHIFT}
+'^': {VK_CONTROL}
+'%': {VK_MENU} a.k.a. Alt key
+```
+
+
+<h2>Activating windows </h2>
+
+
+
+<table>
+  <tr>
+  </tr>
+</table>
+
+
+
+```python
+# lists all current windows and their hwnds, pid ...
+mkey.get_all_windows()
+
+ WindowInfo(pid=24880, title='tooltips_class32', windowtext='', hwnd=38931464, length=1, tid=14156, status='invisible', coords_client=(0, 0, 0, 0), dim_client=(0, 0), coords_win=(0, 0, 0, 0), dim_win=(0, 0), class_name='tooltips_class32', path='C:\\Windows\\explorer.exe'),
+ WindowInfo(pid=24916, title='IME', windowtext='Default IME', hwnd=333592, length=12, tid=6716, status='invisible', coords_client=(0, 0, 0, 0), dim_client=(0, 0), coords_win=(0, 0, 0, 0), dim_win=(0, 0), class_name='IME', path='C:\\Windows\\System32\\notepad.exe'),
+ WindowInfo(pid=24916, title='IME', windowtext='Default IME', hwnd=1706956, length=12, tid=20004, status='invisible', coords_client=(0, 0, 0, 0), dim_client=(0, 0), coords_win=(0, 0, 0, 0), dim_win=(0, 0), class_name='IME', path='C:\\Windows\\System32\\notepad.exe'),
+ WindowInfo(pid=24916, title='MSCTFIME UI', windowtext='MSCTFIME UI', hwnd=35652702, length=12, tid=20004, status='invisible', coords_client=(0, 0, 0, 0), dim_client=(0, 0), coords_win=(0, 0, 0, 0), dim_win=(0, 0), class_name='MSCTFIME UI', path='C:\\Windows\\System32\\notepad.exe'),
+ WindowInfo(pid=24916, title='Notepad', windowtext='*Untitled - Notepad', hwnd=10290540, length=20, tid=20004, status='visible', coords_client=(0, 840, 0, 519), dim_client=(840, 519), coords_win=(714, 1570, 196, 774), dim_win=(856, 578), class_name='Notepad', path='C:\\Windows\\System32\\notepad.exe'),
+ WindowInfo(pid=24916, title='WorkerW', windowtext='', hwnd=984520, length=1, tid=6716, status='invisible', coords_client=(0, 120, 0, 0), dim_client=(120, 0), coords_win=(0, 136, 0, 39), dim_win=(136, 39), class_name='WorkerW', path='C:\\Windows\\System32\\notepad.exe')]
+
+```
+
+
+
+```python
+# pass and hwnd (code above) as argument.
+mkey.activate_window(10290540) # usually this is enough to activate a window 
+
+#if not, use this method 
+# Activating a window is sometimes tricky. This method forces the activation of the window and works quite often when other methods don't 
+mkey.force_activate_window(17630556) 
+```
+
+
+
+```python
+# Pins a window on top of all others. 
+mkey.activate_topmost(17630556)
+
+# Restore the normal hierarchy. 
+# This method is helpful when one of your windows gets stuck during the automation in the topmost position
+mkey.deactivate_topmost(17630556)
+
+
+```
+
+
+
+```python
+# Some apps hide the cursor, here can you check it 
+mkey.is_cursor_shown ()
+True
+```
+
+
+
+```python
+# Shows you the coordinates of the current cursor position. Press ctrl+l when you have found the right coordinates.
+mkey.start_showing_cursor_position(exit_keys='ctrl+l')
+```
+
+
+
+```python
+mkey.get_single_element_from_coords(200,200)
+
+WindowInfo(parent=-1, pid=20440, title='Edit', windowtext='', hwnd=592576, length=1, tid=17252, status='visible', coords_client=(0, 1903, 0, 1007), dim_client=(1903, 1007), coords_win=(0, 1920, 43, 1050), dim_win=(1920, 1007), class_name='Edit', path='C:\\Windows\\System32\\notepad.exe')
+
+
+
+mkey.get_elements_from_coords(200,200)
+
+{'element': WindowInfo(parent=-1, pid=20440, title='Edit', windowtext='', hwnd=592576, length=1, tid=17252, status='visible', coords_client=(0, 1903, 0, 1007), dim_client=(1903, 1007), coords_win=(0, 1920, 43, 1050), dim_win=(1920, 1007), class_name='Edit', path='C:\\Windows\\System32\\notepad.exe'),
+ 'family': [WindowInfo(parent=-1, pid=20440, title='Edit', windowtext='', hwnd=592576, length=1, tid=17252, status='visible', coords_client=(0, 1903, 0, 1007), dim_client=(1903, 1007), coords_win=(0, 1920, 43, 1050), dim_win=(1920, 1007), class_name='Edit', path='C:\\Windows\\System32\\notepad.exe'),
+  WindowInfo(parent=-1, pid=20440, title='Notepad', windowtext='*Untitled - Notepad', hwnd=1051364, length=20, tid=17252, status='visible', coords_client=(0, 1920, 0, 1007), dim_client=(1920, 1007), coords_win=(-8, 1928, -8, 1058), dim_win=(1936, 1066), class_name='Notepad', path='C:\\Windows\\System32\\notepad.exe'),
+  WindowInfo(parent=-1, pid=20440, title='msctls_statusbar32', windowtext='', hwnd=2886324, length=1, tid=17252, status='invisible', coords_client=(0, 484, 0, 23), dim_client=(484, 23), coords_win=(0, 484, 461, 484), dim_win=(484, 23), class_name='msctls_statusbar32', path='C:\\Windows\\System32\\notepad.exe'),
+  WindowInfo(parent=-1, pid=784, title='#32769', windowtext='', hwnd=65552, length=1, tid=984, status='visible', coords_client=(0, 1920, 0, 1080), dim_client=(1920, 1080), coords_win=(0, 1920, 0, 1080), dim_win=(1920, 1080), class_name='#32769', path='')]}
+  
+  
+mkey.get_elements_from_hwnd(2886324)
+
+{'element': WindowInfo(parent=-1, pid=20440, title='msctls_statusbar32', windowtext='', hwnd=2886324, length=1, tid=17252, status='invisible', coords_client=(0, 484, 0, 23), dim_client=(484, 23), coords_win=(0, 484, 461, 484), dim_win=(484, 23), class_name='msctls_statusbar32', path='C:\\Windows\\System32\\notepad.exe'),
+ 'family': [WindowInfo(parent=-1, pid=20440, title='Edit', windowtext='', hwnd=592576, length=1, tid=17252, status='visible', coords_client=(0, 1903, 0, 1007), dim_client=(1903, 1007), coords_win=(0, 1920, 43, 1050), dim_win=(1920, 1007), class_name='Edit', path='C:\\Windows\\System32\\notepad.exe'),
+  WindowInfo(parent=-1, pid=20440, title='Notepad', windowtext='*Untitled - Notepad', hwnd=1051364, length=20, tid=17252, status='visible', coords_client=(0, 1920, 0, 1007), dim_client=(1920, 1007), coords_win=(-8, 1928, -8, 1058), dim_win=(1936, 1066), class_name='Notepad', path='C:\\Windows\\System32\\notepad.exe'),
+  WindowInfo(parent=-1, pid=20440, title='msctls_statusbar32', windowtext='', hwnd=2886324, length=1, tid=17252, status='invisible', coords_client=(0, 484, 0, 23), dim_client=(484, 23), coords_win=(0, 484, 461, 484), dim_win=(484, 23), class_name='msctls_statusbar32', path='C:\\Windows\\System32\\notepad.exe'),
+  WindowInfo(parent=-1, pid=784, title='#32769', windowtext='', hwnd=65552, length=1, tid=984, status='visible', coords_client=(0, 1920, 0, 1080), dim_client=(1920, 1080), coords_win=(0, 1920, 0, 1080), dim_win=(1920, 1080), class_name='#32769', path='')]}
+
+
+mkey.get_single_element_from_hwnd(10290540)
+
+Out[18]: WindowInfo(parent=-1, pid=24916, title='Notepad', windowtext='*Untitled - Notepad', hwnd=10290540, length=20, tid=20004, status='visible', coords_client=(0, 840, 0, 519), dim_client=(840, 519), coords_win=(714, 1570, 196, 774), dim_win=(856, 578), class_name='Notepad', path='C:\\Windows\\System32\\notepad.exe')
+```
+
+
+
+```python
+# Gets the rgb values from coordinates and shows the values simultaneously, press ctrl+c when you are done, the method will return a list with all coordinates and colors. 
+rgblist = mkey.show_rgb_values_at_mouse_position(        
+        sleeptime=0.01,
+        on_left_click=False,
+        on_right_click=False,
+        rgb_values=True,
+        rgba_values=True,
+        coords=True,
+        time_value=True,) 
+```
+
+
+
+```python
+# Getting the screen resolution
+mkey.get_screen_resolution()
+(1920, 1080)
+
+mkey.get_active_window()
+WindowInfo(pid=11144, title='SunAwtFrame', windowtext='Python Console - dfdir', hwnd=30283760, length=23, tid=6976, status='visible', coords_client=(0, 1921, 0, 996), dim_client=(1921, 996), coords_win=(2039, 3976, 54, 1058), dim_win=(1937, 1004), class_name='SunAwtFrame', path='C:\\Program Files\\JetBrains\\PyCharm Community Edition 2020.3\\bin\\pycharm64.exe')
+
+mkey.get_cursor_position() # executed only once
+(2436, 994)
+```
+
```

#### html2text {}

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1 Name: mousekey Version: 0.11 Summary: Automates mouse/
-keyboard, works with games like Roblox! Home-page: https://github.com/
-hansalemaos/mousekey Author: Johannes Fischer Author-email:
-gmail.com> License: MIT Keywords: automate,keystroke,mouse,games,pyautogui
-Classifier: Development Status :: 4 - Beta Classifier: Programming Language ::
-Python :: 3 :: Only Classifier: Programming Language :: Python :: 3.9
-Classifier: Topic :: Scientific/Engineering :: Visualization Classifier: Topic
-:: Software Development :: Libraries :: Python Modules Classifier: Topic ::
-Text Editors :: Text Processing Classifier: Topic :: Text Processing :: General
-Classifier: Topic :: Text Processing :: Indexing Classifier: Topic :: Text
-Processing :: Filters Classifier: Topic :: Utilities Description-Content-Type:
-text/markdown License-File: LICENSE.rst
 ***** mousekey *****
 * Works with multi screens * Keyboard and mouse can be used in Games like
 Roblox * Has only a few dependencies (all of them pure python except NumPy) *
 Can simulate human-like mouse movement * Facilitates multi key presses
 ***** Check out the videos *****
 **** Some methods ****
 [https://img.youtube.com/vi/1YugTBZBiyE/0.jpg]
```

### Comparing `mousekey-0.11/README.md` & `mousekey-0.12/mousekey/README.MD`

 * *Files identical despite different names*

### Comparing `mousekey-0.11/mousekey/README.MD` & `mousekey-0.12/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,25 @@
+Metadata-Version: 2.1
+Name: mousekey
+Version: 0.12
+Summary: Automates mouse/keyboard, works with games like Roblox!
+Home-page: https://github.com/hansalemaos/mousekey
+Author: Johannes Fischer
+Author-email: aulasparticularesdealemaosp@gmail.com
+License: MIT
+Keywords: automate,keystroke,mouse,games,pyautogui
+Classifier: Development Status :: 4 - Beta
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Utilities
+Description-Content-Type: text/markdown
+License-File: LICENSE.rst
+
+
 <h2>mousekey</h2>
 
 
 
 
 * Works with multi screens
 * Keyboard and mouse can be used in Games like Roblox
```

#### html2text {}

```diff
@@ -1,7 +1,16 @@
+Metadata-Version: 2.1 Name: mousekey Version: 0.12 Summary: Automates mouse/
+keyboard, works with games like Roblox! Home-page: https://github.com/
+hansalemaos/mousekey Author: Johannes Fischer Author-email:
+aulasparticularesdealemaosp@gmail.com License: MIT Keywords:
+automate,keystroke,mouse,games,pyautogui Classifier: Development Status :: 4 -
+Beta Classifier: Programming Language :: Python :: 3 :: Only Classifier:
+Programming Language :: Python :: 3.10 Classifier: Topic :: Software
+Development :: Libraries :: Python Modules Classifier: Topic :: Utilities
+Description-Content-Type: text/markdown License-File: LICENSE.rst
 ***** mousekey *****
 * Works with multi screens * Keyboard and mouse can be used in Games like
 Roblox * Has only a few dependencies (all of them pure python except NumPy) *
 Can simulate human-like mouse movement * Facilitates multi key presses
 ***** Check out the videos *****
 **** Some methods ****
 [https://img.youtube.com/vi/1YugTBZBiyE/0.jpg]
```

### Comparing `mousekey-0.11/mousekey/__init__.py` & `mousekey-0.12/mousekey/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 import time
 import ctypes
 import six
 import keyboard as key_b
 from ctypes_rgb_values import get_rgb_values
 from ctypes_window_info import get_window_infos
 from flatten_everything import flatten_everything, ProtectedTuple
+
 BlockInput = ctypes.windll.user32.BlockInput
 BlockInput.argtypes = [wintypes.BOOL]
 BlockInput.restype = wintypes.BOOL
 
 childcounter = sys.modules[__name__]
 childcounter.rightnow = None
 
@@ -287,48 +288,48 @@
                     j[0]
                     for j in list(
                         set(
                             flatten_everything(
                                 [
                                     ProtectedTuple(m)
                                     for m in [
-                                        find_elements(r)
-                                        for r in list(
-                                            flatten_everything(
+                                    find_elements(r)
+                                    for r in list(
+                                        flatten_everything(
+                                            [
                                                 [
-                                                    [
-                                                        list(
-                                                            set(
-                                                                [
-                                                                    z
-                                                                    for z in flatten_everything(
-                                                                        GetParent(p)
-                                                                    )
-                                                                    if isinstance(
-                                                                        z, int
-                                                                    )
-                                                                ]
+                                                    list(
+                                                        set(
+                                                            [
+                                                                z
+                                                                for z in flatten_everything(
+                                                                GetParent(p)
                                                             )
-                                                        )
-                                                        for p in flatten_everything(
-                                                            [[y.hwnd for y in x]]
-                                                        )
-                                                    ]
-                                                    for x in (
-                                                        [
-                                                            find_elements(tra)
-                                                            for tra in get_all_children(
-                                                                x.hwnd
+                                                                if isinstance(
+                                                                z, int
                                                             )
-                                                        ]
+                                                            ]
+                                                        )
                                                     )
+                                                    for p in flatten_everything(
+                                                    [[y.hwnd for y in x]]
+                                                )
+                                                ]
+                                                for x in (
+                                                [
+                                                    find_elements(tra)
+                                                    for tra in get_all_children(
+                                                    x.hwnd
+                                                )
                                                 ]
                                             )
+                                            ]
                                         )
-                                    ]
+                                    )
+                                ]
                                 ]
                             )
                         )
                     )
                 ),
             }
             for x in child
@@ -353,15 +354,14 @@
 
 def start_failsafe(hotkey="ctrl+e"):
     key_b.add_hotkey(hotkey, failsafe_kill)
 
 
 SHORT = ctypes.c_short
 
-
 VK_LBUTTON = 0x01  # Left mouse button
 VK_RBUTTON = 0x02  # Right mouse button
 VK_CANCEL = 0x03  # Control-break processing
 VK_MBUTTON = 0x04  # Middle mouse button (three-button mouse)
 VK_XBUTTON1 = 0x05  # X1 mouse button
 VK_XBUTTON2 = 0x06  # X2 mouse button
 VK_BACK = 0x08  # BACKSPACE key
@@ -1039,15 +1039,14 @@
         lib.SendInput(1, byref(i), sizeof(INPUT))
         i.ki.dwFlags |= KEYEVENTF_KEYUP
         lib.SendInput(1, byref(i), sizeof(INPUT))
 
 
 LPINPUT = ctypes.POINTER(INPUT)
 
-
 user32.SendInput.errcheck = _check_count
 user32.SendInput.argtypes = (
     wintypes.UINT,
     LPINPUT,
     ctypes.c_int,
 )
 
@@ -1096,16 +1095,16 @@
     windowsInput = Input(emptyLong, inputList)
     ctypes.windll.user32.SendInput(
         1, ctypes.pointer(windowsInput), ctypes.sizeof(windowsInput)
     )
 
 
 def move(
-    x,
-    y,
+        x,
+        y,
 ):
     relative = False
     mouseFlag = MOUSEEVENTF_MOVE
 
     if not relative:
         mouseFlag |= MOUSEEVENTF_ABSOLUTE
         xr, yr = get_resolution()
@@ -1160,22 +1159,22 @@
     out = a.astype(int)
     idx = np.random.choice(a.size, n, replace=False)
     out.flat[idx] += np.random.randint(low=low, high=high, size=n)
     return out
 
 
 def natural_mouse_movement(
-    x,
-    y,
-    min_variation=-2,
-    max_variation=2,
-    use_every=1,
-    sleeptime=(0.005, 0.009),
-    print_coords=True,
-    percent=90,
+        x,
+        y,
+        min_variation=-2,
+        max_variation=2,
+        use_every=1,
+        sleeptime=(0.005, 0.009),
+        print_coords=True,
+        percent=90,
 ):
     nowx, nowy = get_cursor()
     coordtomove = x, y
     futx, futy = coordtomove
     allco = np.array([[nowx, nowy], [futx, futy]])
 
     alla = calculate_all_coords(allco)
@@ -1195,19 +1194,19 @@
             print(f"{x}         ", end="\r")
 
         move(int(x[0]), int(x[1]))
         time.sleep(uniform(*sleeptime))
 
 
 def left_click_xy_natural_relative(
-    x,
-    y,
-    delay=0.1,
-    sleeptime=(0.00005, 0.00009),
-    print_coords=True,
+        x,
+        y,
+        delay=0.1,
+        sleeptime=(0.00005, 0.00009),
+        print_coords=True,
 ):
     natural_mouse_movement_relative(
         x,
         y,
         sleeptime=sleeptime,
         print_coords=print_coords,
     )
@@ -1225,18 +1224,18 @@
             yield list(x)
     else:
         for x in logsplit(args[0]):
             yield list(x)
 
 
 def natural_mouse_movement_relative(
-    x,
-    y,
-    sleeptime=(0.00005, 0.00009),
-    print_coords=True,
+        x,
+        y,
+        sleeptime=(0.00005, 0.00009),
+        print_coords=True,
 ):
     nowx, nowy = 0, 0
     coordtomove = x * 2, y * 2
     futx, futy = coordtomove
     allco = np.array([[nowx, nowy], [futx, futy]])
     alla = calculate_all_coords(allco)
     alla = np.vstack([alla, [futx, futy]])
@@ -1253,29 +1252,53 @@
 
 def left_click(delay=0.1):
     _mouse_click(MOUSEEVENTF_LEFTDOWN)
     time.sleep(delay)
     _mouse_click(MOUSEEVENTF_LEFTUP)
 
 
+def left_mouse_down():
+    _mouse_click(MOUSEEVENTF_LEFTDOWN)
+
+
+def left_mouse_up():
+    _mouse_click(MOUSEEVENTF_LEFTUP)
+
+
+def right_mouse_down():
+    _mouse_click(MOUSEEVENTF_RIGHTDOWN)
+
+
+def right_mouse_up():
+    _mouse_click(MOUSEEVENTF_RIGHTUP)
+
+
+def middle_mouse_down():
+    _mouse_click(MOUSEEVENTF_MIDDLEDOWN)
+
+
+def middle_mouse_up():
+    _mouse_click(MOUSEEVENTF_MIDDLEUP)
+
+
 def left_click_xy(x, y, delay=0.1):
     move(x, y)
     left_click(delay=delay)
 
 
 def left_click_xy_natural(
-    x,
-    y,
-    delay=0.1,
-    min_variation=-3,
-    max_variation=3,
-    use_every=4,
-    sleeptime=(0.005, 0.009),
-    print_coords=True,
-    percent=90,
+        x,
+        y,
+        delay=0.1,
+        min_variation=-3,
+        max_variation=3,
+        use_every=4,
+        sleeptime=(0.005, 0.009),
+        print_coords=True,
+        percent=90,
 ):
     natural_mouse_movement(
         x,
         y,
         min_variation=min_variation,
         max_variation=max_variation,
         use_every=use_every,
@@ -1294,23 +1317,23 @@
 
 def right_click_xy(x, y, delay=0.1):
     move(x, y)
     right_click(delay=delay)
 
 
 def right_click_xy_natural(
-    x,
-    y,
-    delay=0.1,
-    min_variation=-1,
-    max_variation=1,
-    use_every=1,
-    sleeptime=(0.005, 0.009),
-    print_coords=True,
-    percent=90,
+        x,
+        y,
+        delay=0.1,
+        min_variation=-1,
+        max_variation=1,
+        use_every=1,
+        sleeptime=(0.005, 0.009),
+        print_coords=True,
+        percent=90,
 ):
     natural_mouse_movement(
         x,
         y,
         min_variation=min_variation,
         max_variation=max_variation,
         use_every=use_every,
@@ -1318,19 +1341,19 @@
         print_coords=print_coords,
         percent=percent,
     )
     right_click(delay=delay)
 
 
 def right_click_xy_natural_relative(
-    x,
-    y,
-    delay=0.1,
-    sleeptime=(0.00005, 0.00009),
-    print_coords=True,
+        x,
+        y,
+        delay=0.1,
+        sleeptime=(0.00005, 0.00009),
+        print_coords=True,
 ):
     natural_mouse_movement_relative(
         x,
         y,
         sleeptime=sleeptime,
         print_coords=print_coords,
     )
@@ -1345,23 +1368,23 @@
 
 def middle_click_xy(x, y, delay=0.1):
     move(x, y)
     middle_click(delay=delay)
 
 
 def middle_click_xy_natural(
-    x,
-    y,
-    delay=0.1,
-    min_variation=-3,
-    max_variation=3,
-    use_every=4,
-    sleeptime=(0.005, 0.009),
-    print_coords=True,
-    percent=90,
+        x,
+        y,
+        delay=0.1,
+        min_variation=-3,
+        max_variation=3,
+        use_every=4,
+        sleeptime=(0.005, 0.009),
+        print_coords=True,
+        percent=90,
 ):
     natural_mouse_movement(
         x,
         y,
         min_variation=min_variation,
         max_variation=max_variation,
         use_every=use_every,
@@ -1369,19 +1392,19 @@
         print_coords=print_coords,
         percent=percent,
     )
     middle_click(delay=delay)
 
 
 def middle_click_xy_relative(
-    x,
-    y,
-    delay=0.1,
-    sleeptime=(0.00005, 0.00009),
-    print_coords=True,
+        x,
+        y,
+        delay=0.1,
+        sleeptime=(0.00005, 0.00009),
+        print_coords=True,
 ):
     natural_mouse_movement_relative(
         x,
         y,
         sleeptime=sleeptime,
         print_coords=print_coords,
     )
@@ -1407,16 +1430,16 @@
     )
     ac = {"pid": pid.value, "foreground": active, "active_window": active_window}
     try:
         return [
             x
             for x in get_window_infos()
             if x.pid == ac["pid"]
-            and x.hwnd == ac["foreground"]
-            and x.tid == ac["active_window"]
+               and x.hwnd == ac["foreground"]
+               and x.tid == ac["active_window"]
         ][0]
     except Exception:
         return []
 
 
 DEBUG = 0
 INPUT_KEYBOARD = 1
@@ -1605,15 +1628,14 @@
     "\\": 0xDC,
     "]": 0xDD,
     "'": 0xDE,
 }
 ascii_vk.update(dict((c, ord(c)) for c in string.ascii_uppercase + string.digits))
 ascii_vk.update(dict((c, ord(c.upper())) for c in string.ascii_lowercase))
 
-
 """
 
 From here on, almost everything is strongly based on pywinauto:
 https://pywinauto.readthedocs.io/en/latest/
 
         Copyright (c) 2017, Mark Mc Mahon and Contributors
     All rights reserved.
@@ -1793,15 +1815,14 @@
 
         return "<{}>".format(" ".join(parts))
 
     __repr__ = __str__
 
 
 class VirtualKeyAction(KeyAction):
-
     """Represents a virtual key action e.g. F9 DOWN, etc
 
     Overrides necessary methods of KeyAction
     """
 
     def _get_key_info(self):
         """Virtual keys have extended flag set"""
@@ -1823,15 +1844,14 @@
         for inp in self.GetInput():
             # send_scancode(inp)
             Press(inp.ki.wVk)
             # win32api.keybd_event(inp.ki.wVk, inp.ki.wScan, inp.ki.dwFlags)
 
 
 class EscapedKeyAction(KeyAction):
-
     """Represents an escaped key action e.g. F9 DOWN, etc
 
     Overrides necessary methods of KeyAction
     """
 
     def _get_key_info(self):
         """EscapedKeyAction doesn't send it as Unicode
@@ -1851,15 +1871,14 @@
         # it works more stable for virtual keys than SendInput
         for inp in self.GetInput():
             # win32api.keybd_event(inp.ki.wVk, inp.ki.wScan, inp.ki.dwFlags)
             Press(inp.ki.wVk)
 
 
 class PauseAction(KeyAction):
-
     """Represents a pause action"""
 
     def __init__(self, how_long):
         self.how_long = how_long
 
     def run(self):
         """Pause for the lenght of time specified"""
@@ -1914,21 +1933,21 @@
     else:
         raise RuntimeError("Unknown code: {}".format(code))
 
     return code_keys
 
 
 def parse_keys(
-    string,
-    with_spaces=False,
-    with_tabs=False,
-    with_newlines=False,
-    modifiers=None,
-    vk_packet=True,
-    activate_window_before=True,
+        string,
+        with_spaces=False,
+        with_tabs=False,
+        with_newlines=False,
+        modifiers=None,
+        vk_packet=True,
+        activate_window_before=True,
 ):
     """Return the parsed keys"""
 
     keys = []
     if not modifiers:
         modifiers = []
 
@@ -1995,20 +2014,20 @@
         elif c == "}":
             raise KeySequenceError("`}` should be preceeded by `{`")
 
         # so it is a normal character
         else:
             # don't output white space unless flags to output have been set
             if (
-                c == " "
-                and not with_spaces
-                or c == "\t"
-                and not with_tabs
-                or c == "\n"
-                and not with_newlines
+                    c == " "
+                    and not with_spaces
+                    or c == "\t"
+                    and not with_tabs
+                    or c == "\n"
+                    and not with_newlines
             ):
                 continue
 
             # output newline
             if c in ("~", "\n"):
                 keys.append(VirtualKeyAction(CODES["ENTER"]))
 
@@ -2043,23 +2062,23 @@
 
 def LoByte(val):
     """Return the low byte of the value"""
     return val & 0xFF
 
 
 def send_keys(
-    handle,
-    keys,
-    pause=0.05,
-    with_spaces=False,
-    with_tabs=False,
-    with_newlines=False,
-    turn_off_numlock=True,
-    vk_packet=True,
-    activate_window_before=True,
+        handle,
+        keys,
+        pause=0.05,
+        with_spaces=False,
+        with_tabs=False,
+        with_newlines=False,
+        turn_off_numlock=True,
+        vk_packet=True,
+        activate_window_before=True,
 ):
     """Parse the keys and type them"""
     sena = (
         ctypes.c_int(handle),
         ctypes.c_int(WM_ACTIVATE),
         ctypes.c_int(WA_ACTIVE),
         ctypes.c_int(0),
@@ -2159,15 +2178,14 @@
 GetMessage.argtypes = [
     POINTER(wintypes.MSG),
     wintypes.HWND,
     wintypes.UINT,
     wintypes.UINT,
 ]
 
-
 SendMessage = ctypes.windll.user32.SendMessageW
 SendMessageA = ctypes.windll.user32.SendMessageA
 
 
 def activate_topmost(hwnd):
     ctypes.windll.user32.BringWindowToTop(hwnd)  # works OK
     HWND_TOPMOST = -1
@@ -2231,20 +2249,20 @@
 def get_fg_window():
     return _get_elements_from_coords(hwnd=ctypes.windll.user32.GetForegroundWindow())[
         "element"
     ]
 
 
 def send_keystrokes(
-    handle,
-    keystrokes,
-    with_spaces=True,
-    with_tabs=True,
-    with_newlines=True,
-    activate_window_before=True,
+        handle,
+        keystrokes,
+        with_spaces=True,
+        with_tabs=True,
+        with_newlines=True,
+        activate_window_before=True,
 ):
     """
     Silently send keystrokes to the control in an inactive window
 
     It parses modifiers Shift(+), Control(^), Menu(%) and Sequences like "{TAB}", "{ENTER}"
     For more information about Sequences and Modifiers navigate to module `keyboard`_
 
@@ -2319,39 +2337,39 @@
 
                 new_keyboard_state[vk] |= 128
                 if shift_state & 1 == 1:
                     new_keyboard_state[VK_SHIFT] |= 128
                 keyboard_state_stack.append(new_keyboard_state)
 
                 lparam = (
-                    repeat << 0
-                    | scan << 16
-                    | (flags & 1) << 24
-                    | context_code << 29
-                    | 0 << 31
+                        repeat << 0
+                        | scan << 16
+                        | (flags & 1) << 24
+                        | context_code << 29
+                        | 0 << 31
                 )
 
                 SetKeyboardState(keyboard_state_stack[-1])
                 PostMessage(handle, down_msg, vk, lparam)
                 if vk == VK_MENU:
                     context_code = 1
 
                 # a delay for keyboard state to take effect
                 time.sleep(0.01)
 
             if key.up and vk > 0:
                 keyboard_state_stack.pop()
 
                 lparam = (
-                    repeat << 0
-                    | scan << 16
-                    | (flags & 1) << 24
-                    | context_code << 29
-                    | 1 << 30
-                    | 1 << 31
+                        repeat << 0
+                        | scan << 16
+                        | (flags & 1) << 24
+                        | context_code << 29
+                        | 1 << 30
+                        | 1 << 31
                 )
 
                 PostMessage(handle, up_msg, vk, lparam)
                 SetKeyboardState(keyboard_state_stack[-1])
 
                 if vk == VK_MENU:
                     context_code = 0
@@ -2426,19 +2444,18 @@
         threadlist[-1].start()
         time.sleep(tim)
         ini += 1
         print(ausfu, tim, k)
     time.sleep(restssleep)
 
 
-
-
 def block_user_input():
     return BlockInput(True)
 
+
 def unblock_user_input():
     return BlockInput(False)
 
 
 class MouseKey:
     def __init__(self):
         self.block_user_input = block_user_input
@@ -2477,14 +2494,20 @@
         self.left_click_xy_natural_relative = left_click_xy_natural_relative
         self.move_to_natural_relative = natural_mouse_movement_relative
         self.right_click_xy_natural_relative = right_click_xy_natural_relative
         self.force_activate_window = force_activate_window
         self.press_keys_simultaneously = press_multiple_keys
         self.press_keys_simultaneously_own_interval = press_multiple_keys_own_interval
         self.show_all_keys = allkeys
+        self.left_mouse_down = left_mouse_down
+        self.left_mouse_up = left_mouse_up
+        self.right_mouse_down = right_mouse_down
+        self.right_mouse_up = right_mouse_up
+        self.middle_mouse_down = middle_mouse_down
+        self.middle_mouse_up = middle_mouse_up
         self.t = kthread.KThread(target=self._get_cursor, name="get_cursor")
         self.show_cur = False
 
     def _kill_coord(self):
         self.show_cur = False
         time.sleep(0.05)
         self.show_cur = True
@@ -2523,22 +2546,22 @@
             self.t = kthread.KThread(target=self._get_cursor, name="get_cursor")
             self.t.start()
 
     def stop_showing_cursor_position(self):
         self.show_cur = False
 
     def show_rgb_values_at_mouse_position(
-        self,
-        sleeptime=0.01,
-        on_left_click=False,
-        on_right_click=False,
-        rgb_values=True,
-        rgba_values=True,
-        coords=True,
-        time_value=True,
+            self,
+            sleeptime=0.01,
+            on_left_click=False,
+            on_right_click=False,
+            rgb_values=True,
+            rgba_values=True,
+            coords=True,
+            time_value=True,
     ):
         return get_rgb_values(
             sleeptime=sleeptime,
             on_left_click=on_left_click,
             on_right_click=on_right_click,
             rgb_values=rgb_values,
             rgba_values=rgba_values,
```

### Comparing `mousekey-0.11/mousekey.egg-info/PKG-INFO` & `mousekey-0.12/mousekey.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,441 +1,436 @@
 Metadata-Version: 2.1
 Name: mousekey
-Version: 0.11
+Version: 0.12
 Summary: Automates mouse/keyboard, works with games like Roblox!
 Home-page: https://github.com/hansalemaos/mousekey
 Author: Johannes Fischer
-Author-email: <aulasparticularesdealemaosp@gmail.com>
+Author-email: aulasparticularesdealemaosp@gmail.com
 License: MIT
 Keywords: automate,keystroke,mouse,games,pyautogui
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Topic :: Scientific/Engineering :: Visualization
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Text Editors :: Text Processing
-Classifier: Topic :: Text Processing :: General
-Classifier: Topic :: Text Processing :: Indexing
-Classifier: Topic :: Text Processing :: Filters
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 License-File: LICENSE.rst
 
 
-<h2>mousekey</h2>
-
-
-
-
-* Works with multi screens
-* Keyboard and mouse can be used in Games like Roblox 
-* Has only a few dependencies (all of them pure python except NumPy)
-* Can simulate human-like mouse movement 
-* Facilitates multi key presses 
-
-
-<h2>Check out the videos</h2>
-<h3>Some methods</h3>
-
-
-<div align="left">
-      <a href="https://www.youtube.com/watch?v=1YugTBZBiyE">
-         <img src="https://img.youtube.com/vi/1YugTBZBiyE/0.jpg" style="width:100%;">
-      </a>
-</div>
-
-<h3>25 minutes of Roblox botting - 900x clicks / 900x keystrokes   </h3>
-
-<div align="left">
-      <a href="https://www.youtube.com/watch?v=OGPoiBnsy1M">
-         <img src="https://img.youtube.com/vi/OGPoiBnsy1M/0.jpg" style="width:100%;">
-      </a>
-</div>
-
-
-
-<h2>Installation</h2>
-
-
-
-```python
-$pip install mousekey
-from mousekey import MouseKey
-mkey = MouseKey()
-
-
-```
-
-
-<h2>Before you start, enable your guardian angel :)   </h2>
-
-
-
-```python
-# Kills the whole process, does always work (even with pure except)
-mkey.enable_failsafekill('ctrl+e')
-
-try:
-    while True:
-        try:
-            print('baba')
-            time.sleep(1)
-        except:
-            pass
-except:
-    pass
-baba
-baba
-baba
-baba
-
-# After pressing ctrl+e:
-Process finished with exit code 1
-```
-
-
-<h2>How to click and move </h2>
-
-
-The click methods should be able to handle any Game
-
-I have tested it with Roblox, which is known for blocking almost everything.
-
-As far as I know, there is no Python module that can handle Roblox [(https://pypi.org/project/ahk/](https://pypi.org/project/ahk/) works, but you need to download ahk.exe) 
-
-<h2>Absolute coordinates</h2>
-
-
-
-```python
-mkey.left_click_xy_natural(
-    200,
-    200,
-    delay=.3, # duration of the mouse click (down - up)
-    min_variation=-3, #  a random value will be added to each pixel  - define the minimum here 
-    max_variation=3,  # a random value will be added to each pixel  - define the maximum here 
-    use_every=4, # use every nth pixel 
-    sleeptime=(0.005, 0.009), # delay between each coordinate
-    print_coords=True, # console output 
-    percent=90, # the lower, the straighter the mouse movement
-) # A logarithm calculation lowers the speed when the cursor is getting close to the destination, like you do it in real life.
-```
-
-
-
-```python
-# Also available: 
-mkey.middle_click_xy_natural
-mkey.right_click_xy_natural
-```
-
-
-
-```python
-# if you don't want to click, only move, use:
-mkey.move_to_natural(100,100) # natural mouse movement
-mkey.move_to(3100,100) = move # no delay 
-```
-
-
-
-```python
-# Moving without delay and clicking:
-mkey.left_click_xy(10,10)
-mkey.right_click_xy(10,10)
-mkey.middle_click_xy(10,10)
-
-#Only clicking:
-mkey.left_click()
-mkey.middle_click()
-mkey.right_click()
-```
-
-
-<h2>Relative coordinates</h2>
-
-
-
-```python
-# For relative coordinates, use: 
-mkey.left_click_xy_natural_relative(
-    50,
-    50,
-    delay=0.1,
-    sleeptime=(0.00005, 0.00009),
-    print_coords=True,
-)
-
-mkey.right_click_xy_natural_relative(
-    x=500,
-    y=500,
-    delay=0.1,
-    sleeptime=(0.00005, 0.00009),
-    print_coords=True,
-)
-```
-
-
-
-```python
-# move and click relatively
-mkey.move_relative
-mkey.middle_click_xy_relative(-100,-100)
-mkey.move_to_natural_relative(300,-400)
-```
-
-
-<h2>Pressing keys</h2>
-
-
-
-```python
-# press a single key
-mkey.force_activate_window(10290540)
-mkey.press_key('f', delay=1) # delay in seconds
-```
-
-
-
-```python
-# You can press as many keys simultaneously as you want. 
-# The first value in each tuple indicates the sleep time before the next key is pressed, and presstime is the delay of the whole action.
-mkey.force_activate_window(10290540)
-mkey.press_keys_simultaneously_own_interval(
-    keystopress=[(0.1, "ctrl"), (0.1, "v")], presstime=.5
-)
-```
-
-
-
-```python
-# This method will calculate the sleep time between each key presses, so you don't have to worry about it. 
-mkey.force_activate_window(10290540)
-mkey.press_keys_simultaneously(
-    keystopress=["alt", "f4", "enter", "enter"],  
-    presstime=1.1,
-    percentofregularpresstime=100,
-)
-```
-
-
-
-```python
-# You can get a list with all available keys here: mkey.show_all_keys
-# I covered different writing styles ('volume_mute', 'VOLUME_MUTE', 'VOLUME MUTE', 'volume mute'), 
-{'control-break processing': 3,
- 'backspace': 8,
- 'tab': 9,
- 'clear': 254,
- 'enter': 13,
- 'shift': 16,
- 'ctrl': 17,
- 'alt': 18,
- 'pause': 19,
- 'caps lock': 20,
- 'ime hangul mode': 21,
- 'ime junja mode': 23,
- 'ime final mode': 24,
- 'ime kanji mode': 25,
- 'esc': 27,
- 'ime convert': 28,
- 'ime nonconvert': 29,
- 'ime accept': 30,
- 'ime mode change request': 31,
- 'spacebar': 32,
- 'page up': 33,
- ...}
-```
-
-
-
-```python
-# You can block the mouse/keyboard input while executing actions.
-# That way, the user can't mess it up. 
-# If something goes wrong, press ctrl+alt+del 
-# This will automatically unlock the mouse/keyboard
-
-# Here is one example. Always use mkey.block_user_input() / mkey.unblock_user_input()
-if mkey.block_user_input():
-    try:
-        for k in range(3):
-            mkey.right_click()
-            sleep(1)
-            mkey.left_click_xy_natural(10, 10)
-            sleep(1)
-    finally:
-        mkey.unblock_user_input()
-```
-
-
-
-
-```python
-# You can send Unicode strings as well
-mkey.force_activate_window(10290540)
-mkey.send_unicode('bababöä')
-```
-
-
-
-```python
-# I have slightly modified 2 methods from pywinauto 
-# Most of the code is from pywinauto, I only changed the way the window gets activated
-mkey.send_keys_to_hwnd(handle=7539468, keys='babadu')
-mkey.send_keystrokes_to_hwnd(handle=7539468, '%{F4}')  # alt+f4
-
-# Here are all keystrokes for those 2 methods:
-https://pywinauto.readthedocs.io/en/latest/code/pywinauto.keyboard.html?highlight=VK_SPACE#pywinauto-keyboard
-
-{SCROLLLOCK}, {VK_SPACE}, {VK_LSHIFT}, {VK_PAUSE}, {VK_MODECHANGE},
-{BACK}, {VK_HOME}, {F23}, {F22}, {F21}, {F20}, {VK_HANGEUL}, {VK_KANJI},
-{VK_RIGHT}, {BS}, {HOME}, {VK_F4}, {VK_ACCEPT}, {VK_F18}, {VK_SNAPSHOT},
-{VK_PA1}, {VK_NONAME}, {VK_LCONTROL}, {ZOOM}, {VK_ATTN}, {VK_F10}, {VK_F22},
-{VK_F23}, {VK_F20}, {VK_F21}, {VK_SCROLL}, {TAB}, {VK_F11}, {VK_END},
-{LEFT}, {VK_UP}, {NUMLOCK}, {VK_APPS}, {PGUP}, {VK_F8}, {VK_CONTROL},
-{VK_LEFT}, {PRTSC}, {VK_NUMPAD4}, {CAPSLOCK}, {VK_CONVERT}, {VK_PROCESSKEY},
-{ENTER}, {VK_SEPARATOR}, {VK_RWIN}, {VK_LMENU}, {VK_NEXT}, {F1}, {F2},
-{F3}, {F4}, {F5}, {F6}, {F7}, {F8}, {F9}, {VK_ADD}, {VK_RCONTROL},
-{VK_RETURN}, {BREAK}, {VK_NUMPAD9}, {VK_NUMPAD8}, {RWIN}, {VK_KANA},
-{PGDN}, {VK_NUMPAD3}, {DEL}, {VK_NUMPAD1}, {VK_NUMPAD0}, {VK_NUMPAD7},
-{VK_NUMPAD6}, {VK_NUMPAD5}, {DELETE}, {VK_PRIOR}, {VK_SUBTRACT}, {HELP},
-{VK_PRINT}, {VK_BACK}, {CAP}, {VK_RBUTTON}, {VK_RSHIFT}, {VK_LWIN}, {DOWN},
-{VK_HELP}, {VK_NONCONVERT}, {BACKSPACE}, {VK_SELECT}, {VK_TAB}, {VK_HANJA},
-{VK_NUMPAD2}, {INSERT}, {VK_F9}, {VK_DECIMAL}, {VK_FINAL}, {VK_EXSEL},
-{RMENU}, {VK_F3}, {VK_F2}, {VK_F1}, {VK_F7}, {VK_F6}, {VK_F5}, {VK_CRSEL},
-{VK_SHIFT}, {VK_EREOF}, {VK_CANCEL}, {VK_DELETE}, {VK_HANGUL}, {VK_MBUTTON},
-{VK_NUMLOCK}, {VK_CLEAR}, {END}, {VK_MENU}, {SPACE}, {BKSP}, {VK_INSERT},
-{F18}, {F19}, {ESC}, {VK_MULTIPLY}, {F12}, {F13}, {F10}, {F11}, {F16},
-{F17}, {F14}, {F15}, {F24}, {RIGHT}, {VK_F24}, {VK_CAPITAL}, {VK_LBUTTON},
-{VK_OEM_CLEAR}, {VK_ESCAPE}, {UP}, {VK_DIVIDE}, {INS}, {VK_JUNJA},
-{VK_F19}, {VK_EXECUTE}, {VK_PLAY}, {VK_RMENU}, {VK_F13}, {VK_F12}, {LWIN},
-{VK_DOWN}, {VK_F17}, {VK_F16}, {VK_F15}, {VK_F14}
-
-'+': {VK_SHIFT}
-'^': {VK_CONTROL}
-'%': {VK_MENU} a.k.a. Alt key
-```
-
-
-<h2>Activating windows </h2>
-
-
-
-<table>
-  <tr>
-  </tr>
-</table>
-
-
-
-```python
-# lists all current windows and their hwnds, pid ...
-mkey.get_all_windows()
-
- WindowInfo(pid=24880, title='tooltips_class32', windowtext='', hwnd=38931464, length=1, tid=14156, status='invisible', coords_client=(0, 0, 0, 0), dim_client=(0, 0), coords_win=(0, 0, 0, 0), dim_win=(0, 0), class_name='tooltips_class32', path='C:\\Windows\\explorer.exe'),
- WindowInfo(pid=24916, title='IME', windowtext='Default IME', hwnd=333592, length=12, tid=6716, status='invisible', coords_client=(0, 0, 0, 0), dim_client=(0, 0), coords_win=(0, 0, 0, 0), dim_win=(0, 0), class_name='IME', path='C:\\Windows\\System32\\notepad.exe'),
- WindowInfo(pid=24916, title='IME', windowtext='Default IME', hwnd=1706956, length=12, tid=20004, status='invisible', coords_client=(0, 0, 0, 0), dim_client=(0, 0), coords_win=(0, 0, 0, 0), dim_win=(0, 0), class_name='IME', path='C:\\Windows\\System32\\notepad.exe'),
- WindowInfo(pid=24916, title='MSCTFIME UI', windowtext='MSCTFIME UI', hwnd=35652702, length=12, tid=20004, status='invisible', coords_client=(0, 0, 0, 0), dim_client=(0, 0), coords_win=(0, 0, 0, 0), dim_win=(0, 0), class_name='MSCTFIME UI', path='C:\\Windows\\System32\\notepad.exe'),
- WindowInfo(pid=24916, title='Notepad', windowtext='*Untitled - Notepad', hwnd=10290540, length=20, tid=20004, status='visible', coords_client=(0, 840, 0, 519), dim_client=(840, 519), coords_win=(714, 1570, 196, 774), dim_win=(856, 578), class_name='Notepad', path='C:\\Windows\\System32\\notepad.exe'),
- WindowInfo(pid=24916, title='WorkerW', windowtext='', hwnd=984520, length=1, tid=6716, status='invisible', coords_client=(0, 120, 0, 0), dim_client=(120, 0), coords_win=(0, 136, 0, 39), dim_win=(136, 39), class_name='WorkerW', path='C:\\Windows\\System32\\notepad.exe')]
-
-```
-
-
-
-```python
-# pass and hwnd (code above) as argument.
-mkey.activate_window(10290540) # usually this is enough to activate a window 
-
-#if not, use this method 
-# Activating a window is sometimes tricky. This method forces the activation of the window and works quite often when other methods don't 
-mkey.force_activate_window(17630556) 
-```
-
-
-
-```python
-# Pins a window on top of all others. 
-mkey.activate_topmost(17630556)
-
-# Restore the normal hierarchy. 
-# This method is helpful when one of your windows gets stuck during the automation in the topmost position
-mkey.deactivate_topmost(17630556)
-
-
-```
-
-
-
-```python
-# Some apps hide the cursor, here can you check it 
-mkey.is_cursor_shown ()
-True
-```
-
-
-
-```python
-# Shows you the coordinates of the current cursor position. Press ctrl+l when you have found the right coordinates.
-mkey.start_showing_cursor_position(exit_keys='ctrl+l')
-```
-
-
-
-```python
-mkey.get_single_element_from_coords(200,200)
-
-WindowInfo(parent=-1, pid=20440, title='Edit', windowtext='', hwnd=592576, length=1, tid=17252, status='visible', coords_client=(0, 1903, 0, 1007), dim_client=(1903, 1007), coords_win=(0, 1920, 43, 1050), dim_win=(1920, 1007), class_name='Edit', path='C:\\Windows\\System32\\notepad.exe')
-
-
-
-mkey.get_elements_from_coords(200,200)
-
-{'element': WindowInfo(parent=-1, pid=20440, title='Edit', windowtext='', hwnd=592576, length=1, tid=17252, status='visible', coords_client=(0, 1903, 0, 1007), dim_client=(1903, 1007), coords_win=(0, 1920, 43, 1050), dim_win=(1920, 1007), class_name='Edit', path='C:\\Windows\\System32\\notepad.exe'),
- 'family': [WindowInfo(parent=-1, pid=20440, title='Edit', windowtext='', hwnd=592576, length=1, tid=17252, status='visible', coords_client=(0, 1903, 0, 1007), dim_client=(1903, 1007), coords_win=(0, 1920, 43, 1050), dim_win=(1920, 1007), class_name='Edit', path='C:\\Windows\\System32\\notepad.exe'),
-  WindowInfo(parent=-1, pid=20440, title='Notepad', windowtext='*Untitled - Notepad', hwnd=1051364, length=20, tid=17252, status='visible', coords_client=(0, 1920, 0, 1007), dim_client=(1920, 1007), coords_win=(-8, 1928, -8, 1058), dim_win=(1936, 1066), class_name='Notepad', path='C:\\Windows\\System32\\notepad.exe'),
-  WindowInfo(parent=-1, pid=20440, title='msctls_statusbar32', windowtext='', hwnd=2886324, length=1, tid=17252, status='invisible', coords_client=(0, 484, 0, 23), dim_client=(484, 23), coords_win=(0, 484, 461, 484), dim_win=(484, 23), class_name='msctls_statusbar32', path='C:\\Windows\\System32\\notepad.exe'),
-  WindowInfo(parent=-1, pid=784, title='#32769', windowtext='', hwnd=65552, length=1, tid=984, status='visible', coords_client=(0, 1920, 0, 1080), dim_client=(1920, 1080), coords_win=(0, 1920, 0, 1080), dim_win=(1920, 1080), class_name='#32769', path='')]}
-  
-  
-mkey.get_elements_from_hwnd(2886324)
-
-{'element': WindowInfo(parent=-1, pid=20440, title='msctls_statusbar32', windowtext='', hwnd=2886324, length=1, tid=17252, status='invisible', coords_client=(0, 484, 0, 23), dim_client=(484, 23), coords_win=(0, 484, 461, 484), dim_win=(484, 23), class_name='msctls_statusbar32', path='C:\\Windows\\System32\\notepad.exe'),
- 'family': [WindowInfo(parent=-1, pid=20440, title='Edit', windowtext='', hwnd=592576, length=1, tid=17252, status='visible', coords_client=(0, 1903, 0, 1007), dim_client=(1903, 1007), coords_win=(0, 1920, 43, 1050), dim_win=(1920, 1007), class_name='Edit', path='C:\\Windows\\System32\\notepad.exe'),
-  WindowInfo(parent=-1, pid=20440, title='Notepad', windowtext='*Untitled - Notepad', hwnd=1051364, length=20, tid=17252, status='visible', coords_client=(0, 1920, 0, 1007), dim_client=(1920, 1007), coords_win=(-8, 1928, -8, 1058), dim_win=(1936, 1066), class_name='Notepad', path='C:\\Windows\\System32\\notepad.exe'),
-  WindowInfo(parent=-1, pid=20440, title='msctls_statusbar32', windowtext='', hwnd=2886324, length=1, tid=17252, status='invisible', coords_client=(0, 484, 0, 23), dim_client=(484, 23), coords_win=(0, 484, 461, 484), dim_win=(484, 23), class_name='msctls_statusbar32', path='C:\\Windows\\System32\\notepad.exe'),
-  WindowInfo(parent=-1, pid=784, title='#32769', windowtext='', hwnd=65552, length=1, tid=984, status='visible', coords_client=(0, 1920, 0, 1080), dim_client=(1920, 1080), coords_win=(0, 1920, 0, 1080), dim_win=(1920, 1080), class_name='#32769', path='')]}
-
-
-mkey.get_single_element_from_hwnd(10290540)
-
-Out[18]: WindowInfo(parent=-1, pid=24916, title='Notepad', windowtext='*Untitled - Notepad', hwnd=10290540, length=20, tid=20004, status='visible', coords_client=(0, 840, 0, 519), dim_client=(840, 519), coords_win=(714, 1570, 196, 774), dim_win=(856, 578), class_name='Notepad', path='C:\\Windows\\System32\\notepad.exe')
-```
-
-
-
-```python
-# Gets the rgb values from coordinates and shows the values simultaneously, press ctrl+c when you are done, the method will return a list with all coordinates and colors. 
-rgblist = mkey.show_rgb_values_at_mouse_position(        
-        sleeptime=0.01,
-        on_left_click=False,
-        on_right_click=False,
-        rgb_values=True,
-        rgba_values=True,
-        coords=True,
-        time_value=True,) 
-```
-
-
-
-```python
-# Getting the screen resolution
-mkey.get_screen_resolution()
-(1920, 1080)
-
-mkey.get_active_window()
-WindowInfo(pid=11144, title='SunAwtFrame', windowtext='Python Console - dfdir', hwnd=30283760, length=23, tid=6976, status='visible', coords_client=(0, 1921, 0, 996), dim_client=(1921, 996), coords_win=(2039, 3976, 54, 1058), dim_win=(1937, 1004), class_name='SunAwtFrame', path='C:\\Program Files\\JetBrains\\PyCharm Community Edition 2020.3\\bin\\pycharm64.exe')
-
-mkey.get_cursor_position() # executed only once
-(2436, 994)
-```
-
+<h2>mousekey</h2>
+
+
+
+
+* Works with multi screens
+* Keyboard and mouse can be used in Games like Roblox 
+* Has only a few dependencies (all of them pure python except NumPy)
+* Can simulate human-like mouse movement 
+* Facilitates multi key presses 
+
+
+<h2>Check out the videos</h2>
+<h3>Some methods</h3>
+
+
+<div align="left">
+      <a href="https://www.youtube.com/watch?v=1YugTBZBiyE">
+         <img src="https://img.youtube.com/vi/1YugTBZBiyE/0.jpg" style="width:100%;">
+      </a>
+</div>
+
+<h3>25 minutes of Roblox botting - 900x clicks / 900x keystrokes   </h3>
+
+<div align="left">
+      <a href="https://www.youtube.com/watch?v=OGPoiBnsy1M">
+         <img src="https://img.youtube.com/vi/OGPoiBnsy1M/0.jpg" style="width:100%;">
+      </a>
+</div>
+
+
+
+<h2>Installation</h2>
+
+
+
+```python
+$pip install mousekey
+from mousekey import MouseKey
+mkey = MouseKey()
+
+
+```
+
+
+<h2>Before you start, enable your guardian angel :)   </h2>
+
+
+
+```python
+# Kills the whole process, does always work (even with pure except)
+mkey.enable_failsafekill('ctrl+e')
+
+try:
+    while True:
+        try:
+            print('baba')
+            time.sleep(1)
+        except:
+            pass
+except:
+    pass
+baba
+baba
+baba
+baba
+
+# After pressing ctrl+e:
+Process finished with exit code 1
+```
+
+
+<h2>How to click and move </h2>
+
+
+The click methods should be able to handle any Game
+
+I have tested it with Roblox, which is known for blocking almost everything.
+
+As far as I know, there is no Python module that can handle Roblox [(https://pypi.org/project/ahk/](https://pypi.org/project/ahk/) works, but you need to download ahk.exe) 
+
+<h2>Absolute coordinates</h2>
+
+
+
+```python
+mkey.left_click_xy_natural(
+    200,
+    200,
+    delay=.3, # duration of the mouse click (down - up)
+    min_variation=-3, #  a random value will be added to each pixel  - define the minimum here 
+    max_variation=3,  # a random value will be added to each pixel  - define the maximum here 
+    use_every=4, # use every nth pixel 
+    sleeptime=(0.005, 0.009), # delay between each coordinate
+    print_coords=True, # console output 
+    percent=90, # the lower, the straighter the mouse movement
+) # A logarithm calculation lowers the speed when the cursor is getting close to the destination, like you do it in real life.
+```
+
+
+
+```python
+# Also available: 
+mkey.middle_click_xy_natural
+mkey.right_click_xy_natural
+```
+
+
+
+```python
+# if you don't want to click, only move, use:
+mkey.move_to_natural(100,100) # natural mouse movement
+mkey.move_to(3100,100) = move # no delay 
+```
+
+
+
+```python
+# Moving without delay and clicking:
+mkey.left_click_xy(10,10)
+mkey.right_click_xy(10,10)
+mkey.middle_click_xy(10,10)
+
+#Only clicking:
+mkey.left_click()
+mkey.middle_click()
+mkey.right_click()
+```
+
+
+<h2>Relative coordinates</h2>
+
+
+
+```python
+# For relative coordinates, use: 
+mkey.left_click_xy_natural_relative(
+    50,
+    50,
+    delay=0.1,
+    sleeptime=(0.00005, 0.00009),
+    print_coords=True,
+)
+
+mkey.right_click_xy_natural_relative(
+    x=500,
+    y=500,
+    delay=0.1,
+    sleeptime=(0.00005, 0.00009),
+    print_coords=True,
+)
+```
+
+
+
+```python
+# move and click relatively
+mkey.move_relative
+mkey.middle_click_xy_relative(-100,-100)
+mkey.move_to_natural_relative(300,-400)
+```
+
+
+<h2>Pressing keys</h2>
+
+
+
+```python
+# press a single key
+mkey.force_activate_window(10290540)
+mkey.press_key('f', delay=1) # delay in seconds
+```
+
+
+
+```python
+# You can press as many keys simultaneously as you want. 
+# The first value in each tuple indicates the sleep time before the next key is pressed, and presstime is the delay of the whole action.
+mkey.force_activate_window(10290540)
+mkey.press_keys_simultaneously_own_interval(
+    keystopress=[(0.1, "ctrl"), (0.1, "v")], presstime=.5
+)
+```
+
+
+
+```python
+# This method will calculate the sleep time between each key presses, so you don't have to worry about it. 
+mkey.force_activate_window(10290540)
+mkey.press_keys_simultaneously(
+    keystopress=["alt", "f4", "enter", "enter"],  
+    presstime=1.1,
+    percentofregularpresstime=100,
+)
+```
+
+
+
+```python
+# You can get a list with all available keys here: mkey.show_all_keys
+# I covered different writing styles ('volume_mute', 'VOLUME_MUTE', 'VOLUME MUTE', 'volume mute'), 
+{'control-break processing': 3,
+ 'backspace': 8,
+ 'tab': 9,
+ 'clear': 254,
+ 'enter': 13,
+ 'shift': 16,
+ 'ctrl': 17,
+ 'alt': 18,
+ 'pause': 19,
+ 'caps lock': 20,
+ 'ime hangul mode': 21,
+ 'ime junja mode': 23,
+ 'ime final mode': 24,
+ 'ime kanji mode': 25,
+ 'esc': 27,
+ 'ime convert': 28,
+ 'ime nonconvert': 29,
+ 'ime accept': 30,
+ 'ime mode change request': 31,
+ 'spacebar': 32,
+ 'page up': 33,
+ ...}
+```
+
+
+
+```python
+# You can block the mouse/keyboard input while executing actions.
+# That way, the user can't mess it up. 
+# If something goes wrong, press ctrl+alt+del 
+# This will automatically unlock the mouse/keyboard
+
+# Here is one example. Always use mkey.block_user_input() / mkey.unblock_user_input()
+if mkey.block_user_input():
+    try:
+        for k in range(3):
+            mkey.right_click()
+            sleep(1)
+            mkey.left_click_xy_natural(10, 10)
+            sleep(1)
+    finally:
+        mkey.unblock_user_input()
+```
+
+
+
+
+```python
+# You can send Unicode strings as well
+mkey.force_activate_window(10290540)
+mkey.send_unicode('bababöä')
+```
+
+
+
+```python
+# I have slightly modified 2 methods from pywinauto 
+# Most of the code is from pywinauto, I only changed the way the window gets activated
+mkey.send_keys_to_hwnd(handle=7539468, keys='babadu')
+mkey.send_keystrokes_to_hwnd(handle=7539468, '%{F4}')  # alt+f4
+
+# Here are all keystrokes for those 2 methods:
+https://pywinauto.readthedocs.io/en/latest/code/pywinauto.keyboard.html?highlight=VK_SPACE#pywinauto-keyboard
+
+{SCROLLLOCK}, {VK_SPACE}, {VK_LSHIFT}, {VK_PAUSE}, {VK_MODECHANGE},
+{BACK}, {VK_HOME}, {F23}, {F22}, {F21}, {F20}, {VK_HANGEUL}, {VK_KANJI},
+{VK_RIGHT}, {BS}, {HOME}, {VK_F4}, {VK_ACCEPT}, {VK_F18}, {VK_SNAPSHOT},
+{VK_PA1}, {VK_NONAME}, {VK_LCONTROL}, {ZOOM}, {VK_ATTN}, {VK_F10}, {VK_F22},
+{VK_F23}, {VK_F20}, {VK_F21}, {VK_SCROLL}, {TAB}, {VK_F11}, {VK_END},
+{LEFT}, {VK_UP}, {NUMLOCK}, {VK_APPS}, {PGUP}, {VK_F8}, {VK_CONTROL},
+{VK_LEFT}, {PRTSC}, {VK_NUMPAD4}, {CAPSLOCK}, {VK_CONVERT}, {VK_PROCESSKEY},
+{ENTER}, {VK_SEPARATOR}, {VK_RWIN}, {VK_LMENU}, {VK_NEXT}, {F1}, {F2},
+{F3}, {F4}, {F5}, {F6}, {F7}, {F8}, {F9}, {VK_ADD}, {VK_RCONTROL},
+{VK_RETURN}, {BREAK}, {VK_NUMPAD9}, {VK_NUMPAD8}, {RWIN}, {VK_KANA},
+{PGDN}, {VK_NUMPAD3}, {DEL}, {VK_NUMPAD1}, {VK_NUMPAD0}, {VK_NUMPAD7},
+{VK_NUMPAD6}, {VK_NUMPAD5}, {DELETE}, {VK_PRIOR}, {VK_SUBTRACT}, {HELP},
+{VK_PRINT}, {VK_BACK}, {CAP}, {VK_RBUTTON}, {VK_RSHIFT}, {VK_LWIN}, {DOWN},
+{VK_HELP}, {VK_NONCONVERT}, {BACKSPACE}, {VK_SELECT}, {VK_TAB}, {VK_HANJA},
+{VK_NUMPAD2}, {INSERT}, {VK_F9}, {VK_DECIMAL}, {VK_FINAL}, {VK_EXSEL},
+{RMENU}, {VK_F3}, {VK_F2}, {VK_F1}, {VK_F7}, {VK_F6}, {VK_F5}, {VK_CRSEL},
+{VK_SHIFT}, {VK_EREOF}, {VK_CANCEL}, {VK_DELETE}, {VK_HANGUL}, {VK_MBUTTON},
+{VK_NUMLOCK}, {VK_CLEAR}, {END}, {VK_MENU}, {SPACE}, {BKSP}, {VK_INSERT},
+{F18}, {F19}, {ESC}, {VK_MULTIPLY}, {F12}, {F13}, {F10}, {F11}, {F16},
+{F17}, {F14}, {F15}, {F24}, {RIGHT}, {VK_F24}, {VK_CAPITAL}, {VK_LBUTTON},
+{VK_OEM_CLEAR}, {VK_ESCAPE}, {UP}, {VK_DIVIDE}, {INS}, {VK_JUNJA},
+{VK_F19}, {VK_EXECUTE}, {VK_PLAY}, {VK_RMENU}, {VK_F13}, {VK_F12}, {LWIN},
+{VK_DOWN}, {VK_F17}, {VK_F16}, {VK_F15}, {VK_F14}
+
+'+': {VK_SHIFT}
+'^': {VK_CONTROL}
+'%': {VK_MENU} a.k.a. Alt key
+```
+
+
+<h2>Activating windows </h2>
+
+
+
+<table>
+  <tr>
+  </tr>
+</table>
+
+
+
+```python
+# lists all current windows and their hwnds, pid ...
+mkey.get_all_windows()
+
+ WindowInfo(pid=24880, title='tooltips_class32', windowtext='', hwnd=38931464, length=1, tid=14156, status='invisible', coords_client=(0, 0, 0, 0), dim_client=(0, 0), coords_win=(0, 0, 0, 0), dim_win=(0, 0), class_name='tooltips_class32', path='C:\\Windows\\explorer.exe'),
+ WindowInfo(pid=24916, title='IME', windowtext='Default IME', hwnd=333592, length=12, tid=6716, status='invisible', coords_client=(0, 0, 0, 0), dim_client=(0, 0), coords_win=(0, 0, 0, 0), dim_win=(0, 0), class_name='IME', path='C:\\Windows\\System32\\notepad.exe'),
+ WindowInfo(pid=24916, title='IME', windowtext='Default IME', hwnd=1706956, length=12, tid=20004, status='invisible', coords_client=(0, 0, 0, 0), dim_client=(0, 0), coords_win=(0, 0, 0, 0), dim_win=(0, 0), class_name='IME', path='C:\\Windows\\System32\\notepad.exe'),
+ WindowInfo(pid=24916, title='MSCTFIME UI', windowtext='MSCTFIME UI', hwnd=35652702, length=12, tid=20004, status='invisible', coords_client=(0, 0, 0, 0), dim_client=(0, 0), coords_win=(0, 0, 0, 0), dim_win=(0, 0), class_name='MSCTFIME UI', path='C:\\Windows\\System32\\notepad.exe'),
+ WindowInfo(pid=24916, title='Notepad', windowtext='*Untitled - Notepad', hwnd=10290540, length=20, tid=20004, status='visible', coords_client=(0, 840, 0, 519), dim_client=(840, 519), coords_win=(714, 1570, 196, 774), dim_win=(856, 578), class_name='Notepad', path='C:\\Windows\\System32\\notepad.exe'),
+ WindowInfo(pid=24916, title='WorkerW', windowtext='', hwnd=984520, length=1, tid=6716, status='invisible', coords_client=(0, 120, 0, 0), dim_client=(120, 0), coords_win=(0, 136, 0, 39), dim_win=(136, 39), class_name='WorkerW', path='C:\\Windows\\System32\\notepad.exe')]
+
+```
+
+
+
+```python
+# pass and hwnd (code above) as argument.
+mkey.activate_window(10290540) # usually this is enough to activate a window 
+
+#if not, use this method 
+# Activating a window is sometimes tricky. This method forces the activation of the window and works quite often when other methods don't 
+mkey.force_activate_window(17630556) 
+```
+
+
+
+```python
+# Pins a window on top of all others. 
+mkey.activate_topmost(17630556)
+
+# Restore the normal hierarchy. 
+# This method is helpful when one of your windows gets stuck during the automation in the topmost position
+mkey.deactivate_topmost(17630556)
+
+
+```
+
+
+
+```python
+# Some apps hide the cursor, here can you check it 
+mkey.is_cursor_shown ()
+True
+```
+
+
+
+```python
+# Shows you the coordinates of the current cursor position. Press ctrl+l when you have found the right coordinates.
+mkey.start_showing_cursor_position(exit_keys='ctrl+l')
+```
+
+
+
+```python
+mkey.get_single_element_from_coords(200,200)
+
+WindowInfo(parent=-1, pid=20440, title='Edit', windowtext='', hwnd=592576, length=1, tid=17252, status='visible', coords_client=(0, 1903, 0, 1007), dim_client=(1903, 1007), coords_win=(0, 1920, 43, 1050), dim_win=(1920, 1007), class_name='Edit', path='C:\\Windows\\System32\\notepad.exe')
+
+
+
+mkey.get_elements_from_coords(200,200)
+
+{'element': WindowInfo(parent=-1, pid=20440, title='Edit', windowtext='', hwnd=592576, length=1, tid=17252, status='visible', coords_client=(0, 1903, 0, 1007), dim_client=(1903, 1007), coords_win=(0, 1920, 43, 1050), dim_win=(1920, 1007), class_name='Edit', path='C:\\Windows\\System32\\notepad.exe'),
+ 'family': [WindowInfo(parent=-1, pid=20440, title='Edit', windowtext='', hwnd=592576, length=1, tid=17252, status='visible', coords_client=(0, 1903, 0, 1007), dim_client=(1903, 1007), coords_win=(0, 1920, 43, 1050), dim_win=(1920, 1007), class_name='Edit', path='C:\\Windows\\System32\\notepad.exe'),
+  WindowInfo(parent=-1, pid=20440, title='Notepad', windowtext='*Untitled - Notepad', hwnd=1051364, length=20, tid=17252, status='visible', coords_client=(0, 1920, 0, 1007), dim_client=(1920, 1007), coords_win=(-8, 1928, -8, 1058), dim_win=(1936, 1066), class_name='Notepad', path='C:\\Windows\\System32\\notepad.exe'),
+  WindowInfo(parent=-1, pid=20440, title='msctls_statusbar32', windowtext='', hwnd=2886324, length=1, tid=17252, status='invisible', coords_client=(0, 484, 0, 23), dim_client=(484, 23), coords_win=(0, 484, 461, 484), dim_win=(484, 23), class_name='msctls_statusbar32', path='C:\\Windows\\System32\\notepad.exe'),
+  WindowInfo(parent=-1, pid=784, title='#32769', windowtext='', hwnd=65552, length=1, tid=984, status='visible', coords_client=(0, 1920, 0, 1080), dim_client=(1920, 1080), coords_win=(0, 1920, 0, 1080), dim_win=(1920, 1080), class_name='#32769', path='')]}
+  
+  
+mkey.get_elements_from_hwnd(2886324)
+
+{'element': WindowInfo(parent=-1, pid=20440, title='msctls_statusbar32', windowtext='', hwnd=2886324, length=1, tid=17252, status='invisible', coords_client=(0, 484, 0, 23), dim_client=(484, 23), coords_win=(0, 484, 461, 484), dim_win=(484, 23), class_name='msctls_statusbar32', path='C:\\Windows\\System32\\notepad.exe'),
+ 'family': [WindowInfo(parent=-1, pid=20440, title='Edit', windowtext='', hwnd=592576, length=1, tid=17252, status='visible', coords_client=(0, 1903, 0, 1007), dim_client=(1903, 1007), coords_win=(0, 1920, 43, 1050), dim_win=(1920, 1007), class_name='Edit', path='C:\\Windows\\System32\\notepad.exe'),
+  WindowInfo(parent=-1, pid=20440, title='Notepad', windowtext='*Untitled - Notepad', hwnd=1051364, length=20, tid=17252, status='visible', coords_client=(0, 1920, 0, 1007), dim_client=(1920, 1007), coords_win=(-8, 1928, -8, 1058), dim_win=(1936, 1066), class_name='Notepad', path='C:\\Windows\\System32\\notepad.exe'),
+  WindowInfo(parent=-1, pid=20440, title='msctls_statusbar32', windowtext='', hwnd=2886324, length=1, tid=17252, status='invisible', coords_client=(0, 484, 0, 23), dim_client=(484, 23), coords_win=(0, 484, 461, 484), dim_win=(484, 23), class_name='msctls_statusbar32', path='C:\\Windows\\System32\\notepad.exe'),
+  WindowInfo(parent=-1, pid=784, title='#32769', windowtext='', hwnd=65552, length=1, tid=984, status='visible', coords_client=(0, 1920, 0, 1080), dim_client=(1920, 1080), coords_win=(0, 1920, 0, 1080), dim_win=(1920, 1080), class_name='#32769', path='')]}
+
+
+mkey.get_single_element_from_hwnd(10290540)
+
+Out[18]: WindowInfo(parent=-1, pid=24916, title='Notepad', windowtext='*Untitled - Notepad', hwnd=10290540, length=20, tid=20004, status='visible', coords_client=(0, 840, 0, 519), dim_client=(840, 519), coords_win=(714, 1570, 196, 774), dim_win=(856, 578), class_name='Notepad', path='C:\\Windows\\System32\\notepad.exe')
+```
+
+
+
+```python
+# Gets the rgb values from coordinates and shows the values simultaneously, press ctrl+c when you are done, the method will return a list with all coordinates and colors. 
+rgblist = mkey.show_rgb_values_at_mouse_position(        
+        sleeptime=0.01,
+        on_left_click=False,
+        on_right_click=False,
+        rgb_values=True,
+        rgba_values=True,
+        coords=True,
+        time_value=True,) 
+```
+
+
+
+```python
+# Getting the screen resolution
+mkey.get_screen_resolution()
+(1920, 1080)
+
+mkey.get_active_window()
+WindowInfo(pid=11144, title='SunAwtFrame', windowtext='Python Console - dfdir', hwnd=30283760, length=23, tid=6976, status='visible', coords_client=(0, 1921, 0, 996), dim_client=(1921, 996), coords_win=(2039, 3976, 54, 1058), dim_win=(1937, 1004), class_name='SunAwtFrame', path='C:\\Program Files\\JetBrains\\PyCharm Community Edition 2020.3\\bin\\pycharm64.exe')
+
+mkey.get_cursor_position() # executed only once
+(2436, 994)
+```
+
```

#### html2text {}

```diff
@@ -1,19 +1,16 @@
-Metadata-Version: 2.1 Name: mousekey Version: 0.11 Summary: Automates mouse/
+Metadata-Version: 2.1 Name: mousekey Version: 0.12 Summary: Automates mouse/
 keyboard, works with games like Roblox! Home-page: https://github.com/
 hansalemaos/mousekey Author: Johannes Fischer Author-email:
-gmail.com> License: MIT Keywords: automate,keystroke,mouse,games,pyautogui
-Classifier: Development Status :: 4 - Beta Classifier: Programming Language ::
-Python :: 3 :: Only Classifier: Programming Language :: Python :: 3.9
-Classifier: Topic :: Scientific/Engineering :: Visualization Classifier: Topic
-:: Software Development :: Libraries :: Python Modules Classifier: Topic ::
-Text Editors :: Text Processing Classifier: Topic :: Text Processing :: General
-Classifier: Topic :: Text Processing :: Indexing Classifier: Topic :: Text
-Processing :: Filters Classifier: Topic :: Utilities Description-Content-Type:
-text/markdown License-File: LICENSE.rst
+aulasparticularesdealemaosp@gmail.com License: MIT Keywords:
+automate,keystroke,mouse,games,pyautogui Classifier: Development Status :: 4 -
+Beta Classifier: Programming Language :: Python :: 3 :: Only Classifier:
+Programming Language :: Python :: 3.10 Classifier: Topic :: Software
+Development :: Libraries :: Python Modules Classifier: Topic :: Utilities
+Description-Content-Type: text/markdown License-File: LICENSE.rst
 ***** mousekey *****
 * Works with multi screens * Keyboard and mouse can be used in Games like
 Roblox * Has only a few dependencies (all of them pure python except NumPy) *
 Can simulate human-like mouse movement * Facilitates multi key presses
 ***** Check out the videos *****
 **** Some methods ****
 [https://img.youtube.com/vi/1YugTBZBiyE/0.jpg]
```

