# Comparing `tmp/PlistParser-2023.7.20.1.tar.gz` & `tmp/PlistParser-2023.7.21.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PlistParser-2023.7.20.1.tar", last modified: Thu Jul 20 09:38:02 2023, max compression
+gzip compressed data, was "PlistParser-2023.7.21.0.tar", last modified: Fri Jul 21 02:10:12 2023, max compression
```

## Comparing `PlistParser-2023.7.20.1.tar` & `PlistParser-2023.7.21.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-20 09:38:02.216878 PlistParser-2023.7.20.1/
--rw-rw-rw-   0        0        0     1072 2023-07-11 01:29:42.000000 PlistParser-2023.7.20.1/LICENSE.txt
--rw-rw-rw-   0        0        0     7271 2023-07-20 09:38:02.215878 PlistParser-2023.7.20.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-20 09:38:02.212878 PlistParser-2023.7.20.1/PlistParser/
--rw-rw-rw-   0        0        0      395 2023-07-11 02:07:16.000000 PlistParser-2023.7.20.1/PlistParser/Base64.py
--rw-rw-rw-   0        0        0       47 2023-07-19 15:38:09.000000 PlistParser-2023.7.20.1/PlistParser/Extend.py
--rw-rw-rw-   0        0        0     4431 2023-07-20 09:35:18.000000 PlistParser-2023.7.20.1/PlistParser/Info.py
--rw-rw-rw-   0        0        0    12713 2023-07-19 14:20:41.000000 PlistParser-2023.7.20.1/PlistParser/Plist.py
--rw-rw-rw-   0        0        0    13025 2023-07-19 09:07:22.000000 PlistParser-2023.7.20.1/PlistParser/PlistParser.py
--rw-rw-rw-   0        0        0      181 2023-07-19 14:38:45.000000 PlistParser-2023.7.20.1/PlistParser/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-20 09:38:02.215878 PlistParser-2023.7.20.1/PlistParser.egg-info/
--rw-rw-rw-   0        0        0     7271 2023-07-20 09:38:02.000000 PlistParser-2023.7.20.1/PlistParser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      306 2023-07-20 09:38:02.000000 PlistParser-2023.7.20.1/PlistParser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-20 09:38:02.000000 PlistParser-2023.7.20.1/PlistParser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-07-20 09:38:02.000000 PlistParser-2023.7.20.1/PlistParser.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     6567 2023-07-20 07:38:01.000000 PlistParser-2023.7.20.1/README.md
--rw-rw-rw-   0        0        0       42 2023-07-20 09:38:02.216878 PlistParser-2023.7.20.1/setup.cfg
--rw-rw-rw-   0        0        0     2192 2023-07-20 04:41:37.000000 PlistParser-2023.7.20.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-21 02:10:12.849343 PlistParser-2023.7.21.0/
+-rw-rw-rw-   0        0        0     1072 2023-07-11 01:29:42.000000 PlistParser-2023.7.21.0/LICENSE.txt
+-rw-rw-rw-   0        0        0     7034 2023-07-21 02:10:12.849343 PlistParser-2023.7.21.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-21 02:10:12.844342 PlistParser-2023.7.21.0/PlistParser/
+-rw-rw-rw-   0        0        0      395 2023-07-11 02:07:16.000000 PlistParser-2023.7.21.0/PlistParser/Base64.py
+-rw-rw-rw-   0        0        0       47 2023-07-19 15:38:09.000000 PlistParser-2023.7.21.0/PlistParser/Extend.py
+-rw-rw-rw-   0        0        0     4431 2023-07-21 02:09:57.000000 PlistParser-2023.7.21.0/PlistParser/Info.py
+-rw-rw-rw-   0        0        0    12713 2023-07-19 14:20:41.000000 PlistParser-2023.7.21.0/PlistParser/Plist.py
+-rw-rw-rw-   0        0        0    13025 2023-07-19 09:07:22.000000 PlistParser-2023.7.21.0/PlistParser/PlistParser.py
+-rw-rw-rw-   0        0        0      181 2023-07-19 14:38:45.000000 PlistParser-2023.7.21.0/PlistParser/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 02:10:12.848342 PlistParser-2023.7.21.0/PlistParser.egg-info/
+-rw-rw-rw-   0        0        0     7034 2023-07-21 02:10:12.000000 PlistParser-2023.7.21.0/PlistParser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      306 2023-07-21 02:10:12.000000 PlistParser-2023.7.21.0/PlistParser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-21 02:10:12.000000 PlistParser-2023.7.21.0/PlistParser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-07-21 02:10:12.000000 PlistParser-2023.7.21.0/PlistParser.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     6330 2023-07-21 02:09:09.000000 PlistParser-2023.7.21.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-21 02:10:12.850343 PlistParser-2023.7.21.0/setup.cfg
+-rw-rw-rw-   0        0        0     2192 2023-07-20 04:41:37.000000 PlistParser-2023.7.21.0/setup.py
```

### Comparing `PlistParser-2023.7.20.1/LICENSE.txt` & `PlistParser-2023.7.21.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PlistParser-2023.7.20.1/PKG-INFO` & `PlistParser-2023.7.21.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PlistParser
-Version: 2023.7.20.1
+Version: 2023.7.21.0
 Summary: Extension package for .plist file parsing
 Home-page: https://github.com/whiteEelsYikes/PlistParser
 Author: white-EelsYikes
 Author-email: 2172989337@qq.com
 Keywords: Plist,PlistParser
 Platform: Windows
 Platform: Linux
@@ -33,29 +33,27 @@
 ### 本库 作者实在肝不动 文档这些就随便写写了 大家把 扩展库 安装好后 主要看源代码文件就行了 见谅
 -------------------
 * 🎫 序言
   * ### `📿讨论`
     * ### [`GitHub`](https://github.com/whiteEelsYikes/PlistParser)
     * [`QQ群群号：PlistParser(822515853)`](https://qm.qq.com/cgi-bin/qm/qr?k=8kVUWBck0_zVoOit738kkHSRxW9UU6Ya&jump_from=webapi&authKey=IeeWqgHhgAnLkaeJgKBQxnBG+A7gb0C3ZjKLM2/6tsDzMz2rbuieSNmMaQzI3mo+) <a target="_blank" href="https://qm.qq.com/cgi-bin/qm/qr?k=8kVUWBck0_zVoOit738kkHSRxW9UU6Ya&jump_from=webapi&authKey=IeeWqgHhgAnLkaeJgKBQxnBG+A7gb0C3ZjKLM2/6tsDzMz2rbuieSNmMaQzI3mo+"><img border="0" src="//pub.idqqimg.com/wpa/images/group.png" alt="PlistParser" title="PlistParser"></a>
   * ## `贡献名单`
-      * `white-EelsYikes`: 邮箱2:<a target="_blank" href="http://mail.qq.com/cgi-bin/qm_share?t=qm_mailme&email=L1hHRltKAkpKQ1xWRkRKXG9eXgFMQEI" style="text-decoration:none;"><img src="http://rescdn.qqmail.com/zh_CN/htmledition/images/function/qm_open/ico_mailme_21.png"/></a> |邮箱2:<a target="_blank" href="http://mail.qq.com/cgi-bin/qm_share?t=qm_mailme&email=TjkmJzorYysrIg4-P2AtISM" style="text-decoration:none;"><img src="http://rescdn.qqmail.com/zh_CN/htmledition/images/function/qm_open/ico_mailme_21.png"/></a>
+      * `white-EelsYikes`: 邮箱1:<a target="_blank" href="http://mail.qq.com/cgi-bin/qm_share?t=qm_mailme&email=L1hHRltKAkpKQ1xWRkRKXG9eXgFMQEI" style="text-decoration:none;"><img src="http://rescdn.qqmail.com/zh_CN/htmledition/images/function/qm_open/ico_mailme_21.png"/></a> |邮箱2: <a target="_blank" href="http://mail.qq.com/cgi-bin/qm_share?t=qm_mailme&email=TjkmJzorYysrIg4-P2AtISM" style="text-decoration:none;"><img src="http://rescdn.qqmail.com/zh_CN/htmledition/images/function/qm_open/ico_mailme_21.png"/></a>
   * ## `赞助名单`
       * `pass`
   
 * 📖 前言
   * #### [`点击查看 GitHub README`](https://github.com/whiteEelsYikes/PlistParser/blob/main/README.md)
   * `停` `实际我并不会用 GitHub 至少写这个文档时不会 有考虑学习 但是我的GitHub会很乱 见谅`
-  * 其实作者甚至不只是 `GitHub` 不会用 `pypi`和`py` 也不是特别会用 如果有什么问题 请多包涵 `谢谢`
-  * 当前该扩展库主要 参考 [`PyPi`](https://pypi.org/project/PlistParser/) 说的即可
   * 本py扩展程序包主要提供了py操作.plist xml 文件的 功能 `特别是对于苹果的 .plist xml 配置文件`
   * 本py扩展程序包将秉承着 `简单` `易用` `轻量` `高扩展` `高自定义` 以及 `高自由度` 来构建程序
   * 程序作者并不从事 .plist 有关职业 比如 `ios开发` `ios软件开发` `ios刷机` `ios检测` 等等 所有该程序不会完全完善(其实连帮忙测bug的人都没有😂)所以本程序可能有一定`BUG`或者不太完善的地方
   * emm 请多多指教 如果有好的想法或者`BUG`等需要反馈的 欢迎 
   * ##### `谢谢(Thank you)`
-  * 关于集成 .pyd .c .cpp cython 声明:
+  * 关于集成 .pyd .c .cpp cython声明:
     * `因为一些原因 可以下载 PlistParser 源代码来按需要自行使用 Cython 编译 .pyd .c .cpp 扩展`
 
 * 🫳 获取 安装 方法
   * [`PyPi`](https://pypi.org/project/PlistParser/)
   * [`GitHub`](https://github.com/whiteEelsYikes/PlistParser)
   * python pip 安装最新版
     * ``python -m pip install PlistParser``
@@ -65,51 +63,51 @@
     * 打开 PyShell 然后执行以下代码验证安装
     * ```python
       from PlistParser import Info
       print('版本:',Info.__version__)
       print(Info.__license__)
       Info.open_project_link()
       ```
-  * 🔖 [`PyPi`](https://pypi.org/project/PlistParser/) 与 [`GitHub`](https://github.com/whiteEelsYikes/PlistParser) 可能存在不同步或者一定差异等情况 主要以 [`PyPi`](https://pypi.org/project/PlistParser/) 为标准
+  * 🔖 [`PyPi`](https://pypi.org/project/PlistParser/) 与 [`GitHub`](https://github.com/whiteEelsYikes/PlistParser) 可能存在不同步或者一定差异等情况 主要以 [`GitHub`](https://github.com/whiteEelsYikes/PlistParser) 为标准
 
 * 🪛🔧 使用方法
   * 🔖 本扩展库为 扩展类型库 所以可能存在很多功能和扩展性 这里 作者提示 
   * 文档教程
     * [`GitHub 文档集`](https://github.com/whiteEelsYikes/PlistParser/tree/main/PlistParser.doc-info) 
     * 在[`PyPi`](https://pypi.org/project/PlistParser/)下载项目压缩包 其中可以找到`PlistParser.doc-info`与`PlistParser.test-s`他们分别保存了项目构建时保留的教程文档以及测试调试文件 可以参考 这里提供下载
     * 🔖 如果您的电脑没有解压软件 我们也推荐了解压程序[`360zip`](http://360yasuo.cn/) 您也可以在[`PyPi`](https://pypi.org/project/PlistParser/)找到该程序 我们也提供下载
-  * 🧑‍💻 关于API
+  * 🧑‍💻 关于`API`
     * 相关库导入
       ```python
       from PlistParser import PlistParser  # .plist 解析器 引擎 提供 主要算法和解析转译支持
       from PlistParser import Plist  # .plist 解析辅助定位器 同时支持 py基本的plist文件定义
       from PlistParser import Base64  # .plist 解析器 base64 加解密 辅助库
       
       from PlistParser import Extend  # .plist 解析器 扩展函数库
       from PlistParser import Info  # .plist 解析器 相关信息
       ```
-    * 相关库的API(接口)
+    * 相关库的`API`(接口)
       * [`GitHub 文档集`](https://github.com/whiteEelsYikes/PlistParser/tree/main/PlistParser.doc-info)
       * 在[`PyPi`](https://pypi.org/project/PlistParser/)下载项目压缩包 其中可以找到`PlistParser.doc-info`与`PlistParser.test-s`他们分别保存了项目构建时保留的教程文档以及测试调试文件 可以参考 这里提供下载
     * 最后
-       * Extend.py库 Info.py库 DisplaceTemplate包
+       * Extend.py库 Info.py库
        * `Extend` `Info` 这两个库/包 可以不用管 因为是预留的 哪怕里面有 `内容` `功能` 实现 哪大概率您也用不到
   * 🛠️ 实例
     * 功能实例
       * 解析一个plist文件
         * `pass`
     * 测试实例
       * 参考项目源码压缩包中的 `PlistParser.test-s` 或 `PlistParser.doc-info` 目录
   * 扩展
     * 基础设计扩展
       * `pass`
     * 高级设计扩展
       * `pass`
     * 🔖 本扩展程序皆可 `继承` `重写` 或者 `修改/补充源代码` 等方式实现 功能的扩展等 使该扩展库更符合 `需求`
-    * 🔖🔖 好了 最后有问题欢迎 `[`GitHub`](https://github.com/whiteEelsYikes/PlistParser)` [`QQ群`](https://qm.qq.com/cgi-bin/qm/qr?k=8kVUWBck0_zVoOit738kkHSRxW9UU6Ya&jump_from=webapi&authKey=IeeWqgHhgAnLkaeJgKBQxnBG+A7gb0C3ZjKLM2/6tsDzMz2rbuieSNmMaQzI3mo+) 讨论 供电功能和用法  等待您来发掘 (`文档写不动了 太肝了`)  
+    * 🔖🔖 好了 最后有问题欢迎 [`GitHub`](https://github.com/whiteEelsYikes/PlistParser)  [`QQ群`](https://qm.qq.com/cgi-bin/qm/qr?k=8kVUWBck0_zVoOit738kkHSRxW9UU6Ya&jump_from=webapi&authKey=IeeWqgHhgAnLkaeJgKBQxnBG+A7gb0C3ZjKLM2/6tsDzMz2rbuieSNmMaQzI3mo+) 讨论 供电功能和用法  等待您来发掘 (`文档写不动了 太肝了`)  
 
 * 总结最后
   * ## `拜拜`
 
 # `完...`
```

### Comparing `PlistParser-2023.7.20.1/PlistParser/Info.py` & `PlistParser-2023.7.21.0/PlistParser/Info.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 
 
-__version__ = '2023.7.20.1'
+__version__ = '2023.7.21.0'
 
 __build_peoples__ = {
     r'white-EelsYikes': '2172989337@qq.com',
 }
 
 __license_body__ = \
     """
```

### Comparing `PlistParser-2023.7.20.1/PlistParser/Plist.py` & `PlistParser-2023.7.21.0/PlistParser/Plist.py`

 * *Files identical despite different names*

### Comparing `PlistParser-2023.7.20.1/PlistParser/PlistParser.py` & `PlistParser-2023.7.21.0/PlistParser/PlistParser.py`

 * *Files identical despite different names*

### Comparing `PlistParser-2023.7.20.1/PlistParser.egg-info/PKG-INFO` & `PlistParser-2023.7.21.0/PlistParser.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PlistParser
-Version: 2023.7.20.1
+Version: 2023.7.21.0
 Summary: Extension package for .plist file parsing
 Home-page: https://github.com/whiteEelsYikes/PlistParser
 Author: white-EelsYikes
 Author-email: 2172989337@qq.com
 Keywords: Plist,PlistParser
 Platform: Windows
 Platform: Linux
@@ -33,29 +33,27 @@
 ### 本库 作者实在肝不动 文档这些就随便写写了 大家把 扩展库 安装好后 主要看源代码文件就行了 见谅
 -------------------
 * 🎫 序言
   * ### `📿讨论`
     * ### [`GitHub`](https://github.com/whiteEelsYikes/PlistParser)
     * [`QQ群群号：PlistParser(822515853)`](https://qm.qq.com/cgi-bin/qm/qr?k=8kVUWBck0_zVoOit738kkHSRxW9UU6Ya&jump_from=webapi&authKey=IeeWqgHhgAnLkaeJgKBQxnBG+A7gb0C3ZjKLM2/6tsDzMz2rbuieSNmMaQzI3mo+) <a target="_blank" href="https://qm.qq.com/cgi-bin/qm/qr?k=8kVUWBck0_zVoOit738kkHSRxW9UU6Ya&jump_from=webapi&authKey=IeeWqgHhgAnLkaeJgKBQxnBG+A7gb0C3ZjKLM2/6tsDzMz2rbuieSNmMaQzI3mo+"><img border="0" src="//pub.idqqimg.com/wpa/images/group.png" alt="PlistParser" title="PlistParser"></a>
   * ## `贡献名单`
-      * `white-EelsYikes`: 邮箱2:<a target="_blank" href="http://mail.qq.com/cgi-bin/qm_share?t=qm_mailme&email=L1hHRltKAkpKQ1xWRkRKXG9eXgFMQEI" style="text-decoration:none;"><img src="http://rescdn.qqmail.com/zh_CN/htmledition/images/function/qm_open/ico_mailme_21.png"/></a> |邮箱2:<a target="_blank" href="http://mail.qq.com/cgi-bin/qm_share?t=qm_mailme&email=TjkmJzorYysrIg4-P2AtISM" style="text-decoration:none;"><img src="http://rescdn.qqmail.com/zh_CN/htmledition/images/function/qm_open/ico_mailme_21.png"/></a>
+      * `white-EelsYikes`: 邮箱1:<a target="_blank" href="http://mail.qq.com/cgi-bin/qm_share?t=qm_mailme&email=L1hHRltKAkpKQ1xWRkRKXG9eXgFMQEI" style="text-decoration:none;"><img src="http://rescdn.qqmail.com/zh_CN/htmledition/images/function/qm_open/ico_mailme_21.png"/></a> |邮箱2: <a target="_blank" href="http://mail.qq.com/cgi-bin/qm_share?t=qm_mailme&email=TjkmJzorYysrIg4-P2AtISM" style="text-decoration:none;"><img src="http://rescdn.qqmail.com/zh_CN/htmledition/images/function/qm_open/ico_mailme_21.png"/></a>
   * ## `赞助名单`
       * `pass`
   
 * 📖 前言
   * #### [`点击查看 GitHub README`](https://github.com/whiteEelsYikes/PlistParser/blob/main/README.md)
   * `停` `实际我并不会用 GitHub 至少写这个文档时不会 有考虑学习 但是我的GitHub会很乱 见谅`
-  * 其实作者甚至不只是 `GitHub` 不会用 `pypi`和`py` 也不是特别会用 如果有什么问题 请多包涵 `谢谢`
-  * 当前该扩展库主要 参考 [`PyPi`](https://pypi.org/project/PlistParser/) 说的即可
   * 本py扩展程序包主要提供了py操作.plist xml 文件的 功能 `特别是对于苹果的 .plist xml 配置文件`
   * 本py扩展程序包将秉承着 `简单` `易用` `轻量` `高扩展` `高自定义` 以及 `高自由度` 来构建程序
   * 程序作者并不从事 .plist 有关职业 比如 `ios开发` `ios软件开发` `ios刷机` `ios检测` 等等 所有该程序不会完全完善(其实连帮忙测bug的人都没有😂)所以本程序可能有一定`BUG`或者不太完善的地方
   * emm 请多多指教 如果有好的想法或者`BUG`等需要反馈的 欢迎 
   * ##### `谢谢(Thank you)`
-  * 关于集成 .pyd .c .cpp cython 声明:
+  * 关于集成 .pyd .c .cpp cython声明:
     * `因为一些原因 可以下载 PlistParser 源代码来按需要自行使用 Cython 编译 .pyd .c .cpp 扩展`
 
 * 🫳 获取 安装 方法
   * [`PyPi`](https://pypi.org/project/PlistParser/)
   * [`GitHub`](https://github.com/whiteEelsYikes/PlistParser)
   * python pip 安装最新版
     * ``python -m pip install PlistParser``
@@ -65,51 +63,51 @@
     * 打开 PyShell 然后执行以下代码验证安装
     * ```python
       from PlistParser import Info
       print('版本:',Info.__version__)
       print(Info.__license__)
       Info.open_project_link()
       ```
-  * 🔖 [`PyPi`](https://pypi.org/project/PlistParser/) 与 [`GitHub`](https://github.com/whiteEelsYikes/PlistParser) 可能存在不同步或者一定差异等情况 主要以 [`PyPi`](https://pypi.org/project/PlistParser/) 为标准
+  * 🔖 [`PyPi`](https://pypi.org/project/PlistParser/) 与 [`GitHub`](https://github.com/whiteEelsYikes/PlistParser) 可能存在不同步或者一定差异等情况 主要以 [`GitHub`](https://github.com/whiteEelsYikes/PlistParser) 为标准
 
 * 🪛🔧 使用方法
   * 🔖 本扩展库为 扩展类型库 所以可能存在很多功能和扩展性 这里 作者提示 
   * 文档教程
     * [`GitHub 文档集`](https://github.com/whiteEelsYikes/PlistParser/tree/main/PlistParser.doc-info) 
     * 在[`PyPi`](https://pypi.org/project/PlistParser/)下载项目压缩包 其中可以找到`PlistParser.doc-info`与`PlistParser.test-s`他们分别保存了项目构建时保留的教程文档以及测试调试文件 可以参考 这里提供下载
     * 🔖 如果您的电脑没有解压软件 我们也推荐了解压程序[`360zip`](http://360yasuo.cn/) 您也可以在[`PyPi`](https://pypi.org/project/PlistParser/)找到该程序 我们也提供下载
-  * 🧑‍💻 关于API
+  * 🧑‍💻 关于`API`
     * 相关库导入
       ```python
       from PlistParser import PlistParser  # .plist 解析器 引擎 提供 主要算法和解析转译支持
       from PlistParser import Plist  # .plist 解析辅助定位器 同时支持 py基本的plist文件定义
       from PlistParser import Base64  # .plist 解析器 base64 加解密 辅助库
       
       from PlistParser import Extend  # .plist 解析器 扩展函数库
       from PlistParser import Info  # .plist 解析器 相关信息
       ```
-    * 相关库的API(接口)
+    * 相关库的`API`(接口)
       * [`GitHub 文档集`](https://github.com/whiteEelsYikes/PlistParser/tree/main/PlistParser.doc-info)
       * 在[`PyPi`](https://pypi.org/project/PlistParser/)下载项目压缩包 其中可以找到`PlistParser.doc-info`与`PlistParser.test-s`他们分别保存了项目构建时保留的教程文档以及测试调试文件 可以参考 这里提供下载
     * 最后
-       * Extend.py库 Info.py库 DisplaceTemplate包
+       * Extend.py库 Info.py库
        * `Extend` `Info` 这两个库/包 可以不用管 因为是预留的 哪怕里面有 `内容` `功能` 实现 哪大概率您也用不到
   * 🛠️ 实例
     * 功能实例
       * 解析一个plist文件
         * `pass`
     * 测试实例
       * 参考项目源码压缩包中的 `PlistParser.test-s` 或 `PlistParser.doc-info` 目录
   * 扩展
     * 基础设计扩展
       * `pass`
     * 高级设计扩展
       * `pass`
     * 🔖 本扩展程序皆可 `继承` `重写` 或者 `修改/补充源代码` 等方式实现 功能的扩展等 使该扩展库更符合 `需求`
-    * 🔖🔖 好了 最后有问题欢迎 `[`GitHub`](https://github.com/whiteEelsYikes/PlistParser)` [`QQ群`](https://qm.qq.com/cgi-bin/qm/qr?k=8kVUWBck0_zVoOit738kkHSRxW9UU6Ya&jump_from=webapi&authKey=IeeWqgHhgAnLkaeJgKBQxnBG+A7gb0C3ZjKLM2/6tsDzMz2rbuieSNmMaQzI3mo+) 讨论 供电功能和用法  等待您来发掘 (`文档写不动了 太肝了`)  
+    * 🔖🔖 好了 最后有问题欢迎 [`GitHub`](https://github.com/whiteEelsYikes/PlistParser)  [`QQ群`](https://qm.qq.com/cgi-bin/qm/qr?k=8kVUWBck0_zVoOit738kkHSRxW9UU6Ya&jump_from=webapi&authKey=IeeWqgHhgAnLkaeJgKBQxnBG+A7gb0C3ZjKLM2/6tsDzMz2rbuieSNmMaQzI3mo+) 讨论 供电功能和用法  等待您来发掘 (`文档写不动了 太肝了`)  
 
 * 总结最后
   * ## `拜拜`
 
 # `完...`
```

### Comparing `PlistParser-2023.7.20.1/README.md` & `PlistParser-2023.7.21.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -12,29 +12,27 @@
 ### 本库 作者实在肝不动 文档这些就随便写写了 大家把 扩展库 安装好后 主要看源代码文件就行了 见谅
 -------------------
 * 🎫 序言
   * ### `📿讨论`
     * ### [`GitHub`](https://github.com/whiteEelsYikes/PlistParser)
     * [`QQ群群号：PlistParser(822515853)`](https://qm.qq.com/cgi-bin/qm/qr?k=8kVUWBck0_zVoOit738kkHSRxW9UU6Ya&jump_from=webapi&authKey=IeeWqgHhgAnLkaeJgKBQxnBG+A7gb0C3ZjKLM2/6tsDzMz2rbuieSNmMaQzI3mo+) <a target="_blank" href="https://qm.qq.com/cgi-bin/qm/qr?k=8kVUWBck0_zVoOit738kkHSRxW9UU6Ya&jump_from=webapi&authKey=IeeWqgHhgAnLkaeJgKBQxnBG+A7gb0C3ZjKLM2/6tsDzMz2rbuieSNmMaQzI3mo+"><img border="0" src="//pub.idqqimg.com/wpa/images/group.png" alt="PlistParser" title="PlistParser"></a>
   * ## `贡献名单`
-      * `white-EelsYikes`: 邮箱2:<a target="_blank" href="http://mail.qq.com/cgi-bin/qm_share?t=qm_mailme&email=L1hHRltKAkpKQ1xWRkRKXG9eXgFMQEI" style="text-decoration:none;"><img src="http://rescdn.qqmail.com/zh_CN/htmledition/images/function/qm_open/ico_mailme_21.png"/></a> |邮箱2:<a target="_blank" href="http://mail.qq.com/cgi-bin/qm_share?t=qm_mailme&email=TjkmJzorYysrIg4-P2AtISM" style="text-decoration:none;"><img src="http://rescdn.qqmail.com/zh_CN/htmledition/images/function/qm_open/ico_mailme_21.png"/></a>
+      * `white-EelsYikes`: 邮箱1:<a target="_blank" href="http://mail.qq.com/cgi-bin/qm_share?t=qm_mailme&email=L1hHRltKAkpKQ1xWRkRKXG9eXgFMQEI" style="text-decoration:none;"><img src="http://rescdn.qqmail.com/zh_CN/htmledition/images/function/qm_open/ico_mailme_21.png"/></a> |邮箱2: <a target="_blank" href="http://mail.qq.com/cgi-bin/qm_share?t=qm_mailme&email=TjkmJzorYysrIg4-P2AtISM" style="text-decoration:none;"><img src="http://rescdn.qqmail.com/zh_CN/htmledition/images/function/qm_open/ico_mailme_21.png"/></a>
   * ## `赞助名单`
       * `pass`
   
 * 📖 前言
   * #### [`点击查看 GitHub README`](https://github.com/whiteEelsYikes/PlistParser/blob/main/README.md)
   * `停` `实际我并不会用 GitHub 至少写这个文档时不会 有考虑学习 但是我的GitHub会很乱 见谅`
-  * 其实作者甚至不只是 `GitHub` 不会用 `pypi`和`py` 也不是特别会用 如果有什么问题 请多包涵 `谢谢`
-  * 当前该扩展库主要 参考 [`PyPi`](https://pypi.org/project/PlistParser/) 说的即可
   * 本py扩展程序包主要提供了py操作.plist xml 文件的 功能 `特别是对于苹果的 .plist xml 配置文件`
   * 本py扩展程序包将秉承着 `简单` `易用` `轻量` `高扩展` `高自定义` 以及 `高自由度` 来构建程序
   * 程序作者并不从事 .plist 有关职业 比如 `ios开发` `ios软件开发` `ios刷机` `ios检测` 等等 所有该程序不会完全完善(其实连帮忙测bug的人都没有😂)所以本程序可能有一定`BUG`或者不太完善的地方
   * emm 请多多指教 如果有好的想法或者`BUG`等需要反馈的 欢迎 
   * ##### `谢谢(Thank you)`
-  * 关于集成 .pyd .c .cpp cython 声明:
+  * 关于集成 .pyd .c .cpp cython声明:
     * `因为一些原因 可以下载 PlistParser 源代码来按需要自行使用 Cython 编译 .pyd .c .cpp 扩展`
 
 * 🫳 获取 安装 方法
   * [`PyPi`](https://pypi.org/project/PlistParser/)
   * [`GitHub`](https://github.com/whiteEelsYikes/PlistParser)
   * python pip 安装最新版
     * ``python -m pip install PlistParser``
@@ -44,51 +42,51 @@
     * 打开 PyShell 然后执行以下代码验证安装
     * ```python
       from PlistParser import Info
       print('版本:',Info.__version__)
       print(Info.__license__)
       Info.open_project_link()
       ```
-  * 🔖 [`PyPi`](https://pypi.org/project/PlistParser/) 与 [`GitHub`](https://github.com/whiteEelsYikes/PlistParser) 可能存在不同步或者一定差异等情况 主要以 [`PyPi`](https://pypi.org/project/PlistParser/) 为标准
+  * 🔖 [`PyPi`](https://pypi.org/project/PlistParser/) 与 [`GitHub`](https://github.com/whiteEelsYikes/PlistParser) 可能存在不同步或者一定差异等情况 主要以 [`GitHub`](https://github.com/whiteEelsYikes/PlistParser) 为标准
 
 * 🪛🔧 使用方法
   * 🔖 本扩展库为 扩展类型库 所以可能存在很多功能和扩展性 这里 作者提示 
   * 文档教程
     * [`GitHub 文档集`](https://github.com/whiteEelsYikes/PlistParser/tree/main/PlistParser.doc-info) 
     * 在[`PyPi`](https://pypi.org/project/PlistParser/)下载项目压缩包 其中可以找到`PlistParser.doc-info`与`PlistParser.test-s`他们分别保存了项目构建时保留的教程文档以及测试调试文件 可以参考 这里提供下载
     * 🔖 如果您的电脑没有解压软件 我们也推荐了解压程序[`360zip`](http://360yasuo.cn/) 您也可以在[`PyPi`](https://pypi.org/project/PlistParser/)找到该程序 我们也提供下载
-  * 🧑‍💻 关于API
+  * 🧑‍💻 关于`API`
     * 相关库导入
       ```python
       from PlistParser import PlistParser  # .plist 解析器 引擎 提供 主要算法和解析转译支持
       from PlistParser import Plist  # .plist 解析辅助定位器 同时支持 py基本的plist文件定义
       from PlistParser import Base64  # .plist 解析器 base64 加解密 辅助库
       
       from PlistParser import Extend  # .plist 解析器 扩展函数库
       from PlistParser import Info  # .plist 解析器 相关信息
       ```
-    * 相关库的API(接口)
+    * 相关库的`API`(接口)
       * [`GitHub 文档集`](https://github.com/whiteEelsYikes/PlistParser/tree/main/PlistParser.doc-info)
       * 在[`PyPi`](https://pypi.org/project/PlistParser/)下载项目压缩包 其中可以找到`PlistParser.doc-info`与`PlistParser.test-s`他们分别保存了项目构建时保留的教程文档以及测试调试文件 可以参考 这里提供下载
     * 最后
-       * Extend.py库 Info.py库 DisplaceTemplate包
+       * Extend.py库 Info.py库
        * `Extend` `Info` 这两个库/包 可以不用管 因为是预留的 哪怕里面有 `内容` `功能` 实现 哪大概率您也用不到
   * 🛠️ 实例
     * 功能实例
       * 解析一个plist文件
         * `pass`
     * 测试实例
       * 参考项目源码压缩包中的 `PlistParser.test-s` 或 `PlistParser.doc-info` 目录
   * 扩展
     * 基础设计扩展
       * `pass`
     * 高级设计扩展
       * `pass`
     * 🔖 本扩展程序皆可 `继承` `重写` 或者 `修改/补充源代码` 等方式实现 功能的扩展等 使该扩展库更符合 `需求`
-    * 🔖🔖 好了 最后有问题欢迎 `[`GitHub`](https://github.com/whiteEelsYikes/PlistParser)` [`QQ群`](https://qm.qq.com/cgi-bin/qm/qr?k=8kVUWBck0_zVoOit738kkHSRxW9UU6Ya&jump_from=webapi&authKey=IeeWqgHhgAnLkaeJgKBQxnBG+A7gb0C3ZjKLM2/6tsDzMz2rbuieSNmMaQzI3mo+) 讨论 供电功能和用法  等待您来发掘 (`文档写不动了 太肝了`)  
+    * 🔖🔖 好了 最后有问题欢迎 [`GitHub`](https://github.com/whiteEelsYikes/PlistParser)  [`QQ群`](https://qm.qq.com/cgi-bin/qm/qr?k=8kVUWBck0_zVoOit738kkHSRxW9UU6Ya&jump_from=webapi&authKey=IeeWqgHhgAnLkaeJgKBQxnBG+A7gb0C3ZjKLM2/6tsDzMz2rbuieSNmMaQzI3mo+) 讨论 供电功能和用法  等待您来发掘 (`文档写不动了 太肝了`)  
 
 * 总结最后
   * ## `拜拜`
 
 # `完...`
```

### Comparing `PlistParser-2023.7.20.1/setup.py` & `PlistParser-2023.7.21.0/setup.py`

 * *Files identical despite different names*

