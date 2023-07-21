# Comparing `tmp/WebtoonScraper-1.0.2.tar.gz` & `tmp/WebtoonScraper-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "WebtoonScraper-1.0.2.tar", last modified: Fri Jul  7 14:00:15 2023, max compression
+gzip compressed data, was "WebtoonScraper-1.1.1.tar", last modified: Fri Jul 21 19:36:40 2023, max compression
```

## Comparing `WebtoonScraper-1.0.2.tar` & `WebtoonScraper-1.1.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-07-07 14:00:15.993418 WebtoonScraper-1.0.2/
--rw-rw-rw-   0        0        0     1089 2023-05-15 00:16:47.000000 WebtoonScraper-1.0.2/LICENSE
--rw-rw-rw-   0        0        0       34 2023-06-30 07:37:22.000000 WebtoonScraper-1.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0    12160 2023-07-07 14:00:15.993418 WebtoonScraper-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0    10741 2023-07-07 13:56:07.000000 WebtoonScraper-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-07 14:00:15.977435 WebtoonScraper-1.0.2/WebtoonScraper/
--rw-rw-rw-   0        0        0      645 2023-07-06 10:40:03.000000 WebtoonScraper-1.0.2/WebtoonScraper/BestChallengeScraper.py
--rw-rw-rw-   0        0        0     5726 2023-07-06 10:39:23.000000 WebtoonScraper-1.0.2/WebtoonScraper/BufftoonScraper.py
--rw-rw-rw-   0        0        0    10280 2023-07-07 13:59:29.000000 WebtoonScraper-1.0.2/WebtoonScraper/FolderManager.py
--rw-rw-rw-   0        0        0     3766 2023-07-06 10:39:12.000000 WebtoonScraper-1.0.2/WebtoonScraper/NaverGameScraper.py
--rw-rw-rw-   0        0        0     6756 2023-07-07 13:17:19.000000 WebtoonScraper-1.0.2/WebtoonScraper/NaverPostScraper.py
--rw-rw-rw-   0        0        0     3653 2023-07-06 10:32:59.000000 WebtoonScraper-1.0.2/WebtoonScraper/NaverWebtoonScraper.py
--rw-rw-rw-   0        0        0    16392 2023-07-07 13:56:04.000000 WebtoonScraper-1.0.2/WebtoonScraper/Scraper.py
--rw-rw-rw-   0        0        0     4370 2023-07-06 10:33:22.000000 WebtoonScraper-1.0.2/WebtoonScraper/TelescopeScraper.py
--rw-rw-rw-   0        0        0     9956 2023-07-06 10:35:05.000000 WebtoonScraper-1.0.2/WebtoonScraper/Webtoon.py
--rw-rw-rw-   0        0        0      650 2023-07-06 10:29:39.000000 WebtoonScraper-1.0.2/WebtoonScraper/WebtoonCanvasScraper.py
--rw-rw-rw-   0        0        0     4458 2023-07-06 10:40:46.000000 WebtoonScraper-1.0.2/WebtoonScraper/WebtoonOriginalsScraper.py
--rw-rw-rw-   0        0        0     1124 2023-07-06 08:12:25.000000 WebtoonScraper-1.0.2/WebtoonScraper/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-07 14:00:15.990225 WebtoonScraper-1.0.2/WebtoonScraper.egg-info/
--rw-rw-rw-   0        0        0    12160 2023-07-07 14:00:15.000000 WebtoonScraper-1.0.2/WebtoonScraper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      702 2023-07-07 14:00:15.000000 WebtoonScraper-1.0.2/WebtoonScraper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 14:00:15.000000 WebtoonScraper-1.0.2/WebtoonScraper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-17 14:16:38.000000 WebtoonScraper-1.0.2/WebtoonScraper.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       37 2023-07-07 14:00:15.000000 WebtoonScraper-1.0.2/WebtoonScraper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-07-07 14:00:15.000000 WebtoonScraper-1.0.2/WebtoonScraper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-07 14:00:15.993418 WebtoonScraper-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1433 2023-07-07 13:56:29.000000 WebtoonScraper-1.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-07 14:00:15.992224 WebtoonScraper-1.0.2/test/
--rw-rw-rw-   0        0        0      217 2023-07-06 11:06:58.000000 WebtoonScraper-1.0.2/test/__init__.py
--rw-rw-rw-   0        0        0     1502 2023-07-07 13:23:14.000000 WebtoonScraper-1.0.2/test/test.py
+drwxrwxrwx   0        0        0        0 2023-07-21 19:36:40.375443 WebtoonScraper-1.1.1/
+-rw-rw-rw-   0        0        0     1089 2023-05-15 00:16:47.000000 WebtoonScraper-1.1.1/LICENSE
+-rw-rw-rw-   0        0        0       34 2023-06-30 07:37:22.000000 WebtoonScraper-1.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0    10220 2023-07-21 19:36:40.374442 WebtoonScraper-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     8801 2023-07-21 19:30:49.000000 WebtoonScraper-1.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-21 19:36:40.355785 WebtoonScraper-1.1.1/WebtoonScraper/
+-rw-rw-rw-   0        0        0    10280 2023-07-20 14:17:03.000000 WebtoonScraper-1.1.1/WebtoonScraper/A_FolderManager.py
+-rw-rw-rw-   0        0        0    11211 2023-07-21 19:17:57.000000 WebtoonScraper-1.1.1/WebtoonScraper/B_Webtoon.py
+-rw-rw-rw-   0        0        0    24754 2023-07-21 19:04:45.000000 WebtoonScraper-1.1.1/WebtoonScraper/C_Scraper.py
+-rw-rw-rw-   0        0        0     3942 2023-07-21 13:05:19.000000 WebtoonScraper-1.1.1/WebtoonScraper/D_NaverWebtoonScraper.py
+-rw-rw-rw-   0        0        0      644 2023-07-21 11:20:47.000000 WebtoonScraper-1.1.1/WebtoonScraper/E_BestChallengeScraper.py
+-rw-rw-rw-   0        0        0     4785 2023-07-21 13:08:33.000000 WebtoonScraper-1.1.1/WebtoonScraper/F_WebtoonOriginalsScraper.py
+-rw-rw-rw-   0        0        0      640 2023-07-21 12:02:11.000000 WebtoonScraper-1.1.1/WebtoonScraper/G_WebtoonCanvasScraper.py
+-rw-rw-rw-   0        0        0     3964 2023-07-21 19:05:52.000000 WebtoonScraper-1.1.1/WebtoonScraper/H_TelescopeScraper.py
+-rw-rw-rw-   0        0        0     5689 2023-07-21 13:10:21.000000 WebtoonScraper-1.1.1/WebtoonScraper/I_BufftoonScraper.py
+-rw-rw-rw-   0        0        0     6051 2023-07-21 13:19:51.000000 WebtoonScraper-1.1.1/WebtoonScraper/J_NaverPostScraper.py
+-rw-rw-rw-   0        0        0     3451 2023-07-21 13:21:27.000000 WebtoonScraper-1.1.1/WebtoonScraper/K_NaverGameScraper.py
+-rw-rw-rw-   0        0        0     1186 2023-07-21 13:34:50.000000 WebtoonScraper-1.1.1/WebtoonScraper/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 19:36:40.369392 WebtoonScraper-1.1.1/WebtoonScraper.egg-info/
+-rw-rw-rw-   0        0        0    10220 2023-07-21 19:36:40.000000 WebtoonScraper-1.1.1/WebtoonScraper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      724 2023-07-21 19:36:40.000000 WebtoonScraper-1.1.1/WebtoonScraper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-21 19:36:40.000000 WebtoonScraper-1.1.1/WebtoonScraper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-17 14:16:38.000000 WebtoonScraper-1.1.1/WebtoonScraper.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       37 2023-07-21 19:36:40.000000 WebtoonScraper-1.1.1/WebtoonScraper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-07-21 19:36:40.000000 WebtoonScraper-1.1.1/WebtoonScraper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-21 19:36:40.375443 WebtoonScraper-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1433 2023-07-21 14:03:11.000000 WebtoonScraper-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-21 19:36:40.373446 WebtoonScraper-1.1.1/test/
+-rw-rw-rw-   0        0        0      217 2023-07-20 17:15:31.000000 WebtoonScraper-1.1.1/test/__init__.py
+-rw-rw-rw-   0        0        0     1649 2023-07-20 16:42:26.000000 WebtoonScraper-1.1.1/test/test.py
```

### Comparing `WebtoonScraper-1.0.2/LICENSE` & `WebtoonScraper-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `WebtoonScraper-1.0.2/PKG-INFO` & `WebtoonScraper-1.1.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WebtoonScraper
-Version: 1.0.2
+Version: 1.1.1
 Summary: Scraping webtoons and some utils for it
 Home-page: https://github.com/ilotoki0804/WebtoonScraper
 Author: ilotoki0804
 Author-email: ilotoki0804@gmail.com
 License: MIT
 Keywords: Webtoon,Webtoon Scraper,Naver Webtoon,Webtoon Downloader,Download Webtoon
 Classifier: License :: OSI Approved :: MIT License
@@ -31,46 +31,60 @@
    ```
 
 # 네이버 웹툰, 베스트 도전만화, 웹툰 오리지널, 웹툰 캔버스, 만화경, 네이버 게임 다운로드하기
 
 버프툰과 네이버 포스트는 아래로 가서 확인하세요.
 
 1. 원하는 웹툰으로 가서 titleid 또는 title_no를 복사하세요.
+   네이버 웹툰/베스트 도전(comic.naver.com):
    ![img](https://raw.githubusercontent.com/ilotoki0804/WebtoonScraper/master/images/naver_webtoon.png)
-   네이버 웹툰과 베스트 도전의 경우 여기에서,
+   웹툰 오리지널/캔버스(webtoons.com):
    ![img](https://raw.githubusercontent.com/ilotoki0804/WebtoonScraper/master/images/webtoons_original.png)
-   웹툰 오리지널과 캔버스의 경우는 여기에서,
+   만화경(manhwakyung.com)
    ![img](https://raw.githubusercontent.com/ilotoki0804/WebtoonScraper/master/images/manhwakyung.png)
-   만화경의 경우는 여기에서,
+   네이버 게임 오리지널 시리즈(game.naver.com/original_series):
    ![img](https://raw.githubusercontent.com/ilotoki0804/WebtoonScraper/master/images/naver_game.png)
-   네이버 게임 오리지널 시리즈의 경우는 여기에서 확인할 수 있습니다.
+   버프툰과 네이버 포스트는 아래의 '버프툰 다운로드하기'섹션과 '네이버 포스트 다운로드하기' 섹션을 참고해 주세요.
 2. 다음의 파이썬 코드를 웹툰이 다운로드되길 원하는 폴더 내에서 실행해 주세요. 웹툰은 정식 연재와 베스트 도전, Webtoons 오리지널과 캔버스, 만화경, 네이버 게임 모두 가능합니다.
 
    ```python
    from WebtoonScraper import Webtoon as wt
 
    # 네이버 웹툰
-   wt.get_webtoon(76648, wt.N) # titleid를 여기에다 붙여넣으세요.
+   wt.get_webtoon(76648, wt.N)  # titleid를 여기에다 붙여넣으세요.
    # 베스트 도전만화
-   wt.get_webtoon(763952, wt.B) # titleid를 여기에다 붙여넣으세요.
+   wt.get_webtoon(763952, wt.B)  # titleid를 여기에다 붙여넣으세요.  # ! 수정
    # 웹툰 오리지널
-   wt.get_webtoon(1435, wt.O) # titleid를 여기에다 붙여넣으세요.
+   wt.get_webtoon(1435, wt.O)  # title_no를 여기에다 붙여넣으세요.
    # 웹툰 캔버스
-   wt.get_webtoon(304446, wt.C) # titleid를 여기에다 붙여넣으세요.
+   wt.get_webtoon(304446, wt.C)  # title_no를 여기에다 붙여넣으세요.
    # 만화경
-   wt.get_webtoon(146, wt.M) # titleid를 여기에다 붙여넣으세요. Webtoon.T 태그도 사용 가능합니다.
+   wt.get_webtoon(146, wt.M)  # titleid를 여기에다 붙여넣으세요. Webtoon.T 태그도 사용 가능합니다.
    # 네이버 게임 오리지널 시리즈
-   wt.get_webtoon(146, wt.G) # titleid를 여기에다 붙여넣으세요.
+   wt.get_webtoon(5, wt.G)  # titleid를 여기에다 붙여넣으세요.
+   # 버프툰
+   cookie = 'cookie here'  # cookie를 여기에다 붙여넣으세요. 자세한 설명은 아래의 '버프툰 다운로드하기'를 참고하세요.
+   wt.get_webtoon(1007888, wt.BF, cookie=cookie)  # titleid를 여기에다 붙여넣으세요.
+   # 네이버 포스트
+   wt.get_webtoon((597061, 19803452), wt.P)  # seriesNo와 memberNo를 각각 붙여넣으세요. 자세한 설명은 아래의 '네이버 포스트 다운받기'를 참고하세요.
    ```
 
    이제 웹툰이 webtoons 폴더에 다운로드됩니다.
 
    cf. 웹툰 태그를 생략하면 해당 웹툰이 어떤 사이트의 웹툰 id인지 자동으로 알아냅니다. 만약 몇몇 태그가 겹친다면 태그에 맞는 수를 입력하는 창에 알맞은 수를 입력하면 됩니다.
 
-   또 merge 태그를 이용하면 webtoon 폴더 내에 있는 모든 웹툰을 자동으로 5화씩 묶습니다.
+   episode_no_range 키워드를 이용하면 특정한 에피소드만 다운로드받을 수 있습니다.
+   ```python
+   wt.get_webtoon(5, wt.G, episode_no_range=(1,20))  # 1화부터 20화까지
+   ```
+
+   merge 키워드를 이용하면 webtoon 폴더 내에 있는 모든 웹툰을 원하는 개수 만큼 묶습니다.
+   ```python
+   wt.get_webtoon(5, wt.G, merge=5)
+   ```
 3. 만화 뷰어 앱을 통해 다운로드한 웹툰을 시청할 수 있습니다.
 
 ## 주의사항
 
 * 중간에 웹툰 다운로드가 멈춘 듯이 보여도 정상입니다. 그대로 가만히 있으면 다운로드가 다시 진행됩니다.
 * 만약 작동하지 않는다면 윈도우에서 Python 3.11.4을 설치하고 앞의 과정을 반복해 보세요.
 
@@ -81,15 +95,15 @@
 로그인하지 않은 상태에서도 웹툰을 다운로드받을 수 있으나, 받을 수 있는 웹툰 수가 매우 적기에 추천하지 않습니다.
 
 1. 웹툰 페이지에 들어가 주소창의 맨 마지막 수를 복사합니다.
 2. 다음의 파이썬 코드를 웹툰이 다운로드되길 원하는 폴더 내에서 실행해 주세요.
    ```python
    from WebtoonScraper import Webtoon as wt
 
-   wt.get_webtoon(1007888, wt.BF) # 복사했던 수를 여기에다 붙여넣으세요.
+   wt.get_webtoon(1007888, wt.BF)  # 복사했던 수를 여기에다 붙여넣으세요.
    ```
 3. 'Enter cookie of 1007888(시리즈 id) (Enter nothing to preceed without cookie)'라는 문구와 함께 입력란이 나오면 그냥 enter를 눌러줍니다.
 4. 로그인하지 않고 볼 수 있는 모든 에피소드가 다운로드됩니다.
 
 ## 로그인한 상태에서 웹툰 다운로드하기
 
 이 과정은 PC를 기준으로 설명합니다. 만약 모바일이라면 Kiwi Browser 등을 통해 다음의 과정을 수행할 수 있습니다.
@@ -99,69 +113,41 @@
 2. 로그인을 하고 f12를 누르고 네트워크 창을 연 뒤 웹툰 페이지에 들어갑니다.
    ![img](https://raw.githubusercontent.com/ilotoki0804/WebtoonScraper/master/images/bufftoon2.png)
 3. 새로고침을 한 뒤 '이름'에 있는 favicon.ico 요청을 클릭하고 나온 창에 '헤더' 탭을 엽니다.
    ![img](https://raw.githubusercontent.com/ilotoki0804/WebtoonScraper/master/images/bufftoon3.png)
 4. 내려서 Cookie: 라고 되어 있는 모든 내용을 복사합니다.
    ![img](https://raw.githubusercontent.com/ilotoki0804/WebtoonScraper/master/images/bufftoon4.png)
 5. 다음의 파이썬 코드를 웹툰이 다운로드되길 원하는 폴더 내에서 실행해 주세요.
-
-   ```python
-   from WebtoonScraper import Webtoon as wt
-
-   wt.get_webtoon(1007888, wt.BF) # 첫 번째로 복사했던 수를 여기에다 붙여넣으세요.
-   ```
-
-   혹은 다음과 같이 cookie를 코드 내에 포함할 수도 있습니다.
-
    ```python
    from WebtoonScraper import Webtoon as wt
    cookie = '두 번째로 복사했던 문자를 여기에다 붙여넣으세요.'
-   wt.get_webtoon(1007888, wt.BF, cookie=cookie) # 첫 번째로 복사했던 수를 여기에다 붙여넣으세요.
+   wt.get_webtoon(1007888, wt.BF, cookie=cookie)  # 첫 번째로 복사했던 수를 여기에다 붙여넣으세요.
    ```
-
-   1. 'Enter cookie of 1007888(시리즈 id) (Enter nothing to proceed without cookie)'라는 문구와 함께 입력란이 나오면 두 번째로 복사했던 일련의 문자열을 붙여넣기합니다.
 6. 로그인하면 볼 수 있는 모든 에피소드가 다운로드됩니다.
 
 ## 주의사항
 
 * get_webtoon에서 cookie를 입력하면 자동으로 버프툰으로 인식합니다.
 
 # 네이버 포스트 다운로드하기
 
 1. 웹툰이 있는 페이지로 가서 seriesNo와 memberNo를 복사하세요. 예시에서는 각각 597061과 19803452입니다.
    ![img](https://raw.githubusercontent.com/ilotoki0804/WebtoonScraper/master/images/naver_post.png)
 2. 다음의 파이썬 코드를 웹툰이 다운로드되길 원하는 폴더 내에서 실행해 주세요.
-
    ```python
    from WebtoonScraper import Webtoon as wt
 
-   wt.get_webtoon(597061, wt.M) # 우선 seriesNo만 여기에 입력해주세요.
+   wt.get_webtoon((597061, 19803452), wt.P)
    ```
-
-   혹은 memberNo를 코드 내에 포함할 수 있습니다.
-
-   ```python
-   from WebtoonScraper import Webtoon as wt
-
-   wt.get_webtoon(597061, wt.M, member_no=19803452)
-   ```
-3. 'Enter memberNo of 597061(해당 웹툰의 seriesNo)'라는 말과 함께 입력란이 나오면 거기에 아까 복사해 놓은 memberNo를 붙여넣습니다.
-   만약 앞에서 이미 member_no를 사용했다면 이 단계는 건너뛰어집니다.
-
-   ```
-   Enter memberNo  of 597061: 19803452
-   ...진행됨...
-   ```
-4. 만화 뷰어 앱을 통해 다운로드한 웹툰을 시청할 수 있습니다.
+3. 만화 뷰어 앱을 통해 다운로드한 웹툰을 시청할 수 있습니다.
 
 ## 주의사항
 
 * 가끔씩 이유 없는 오류가 발생할 수 있습니다. 그럴 때는 조금 시간이 지난 후에 다시 시도해 보세요.
-* 네이버 포스트는 titleid를 get_webtoon_platform으로 알아낼 수 없습니다.
-* member_no를 입력하면 자동으로 포스트로 인식됩니다.
+* tuple를 입력하면 자동으로 포스트로 인식됩니다.
 
 # 여러 회차 하나로 묶기
 
 1. 웹툰을 상기한 대로 다운로드받습니다.
 2. 다음과 같이 코드를 짭니다.
    ```python
    from WebtoonScraper import FolderManager
@@ -185,31 +171,18 @@
    from WebtoonScraper import FolderManager
 
    fm= FolderManager()
    fm.restore_webtoons_in_directory()
    ```
 3. 'webtoon' 폴더에 있던 모든 웹툰이 웹툰을 처음 다운로드했던 상태로 되돌아갑니다.
 
-# QNA
-
-## 회차 번호 관련
-
-### 문제와 이유
-
-회차가 띄엄띄엄 있거나 설정된 회차 번호가 작가가 설정한 회차 번호와 다르거나 회차 묶기를 사용했는데 묶인 회차 수가 설정한 수보다 더 적은 이유는 다음과 같습니다.
-이 프로젝트에서 웹툰의 회차 번호는 ID를 기준으로 합니다. 이는 작가가 정한 회차와는 다를 수 있습니다. 작가가 프롤로그부터 시작하는 경우(프로젝트의 회차 번호가 하나 빠름), 작가가 리메이크를 해서 전에 있던 작품을 제거해 ID가 연속적으로 있지 않는 경우(주로 베도에서 일어남/회차 번호가 띄엄띄엄하게 있음), 논란이나 작가 실수 등으로 회차가 삭제된 경우(한 회차를 건너띔) 등에서 ID가 불연속적이거나 작품과 일치하기 않는 경우가 생기게 됩니다.
-
-### ID를 회차 번호로 그대로 사용하는 이유
-
-우선 작가가 설정한 회차 번호에 맞추는 것은 힘듭니다. 우선 번호가 어디에 있을지 알기 어렵고, 프롤로그가 있을지 없을지 알 수 없으며, 여러 화에 걸쳐 같은 에피소드를 진행하는 경우도 있고, 외전으로 본편의 회차에서 분리된 화를 운영하는 경우가 있어 화에 맞추어서 번호를 정하는 것을 어렵습니다.
-1부터 시작해서 끝까지 일정한 번호를 유지하는 것도 고려해볼 만하나 만약 그렇게 된다면 무결성 체크를 사용하기 어렵게 됩니다.
-따라서 작가가 설정한 회차를 그대로 사용하는 것도 어렵고, 만약 가능하다 할 지라도 무결성 체크를 포기하기 어렵기 때문에 현재는 ID를 회차 번호로 사용하고 있습니다.
-
 # Relese Note
 
+1.1.1: 내부 모듈 이름 변경, merge option 추가, abstractmethod들의 일반 구현 추가
+
 1.0.2: 대형 리팩토링, get_webtoon_platform 비동기 방식으로 속도 개선, 상대경로로 변경, 테스트 추가
 
 1.0.1: 코드 개선 및 리팩토링, api를 통한 로직으로 변경 (버그가 많기에 사용을 권장하지 않음)
 
 1.0.0: 네이버 게임 추가, FolderManager 리펙토링 및 개선, 정식 버전, docs 개선
 
 0.1.1: 네이버 포스트 추가, readme 작성, pbar 표시 내용 변경, 버그 수정
```

### Comparing `WebtoonScraper-1.0.2/README.md` & `WebtoonScraper-1.1.1/WebtoonScraper.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,25 @@
+Metadata-Version: 2.1
+Name: WebtoonScraper
+Version: 1.1.1
+Summary: Scraping webtoons and some utils for it
+Home-page: https://github.com/ilotoki0804/WebtoonScraper
+Author: ilotoki0804
+Author-email: ilotoki0804@gmail.com
+License: MIT
+Keywords: Webtoon,Webtoon Scraper,Naver Webtoon,Webtoon Downloader,Download Webtoon
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+이 설명은 최신 버전이 아닐 수 있습니다. 만약 최신 버전을 확인하고 싶으시다면 [여기](https://github.com/ilotoki0804/WebtoonScraper)를 참고하세요.
 # WebtoonScraper
 
 웹툰을 다운로드하는 프로젝트입니다.
 
 네이버 웹툰, 베스트 도전만화, 웹툰 오리지널, 웹툰 캔버스, 만화경, 버프툰, 네이버 포스트, 네이버 게임을 지원합니다.
 
 # 시작하기
@@ -13,46 +31,60 @@
    ```
 
 # 네이버 웹툰, 베스트 도전만화, 웹툰 오리지널, 웹툰 캔버스, 만화경, 네이버 게임 다운로드하기
 
 버프툰과 네이버 포스트는 아래로 가서 확인하세요.
 
 1. 원하는 웹툰으로 가서 titleid 또는 title_no를 복사하세요.
-   ![img](images/naver_webtoon.png)
-   네이버 웹툰과 베스트 도전의 경우 여기에서,
-   ![img](images/webtoons_original.png)
-   웹툰 오리지널과 캔버스의 경우는 여기에서,
-   ![img](images/manhwakyung.png)
-   만화경의 경우는 여기에서,
-   ![img](images/naver_game.png)
-   네이버 게임 오리지널 시리즈의 경우는 여기에서 확인할 수 있습니다.
+   네이버 웹툰/베스트 도전(comic.naver.com):
+   ![img](https://raw.githubusercontent.com/ilotoki0804/WebtoonScraper/master/images/naver_webtoon.png)
+   웹툰 오리지널/캔버스(webtoons.com):
+   ![img](https://raw.githubusercontent.com/ilotoki0804/WebtoonScraper/master/images/webtoons_original.png)
+   만화경(manhwakyung.com)
+   ![img](https://raw.githubusercontent.com/ilotoki0804/WebtoonScraper/master/images/manhwakyung.png)
+   네이버 게임 오리지널 시리즈(game.naver.com/original_series):
+   ![img](https://raw.githubusercontent.com/ilotoki0804/WebtoonScraper/master/images/naver_game.png)
+   버프툰과 네이버 포스트는 아래의 '버프툰 다운로드하기'섹션과 '네이버 포스트 다운로드하기' 섹션을 참고해 주세요.
 2. 다음의 파이썬 코드를 웹툰이 다운로드되길 원하는 폴더 내에서 실행해 주세요. 웹툰은 정식 연재와 베스트 도전, Webtoons 오리지널과 캔버스, 만화경, 네이버 게임 모두 가능합니다.
 
    ```python
    from WebtoonScraper import Webtoon as wt
 
    # 네이버 웹툰
-   wt.get_webtoon(76648, wt.N) # titleid를 여기에다 붙여넣으세요.
+   wt.get_webtoon(76648, wt.N)  # titleid를 여기에다 붙여넣으세요.
    # 베스트 도전만화
-   wt.get_webtoon(763952, wt.B) # titleid를 여기에다 붙여넣으세요.
+   wt.get_webtoon(763952, wt.B)  # titleid를 여기에다 붙여넣으세요.  # ! 수정
    # 웹툰 오리지널
-   wt.get_webtoon(1435, wt.O) # titleid를 여기에다 붙여넣으세요.
+   wt.get_webtoon(1435, wt.O)  # title_no를 여기에다 붙여넣으세요.
    # 웹툰 캔버스
-   wt.get_webtoon(304446, wt.C) # titleid를 여기에다 붙여넣으세요.
+   wt.get_webtoon(304446, wt.C)  # title_no를 여기에다 붙여넣으세요.
    # 만화경
-   wt.get_webtoon(146, wt.M) # titleid를 여기에다 붙여넣으세요. Webtoon.T 태그도 사용 가능합니다.
+   wt.get_webtoon(146, wt.M)  # titleid를 여기에다 붙여넣으세요. Webtoon.T 태그도 사용 가능합니다.
    # 네이버 게임 오리지널 시리즈
-   wt.get_webtoon(146, wt.G) # titleid를 여기에다 붙여넣으세요.
+   wt.get_webtoon(5, wt.G)  # titleid를 여기에다 붙여넣으세요.
+   # 버프툰
+   cookie = 'cookie here'  # cookie를 여기에다 붙여넣으세요. 자세한 설명은 아래의 '버프툰 다운로드하기'를 참고하세요.
+   wt.get_webtoon(1007888, wt.BF, cookie=cookie)  # titleid를 여기에다 붙여넣으세요.
+   # 네이버 포스트
+   wt.get_webtoon((597061, 19803452), wt.P)  # seriesNo와 memberNo를 각각 붙여넣으세요. 자세한 설명은 아래의 '네이버 포스트 다운받기'를 참고하세요.
    ```
 
    이제 웹툰이 webtoons 폴더에 다운로드됩니다.
 
    cf. 웹툰 태그를 생략하면 해당 웹툰이 어떤 사이트의 웹툰 id인지 자동으로 알아냅니다. 만약 몇몇 태그가 겹친다면 태그에 맞는 수를 입력하는 창에 알맞은 수를 입력하면 됩니다.
 
-   또 merge 태그를 이용하면 webtoon 폴더 내에 있는 모든 웹툰을 자동으로 5화씩 묶습니다.
+   episode_no_range 키워드를 이용하면 특정한 에피소드만 다운로드받을 수 있습니다.
+   ```python
+   wt.get_webtoon(5, wt.G, episode_no_range=(1,20))  # 1화부터 20화까지
+   ```
+
+   merge 키워드를 이용하면 webtoon 폴더 내에 있는 모든 웹툰을 원하는 개수 만큼 묶습니다.
+   ```python
+   wt.get_webtoon(5, wt.G, merge=5)
+   ```
 3. 만화 뷰어 앱을 통해 다운로드한 웹툰을 시청할 수 있습니다.
 
 ## 주의사항
 
 * 중간에 웹툰 다운로드가 멈춘 듯이 보여도 정상입니다. 그대로 가만히 있으면 다운로드가 다시 진행됩니다.
 * 만약 작동하지 않는다면 윈도우에서 Python 3.11.4을 설치하고 앞의 과정을 반복해 보세요.
 
@@ -63,87 +95,59 @@
 로그인하지 않은 상태에서도 웹툰을 다운로드받을 수 있으나, 받을 수 있는 웹툰 수가 매우 적기에 추천하지 않습니다.
 
 1. 웹툰 페이지에 들어가 주소창의 맨 마지막 수를 복사합니다.
 2. 다음의 파이썬 코드를 웹툰이 다운로드되길 원하는 폴더 내에서 실행해 주세요.
    ```python
    from WebtoonScraper import Webtoon as wt
 
-   wt.get_webtoon(1007888, wt.BF) # 복사했던 수를 여기에다 붙여넣으세요.
+   wt.get_webtoon(1007888, wt.BF)  # 복사했던 수를 여기에다 붙여넣으세요.
    ```
 3. 'Enter cookie of 1007888(시리즈 id) (Enter nothing to preceed without cookie)'라는 문구와 함께 입력란이 나오면 그냥 enter를 눌러줍니다.
 4. 로그인하지 않고 볼 수 있는 모든 에피소드가 다운로드됩니다.
 
 ## 로그인한 상태에서 웹툰 다운로드하기
 
 이 과정은 PC를 기준으로 설명합니다. 만약 모바일이라면 Kiwi Browser 등을 통해 다음의 과정을 수행할 수 있습니다.
 
 1. 웹툰 페이지에 들어가 주소창의 맨 마지막 수를 복사합니다. 이 예시에서는 1007888입니다.
-   ![img](images/bufftoon1.png)
+   ![img](https://raw.githubusercontent.com/ilotoki0804/WebtoonScraper/master/images/bufftoon1.png)
 2. 로그인을 하고 f12를 누르고 네트워크 창을 연 뒤 웹툰 페이지에 들어갑니다.
-   ![img](images/bufftoon2.png)
+   ![img](https://raw.githubusercontent.com/ilotoki0804/WebtoonScraper/master/images/bufftoon2.png)
 3. 새로고침을 한 뒤 '이름'에 있는 favicon.ico 요청을 클릭하고 나온 창에 '헤더' 탭을 엽니다.
-   ![img](images/bufftoon3.png)
+   ![img](https://raw.githubusercontent.com/ilotoki0804/WebtoonScraper/master/images/bufftoon3.png)
 4. 내려서 Cookie: 라고 되어 있는 모든 내용을 복사합니다.
-   ![img](images/bufftoon4.png)
+   ![img](https://raw.githubusercontent.com/ilotoki0804/WebtoonScraper/master/images/bufftoon4.png)
 5. 다음의 파이썬 코드를 웹툰이 다운로드되길 원하는 폴더 내에서 실행해 주세요.
-
-   ```python
-   from WebtoonScraper import Webtoon as wt
-
-   wt.get_webtoon(1007888, wt.BF) # 첫 번째로 복사했던 수를 여기에다 붙여넣으세요.
-   ```
-
-   혹은 다음과 같이 cookie를 코드 내에 포함할 수도 있습니다.
-
    ```python
    from WebtoonScraper import Webtoon as wt
    cookie = '두 번째로 복사했던 문자를 여기에다 붙여넣으세요.'
-   wt.get_webtoon(1007888, wt.BF, cookie=cookie) # 첫 번째로 복사했던 수를 여기에다 붙여넣으세요.
+   wt.get_webtoon(1007888, wt.BF, cookie=cookie)  # 첫 번째로 복사했던 수를 여기에다 붙여넣으세요.
    ```
-
-   1. 'Enter cookie of 1007888(시리즈 id) (Enter nothing to proceed without cookie)'라는 문구와 함께 입력란이 나오면 두 번째로 복사했던 일련의 문자열을 붙여넣기합니다.
 6. 로그인하면 볼 수 있는 모든 에피소드가 다운로드됩니다.
 
 ## 주의사항
 
 * get_webtoon에서 cookie를 입력하면 자동으로 버프툰으로 인식합니다.
 
 # 네이버 포스트 다운로드하기
 
 1. 웹툰이 있는 페이지로 가서 seriesNo와 memberNo를 복사하세요. 예시에서는 각각 597061과 19803452입니다.
-   ![img](images/naver_post.png)
+   ![img](https://raw.githubusercontent.com/ilotoki0804/WebtoonScraper/master/images/naver_post.png)
 2. 다음의 파이썬 코드를 웹툰이 다운로드되길 원하는 폴더 내에서 실행해 주세요.
-
-   ```python
-   from WebtoonScraper import Webtoon as wt
-
-   wt.get_webtoon(597061, wt.M) # 우선 seriesNo만 여기에 입력해주세요.
-   ```
-
-   혹은 memberNo를 코드 내에 포함할 수 있습니다.
-
    ```python
    from WebtoonScraper import Webtoon as wt
 
-   wt.get_webtoon(597061, wt.M, member_no=19803452)
-   ```
-3. 'Enter memberNo of 597061(해당 웹툰의 seriesNo)'라는 말과 함께 입력란이 나오면 거기에 아까 복사해 놓은 memberNo를 붙여넣습니다.
-   만약 앞에서 이미 member_no를 사용했다면 이 단계는 건너뛰어집니다.
-
-   ```
-   Enter memberNo  of 597061: 19803452
-   ...진행됨...
+   wt.get_webtoon((597061, 19803452), wt.P)
    ```
-4. 만화 뷰어 앱을 통해 다운로드한 웹툰을 시청할 수 있습니다.
+3. 만화 뷰어 앱을 통해 다운로드한 웹툰을 시청할 수 있습니다.
 
 ## 주의사항
 
 * 가끔씩 이유 없는 오류가 발생할 수 있습니다. 그럴 때는 조금 시간이 지난 후에 다시 시도해 보세요.
-* 네이버 포스트는 titleid를 get_webtoon_platform으로 알아낼 수 없습니다.
-* member_no를 입력하면 자동으로 포스트로 인식됩니다.
+* tuple를 입력하면 자동으로 포스트로 인식됩니다.
 
 # 여러 회차 하나로 묶기
 
 1. 웹툰을 상기한 대로 다운로드받습니다.
 2. 다음과 같이 코드를 짭니다.
    ```python
    from WebtoonScraper import FolderManager
@@ -167,31 +171,18 @@
    from WebtoonScraper import FolderManager
 
    fm= FolderManager()
    fm.restore_webtoons_in_directory()
    ```
 3. 'webtoon' 폴더에 있던 모든 웹툰이 웹툰을 처음 다운로드했던 상태로 되돌아갑니다.
 
-# QNA
-
-## 회차 번호 관련
-
-### 문제와 이유
-
-회차가 띄엄띄엄 있거나 설정된 회차 번호가 작가가 설정한 회차 번호와 다르거나 회차 묶기를 사용했는데 묶인 회차 수가 설정한 수보다 더 적은 이유는 다음과 같습니다.
-이 프로젝트에서 웹툰의 회차 번호는 ID를 기준으로 합니다. 이는 작가가 정한 회차와는 다를 수 있습니다. 작가가 프롤로그부터 시작하는 경우(프로젝트의 회차 번호가 하나 빠름), 작가가 리메이크를 해서 전에 있던 작품을 제거해 ID가 연속적으로 있지 않는 경우(주로 베도에서 일어남/회차 번호가 띄엄띄엄하게 있음), 논란이나 작가 실수 등으로 회차가 삭제된 경우(한 회차를 건너띔) 등에서 ID가 불연속적이거나 작품과 일치하기 않는 경우가 생기게 됩니다.
-
-### ID를 회차 번호로 그대로 사용하는 이유
-
-우선 작가가 설정한 회차 번호에 맞추는 것은 힘듭니다. 우선 번호가 어디에 있을지 알기 어렵고, 프롤로그가 있을지 없을지 알 수 없으며, 여러 화에 걸쳐 같은 에피소드를 진행하는 경우도 있고, 외전으로 본편의 회차에서 분리된 화를 운영하는 경우가 있어 화에 맞추어서 번호를 정하는 것을 어렵습니다.
-1부터 시작해서 끝까지 일정한 번호를 유지하는 것도 고려해볼 만하나 만약 그렇게 된다면 무결성 체크를 사용하기 어렵게 됩니다.
-따라서 작가가 설정한 회차를 그대로 사용하는 것도 어렵고, 만약 가능하다 할 지라도 무결성 체크를 포기하기 어렵기 때문에 현재는 ID를 회차 번호로 사용하고 있습니다.
-
 # Relese Note
 
+1.1.1: 내부 모듈 이름 변경, merge option 추가, abstractmethod들의 일반 구현 추가
+
 1.0.2: 대형 리팩토링, get_webtoon_platform 비동기 방식으로 속도 개선, 상대경로로 변경, 테스트 추가
 
 1.0.1: 코드 개선 및 리팩토링, api를 통한 로직으로 변경 (버그가 많기에 사용을 권장하지 않음)
 
 1.0.0: 네이버 게임 추가, FolderManager 리펙토링 및 개선, 정식 버전, docs 개선
 
 0.1.1: 네이버 포스트 추가, readme 작성, pbar 표시 내용 변경, 버그 수정
```

### Comparing `WebtoonScraper-1.0.2/WebtoonScraper/BestChallengeScraper.py` & `WebtoonScraper-1.1.1/WebtoonScraper/E_BestChallengeScraper.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 '''Download Webtoons from Naver Webtoon Best Challenge.'''
-if __name__ == "__main__":
-    from NaverWebtoonScraper import NaverWebtoonScraper
+if __name__ in ("__main__", "E_BestChallengeScraper"):
+    from D_NaverWebtoonScraper import NaverWebtoonScraper
 else:
-    from .NaverWebtoonScraper import NaverWebtoonScraper
+    from .D_NaverWebtoonScraper import NaverWebtoonScraper
 
 
 class BestChallengeScraper(NaverWebtoonScraper):
-    def __init__(self, pbar_independent=False, short_connection=False):
-        super().__init__(pbar_independent, short_connection)
+    def __init__(self, pbar_independent=False):
+        super().__init__(pbar_independent)
         self.BASE_URL = 'https://comic.naver.com/bestChallenge'
         self.EPISODE_IMAGES_URL_SELECTOR = '#comic_view_area > div > img'
 
 
 if __name__ == '__main__':
     wt = BestChallengeScraper()
-    wt.get_webtoon(763952)  # 과학고
+    wt.download_one_webtoon(763952)  # 과학고
```

### Comparing `WebtoonScraper-1.0.2/WebtoonScraper/BufftoonScraper.py` & `WebtoonScraper-1.1.1/WebtoonScraper/I_BufftoonScraper.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,84 +1,80 @@
 '''Download Webtoons from Bufftoon.'''
 import re
 from pathlib import Path
 import time
 from async_lru import alru_cache
 
-if __name__ == "__main__":
-    from WebtoonScraper.Scraper import Scraper
+if __name__ in ("__main__", "I_BufftoonScraper"):
+    from C_Scraper import Scraper
 else:
-    from .Scraper import Scraper
+    from .C_Scraper import Scraper
 
 
 class BufftoonScraper(Scraper):
     '''Scrape webtoons from Bufftoon.'''
-    def __init__(self, pbar_independent: bool = False, short_connection: bool = False, cookie: str = ''):
-        super().__init__(pbar_independent, short_connection)
+    def __init__(self, pbar_independent: bool = False, cookie: str = ''):
+        super().__init__(pbar_independent)
         self.BASE_URL = 'https://bufftoon.plaync.com'
-        if not short_connection:
-            self.IS_STABLE_CONNECTION = True
-        self.COOKIE = cookie
+        self.IS_STABLE_CONNECTION = True
+        self.COOKIE: str = cookie
 
     @alru_cache(maxsize=4)
-    async def _get_webtoon_infomation(self, titleid, get_payment: bool = False, limit: int = 500):
+    async def get_webtoon_data(self, titleid, get_payment: bool = False, get_login_requiered: bool | None = None,limit: int = 500):
         url = f'https://api-bufftoon.plaync.com/v2/series/{titleid}/episodes?sortType=2&offset=0&limit={limit}'
         raw_data = await self.get_internet('requests', url)
         raw_data = raw_data.json()
-        subtitles = {}
-        episode_ids = {}
+        subtitles = []
+        episode_ids = []
+        if get_login_requiered is None:
+            get_login_requiered = bool(self.COOKIE)
         for raw_episode in raw_data['result']['episodes']:
             if not get_payment and raw_episode['isPaymentEpisode']:
                 print(f"Episode '{raw_episode['title']}' is not free of charge episode. It won't be downloaded.")
                 continue
-            if not self.COOKIE and not raw_episode['isOpenFreeEpisode']:
+            if not get_login_requiered and not raw_episode['isOpenFreeEpisode']:
                 print(f"Episode '{raw_episode['title']}' is not opened for non-login users. It'll be not downloaded.")
                 continue
             episode_no = raw_episode['episodeOrder']
             raw_episode_id = raw_episode['listImgPath']
             episode_id = int(re.search(rf'(?<=contents\/.\/{titleid}\/)(\d+)(?=\/)', raw_episode_id)[0])
-            episode_ids[episode_no] = episode_id
-            subtitles[episode_no] = raw_episode['title']
-        return subtitles, episode_ids
+            episode_ids.append(episode_id)
+            subtitles.append(raw_episode['title'])
+        return {'subtitles': subtitles, 'episode_ids': episode_ids}
 
-    async def get_title(self, titleid, file_acceptable):
+    async def get_title(self, titleid):
         url = f'https://bufftoon.plaync.com/series/{titleid}'
         title = await self.get_internet(get_type='soup_select_one', url=url,
                                         selector='#content > div > div > div.series-info > div.cont > div.title')
-        title = title.text.strip()
-        if file_acceptable:
-            title = self.get_acceptable_file_name(title)
-        return title
+        if title is None:
+            raise ValueError('Bufftoon may change their API specification. Contect Developer to update program.')
+        return title.text.strip()
 
     async def save_webtoon_thumbnail(self, titleid, title, thumbnail_dir):
         url = f'https://bufftoon.plaync.com/series/{titleid}'
-        image_url = await self.get_internet(get_type='soup_select_one', url=url,
+        image_url_original = await self.get_internet(get_type='soup_select_one', url=url,
                                             selector='#content > div > div > div.series-info > div.img')
-        image_url = image_url['style']
+        if not image_url_original:
+            raise ConnectionError('Bufftoon changed their api specification. Contect developer to update save_webtoon_thumbnail.')
+        image_url = image_url_original['style']
         image_url = re.search(r'(?<=background-image:url\().+(?=\);)', image_url)[0]
         image_extension = self.get_file_extension(image_url)
         image_raw = await self.get_internet(get_type='requests', url=image_url)
         image_raw = image_raw.content
         Path(f'{thumbnail_dir}/{title}.{image_extension}').write_bytes(image_raw)
 
     async def get_all_episode_no(self, titleid):
-        _, episode_ids = await self._get_webtoon_infomation(titleid)
-        return list(episode_ids)
+        return await super().get_all_episode_no(titleid)
 
-    async def get_subtitle(self, titleid, episode_no, file_acceptable, sleep=True):
+    async def get_subtitle(self, titleid, episode_no, sleep=True):
         if sleep:
             time.sleep(1)
-        subtitles, _ = await self._get_webtoon_infomation(titleid)
-        subtitle = subtitles[episode_no]
-        if file_acceptable:
-            subtitle = self.get_acceptable_file_name(subtitle)
-        return subtitle
+        return await super().get_subtitle(titleid, episode_no)
 
     async def get_episode_images_url(self, titleid, episode_no):
-        # sourcery skip: de-morgan
         HEADERS = {
             'Accept': 'text/html,application/xhtml+xml,application/xml;q=0.9,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.7',
             'Accept-Encoding': 'gzip, deflate, br',
             'Accept-Language': 'ko,en-US;q=0.9,en;q=0.8',
             'Cache-Control': 'max-age=0',
             'Connection': 'keep-alive',
             'Cookie': self.COOKIE,
@@ -93,22 +89,22 @@
             'Sec-Fetch-Mode': 'navigate',
             'Sec-Fetch-Site': 'same-origin',
             'Sec-Fetch-User': '?1',
             'Sec-Gpc': '1',
             'Upgrade-Insecure-Requests': '1',
             'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/114.0.0.0 Safari/537.36 Edg/114.0.1823.43',
         }
-        _, episode_ids = await self._get_webtoon_infomation(titleid)
-        url = f'{self.BASE_URL}/series/{titleid}/{episode_ids[episode_no]}'
+        episode_id = await self.episode_no_to_episode_id(titleid, episode_no)
+        url = f'{self.BASE_URL}/series/{titleid}/{episode_id}'
         selector = '#content > div > div > div.viewer-wrapper > div > img'
         episode_images_url = await self.get_internet(get_type='soup_select', url=url,
                                                      selector=selector, headers=HEADERS)
 
-        return [element['src'] for element in episode_images_url if not ('agerate' in element['src'] or 'ctguide' in element['src'])]
+        return [element['src'] for element in episode_images_url]
 
     async def download_single_image(self, episode_dir: Path, url: str, image_no: int) -> None:
-        super().download_single_image(episode_dir, url, image_no, 'png')
+        await super().download_single_image(episode_dir, url, image_no, 'png')
 
 
 if __name__ == '__main__':
     wt = BufftoonScraper()
-    wt.get_webtoon(1007888)  # 겜덕툰
+    wt.download_one_webtoon(1007888)  # 겜덕툰
```

### Comparing `WebtoonScraper-1.0.2/WebtoonScraper/FolderManager.py` & `WebtoonScraper-1.1.1/WebtoonScraper/A_FolderManager.py`

 * *Files identical despite different names*

### Comparing `WebtoonScraper-1.0.2/WebtoonScraper/NaverGameScraper.py` & `WebtoonScraper-1.1.1/WebtoonScraper/K_NaverGameScraper.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,89 +1,83 @@
 '''Download Webtoons from Naver Post.'''
 
 import contextlib
-from pathlib import Path
+# from pathlib import Path
 from itertools import count
 import json
 from async_lru import alru_cache
 
-if __name__ == "__main__":
-    from Scraper import Scraper
+if __name__ in ("__main__", "K_NaverGameScraper"):
+    from C_Scraper import Scraper
 else:
-    from .Scraper import Scraper
+    from .C_Scraper import Scraper
 
 
 class NaverGameScraper(Scraper):
     '''Scrape webtoons from Naver Post.'''
-    def __init__(self, pbar_independent=False, short_connection=False):
-        super().__init__(pbar_independent, short_connection)
+    def __init__(self, pbar_independent=False):
+        super().__init__(pbar_independent)
         self.BASE_URL = 'https://game.naver.com/original_series'
-        if not short_connection:
-            self.IS_STABLE_CONNECTION = True
+        self.IS_STABLE_CONNECTION: bool = True
 
     @alru_cache(maxsize=4)
     async def _get_webtoon_infomation(self, titleid):
         url = f'https://apis.naver.com/nng_main/nng_main/original/series/{titleid}'
         webtoon_raw_data = await self.get_internet(get_type='requests', url=url)
         webtoon_raw_data = webtoon_raw_data.json()
         title = webtoon_raw_data['content']['seriesName']
         thumbnail = webtoon_raw_data['content']['seriesImage']['verticalLogoImageUrl']
         return title, thumbnail
 
     @alru_cache(maxsize=4)
-    async def _get_episode_infomation(self, titleid, episode_max_limit=500):
+    async def get_webtoon_data(self, titleid, episode_max_limit=500):
         # 여러 시즌을 하나로 통합
         content_raw_data = []
         for season in count(1):
-            url = f'https://apis.naver.com/nng_main/nng_main/original/series/{titleid}/seasons/{season}/contents'\
-                  f'?direction=NEXT&pagingType=CURSOR&sort=FIRST&limit={episode_max_limit}'
+            url = (f'https://apis.naver.com/nng_main/nng_main/original/series/{titleid}/seasons/{season}/contents'
+                   f'?direction=NEXT&pagingType=CURSOR&sort=FIRST&limit={episode_max_limit}')
             res = await self.get_internet(get_type='requests', url=url)
             res = res.json()
             if not res['content']:
                 break
             content_raw_data += res['content']['data']
 
         # 부제목, 이미지 데이터 불러옴
-        episodes_data = {}
+        # episodes_data = {}
+        subtitles = []
+        episode_images_url = []
+        episode_ids = []
         for i, episode in enumerate(content_raw_data, 1):
             subtitle = episode['feed']['title']
             content_json_data = json.loads(episode['feed']['contents'])
             image_urls = []
             for image_url in content_json_data['document']['components']:
                 with contextlib.suppress(KeyError):
                     image_urls.append(image_url['src'])
-            episodes_data[i] = {'subtitle': subtitle, 'image_urls': image_urls}
+            # episodes_data[i] = {'subtitle': subtitle, 'image_urls': image_urls}
+            episode_ids.append(i)
+            subtitles.append(subtitle)
+            episode_images_url.append(image_urls)
 
-        return episodes_data
+        title, thumbnail = await self._get_webtoon_infomation(titleid)
 
-    async def get_title(self, titleid, file_acceptable=True):
-        title, _ = await self._get_webtoon_infomation(titleid)
-        if file_acceptable:
-            title = self.get_acceptable_file_name(title)
-        return title
+        return {'subtitles': subtitles, 'episode_images_url': episode_images_url, 'episode_ids': episode_ids, 'title': title, 'webtoon_thumbnail': thumbnail}
+
+    async def get_title(self, titleid):
+        return await super().get_title(titleid)
 
     async def save_webtoon_thumbnail(self, titleid, title, thumbnail_dir):
-        _, image_url = await self._get_webtoon_infomation(titleid)
-        image_extension = self.get_file_extension(image_url)
-        image_raw = await self.get_internet(get_type='requests', url=image_url)
-        image_raw = image_raw.content
-        Path(f'{thumbnail_dir}/{title}.{image_extension}').write_bytes(image_raw)
+        return await super().save_webtoon_thumbnail(titleid, title, thumbnail_dir)
 
     async def get_all_episode_no(self, titleid):
-        episodes_data = await self._get_episode_infomation(titleid)
-        return list(episodes_data)
+        return await super().get_all_episode_no(titleid)
 
-    async def get_subtitle(self, titleid, episode_no, file_acceptable):
-        episodes_data = await self._get_episode_infomation(titleid)
-        subtitle = episodes_data[episode_no]['subtitle']
-        if file_acceptable:
-            subtitle = self.get_acceptable_file_name(subtitle)
-        return subtitle
+    async def get_subtitle(self, titleid, episode_no):
+        return await super().get_subtitle(titleid, episode_no)
 
     async def get_episode_images_url(self, titleid, episode_no):
-        episodes_data = await self._get_episode_infomation(titleid)
-        return episodes_data[episode_no]['image_urls']
+        return await super().get_episode_images_url(titleid, episode_no)
 
 
 if __name__ == '__main__':
     wt = NaverGameScraper()
-    wt.get_webtoon(5)  # 모배툰
+    wt.download_one_webtoon(5)  # 모배툰
```

### Comparing `WebtoonScraper-1.0.2/WebtoonScraper/NaverPostScraper.py` & `WebtoonScraper-1.1.1/WebtoonScraper/J_NaverPostScraper.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,107 +1,99 @@
 '''Download Webtoons from Naver Post.'''
 # TODO: subtitle_list에서 subtitles로 변경하기
 
 from pathlib import Path
 from itertools import count
 import asyncio
+# import logging
+
 from async_lru import alru_cache
 import demjson3
 from bs4 import BeautifulSoup
 
-if __name__ == "__main__":
-    from Scraper import Scraper
+if __name__ in ("__main__", "J_NaverPostScraper"):
+    # logging.warning('Using ')
+    from C_Scraper import Scraper
 else:
-    from .Scraper import Scraper
+    from .C_Scraper import Scraper
 
 
 class NaverPostScraper(Scraper):
     '''Scrape webtoons from Naver Post.'''
-    def __init__(self, pbar_independent=False, short_connection=False):
-        super().__init__(pbar_independent, short_connection)
+    def __init__(self, pbar_independent=False):
+        super().__init__(pbar_independent)
+        self.IS_STABLE_CONNECTION = True
         self.BASE_URL = 'https://post.naver.com'
-        if not short_connection:
-            self.IS_STABLE_CONNECTION = True
-
-    def download_one_webtoon(self, titleid: int, member_no: int,  value_range: tuple | int | None = None) -> None:
-        """async를 사용하지 않는 일반 상태일 경우 사용하는 함수이다. 사용법은 download_one_webtoon_async와 동일하다."""
-        asyncio.run(self.download_one_webtoon_async(titleid, member_no,  value_range))
-
-    async def download_one_webtoon_async(self, titleid, member_no: int, episode_no_range: tuple | int | None = None) -> None:
-        """포스트는 member_no도 받아야 하기 때문에 불가피하게 수정이 필요."""
-        self.member_no = member_no
-        await super().download_one_webtoon_async(titleid, episode_no_range)
 
     @alru_cache(maxsize=4)
-    async def _get_webtoon_infomation(self, titleid: int) -> list:
+    async def get_webtoon_data(self, titleid: tuple[int, int]) -> dict[str, list]:
         # sourcery skip: for-append-to-extend, list-comprehension, move-assign-in-block
-        subtitle_list = []
+        series_no, member_no = titleid
+        subtitle_list: list[str] = []
+        episode_id_list: list[int] = []
+        prev_data = None
         for i in count(1):
-            subtitle_sublist = []
             # n번째 리스트 불러옴
-            url = f'https://post.naver.com/my/series/detail/more.nhn?memberNo={self.member_no}&seriesNo={titleid}&lastSortOrder=49&prevVolumeNo=&fromNo={i}&totalCount=68'
+            url = (f'https://post.naver.com/my/series/detail/more.nhn'
+                   f'?memberNo={member_no}&seriesNo={series_no}&lastSortOrder=49'
+                   f'&prevVolumeNo=&fromNo={i}&totalCount=68')
             # print(url)
-            response = await self.get_internet('requests', url)
+            response_text: str = (await self.get_internet('requests', url)).text
 
             # 네이버는 기본적으로 json이 망가져 있기에 json이 망가져 있어도 parse를 해주는 demjson이 필요
-            demres = demjson3.decode(response.text)['html']
-            soup = BeautifulSoup(demres, 'html.parser')
+            decoded_response_data: str = demjson3.decode(response_text)['html']
+            soup = BeautifulSoup(decoded_response_data, 'html.parser')
 
             # subtitle data만듦.
             for tag in soup.select('ul > li > a > div > span.ell'):
-                subtitle_sublist.append({'subtitle': tag.text.strip()})
-            for j, tag in enumerate(soup.select('ul > li > a > div > span.spot_post_like')):
-                # 버려지는 값은 member_no/그냥 member_no라고 해도 되지만 혹시 모를 corruption을 막기 위한 조치
+                # subtitle_list.append({'subtitle': tag.text.strip()})
+                subtitle_list.append(tag.text.strip())
+            for tag in soup.select('ul > li > a > div > span.spot_post_like'):
                 episode_id, _ = map(int, tag['data-cid'].split('_'))
-                subtitle_sublist[j].update({'episode_id': episode_id, 'member_no': self.member_no})
+                episode_id_list.append(episode_id)
 
-            # 지금 받아온 데이터가 이전 데이터와 같은지 확인
-            if subtitle_sublist == subtitle_list[-len(subtitle_sublist):]:
+            if prev_data == decoded_response_data:
                 break
-            else:
-                subtitle_list += subtitle_sublist
+
+            prev_data = decoded_response_data
+
         # 1화부터로 변경
-        return subtitle_list[::-1]
+        return {'subtitles': subtitle_list[::-1], 'episode_ids': episode_id_list[::-1]}
 
-    async def get_title(self, titleid, file_acceptable=True):
-        url = f'https://m.post.naver.com/my/series/detail.naver?seriesNo={titleid}&memberNo={self.member_no}'
-        title = await self.get_internet(get_type='soup_select_one', url=url,
-                                        selector='h2.tit_series > span')
-        title = title.text.strip()
-        if file_acceptable:
-            title = self.get_acceptable_file_name(title)
-        return title
-
-    async def save_webtoon_thumbnail(self, titleid, title, thumbnail_dir):
-        url = f'https://m.post.naver.com/my/series/detail.naver?seriesNo={titleid}&memberNo={self.member_no}'
-        image_url = await self.get_internet(get_type='soup_select_one', url=url,
+    async def get_title(self, titleid: tuple[int, int]):
+        series_no, member_no = titleid
+        url = f'https://m.post.naver.com/my/series/detail.naver?seriesNo={series_no}&memberNo={member_no}'
+        title: str = (await self.get_internet(get_type='soup_select_one', url=url,
+                                              selector='h2.tit_series > span')).text
+        return title.strip()
+
+    async def save_webtoon_thumbnail(self, titleid: tuple[int, int], title, thumbnail_dir):
+        series_no, member_no = titleid
+        url = f'https://m.post.naver.com/my/series/detail.naver?seriesNo={series_no}&memberNo={member_no}'
+        image_url_original = await self.get_internet(get_type='soup_select_one', url=url,
                                             selector='meta[property="og:image"]')
-        image_url = image_url['content']
+        if not image_url_original:
+            raise ConnectionError('Naver Post changed their api specification. Contect developer to update save_webtoon_thumbnail.')
+        image_url: str = image_url_original['content']
         image_extension = self.get_file_extension(image_url)
-        image_raw = await self.get_internet(get_type='requests', url=image_url)
-        image_raw = image_raw.content
+        image_raw: bytes = (await self.get_internet(get_type='requests', url=image_url)).content
         Path(f'{thumbnail_dir}/{title}.{image_extension}').write_bytes(image_raw)
+        (thumbnail_dir / f'{title}.{image_extension}').write_bytes(image_raw)
 
     async def get_all_episode_no(self, titleid):
         """1부터 시작하니 주의!!"""
-        subtitle_list = await self._get_webtoon_infomation(titleid)
-        return (i + 1 for i in range(len(subtitle_list)))
+        return await super().get_all_episode_no(titleid)
 
-    async def get_subtitle(self, titleid, episode_no, file_acceptable):
-        subtitle_list = await self._get_webtoon_infomation(titleid)
-        subtitle_info = subtitle_list[episode_no - 1]
-        subtitle = subtitle_info['subtitle']
-        if file_acceptable:
-            subtitle = self.get_acceptable_file_name(subtitle)
-        return subtitle
+    async def get_subtitle(self, titleid, episode_no):
+        return await super().get_subtitle(titleid, episode_no)
 
     async def get_episode_images_url(self, titleid, episode_no, attempt=3):
-        subtitle_list = await self._get_webtoon_infomation(titleid)
-        episode_id = subtitle_list[episode_no - 1]['episode_id']
-        url = f'https://post.naver.com/viewer/postView.naver?volumeNo={episode_id}&memberNo={self.member_no}&navigationType=push'
+        series_no, member_no = titleid
+        episode_id = await self.episode_no_to_episode_id(titleid, episode_no)
+        url = f'https://post.naver.com/viewer/postView.naver?volumeNo={episode_id}&memberNo={member_no}&navigationType=push'
         for _ in range(attempt):
             content = await self.get_internet(get_type='soup_select_one', url=url,
                                               selector='#__clipContent')
             if content is None:
                 # '존재하지 않는 포스트입니다'하는 경고가 뜬 후 사이트가 받아지지 않는 오류
                 # 아마 episode_id에 titleid가 잘못 들어가면 생기는 오류로 추정하지만
                 # 정확한 이유는 불명, 가끔씩 생기는 문제.
@@ -111,22 +103,25 @@
         else:
             raise ConnectionError('Unknown error occurred. Please try again later.')
         content = content.text
         soup_content = BeautifulSoup(content, 'html.parser')
 
         # 문서 내에 있는 모든 이미지 링크를 불러옴
         selector = 'div.se_component_wrap.sect_dsc.__se_component_area > div > div > div > div > a > img'
-        episode_images_url = [tag['data-src'] for tag in soup_content.select(selector)]
+        episode_images_url: list[str] = [tag['data-src'] for tag in soup_content.select(selector)]
 
         return [url for url in episode_images_url
                 if not url.startswith('https://mail.naver.com/read/image/')]
 
 
 if __name__ == '__main__':
+    # logger = logging.getLogger()
+    # logger.setLevel(logging.INFO)
+
     wt = NaverPostScraper()
-    wt.download_one_webtoon(597061, 19803452)  # 겜덕겜소
+    wt.download_one_webtoon((597061, 19803452))  # 겜덕겜소
 
-    # asyncio.run(wt.get_data(625402, 19803452))
+    asyncio.run(wt.get_webtoon_data((577056, 19803452)))  # 겜덕툰
 
     # wt = NaverPostScraper()
     # wt.member_no = 19803452
     # print(asyncio.run(wt.get_episode_images_url(577056, 2)))
```

### Comparing `WebtoonScraper-1.0.2/WebtoonScraper/NaverWebtoonScraper.py` & `WebtoonScraper-1.1.1/WebtoonScraper/D_NaverWebtoonScraper.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,81 +1,85 @@
 '''Download Webtoons from Naver Webtoon.'''
 from itertools import count
 from async_lru import alru_cache
 
-if __name__ == "__main__":
-    from Scraper import Scraper
+if __name__ in ("__main__", "D_NaverWebtoonScraper"):
+    from C_Scraper import Scraper
 else:
-    from .Scraper import Scraper
+    # from Scraper import Scraper
+    from .C_Scraper import Scraper
 
 
 class NaverWebtoonScraper(Scraper):
     '''Scrape webtoons from Naver Webtoon.'''
-    def __init__(self, pbar_independent=False, short_connection=False):
-        super().__init__(pbar_independent, short_connection)
+    def __init__(self, pbar_independent=False):
+        super().__init__(pbar_independent)
         self.BASE_URL = 'https://comic.naver.com/webtoon'
-        if not short_connection:
-            self.IS_STABLE_CONNECTION = True
+        self.IS_STABLE_CONNECTION = True
         self.EPISODE_IMAGES_URL_SELECTOR = '#sectionContWide > img'  # for best challenge
 
     @alru_cache(maxsize=4)
-    async def _get_webtoon_data(self, titleid: int):
+    async def get_webtoon_data(self, titleid: int):
         prev_articleList = []
-        subtitles = {}
+        subtitles = []
+        episode_id = []
         for i in count(1):
             url = f"https://comic.naver.com/api/article/list?titleId={titleid}&page={i}&sort=ASC"
             res = await self.get_internet('requests', url)
             res = res.json()
 
             curr_articleList = res["articleList"]
             if prev_articleList == curr_articleList:
                 break
             for article in curr_articleList:
-                subtitles[article["no"]] = article["subtitle"]
+                # subtitles[article["no"]] = article["subtitle"]
+                subtitles.append(article["subtitle"])
+                episode_id.append(article["no"])
 
             prev_articleList = curr_articleList
 
-        return subtitles
+        return {'subtitles': subtitles, 'episode_ids': episode_id}
 
-    async def get_title(self, titleid, file_acceptable):
+    async def get_title(self, titleid):
         url = f'{self.BASE_URL}/list?titleId={titleid}'
         title = await self.get_internet(get_type='soup_select_one', url=url,
                                         selector='meta[property="og:title"]')
-        title = title['content']
-        if file_acceptable:
-            title = self.get_acceptable_file_name(title)
-        return title
+        if not title:
+            raise ConnectionError('Naver Webtoon changed their api specification. Contect developer to update get_title.')
+        return title['content']
 
     async def save_webtoon_thumbnail(self, titleid, title, thumbnail_dir):
         url = f'{self.BASE_URL}/list?titleId={titleid}'
-        image_url = await self.get_internet(get_type='soup_select_one', url=url,
-                                            selector='meta[property="og:image"]')
-        image_url = image_url['content']
+        image_url_tag = await self.get_internet(get_type='soup_select_one', url=url,
+                                                selector='meta[property="og:image"]')
+        if not image_url_tag:
+            raise ConnectionError('Naver Webtoon changed their api specification. Contect developer to update get_title.')
+        image_url: str = image_url_tag['content']
         image_extension = self.get_file_extension(image_url)
         image_raw = await self.get_internet(get_type='requests', url=image_url)
         image_raw = image_raw.content
         image_path = thumbnail_dir / f'{title}.{image_extension}'
         image_path.write_bytes(image_raw)
 
     async def get_all_episode_no(self, titleid):
-        subtitles = await self._get_webtoon_data(titleid)
-        return list(subtitles)
+        return await super().get_all_episode_no(titleid)
 
-    async def get_subtitle(self, titleid, episode_no, file_acceptable):
-        subtitles = await self._get_webtoon_data(titleid)
-        subtitle = subtitles[episode_no]
-
-        return self.get_acceptable_file_name(subtitle) if file_acceptable else subtitle
+    async def get_subtitle(self, titleid, episode_no):
+        return await super().get_subtitle(titleid, episode_no)
 
     async def get_episode_images_url(self, titleid, episode_no):
         # sourcery skip: de-morgan
-        url = f'{self.BASE_URL}/detail?titleId={titleid}&no={episode_no}'
+        episode_id = await self.episode_no_to_episode_id(titleid, episode_no)
+        url = f'{self.BASE_URL}/detail?titleId={titleid}&no={episode_id}'
         episode_images_url = await self.get_internet(get_type='soup_select', url=url,
                                                      selector=self.EPISODE_IMAGES_URL_SELECTOR)
-        return [element['src'] for element in episode_images_url if not ('agerate' in element['src'] or 'ctguide' in element['src'])]
+        return [
+            element['src'] for element in episode_images_url
+            if not ('agerate' in element['src'] or 'ctguide' in element['src'])
+        ]
 
 
 if __name__ == '__main__':
     wt = NaverWebtoonScraper()
     wt.download_one_webtoon(809590)  # 이번 생
 
     # # get_internet test(Scraper는 abstract class라 직접 실행이 불가해서 대신 사용)
```

### Comparing `WebtoonScraper-1.0.2/WebtoonScraper/Scraper.py` & `WebtoonScraper-1.1.1/WebtoonScraper/C_Scraper.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,65 +1,167 @@
 """Abstract Class of all scrapers."""
-# TODO: file_acceptable built-in으로 만들기
-# TODO: titleid tuple도 허용해서 NPScraper에서 이용할 수 있도록 하기
-# TODO: get_webtoon 리스트 형식으로 변경하기
+# solved: file_acceptable built-in으로 만들기
+# solved: titleid tuple도 허용해서 NPScraper에서 이용할 수 있도록 하기
+# SOLVED: get_data 시 list로 정보 받아오기
+# TODO: None 대신 NoReturn 사용하기
+# TODO: download vs save : 용어 정리하기
+# TODO: 카카오 웹툰/카카오 페이지 웹툰, 레진 코믹스도 만들기 (HURRY!)
+# FIXME: episode_no와 episode_id를 구분해야 함!!!
+# TODO: short_connection 등 docs 추가하기
+# TODO: Webtoon get_webtoon_platform 조금 더 잘 만들 방법 강구하기
 import re
 import os
 import asyncio
 import shutil
 import html
 from pathlib import Path
-from typing import Iterable, Literal
+# from typing import Iterable, Literal
+from typing import Literal
 from abc import abstractmethod, ABCMeta
+# from collections import namedtuple
+# from contextlib import suppress
+from typing import overload
+# import logging
 
 import requests
 from requests.exceptions import ConnectionError
 from bs4 import BeautifulSoup as bs
 from bs4.element import Tag
 from tqdm import tqdm
+from async_lru import alru_cache
+
+if __name__ in ("__main__", "C_Scraper"):
+    from A_FolderManager import FolderManager
+else:
+    from .A_FolderManager import FolderManager
+
+TitleId = int | tuple[int, int]
 
 
 class Scraper(metaclass=ABCMeta):
     """Abstract class of all scrapers.
 
     init, get_internet, 전반적인 로직 등은 모두 이 페이지에서 관리하고, 구체적인 다운로드 방법은 각각의 scraper들에게 맡깁니다.
     따라서 썸네일을 받아오거나 한 회차의 이미지 URL을 불러오는 등의 역할은 각자 scraper들에 구현되어 있습니다.
     """
 
-    def __init__(self, pbar_independent: bool = False, short_connection=False) -> None:
+    def __init__(self, pbar_independent: bool = False) -> None:
         """시작에 필요한 여러가지를 관여합니다.
 
         header, timeout을 구성하고 set_folders()를 호출합니다.
 
         Args:
             pbar_independent: 만약 True라면 tqdm을 이용해서 로그를 표시하고, False라면 print를 통해서 로그를 표시합니다.
-            short_connection:
-                만약 True라면 timeout를 3초로 짧게 잡고 IS_STABLE_CONNECTION(거짓일 경우, 연결에 실패하면 재시도를 함.)을 False로 합니다.
-                False라면 기본 설정을 유지하고 timeout도 길게(120초) 유지합니다.
         """
         # BASE_URL and IS_STABLE_CONNECTION have to be defined!
         self.HEADERS = {
             'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 '
             '(KHTML, like Gecko) Chrome/113.0.0.0 Safari/537.36'
         }
         self.BASE_DIR = 'webtoon'
         self.TIMEOUT = 120
         self.PBAR_INDEPENDENT = pbar_independent
-        if short_connection:
+        self.IS_STABLE_CONNECTION = None  # IS_STABLE_CONNECTION must be defined!
+        self.short_connection = False
+
+    @property
+    def short_connection(self):
+        return self._short_connection
+
+    @short_connection.setter
+    def short_connection(self, short_connection: bool):
+        """
+        이 함수는 short_connection을 설정합니다.
+        short_connection에는 특징이 있는데, True로 바꾸는 순간 그 전에 설정한 IS_STABLE_CONNECTION과
+        TIMEOUT이 날아가고 각각 False와 3으로 변합니다. 이 함수는 short_connection을 False로 바꿀 때
+        기존의 설정으로 돌아갈 수 있도록 돕습니다.
+
+        Args:
+            short_connection(bool):
+                만약 True라면 timeout를 3초로 짧게 잡고 IS_STABLE_CONNECTION(거짓일 경우, 연결에 실패하면 재시도를 함.)을 False로 합니다.
+                False라면 기본 설정을 유지하고 timeout도 길게(120초) 유지합니다.
+
+        Exceptions:
+            AttributeError: short_connection 값을 선언하기 이전에 반드시 self.IS_STABLE_CONNECTION과
+                self.TIMEOUT을 선언해야 합니다. 만약 그렇지 않으면 AttributeError가 raise됩니다.
+        """
+        def save_prev_settings():
+            # is_stable_connection and timeout must be defined prior to short_connection.
+            self._prev_IS_STABLE_CONNECTION = self.IS_STABLE_CONNECTION
+            self._prev_TIMEOUT = self.TIMEOUT
             self.TIMEOUT = 3
-            self.IS_STABLE_CONNECTION = False
 
-    async def get_internet(
-            self,
-            get_type: Literal['requests', 'soup', 'soup_select', 'soup_select_one'],
-            url: str,
-            selector: str = None,
-            is_run_in_executor: bool = False,
-            attempt: int = 10,
-            headers=None
+        def load_prev_settings():
+            self.IS_STABLE_CONNECTION = self._prev_IS_STABLE_CONNECTION
+            self.TIMEOUT = self._prev_TIMEOUT
+
+        if not hasattr(self, '_short_connection'):
+            if short_connection:
+                self._prev_IS_STABLE_CONNECTION = None  # to suppress error
+                self._prev_TIMEOUT = None  # to suppress error
+                save_prev_settings()
+        else:
+            if short_connection and not self._short_connection:
+                save_prev_settings()
+            else:
+                load_prev_settings()
+        self._short_connection = short_connection
+
+    @overload
+    async def get_internet(  # noqa
+        self,
+        get_type: Literal['requests'],
+        url: str,
+        selector: None = None,
+        is_run_in_executor: bool = False,
+        attempt: int = 10,
+        headers: dict | None = None
+    ) -> requests.Response: ...
+
+    @overload
+    async def get_internet(  # noqa
+        self,
+        get_type: Literal['soup'],
+        url: str,
+        selector: None = None,
+        is_run_in_executor: bool = False,
+        attempt: int = 10,
+        headers: dict | None = None
+    ) -> bs: ...
+
+    @overload
+    async def get_internet(  # noqa
+        self,
+        get_type: Literal['soup_select'],
+        url: str,
+        selector: str,
+        is_run_in_executor: bool = False,
+        attempt: int = 10,
+        headers: dict | None = None
+    ) -> list: ...
+
+    @overload
+    async def get_internet(  # noqa
+        self,
+        get_type: Literal['soup_select_one'],
+        url: str,
+        selector: str,
+        is_run_in_executor: bool = False,
+        attempt: int = 10,
+        headers: dict | None = None
+    ) -> Tag | None: ...
+
+    async def get_internet(  # noqa
+        self,
+        get_type: Literal['requests', 'soup', 'soup_select', 'soup_select_one'],
+        url: str,
+        selector: str | None = None,
+        is_run_in_executor: bool = False,
+        attempt: int = 10,
+        headers: dict | None = None
     ) -> requests.Response | bs | list | Tag | None:
         """Get response/beautifulsoup/beautifulsoup tag list/beautifulsoup tag from internet.
 
         Args:
             get_type:
                 인터넷에서 url로부터 받은 것으로부터 할 것이 무엇인지를 결정합니다.
 
@@ -99,27 +201,31 @@
 
         if not headers:
             headers = self.HEADERS
 
         if self.IS_STABLE_CONNECTION:
             response = await send_get_request()
         else:
+            response = requests.Response()
+            is_success = False
             for _ in range(attempt):
-                is_success = False
                 try:
                     response = await send_get_request()
-                    is_success = True
-                    break
                 except ConnectionError:
                     print('A connection error occured. But don\'t worry. It should be normal process. Retrying...')
+                else:
+                    is_success = True
+                    break
             if not is_success:
                 raise ConnectionError('Trying hard but failed. Maybe low attempt or timeout settizng is reason.'
                                       ' Trying increasing attempt time or timeout. Or sometimes it is caused by invaild titleid.')
 
         if get_type in ('soup', 'soup_select', 'soup_select_one'):
+            if selector is None:
+                raise ValueError('Selector can\'t be None.')
             soup = bs(response.text, "html.parser")
             if get_type == 'soup':
                 return soup
             if get_type == 'soup_select':
                 return soup.select(selector)
             if get_type == 'soup_select_one':
                 return soup.select_one(selector)
@@ -162,99 +268,90 @@
         """
         serch_result: re.Match | None = re.search(r'(?<=[.])(jpg|png|jpeg|gif)(?=[?].+$|$)', filename_or_url, re.I)
 
         return None if serch_result is None else serch_result[0]
         # return filename_or_url.split('.')[-1].lower()
 
     @staticmethod
-    def get_acceptable_file_name(file_or_diretory_name: str, strict_checking: bool = False) -> str:
+    def get_safe_file_name(file_or_diretory_name: str) -> str:
         """Translate file or diretory name to accaptable name.
 
         Caution: Don't put here diretory path beacause it will translate slash and backslash to acceptable(and cannot be used for going directory) name.
         """
+        # sourcery skip: remove-zero-from-range
         table = str.maketrans('\\/:*?"<>|\t\n', '⧵／：＊？＂＜＞∣   ')
+        table.update(
+            {i: 32 for i in range(0, 31)}
+        )
 
         processed = html.unescape(file_or_diretory_name)  # change things like "&amp;" to "'".
 
         processed = processed.translate(table).strip()
 
         processed = re.sub(r'\.$', '．', processed)
 
-        if strict_checking:
-            return ''.join(
-                ' '
-                if ord(chractor)
-                in {
-                    0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15, 16, 17, 18, 19, 20,
-                    21, 22, 23, 24, 25, 26, 27, 28, 29, 30, 31, 34, 42, 58, 60, 62, 63, 124,
-                }
-                else chractor
-                for chractor in processed
-            )
         return processed
 
     @property
     def BASE_DIR(self):
         return self._BASE_DIR
 
     @BASE_DIR.setter
     def BASE_DIR(self, BASE_DIR):
         self._BASE_DIR = Path(BASE_DIR)
 
 ################################## MAIN ACTION ##################################
 
-    def download_one_webtoon(self, titleid: int, value_range: tuple | int | None = None) -> None:
+    def download_one_webtoon(self, titleid: TitleId, episode_no_range: tuple[int, int] | int | None = None, merge: int | None = None) -> None:
         """async를 사용하지 않는 일반 상태일 경우 사용하는 함수이다. 사용법은 download_one_webtoon_async와 동일하다."""
-        asyncio.run(self.download_one_webtoon_async(titleid, value_range))
+        asyncio.run(self.download_one_webtoon_async(titleid, episode_no_range, merge))
 
-    async def download_one_webtoon_async(self, titleid, episode_no_range: tuple | int | None = None) -> None:
+    async def download_one_webtoon_async(self, titleid: TitleId, episode_no_range: tuple[int, int] | int | None = None, merge: int | None = None) -> None:
         """웹툰 다운로드의 주죽이 되는 함수. 이 함수를 통해 웹툰을 다운로드한다.
 
         주의: 유료 회차는 다운로드받을 수 없다.
         :titleid: 다운로드할 웹툰의 titleid 혹은 title_no를 입력한다.
         :episode_no_range: 다운로드할 회차를 정한다.
                                 tuple일 경우: (처음, 끝) 순서로 값을 받는다. 이때 끝을 포함한다.
                                     예) (1,10): 1회차부터 10회차를 다운로드함
                                 int일 경우: 한 회차만 다운로드 받는다.
                                 None일 경우: 웹툰의 모든 회차를 다운로드 받는다.
+        :merge: 웹툰을 모두 다운로드 받은 뒤 웹툰을 묶는다.
         """
         self.loop = asyncio.get_running_loop()
 
-        title = await self.get_title(titleid, file_acceptable=True)
+        title = self.get_safe_file_name(await self.get_title(titleid))
         webtoon_dir = self.BASE_DIR / f'{title}({titleid})'
         self.webtoon_dir = webtoon_dir
 
         webtoon_dir.mkdir(parents=True, exist_ok=True)
 
         await self.save_webtoon_thumbnail(titleid, title, webtoon_dir)
 
+        episode_no_list = await self.get_all_episode_no(titleid)
         if not episode_no_range:
-            titleids = await self.get_all_episode_no(titleid)
+            episode_no_list_plus_1 = range(1, len(episode_no_list) + 1)
         elif isinstance(episode_no_range, int):
-            titleids = (episode_no_range,)
+            episode_no_list_plus_1 = (episode_no_range,)
         else:
             start, end = episode_no_range
-            titleids = range(start, end + 1)
+            episode_no_list_plus_1 = range(start, end + 1)
 
-        self.pbar = tqdm(list(titleids))
+        # episode_nos_plus_1 starts with 1, but episode_no starts with 0, so it needs to be subtracted from 1
+        self.pbar = tqdm([i - 1 for i in episode_no_list_plus_1])
         for episode_no in self.pbar:
             await self.download_one_episode(episode_no, titleid, webtoon_dir)
         print(f'A webtoon {title} download ended.')
 
-    @abstractmethod
-    async def get_title(self, titleid: int, file_acceptable: bool) -> str:
-        """웹툰의 title을 불러온다."""
-
-    @abstractmethod
-    async def save_webtoon_thumbnail(self, titleid: int, title: str, thumbnail_dir: Path) -> None:
-        """웹툰의 썸네일을 불러오고 thumbnail_dir에 저장한다."""
-
-    @abstractmethod
-    async def get_all_episode_no(self, titleid: int) -> Iterable:
-        """웹툰에서 전체 에피소드를 가져온다."""
+        if merge is not None:
+            print('Merging webtoon has started...')
+            fd = FolderManager()
+            print(webtoon_dir, fd)
+            fd.merge_webtoon_episodes(webtoon_dir, 5)
+            print('Merging webtoon ended.')
 
     def _check_validate_of_files(self, episode_dir: Path, episode_no: int, image_urls: list, subtitle: str) -> None | bool:
         """episode_dir를 생성하고 이미 있다면 해당 폴더 내 내용물이 적합한지 조사한다.
 
         None를 return한다면 회차를 다운로드해야 한다는 의미이다.
         True를 return하면 해당 회차가 이미 완전히 다운로드되어 있으며, 따라서 다운로드를 지속할 이유가 없음을 의미한다.
         """
@@ -267,52 +364,126 @@
                 self._set_pbar(f'{subtitle} is not vaild. Automatically restore files.')
                 shutil.rmtree(episode_dir)
                 episode_dir.mkdir()
             else:
                 self._set_pbar(f'skipping {subtitle}')
                 return True
 
-    async def download_one_episode(self, episode_no: int, titleid: int, webtoon_dir: Path) -> None:
+    async def download_one_episode(self, episode_no: int, titleid: TitleId, webtoon_dir: Path) -> None:
         """한 회차를 다운로드받는다."""
-        subtitle = await self.get_subtitle(titleid, episode_no, file_acceptable=True)
+        subtitle = self.get_safe_file_name(await self.get_subtitle(titleid, episode_no))
 
         if not subtitle:
             print(f'this episode is not free or not yet created. This episode won\'t be loaded. {episode_no=}')
             self._set_pbar('unknown episode')
             return
 
         episode_images_url = await self.get_episode_images_url(titleid, episode_no)
 
-        episode_dir = webtoon_dir / f'{episode_no:04d}. {subtitle}'
+        episode_dir = webtoon_dir / f'{episode_no + 1:04d}. {subtitle}'
         if self._check_validate_of_files(episode_dir, episode_no, episode_images_url, subtitle):
             return
 
         self._set_pbar(f'downloading {subtitle}')
         get_image_coroutines = (self.download_single_image(episode_dir, element, i) for i, element in enumerate(episode_images_url))
         await asyncio.gather(*get_image_coroutines)
 
-    @abstractmethod
-    async def get_subtitle(self, titleid: int, episode_no: int, file_acceptable: bool) -> str:
-        """부제목, 즉 회차의 제목을 불러온다."""
-
-    @abstractmethod
-    async def get_episode_images_url(self, titleid: int, episode_no: int) -> list:
-        """해당 회차를 구성하는 이미지들을 불러온다."""
-
     async def download_single_image(self, episode_dir: Path, url: str, image_no: int, default_file_extension: str | None = None) -> None:
         """Download image from url and returns to {episode_dir}/{file_name(translated to accactable name)}."""
         image_extension = self.get_file_extension(url)
 
         # for Bufftoon
         if image_extension is None:
-            if default_file_extension is not None:
+            if default_file_extension is None:
                 raise ValueError('File extension not detected.')
             image_extension = default_file_extension
 
         file_name = f'{image_no:03d}.{image_extension}'
 
         # self._set_pbar(f'{episode_dir}|{file_name}')
-        image_raw = await self.get_internet(get_type='requests', url=url, is_run_in_executor=True)
-        image_raw = image_raw.content
+        image_raw: bytes = (await self.get_internet(get_type='requests', url=url, is_run_in_executor=True)).content
 
         file_dir = episode_dir / file_name
         file_dir.write_bytes(image_raw)
+
+    @abstractmethod
+    async def get_all_episode_no(self, titleid: TitleId) -> list:
+        """웹툰에서 전체 에피소드를 가져온다."""
+        return (await self.get_webtoon_data(titleid))['episode_ids']
+
+    async def episode_no_to_episode_id(self, titleid: TitleId, episode_no: int, reverse: bool = False) -> int:
+        """reverse가 참일 경우 반대로 episode_id에서 episode_no를 불러옴."""
+        if not reverse:
+            return (await self.get_all_episode_no(titleid))[episode_no]
+        else:
+            return (await self.get_all_episode_no(titleid)).index(episode_no)
+
+    @abstractmethod
+    async def get_title(self, titleid: TitleId) -> str:
+        """웹툰의 title을 불러온다. 기본 구현을 사용할 시 super()를 이용하세요."""
+        return (await self.get_webtoon_data(titleid))['title']
+
+    @abstractmethod
+    async def get_subtitle(self, titleid: TitleId, episode_no: int) -> str:
+        """부제목, 즉 회차의 제목을 불러온다. 기본 구현을 사용할 시 super()를 이용하세요."""
+        return (await self.get_webtoon_data(titleid))['subtitles'][episode_no]
+
+    @abstractmethod
+    async def save_webtoon_thumbnail(self, titleid: TitleId, title: str, thumbnail_dir: Path) -> None:
+        """웹툰의 썸네일을 불러오고 thumbnail_dir에 저장합니다. 기본 구현을 사용할 시 super()를 이용하세요."""
+        thumbnail_data: str | tuple[bytes, str] = (await self.get_webtoon_data(titleid))['webtoon_thumbnail']
+        if isinstance(thumbnail_data, str):  # It means thumnail_data is URL
+            image_extension = self.get_file_extension(thumbnail_data)
+            image_raw = (await self.get_internet(get_type='requests', url=thumbnail_data)).content
+        elif isinstance(thumbnail_data, tuple):  # It means thumnail_data is raw image data
+            image_raw, image_extension = thumbnail_data
+        else:
+            raise ValueError('Thumbnail_data is invalid; It must be string or bytes.')
+
+        image_path = thumbnail_dir / f'{title}.{image_extension}'
+        image_path.write_bytes(image_raw)
+
+    @abstractmethod
+    async def get_episode_images_url(self, titleid: TitleId, episode_no: int) -> list:
+        """해당 회차를 구성하는 이미지들을 불러온다. 기본 구현을 사용할 시 super()를 이용하세요."""
+        return (await self.get_webtoon_data(titleid))['episode_images_url'][episode_no]
+
+    @overload
+    async def get_webtoon_data(self, titleid: TitleId) -> dict[Literal['title'], str]: ... # noqa
+
+    @overload
+    async def get_webtoon_data(self, titleid: TitleId) -> dict[Literal['subtitles'], list[str]]: ... # noqa
+
+    @overload
+    async def get_webtoon_data(self, titleid: TitleId) -> dict[Literal['webtoon_thumbnail'], str | tuple[bytes | str]]: ... # noqa
+
+    @overload
+    async def get_webtoon_data(self, titleid: TitleId) -> dict[Literal['episode_images_url'], list[list[str]]]: ... # noqa
+
+    @overload
+    async def get_webtoon_data(self, titleid: TitleId) -> dict[Literal['episode_ids'], list[str]]: ... # noqa
+
+    @abstractmethod
+    @alru_cache(maxsize=4)
+    async def get_webtoon_data(self, titleid: TitleId) \
+        -> dict[Literal['title', 'subtitles', 'webtoon_thumbnail', 'episode_images_url', 'episode_ids'],
+                list[str] | list[list[str]] | str | bytes | tuple[bytes | str]]:
+        """웹툰에서 데이터를 불러옵니다. 많이 불리기 때문에 무조건 @lru_cache를 사용해야 합니다.
+
+        Args:
+            titleid (TitleId): titleid를 받습니다.
+
+        Returns:
+            dict: key에 따라 각각 자동으로 불러올 정보를 정의합니다.
+                keys:
+                    'title' (str): 웹툰의 제목 정보를 불러옵니다.
+                    'subtitles' (list[str]): 웹툰의 부제목(에피소드 제목) 정보를 불러옵니다.
+                    'webtoon_thumbnail' (str/tuple[bytes, str]): 웹툰의 썸네일 정보를 불러옵니다.
+                        만약 값이 string일 경우는 URL로 추론하고 URL에서 정보를 불러오지만,
+                        tuple일 경우에는 thumbnail raw data와 file extension으로 추론하고 thumbnail_dir에 저장합니다.
+                    'episode_ids' (list(int)): episode id list를 불러옵니다.
+                    'episode_images_url' (list[list[str]]): 실제 웹툰 이미지들의 url로 구성된 list입니다.
+                        다만 이렇게 많은 양을 메모리에 올려놓는 것은 부담이 될 수 있습니다.
+                이 key 중에서 없는 것이 있어도 상관 없습니다. 다만 그럴 경우 직접 구현하여야 합니다.
+                만약 함수들이 독립적이고 각자 구현될 수 있다면 한 데에 모아 구현하는 것보다 각각에 해당하는 함수들에
+                구현하고 super()를 이용하는 것이 합리적입니다.
+        """
```

### Comparing `WebtoonScraper-1.0.2/WebtoonScraper/TelescopeScraper.py` & `WebtoonScraper-1.1.1/WebtoonScraper/F_WebtoonOriginalsScraper.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,100 +1,98 @@
-"""Download Webtoons from Manhwakyung."""
-import time
 
+'''Download Webtoons from Webtoon Originals.
+'''
+from bs4 import BeautifulSoup as bs
 from async_lru import alru_cache
 
-if __name__ == "__main__":
-    from Scraper import Scraper
+if __name__ in ("__main__", "F_WebtoonOriginalsScraper"):
+    from C_Scraper import Scraper
 else:
-    from .Scraper import Scraper
+    from .C_Scraper import Scraper
 
 
-class TelescopeScraper(Scraper):
-    """Scrape webtoons from Manhwakyung."""
-
-    def __init__(self, pbar_independent=False, short_connection=False):
-        super().__init__(pbar_independent, short_connection)
-        self.BASE_URL = 'https://www.manhwakyung.com'
+class WebtoonOriginalsScraper(Scraper):
+    '''Scrape webtoons from Webtoon Originals.'''
+    def __init__(self, pbar_independent=False):
+        super().__init__(pbar_independent)
+        self.BASE_URL = 'https://www.webtoons.com/en/fantasy/watermelon'
         self.IS_STABLE_CONNECTION = False
-        self.TIMEOUT = 3
+        self.HEADERS = {
+            'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/113.0.0.0 Safari/537.36',
+            "Referer": "http://www.webtoons.com"
+        }
 
-    async def download_one_webtoon_async(self, titleid, episode_no_range: tuple | int | None = None):
-        self.title, self.list_thumbnail_url, self.grid_thumbnail_url, self.episode_infomation = await self._get_webtoon_infomation(titleid)
-        await super().download_one_webtoon_async(titleid, episode_no_range)
+    async def get_title(self, titleid):
+        url = f'{self.BASE_URL}/list?title_no={titleid}'
+        title = await self.get_internet(get_type='soup_select_one', url=url,
+                                        selector='meta[property="og:title"]')
+        if not title:
+            raise ConnectionError('Webtoon Originals changed their api specification. Contect developer to update get_title.')
+        return title['content']
 
     @alru_cache(maxsize=4)
-    async def _get_webtoon_infomation(self, titleid):
-        XHR_HEADER = {
-            "authority": 'api.manhwakyung.com',
-            "method": 'GET',
-            "path": f'/episodes?titleId={titleid}',
-            "scheme": 'https',
-            "accept": 'application/json, text/plain, */*',
-            "accept-encoding": 'gzip, deflate, br',
-            "accept-language": 'ko,en-US;q=0.9,en;q=0.8',
-            "dnt": '1',
-            "main-domain": 'MANHWAKYUNG',
-            "origin": 'https://www.manhwakyung.com',
-            "referer": 'https://www.manhwakyung.com/',
-            "sec-ch-ua": '"Microsoft Edge";v="113", "Chromium";v="113", "Not-A.Brand";v="24"',
-            "sec-ch-ua-mobile": '?0',
-            "sec-ch-ua-platform": '"Windows"',
-            "sec-fetch-dest": 'empty',
-            "sec-fetch-mode": 'cors',
-            "sec-fetch-site": 'same-site',
-            "sec-gpc": '1',
-            "user-agent": 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/113.0.0.0 Safari/537.36 Edg/113.0.1774.57',
-            "version": '3'
-        }
-        seasons = await self.get_internet('requests', f'https://api.manhwakyung.com/episodes?titleId={titleid}', headers=XHR_HEADER)
-        seasons = seasons.json()
-        episodes = []
-        for season in seasons['seasons']:
-            episodes += season['episodes']
-
-        # about webtoon
-        title = episodes[0]['title']['name']
-        list_thumbnail_url = episodes[0]['title']['listThumbnailImageUrl']
-        grid_thumbnail_url = episodes[0]['title']['gridThumbnailImageUrl']
-
-        # about episode
-        episode_infomation = {}
-        for episode in episodes:
-            subtitle = episode['name']
-            episode_no = episode['episodeNumber']
-            episode_id = episode['id']
-            episode_infomation[episode_no] = {'subtitle': subtitle, 'episode_id': episode_id}
-
-        return title, list_thumbnail_url, grid_thumbnail_url, episode_infomation
+    async def get_webtoon_data(self, titleid):
+        # getting title_no
+        url = f'{self.BASE_URL}/list?title_no={titleid}'
+        title_no_tag = await self.get_internet('soup_select_one', url, '#_listUl > li')
+        if not title_no_tag:
+            raise ConnectionError('Webtoon Originals changed their api specification. Contect developer to update get_title.')
+        title_no = int(title_no_tag['data-episode-no'])
+
+        # getting list of titles
+        selector = '#_bottomEpisodeList > div.episode_cont > ul > li'
+        url = f'{self.BASE_URL}/prologue/viewer?title_no={titleid}&episode_no={title_no}'
+        selected = await self.get_internet(get_type='soup_select', url=url,
+                                           selector=selector)
+
+        subtitles = []
+        episode_ids = []
+        for element in selected:
+            episode_no = int(element["data-episode-no"])
+            # subtitles[episode_no] = element.select_one("span.subj").text
+            subtitles.append(element.select_one("span.subj").text)
+            episode_ids.append(episode_no)
 
-    async def get_title(self, titleid, file_acceptable):
-        return self.title
+        return {'subtitles': subtitles, 'episode_ids': episode_ids}
 
     async def save_webtoon_thumbnail(self, titleid, title, thumbnail_dir):
-        image_url = self.grid_thumbnail_url
+        url = f'{self.BASE_URL}/list?title_no={titleid}'
+        image_url_original = await self.get_internet(get_type='soup_select_one', url=url,
+                                                     selector='meta[property="og:image"]')
+        if not image_url_original:
+            raise ConnectionError('Webtoon Originals changed their api specification. Contect developer to update get_title.')
+        image_url: str = image_url_original['content']
         image_extension = self.get_file_extension(image_url)
         image_raw = await self.get_internet(get_type='requests', url=image_url)
         image_raw = image_raw.content
         thumbnail_file = thumbnail_dir / f'{title}.{image_extension}'
         thumbnail_file.write_bytes(image_raw)
 
+    async def save_real_webtoon_thumbnail(self, titleid, title, thumbnail_dir):
+        '''save another form of thumbnail.'''
+        url = f'{self.BASE_URL}/rss?title_no={titleid}'
+        response = await self.get_internet(get_type='requests', url=url)
+        soup = bs(response.text, 'xml')
+        image_url = soup.select_one('channel > image > url').text
+        image_extension = self.get_file_extension(image_url)
+        image_raw = await self.get_internet(get_type='requests', url=image_url)
+        image_raw = image_raw.content
+        thumbnail_path = thumbnail_dir / f'{title}.{image_extension}'
+        thumbnail_path.write_bytes(image_raw)
+
     async def get_all_episode_no(self, titleid):
-        return reversed(self.episode_infomation)
+        return await super().get_all_episode_no(titleid)
 
-    async def get_subtitle(self, titleid, episode_no, file_acceptable):
-        time.sleep(1)
-        subtitle = self.episode_infomation[episode_no]['subtitle']
-        if file_acceptable:
-            subtitle = self.get_acceptable_file_name(subtitle)
-        return subtitle
+    async def get_subtitle(self, titleid, episode_no):
+        return await super().get_subtitle(titleid, episode_no)
 
     async def get_episode_images_url(self, titleid, episode_no):
-        episode_id = self.episode_infomation[episode_no]['episode_id']
-        elemetents = await self.get_internet('soup_select', f'https://www.manhwakyung.com/episode/{episode_id}',
-                                             '#__next > div.css-0.euvlwci0 > div.css-0.ebi66ty0 > div > div > img')
-        return [element.get('data-src') for element in elemetents]
+        episode_id = await self.episode_no_to_episode_id(titleid, episode_no)
+        url = f'{self.BASE_URL}/prologue/viewer?title_no={titleid}&episode_no={episode_id}'
+        episode_images_url = await self.get_internet(get_type='soup_select', url=url,
+                                                     selector='#_imageList > img')
+        return [element['data-url'] for element in episode_images_url]
 
 
 if __name__ == '__main__':
-    wt = TelescopeScraper()
-    wt.download_one_webtoon(137)  # 물망초
+    wt = WebtoonOriginalsScraper()
+    wt.download_one_webtoon(5291)  # Wumpus
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `WebtoonScraper-1.0.2/WebtoonScraper/Webtoon.py` & `WebtoonScraper-1.1.1/WebtoonScraper/B_Webtoon.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 """Download webtoons automatiallly or easily"""
 
 import asyncio
 import contextlib
 from itertools import starmap
 
-if __name__ == "__main__":
-    from NaverWebtoonScraper import NaverWebtoonScraper
-    from FolderManager import FolderManager
-    from WebtoonOriginalsScraper import WebtoonOriginalsScraper
-    from BestChallengeScraper import BestChallengeScraper
-    from WebtoonCanvasScraper import WebtoonCanvasScraper
-    from TelescopeScraper import TelescopeScraper
-    from BufftoonScraper import BufftoonScraper
-    from NaverPostScraper import NaverPostScraper
-    from NaverGameScraper import NaverGameScraper
+if __name__ in ("__main__", "B_Webtoon"):
+    from A_FolderManager import FolderManager
+    from D_NaverWebtoonScraper import NaverWebtoonScraper
+    from E_BestChallengeScraper import BestChallengeScraper
+    from F_WebtoonOriginalsScraper import WebtoonOriginalsScraper
+    from G_WebtoonCanvasScraper import WebtoonCanvasScraper
+    from H_TelescopeScraper import TelescopeScraper
+    from I_BufftoonScraper import BufftoonScraper
+    from J_NaverPostScraper import NaverPostScraper
+    from K_NaverGameScraper import NaverGameScraper
 else:
-    from .NaverWebtoonScraper import NaverWebtoonScraper
-    from .FolderManager import FolderManager
-    from .WebtoonOriginalsScraper import WebtoonOriginalsScraper
-    from .BestChallengeScraper import BestChallengeScraper
-    from .WebtoonCanvasScraper import WebtoonCanvasScraper
-    from .TelescopeScraper import TelescopeScraper
-    from .BufftoonScraper import BufftoonScraper
-    from .NaverPostScraper import NaverPostScraper
-    from .NaverGameScraper import NaverGameScraper
+    from .A_FolderManager import FolderManager
+    from .D_NaverWebtoonScraper import NaverWebtoonScraper
+    from .E_BestChallengeScraper import BestChallengeScraper
+    from .F_WebtoonOriginalsScraper import WebtoonOriginalsScraper
+    from .G_WebtoonCanvasScraper import WebtoonCanvasScraper
+    from .H_TelescopeScraper import TelescopeScraper
+    from .I_BufftoonScraper import BufftoonScraper
+    from .J_NaverPostScraper import NaverPostScraper
+    from .K_NaverGameScraper import NaverGameScraper
 
 N = NAVER_WEBTOON = 'naver_webtoon'
 B = BEST_CHALLENGE = 'best_challenge'
-O = ORIGINALS = 'originals'
+O = ORIGINALS = 'originals'  # noqa
 C = CANVAS = 'canvas'
 T = M = TELESCOPE = 'telescope'
 BF = BUFFTOON = 'bufftoon'
 P = POST = NAVER_POST = 'naver_post'
 G = NAVER_GAME = 'naver_game'
 
 
-async def get_webtoon_platform(webtoon_id: int, is_auto_select=False) -> str:
+async def get_webtoon_platform(webtoon_id: int, is_auto_select=False) -> str | None:  # noqa
     # sourcery skip: low-code-quality
     """If webtoon is best challenge, this returns True. Otherwise, False."""
     loop = asyncio.get_running_loop()
 
     async def skip_when_errored(func, platform_name):
         try:
             # await func()
@@ -48,14 +48,15 @@
         except Exception as e:
             print(f'An error occured. Skipping {platform_name}')
             print(f'error: {e}')
 
     available_webtoon = []
     # 네이버 게임은 제목을 받는 데 특수한 함수가 필요하기 때문에 이 클래스를 이용
     webtoonscraper = NaverGameScraper()
+    webtoonscraper.IS_STABLE_CONNECTION = False
 
     # 네이버 웹툰
     async def naver_webtoon_fetch():
         title = await webtoonscraper.get_internet('soup_select_one', f'https://comic.naver.com/webtoon/detail?titleId={webtoon_id}', 'span.text')
         with contextlib.suppress(AttributeError):
             title = title.text
             if title:
@@ -71,23 +72,23 @@
             if title:
                 available_webtoon.append((BEST_CHALLENGE, title))
     # await skip_when_errored(best_challenge_fetch, BEST_CHALLENGE)
 
     # 만화경
     async def telescope_fetch():
         title = await webtoonscraper.get_internet('soup_select_one', f'https://www.manhwakyung.com/title/{webtoon_id}', 'meta[property="og:title"]')
-        title = title["content"][:-6]
+        title = title["content"].removesuffix(' | 만화경')
         title = None if title == "에러 페이지" else title
         if title:
             available_webtoon.append((TELESCOPE, title))
     # await skip_when_errored(telescope_fetch, TELESCOPE)
 
     # 버프툰
     async def bufftoon_fetch():
-        title = await webtoonscraper.get_internet('soup_select_one', f'https://bufftoon.plaync.com/series/{webtoon_id}', 'meta[property="og:title"]')
+        title = (await webtoonscraper.get_internet('soup_select_one', f'https://bufftoon.plaync.com/series/{webtoon_id}', 'meta[property="og:title"]'))
         title = title["content"]
         title = None if title == "이야기 던전에 입장하라, 버프툰" else title
         if title:
             available_webtoon.append((BUFFTOON, title))
     # await skip_when_errored(bufftoon_fetch, BUFFTOON)
 
     # 네이버 게임
@@ -97,16 +98,17 @@
             if title:
                 available_webtoon.append((NAVER_GAME, title))
         webtoonscraper.IS_STABLE_CONNECTION = False
     # await skip_when_errored(naver_game_fetch, NAVER_GAME)
 
     # originals
     async def originals_fetch():
-        title = await webtoonscraper.get_internet('soup_select_one', f'https://www.webtoons.com/en/fantasy/watermelon/list?title_no={webtoon_id}',
-                                                  'meta[property="og:title"]')
+        title_original = (await webtoonscraper.get_internet('soup_select_one', f'https://www.webtoons.com/en/fantasy/watermelon/list?title_no={webtoon_id}',
+                                                            'meta[property="og:title"]'))
+        title = title_original['content'] if title_original is not None else None
         if title:
             available_webtoon.append((ORIGINALS, title))
     # await skip_when_errored(originals_fetch, ORIGINALS)
 
     # canvas
     async def canvas_fetch():
         title = await webtoonscraper.get_internet('soup_select_one', f'https://www.webtoons.com/en/challenge/meme-girls/list?title_no={webtoon_id}',
@@ -127,23 +129,23 @@
             (originals_fetch, ORIGINALS),
             (canvas_fetch, CANVAS)
         )
     )
     await asyncio.gather(*webtoon_getters)
 
     # 베스트 도전과 네이버 웹툰이 겹치고 둘의 제목이 같을 경우 베스트 도전을 배제함.
+    nw_title, bc_title, bc_order = None, None, 0
     for i, (platform, title) in enumerate(available_webtoon):
         if platform == NAVER_WEBTOON:
             nw_title = title
         if platform == BEST_CHALLENGE:
             bc_title = title
             bc_order = i
-    with contextlib.suppress(UnboundLocalError):
-        if nw_title == bc_title:
-            del available_webtoon[bc_order]
+    if nw_title == bc_title != None:  # noqa
+        del available_webtoon[bc_order]
 
     if (webtoon_length := len(available_webtoon)) == 1:
         print(f'Webtoon\'s platform is assumed to be {available_webtoon[0][0]}')
         return available_webtoon[0][0]
     elif webtoon_length == 0:
         print(f'There\'s no webtoon that webtoon ID is {webtoon_id}.')
     else:
@@ -154,15 +156,15 @@
                 platform_no = input('Multiple webtoon is searched. Please type number of webtoon you want to download(enter nothing to select no.1): ')
             else:
                 platform_no = ''
             platform_no = 1 if platform_no == '' else int(platform_no)
             try:
                 selected_platform, selected_webtoon = available_webtoon[platform_no - 1]
             except IndexError:
-                print('Exceeded the range of webtoons.')
+                raise ValueError('Exceeded the range of webtoons.')
             print(f'Webtoon {selected_webtoon} is selected.')
             return selected_platform
         except ValueError as e:
             raise ValueError('Webtoon ID should be integer.') from e
 
 
 async def get_scraper_instance(webtoon_type: str):
@@ -179,53 +181,76 @@
     elif webtoon_type.lower() == BUFFTOON:
         webtoonscraper = BufftoonScraper()
     elif webtoon_type.lower() == NAVER_POST:
         webtoonscraper = NaverPostScraper()
     elif webtoon_type.lower() == NAVER_GAME:
         webtoonscraper = NaverGameScraper()
     else:
-        raise ValueError('webtoon_type should be among naver_webtoon, best_challenge, originals, canvas, telescope, and naver_game.')
+        raise ValueError('webtoon_type should be among naver_webtoon, best_challenge, originals, canvas, bufftoon, telescope, naver_post, and naver_game.')
     return webtoonscraper
 
 
 async def get_webtoon_async(
-        webtoon_id: int,
+        webtoon_id: int | tuple[int, int],
         webtoon_type: None | str = None,
         *,
         merge: None | int = None,
         cookie: None | str = None,
-        member_no: None | int = None,
-        is_auto_select=False
+        is_auto_select=False,
+        episode_no_range: tuple[int, int] | int | None = None,
 ) -> None:
-
-    if webtoon_type is None:
-        webtoon_type = await get_webtoon_platform(webtoon_id, is_auto_select)
-    webtoonscraper = await get_scraper_instance(webtoon_type)
-    if webtoon_type.lower() == BUFFTOON or cookie is not None:
-        if cookie is None:
+    def set_cookie(cookie):
+        webtoonscraper = BufftoonScraper()
+        if cookie:
             webtoonscraper.COOKIE = cookie
         else:
             webtoonscraper.COOKIE = input(f'Enter cookie of {webtoon_id} (Enter nothing to proceed without cookie): ')
-    if webtoon_type.lower() == NAVER_POST or member_no is not None:
-        if not member_no:
-            member_no = int(input(f'Enter memberNo of {webtoon_id}: '))
-        await webtoonscraper.download_one_webtoon_async(titleid=webtoon_id, member_no=member_no)
+        return webtoonscraper
+
+    if cookie is None:
+        if isinstance(webtoon_id, tuple):
+            webtoon_type = NAVER_POST
+        elif webtoon_type is None:
+            webtoon_type = await get_webtoon_platform(webtoon_id, is_auto_select)
+            if webtoon_type is None:
+                raise ValueError('You must select item.')
+
+        if webtoon_type.lower() == BUFFTOON:
+            webtoonscraper = set_cookie(cookie)
+        else:
+            webtoonscraper = await get_scraper_instance(webtoon_type)
     else:
-        await webtoonscraper.download_one_webtoon_async(titleid=webtoon_id)
-    if merge:
-        fd = FolderManager()
-        fd.merge_webtoon_episodes(webtoonscraper.webtoon_dir)
+        webtoonscraper = set_cookie(cookie)
+
+    # if webtoon_type is None and cookie is None:
+    #     if isinstance(webtoon_id, tuple):
+    #         webtoon_type = NAVER_POST
+    #     else:
+    #         webtoon_type = await get_webtoon_platform(webtoon_id, is_auto_select)
+    #         if webtoon_type is None:
+    #             raise ValueError('You must select item.')
+
+    # if cookie is not None or webtoon_type.lower() == BUFFTOON:
+    #     webtoonscraper = await get_scraper_instance(BUFFTOON)
+    #     if cookie:
+    #         webtoonscraper.COOKIE = cookie
+    #     else:
+    #         webtoonscraper.COOKIE = input(f'Enter cookie of {webtoon_id} (Enter nothing to proceed without cookie): ')
+    # else:
+    #     webtoonscraper = await get_scraper_instance(webtoon_type)
 
+    await webtoonscraper.download_one_webtoon_async(webtoon_id, episode_no_range, merge=merge)
 
 def get_webtoon(
     webtoon_id: int,
     webtoon_type: str | None = None,
     *,
-    merge: None | int | bool = None,
+    merge: None | int = None,
     cookie: None | str = None,
-    member_no: None | int = None
+    episode_no_range: tuple[int, int] | int | None = None,
 ) -> None:
-    asyncio.run(get_webtoon_async(webtoon_id, webtoon_type, merge=merge, cookie=cookie, member_no=member_no))
+    asyncio.run(get_webtoon_async(webtoon_id, webtoon_type, merge=merge, cookie=cookie, episode_no_range=episode_no_range))
 
 
 if __name__ == '__main__':
-    asyncio.run(get_webtoon_platform(18))  # 네이버 게임
+    # asyncio.run(get_webtoon_platform(18))  # 네이버 게임
+    asyncio.run(get_webtoon_platform(1022))  # 오리지널스
```

### Comparing `WebtoonScraper-1.0.2/WebtoonScraper/WebtoonOriginalsScraper.py` & `WebtoonScraper-1.1.1/WebtoonScraper/H_TelescopeScraper.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,97 +1,93 @@
-'''Download Webtoons from Webtoon Originals.
-'''
-from bs4 import BeautifulSoup as bs
+"""Download Webtoons from Manhwakyung."""
+import time
+
 from async_lru import alru_cache
 
-if __name__ == "__main__":
-    from Scraper import Scraper
+if __name__ in ("__main__", "H_TelescopeScraper"):
+    from C_Scraper import Scraper
 else:
-    from .Scraper import Scraper
+    from .C_Scraper import Scraper
 
 
-class WebtoonOriginalsScraper(Scraper):
-    '''Scrape webtoons from Webtoon Originals.'''
-    def __init__(self, pbar_independent=False, short_connection=False):
-        super().__init__(pbar_independent, short_connection)
-        self.BASE_URL = 'https://www.webtoons.com/en/fantasy/watermelon'
-        self.IS_STABLE_CONNECTION = False
-        self.USER_AGENT = {
-            'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/113.0.0.0 Safari/537.36',
-            "Referer": "http://www.webtoons.com"
-        }
+class TelescopeScraper(Scraper):
+    """Scrape webtoons from Manhwakyung."""
 
-    async def get_title(self, titleid, file_acceptable):
-        url = f'{self.BASE_URL}/list?title_no={titleid}'
-        title = await self.get_internet(get_type='soup_select_one', url=url,
-                                        selector='meta[property="og:title"]')
-        title = title['content']
-        if file_acceptable:
-            title = self.get_acceptable_file_name(title)
-        return title
+    def __init__(self, pbar_independent=False):
+        super().__init__(pbar_independent)
+        self.BASE_URL = 'https://www.manhwakyung.com'
+        self.IS_STABLE_CONNECTION = False
+        self.TIMEOUT = 3
 
     @alru_cache(maxsize=4)
-    async def _get_webtoon_infomation(self, titleid):
-        # getting title_no
-        url = f'{self.BASE_URL}/list?title_no={titleid}'
-        title_no = await self.get_internet('soup_select_one', url, '#_listUl > li')
-        title_no = int(title_no['data-episode-no'])
-
-        # getting list of titles
-        selector = '#_bottomEpisodeList > div.episode_cont > ul > li'
-        url = f'{self.BASE_URL}/prologue/viewer?title_no={titleid}&episode_no={title_no}'
-        selected = await self.get_internet(get_type='soup_select', url=url,
-                                           selector=selector)
-
-        subtitles = {}
-        for element in selected:
-            episode_no = int(element["data-episode-no"])
-            subtitles[episode_no] = element.select_one("span.subj").text
+    async def get_webtoon_data(self, titleid):
+        XHR_HEADER = {
+            "authority": 'api.manhwakyung.com',
+            "method": 'GET',
+            "path": f'/episodes?titleId={titleid}',
+            "scheme": 'https',
+            "accept": 'application/json, text/plain, */*',
+            "accept-encoding": 'gzip, deflate, br',
+            "accept-language": 'ko,en-US;q=0.9,en;q=0.8',
+            "dnt": '1',
+            "main-domain": 'MANHWAKYUNG',
+            "origin": 'https://www.manhwakyung.com',
+            "referer": 'https://www.manhwakyung.com/',
+            "sec-ch-ua": '"Microsoft Edge";v="113", "Chromium";v="113", "Not-A.Brand";v="24"',
+            "sec-ch-ua-mobile": '?0',
+            "sec-ch-ua-platform": '"Windows"',
+            "sec-fetch-dest": 'empty',
+            "sec-fetch-mode": 'cors',
+            "sec-fetch-site": 'same-site',
+            "sec-gpc": '1',
+            "user-agent": 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/113.0.0.0 Safari/537.36 Edg/113.0.1774.57',
+            "version": '3'
+        }
+        seasons = await self.get_internet('requests', f'https://api.manhwakyung.com/episodes?titleId={titleid}', headers=XHR_HEADER)
+        seasons = seasons.json()
+        episodes = []
+        for season in seasons['seasons']:
+            episodes += season['episodes']
+
+        # about webtoon
+        title = episodes[0]['title']['name']
+        list_thumbnail_url = episodes[0]['title']['listThumbnailImageUrl']
+        grid_thumbnail_url = episodes[0]['title']['gridThumbnailImageUrl']
+
+        # about episode
+        subtitles = []
+        episode_ids = []
+        for episode in episodes:
+            subtitle = episode['name']
+            episode_no = episode['episodeNumber']
+            episode_id = episode['id']
+            # episode_infomation[episode_no] = {'subtitle': subtitle, 'episode_id': episode_id}
+            subtitles.append(subtitle)
+            episode_ids.append(episode_id)
+
+        # list_thumbnail_url
+        return {'title': title, 'webtoon_thumbnail': grid_thumbnail_url, 'subtitles': subtitles[::-1], 'episode_ids': episode_ids[::-1]}
 
-        return subtitles
+    async def get_title(self, titleid):
+        return await super().get_title(titleid)
 
     async def save_webtoon_thumbnail(self, titleid, title, thumbnail_dir):
-        url = f'{self.BASE_URL}/list?title_no={titleid}'
-        image_url = await self.get_internet(get_type='soup_select_one', url=url,
-                                            selector='meta[property="og:image"]')
-        image_url = image_url['content']
-        image_extension = self.get_file_extension(image_url)
-        image_raw = await self.get_internet(get_type='requests', url=image_url)
-        image_raw = image_raw.content
-        thumbnail_file = thumbnail_dir / f'{title}.{image_extension}'
-        thumbnail_file.write_bytes(image_raw)
-
-    async def save_real_webtoon_thumbnail(self, titleid, title, thumbnail_dir):
-        '''save another form of thumbnail.'''
-        url = f'{self.BASE_URL}/rss?title_no={titleid}'
-        response = await self.get_internet(get_type='requests', url=url)
-        soup = bs(response.text, 'xml')
-        image_url = soup.select_one('channel > image > url').text
-        image_extension = self.get_file_extension(image_url)
-        image_raw = await self.get_internet(get_type='requests', url=image_url)
-        image_raw = image_raw.content
-        thumbnail_path = thumbnail_dir / f'{title}.{image_extension}'
-        thumbnail_path.write_bytes(image_raw)
+        return await super().save_webtoon_thumbnail(titleid, title, thumbnail_dir)
 
     async def get_all_episode_no(self, titleid):
-        subtitles = await self._get_webtoon_infomation(titleid)
-        return list(subtitles)
+        return await super().get_all_episode_no(titleid)
 
-    async def get_subtitle(self, titleid, episode_no, file_acceptable):
-        subtitles = await self._get_webtoon_infomation(titleid)
-        subtitle = subtitles[episode_no]
-
-        return self.get_acceptable_file_name(subtitle) if file_acceptable else subtitle
+    async def get_subtitle(self, titleid, episode_no):
+        time.sleep(1)  # 없으면 작동 안 함.
+        return await super().get_subtitle(titleid, episode_no)
 
     async def get_episode_images_url(self, titleid, episode_no):
-        url = f'{self.BASE_URL}/prologue/viewer?title_no={titleid}&episode_no={episode_no}'
-        episode_images_url = await self.get_internet(get_type='soup_select', url=url,
-                                                     selector='#_imageList > img')
-        return [
-            element['data-url']
-            for element in episode_images_url
-            if not ('agerate' in element['src'] or 'ctguide' in element['src'])
-        ]
+        # episode_id: int = (await self.get_webtoon_data(titleid))['episode_ids'][episode_no]
+        episode_id: int = await self.episode_no_to_episode_id(titleid, episode_no)
+        elemetents = await self.get_internet('soup_select', f'https://www.manhwakyung.com/episode/{episode_id}',
+                                             '#__next > div.css-0.euvlwci0 > div.css-0.ebi66ty0 > div > div > img')
+        return [element.get('data-src') for element in elemetents]
+
 
 if __name__ == '__main__':
-    wt = WebtoonOriginalsScraper()
-    wt.download_one_webtoon(5291)  # Wumpus
+    wt = TelescopeScraper()
+    wt.download_one_webtoon(137)  # 물망초
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `WebtoonScraper-1.0.2/WebtoonScraper/__init__.py` & `WebtoonScraper-1.1.1/WebtoonScraper/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 if __name__ == "__main__":
-    from NaverWebtoonScraper import NaverWebtoonScraper
-    from FolderManager import FolderManager
-    from WebtoonOriginalsScraper import WebtoonOriginalsScraper
-    from BestChallengeScraper import BestChallengeScraper
-    from WebtoonCanvasScraper import WebtoonCanvasScraper
-    import Webtoon
-    from TelescopeScraper import TelescopeScraper
-    from BufftoonScraper import BufftoonScraper
-    from NaverPostScraper import NaverPostScraper
-    from NaverGameScraper import NaverGameScraper
+    from A_FolderManager import FolderManager
+    import B_Webtoon as Webtoon
+    from D_NaverWebtoonScraper import NaverWebtoonScraper
+    from E_BestChallengeScraper import BestChallengeScraper
+    from F_WebtoonOriginalsScraper import WebtoonOriginalsScraper
+    from G_WebtoonCanvasScraper import WebtoonCanvasScraper
+    from H_TelescopeScraper import TelescopeScraper
+    from I_BufftoonScraper import BufftoonScraper
+    from J_NaverPostScraper import NaverPostScraper
+    from K_NaverGameScraper import NaverGameScraper
 else:
-    from .NaverWebtoonScraper import NaverWebtoonScraper
-    from .FolderManager import FolderManager
-    from .WebtoonOriginalsScraper import WebtoonOriginalsScraper
-    from .BestChallengeScraper import BestChallengeScraper
-    from .WebtoonCanvasScraper import WebtoonCanvasScraper
-    from . import Webtoon
-    from .TelescopeScraper import TelescopeScraper
-    from .BufftoonScraper import BufftoonScraper
-    from .NaverPostScraper import NaverPostScraper
-    from .NaverGameScraper import NaverGameScraper
+    from .A_FolderManager import FolderManager
+    from . import B_Webtoon as Webtoon
+    from .D_NaverWebtoonScraper import NaverWebtoonScraper
+    from .E_BestChallengeScraper import BestChallengeScraper
+    from .F_WebtoonOriginalsScraper import WebtoonOriginalsScraper
+    from .G_WebtoonCanvasScraper import WebtoonCanvasScraper
+    from .H_TelescopeScraper import TelescopeScraper
+    from .I_BufftoonScraper import BufftoonScraper
+    from .J_NaverPostScraper import NaverPostScraper
+    from .K_NaverGameScraper import NaverGameScraper
 
 if __name__ == '__main__':
     print('Testing codes.')
```

### Comparing `WebtoonScraper-1.0.2/WebtoonScraper.egg-info/PKG-INFO` & `WebtoonScraper-1.1.1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,7 @@
-Metadata-Version: 2.1
-Name: WebtoonScraper
-Version: 1.0.2
-Summary: Scraping webtoons and some utils for it
-Home-page: https://github.com/ilotoki0804/WebtoonScraper
-Author: ilotoki0804
-Author-email: ilotoki0804@gmail.com
-License: MIT
-Keywords: Webtoon,Webtoon Scraper,Naver Webtoon,Webtoon Downloader,Download Webtoon
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-이 설명은 최신 버전이 아닐 수 있습니다. 만약 최신 버전을 확인하고 싶으시다면 [여기](https://github.com/ilotoki0804/WebtoonScraper)를 참고하세요.
 # WebtoonScraper
 
 웹툰을 다운로드하는 프로젝트입니다.
 
 네이버 웹툰, 베스트 도전만화, 웹툰 오리지널, 웹툰 캔버스, 만화경, 버프툰, 네이버 포스트, 네이버 게임을 지원합니다.
 
 # 시작하기
@@ -31,46 +13,60 @@
    ```
 
 # 네이버 웹툰, 베스트 도전만화, 웹툰 오리지널, 웹툰 캔버스, 만화경, 네이버 게임 다운로드하기
 
 버프툰과 네이버 포스트는 아래로 가서 확인하세요.
 
 1. 원하는 웹툰으로 가서 titleid 또는 title_no를 복사하세요.
-   ![img](https://raw.githubusercontent.com/ilotoki0804/WebtoonScraper/master/images/naver_webtoon.png)
-   네이버 웹툰과 베스트 도전의 경우 여기에서,
-   ![img](https://raw.githubusercontent.com/ilotoki0804/WebtoonScraper/master/images/webtoons_original.png)
-   웹툰 오리지널과 캔버스의 경우는 여기에서,
-   ![img](https://raw.githubusercontent.com/ilotoki0804/WebtoonScraper/master/images/manhwakyung.png)
-   만화경의 경우는 여기에서,
-   ![img](https://raw.githubusercontent.com/ilotoki0804/WebtoonScraper/master/images/naver_game.png)
-   네이버 게임 오리지널 시리즈의 경우는 여기에서 확인할 수 있습니다.
+   네이버 웹툰/베스트 도전(comic.naver.com):
+   ![img](images/naver_webtoon.png)
+   웹툰 오리지널/캔버스(webtoons.com):
+   ![img](images/webtoons_original.png)
+   만화경(manhwakyung.com)
+   ![img](images/manhwakyung.png)
+   네이버 게임 오리지널 시리즈(game.naver.com/original_series):
+   ![img](images/naver_game.png)
+   버프툰과 네이버 포스트는 아래의 '버프툰 다운로드하기'섹션과 '네이버 포스트 다운로드하기' 섹션을 참고해 주세요.
 2. 다음의 파이썬 코드를 웹툰이 다운로드되길 원하는 폴더 내에서 실행해 주세요. 웹툰은 정식 연재와 베스트 도전, Webtoons 오리지널과 캔버스, 만화경, 네이버 게임 모두 가능합니다.
 
    ```python
    from WebtoonScraper import Webtoon as wt
 
    # 네이버 웹툰
-   wt.get_webtoon(76648, wt.N) # titleid를 여기에다 붙여넣으세요.
+   wt.get_webtoon(76648, wt.N)  # titleid를 여기에다 붙여넣으세요.
    # 베스트 도전만화
-   wt.get_webtoon(763952, wt.B) # titleid를 여기에다 붙여넣으세요.
+   wt.get_webtoon(763952, wt.B)  # titleid를 여기에다 붙여넣으세요.  # ! 수정
    # 웹툰 오리지널
-   wt.get_webtoon(1435, wt.O) # titleid를 여기에다 붙여넣으세요.
+   wt.get_webtoon(1435, wt.O)  # title_no를 여기에다 붙여넣으세요.
    # 웹툰 캔버스
-   wt.get_webtoon(304446, wt.C) # titleid를 여기에다 붙여넣으세요.
+   wt.get_webtoon(304446, wt.C)  # title_no를 여기에다 붙여넣으세요.
    # 만화경
-   wt.get_webtoon(146, wt.M) # titleid를 여기에다 붙여넣으세요. Webtoon.T 태그도 사용 가능합니다.
+   wt.get_webtoon(146, wt.M)  # titleid를 여기에다 붙여넣으세요. Webtoon.T 태그도 사용 가능합니다.
    # 네이버 게임 오리지널 시리즈
-   wt.get_webtoon(146, wt.G) # titleid를 여기에다 붙여넣으세요.
+   wt.get_webtoon(5, wt.G)  # titleid를 여기에다 붙여넣으세요.
+   # 버프툰
+   cookie = 'cookie here'  # cookie를 여기에다 붙여넣으세요. 자세한 설명은 아래의 '버프툰 다운로드하기'를 참고하세요.
+   wt.get_webtoon(1007888, wt.BF, cookie=cookie)  # titleid를 여기에다 붙여넣으세요.
+   # 네이버 포스트
+   wt.get_webtoon((597061, 19803452), wt.P)  # seriesNo와 memberNo를 각각 붙여넣으세요. 자세한 설명은 아래의 '네이버 포스트 다운받기'를 참고하세요.
    ```
 
    이제 웹툰이 webtoons 폴더에 다운로드됩니다.
 
    cf. 웹툰 태그를 생략하면 해당 웹툰이 어떤 사이트의 웹툰 id인지 자동으로 알아냅니다. 만약 몇몇 태그가 겹친다면 태그에 맞는 수를 입력하는 창에 알맞은 수를 입력하면 됩니다.
 
-   또 merge 태그를 이용하면 webtoon 폴더 내에 있는 모든 웹툰을 자동으로 5화씩 묶습니다.
+   episode_no_range 키워드를 이용하면 특정한 에피소드만 다운로드받을 수 있습니다.
+   ```python
+   wt.get_webtoon(5, wt.G, episode_no_range=(1,20))  # 1화부터 20화까지
+   ```
+
+   merge 키워드를 이용하면 webtoon 폴더 내에 있는 모든 웹툰을 원하는 개수 만큼 묶습니다.
+   ```python
+   wt.get_webtoon(5, wt.G, merge=5)
+   ```
 3. 만화 뷰어 앱을 통해 다운로드한 웹툰을 시청할 수 있습니다.
 
 ## 주의사항
 
 * 중간에 웹툰 다운로드가 멈춘 듯이 보여도 정상입니다. 그대로 가만히 있으면 다운로드가 다시 진행됩니다.
 * 만약 작동하지 않는다면 윈도우에서 Python 3.11.4을 설치하고 앞의 과정을 반복해 보세요.
 
@@ -81,87 +77,59 @@
 로그인하지 않은 상태에서도 웹툰을 다운로드받을 수 있으나, 받을 수 있는 웹툰 수가 매우 적기에 추천하지 않습니다.
 
 1. 웹툰 페이지에 들어가 주소창의 맨 마지막 수를 복사합니다.
 2. 다음의 파이썬 코드를 웹툰이 다운로드되길 원하는 폴더 내에서 실행해 주세요.
    ```python
    from WebtoonScraper import Webtoon as wt
 
-   wt.get_webtoon(1007888, wt.BF) # 복사했던 수를 여기에다 붙여넣으세요.
+   wt.get_webtoon(1007888, wt.BF)  # 복사했던 수를 여기에다 붙여넣으세요.
    ```
 3. 'Enter cookie of 1007888(시리즈 id) (Enter nothing to preceed without cookie)'라는 문구와 함께 입력란이 나오면 그냥 enter를 눌러줍니다.
 4. 로그인하지 않고 볼 수 있는 모든 에피소드가 다운로드됩니다.
 
 ## 로그인한 상태에서 웹툰 다운로드하기
 
 이 과정은 PC를 기준으로 설명합니다. 만약 모바일이라면 Kiwi Browser 등을 통해 다음의 과정을 수행할 수 있습니다.
 
 1. 웹툰 페이지에 들어가 주소창의 맨 마지막 수를 복사합니다. 이 예시에서는 1007888입니다.
-   ![img](https://raw.githubusercontent.com/ilotoki0804/WebtoonScraper/master/images/bufftoon1.png)
+   ![img](images/bufftoon1.png)
 2. 로그인을 하고 f12를 누르고 네트워크 창을 연 뒤 웹툰 페이지에 들어갑니다.
-   ![img](https://raw.githubusercontent.com/ilotoki0804/WebtoonScraper/master/images/bufftoon2.png)
+   ![img](images/bufftoon2.png)
 3. 새로고침을 한 뒤 '이름'에 있는 favicon.ico 요청을 클릭하고 나온 창에 '헤더' 탭을 엽니다.
-   ![img](https://raw.githubusercontent.com/ilotoki0804/WebtoonScraper/master/images/bufftoon3.png)
+   ![img](images/bufftoon3.png)
 4. 내려서 Cookie: 라고 되어 있는 모든 내용을 복사합니다.
-   ![img](https://raw.githubusercontent.com/ilotoki0804/WebtoonScraper/master/images/bufftoon4.png)
+   ![img](images/bufftoon4.png)
 5. 다음의 파이썬 코드를 웹툰이 다운로드되길 원하는 폴더 내에서 실행해 주세요.
-
-   ```python
-   from WebtoonScraper import Webtoon as wt
-
-   wt.get_webtoon(1007888, wt.BF) # 첫 번째로 복사했던 수를 여기에다 붙여넣으세요.
-   ```
-
-   혹은 다음과 같이 cookie를 코드 내에 포함할 수도 있습니다.
-
    ```python
    from WebtoonScraper import Webtoon as wt
    cookie = '두 번째로 복사했던 문자를 여기에다 붙여넣으세요.'
-   wt.get_webtoon(1007888, wt.BF, cookie=cookie) # 첫 번째로 복사했던 수를 여기에다 붙여넣으세요.
+   wt.get_webtoon(1007888, wt.BF, cookie=cookie)  # 첫 번째로 복사했던 수를 여기에다 붙여넣으세요.
    ```
-
-   1. 'Enter cookie of 1007888(시리즈 id) (Enter nothing to proceed without cookie)'라는 문구와 함께 입력란이 나오면 두 번째로 복사했던 일련의 문자열을 붙여넣기합니다.
 6. 로그인하면 볼 수 있는 모든 에피소드가 다운로드됩니다.
 
 ## 주의사항
 
 * get_webtoon에서 cookie를 입력하면 자동으로 버프툰으로 인식합니다.
 
 # 네이버 포스트 다운로드하기
 
 1. 웹툰이 있는 페이지로 가서 seriesNo와 memberNo를 복사하세요. 예시에서는 각각 597061과 19803452입니다.
-   ![img](https://raw.githubusercontent.com/ilotoki0804/WebtoonScraper/master/images/naver_post.png)
+   ![img](images/naver_post.png)
 2. 다음의 파이썬 코드를 웹툰이 다운로드되길 원하는 폴더 내에서 실행해 주세요.
-
-   ```python
-   from WebtoonScraper import Webtoon as wt
-
-   wt.get_webtoon(597061, wt.M) # 우선 seriesNo만 여기에 입력해주세요.
-   ```
-
-   혹은 memberNo를 코드 내에 포함할 수 있습니다.
-
    ```python
    from WebtoonScraper import Webtoon as wt
 
-   wt.get_webtoon(597061, wt.M, member_no=19803452)
-   ```
-3. 'Enter memberNo of 597061(해당 웹툰의 seriesNo)'라는 말과 함께 입력란이 나오면 거기에 아까 복사해 놓은 memberNo를 붙여넣습니다.
-   만약 앞에서 이미 member_no를 사용했다면 이 단계는 건너뛰어집니다.
-
-   ```
-   Enter memberNo  of 597061: 19803452
-   ...진행됨...
+   wt.get_webtoon((597061, 19803452), wt.P)
    ```
-4. 만화 뷰어 앱을 통해 다운로드한 웹툰을 시청할 수 있습니다.
+3. 만화 뷰어 앱을 통해 다운로드한 웹툰을 시청할 수 있습니다.
 
 ## 주의사항
 
 * 가끔씩 이유 없는 오류가 발생할 수 있습니다. 그럴 때는 조금 시간이 지난 후에 다시 시도해 보세요.
-* 네이버 포스트는 titleid를 get_webtoon_platform으로 알아낼 수 없습니다.
-* member_no를 입력하면 자동으로 포스트로 인식됩니다.
+* tuple를 입력하면 자동으로 포스트로 인식됩니다.
 
 # 여러 회차 하나로 묶기
 
 1. 웹툰을 상기한 대로 다운로드받습니다.
 2. 다음과 같이 코드를 짭니다.
    ```python
    from WebtoonScraper import FolderManager
@@ -185,31 +153,18 @@
    from WebtoonScraper import FolderManager
 
    fm= FolderManager()
    fm.restore_webtoons_in_directory()
    ```
 3. 'webtoon' 폴더에 있던 모든 웹툰이 웹툰을 처음 다운로드했던 상태로 되돌아갑니다.
 
-# QNA
-
-## 회차 번호 관련
-
-### 문제와 이유
-
-회차가 띄엄띄엄 있거나 설정된 회차 번호가 작가가 설정한 회차 번호와 다르거나 회차 묶기를 사용했는데 묶인 회차 수가 설정한 수보다 더 적은 이유는 다음과 같습니다.
-이 프로젝트에서 웹툰의 회차 번호는 ID를 기준으로 합니다. 이는 작가가 정한 회차와는 다를 수 있습니다. 작가가 프롤로그부터 시작하는 경우(프로젝트의 회차 번호가 하나 빠름), 작가가 리메이크를 해서 전에 있던 작품을 제거해 ID가 연속적으로 있지 않는 경우(주로 베도에서 일어남/회차 번호가 띄엄띄엄하게 있음), 논란이나 작가 실수 등으로 회차가 삭제된 경우(한 회차를 건너띔) 등에서 ID가 불연속적이거나 작품과 일치하기 않는 경우가 생기게 됩니다.
-
-### ID를 회차 번호로 그대로 사용하는 이유
-
-우선 작가가 설정한 회차 번호에 맞추는 것은 힘듭니다. 우선 번호가 어디에 있을지 알기 어렵고, 프롤로그가 있을지 없을지 알 수 없으며, 여러 화에 걸쳐 같은 에피소드를 진행하는 경우도 있고, 외전으로 본편의 회차에서 분리된 화를 운영하는 경우가 있어 화에 맞추어서 번호를 정하는 것을 어렵습니다.
-1부터 시작해서 끝까지 일정한 번호를 유지하는 것도 고려해볼 만하나 만약 그렇게 된다면 무결성 체크를 사용하기 어렵게 됩니다.
-따라서 작가가 설정한 회차를 그대로 사용하는 것도 어렵고, 만약 가능하다 할 지라도 무결성 체크를 포기하기 어렵기 때문에 현재는 ID를 회차 번호로 사용하고 있습니다.
-
 # Relese Note
 
+1.1.1: 내부 모듈 이름 변경, merge option 추가, abstractmethod들의 일반 구현 추가
+
 1.0.2: 대형 리팩토링, get_webtoon_platform 비동기 방식으로 속도 개선, 상대경로로 변경, 테스트 추가
 
 1.0.1: 코드 개선 및 리팩토링, api를 통한 로직으로 변경 (버그가 많기에 사용을 권장하지 않음)
 
 1.0.0: 네이버 게임 추가, FolderManager 리펙토링 및 개선, 정식 버전, docs 개선
 
 0.1.1: 네이버 포스트 추가, readme 작성, pbar 표시 내용 변경, 버그 수정
```

### Comparing `WebtoonScraper-1.0.2/WebtoonScraper.egg-info/SOURCES.txt` & `WebtoonScraper-1.1.1/WebtoonScraper.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.py
-WebtoonScraper/BestChallengeScraper.py
-WebtoonScraper/BufftoonScraper.py
-WebtoonScraper/FolderManager.py
-WebtoonScraper/NaverGameScraper.py
-WebtoonScraper/NaverPostScraper.py
-WebtoonScraper/NaverWebtoonScraper.py
-WebtoonScraper/Scraper.py
-WebtoonScraper/TelescopeScraper.py
-WebtoonScraper/Webtoon.py
-WebtoonScraper/WebtoonCanvasScraper.py
-WebtoonScraper/WebtoonOriginalsScraper.py
+WebtoonScraper/A_FolderManager.py
+WebtoonScraper/B_Webtoon.py
+WebtoonScraper/C_Scraper.py
+WebtoonScraper/D_NaverWebtoonScraper.py
+WebtoonScraper/E_BestChallengeScraper.py
+WebtoonScraper/F_WebtoonOriginalsScraper.py
+WebtoonScraper/G_WebtoonCanvasScraper.py
+WebtoonScraper/H_TelescopeScraper.py
+WebtoonScraper/I_BufftoonScraper.py
+WebtoonScraper/J_NaverPostScraper.py
+WebtoonScraper/K_NaverGameScraper.py
 WebtoonScraper/__init__.py
 WebtoonScraper.egg-info/PKG-INFO
 WebtoonScraper.egg-info/SOURCES.txt
 WebtoonScraper.egg-info/dependency_links.txt
 WebtoonScraper.egg-info/not-zip-safe
 WebtoonScraper.egg-info/requires.txt
 WebtoonScraper.egg-info/top_level.txt
```

### Comparing `WebtoonScraper-1.0.2/setup.py` & `WebtoonScraper-1.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 long_description += Path('README.md').read_text(encoding='utf-8')
 # 사진 대체
 repl = r'![\g<1>](https://raw.githubusercontent.com/ilotoki0804/WebtoonScraper/master/\g<2>)'
 long_description = re.sub(r'!\[(.+?)\]\((images\/.+?)\)', repl, long_description)
 
 setup(
     name='WebtoonScraper',
-    version='1.0.2',
+    version='1.1.1',
     description='Scraping webtoons and some utils for it',
     author='ilotoki0804',
     author_email='ilotoki0804@gmail.com',
     long_description=long_description,
     long_description_content_type='text/markdown',
     license='MIT',
     url='https://github.com/ilotoki0804/WebtoonScraper',
```

### Comparing `WebtoonScraper-1.0.2/test/test.py` & `WebtoonScraper-1.1.1/test/test.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import asyncio
+import logging
 
-if __name__ == "__main__":
+if __name__ in ("__main__", "test"):
     # 파일을 이용하는 것은 아님. 만약 제대로 사용하려면 상대 경로로 실행해야 함.
-    from WebtoonScraper import Webtoon as wt
-    from WebtoonScraper import FolderManager
+    logging.warning('파일이 아닌 WebtoonScraper 모듈에서 실행되고 있습니다.')
+    from WebtoonScraper import B_Webtoon as wt
+    from WebtoonScraper import A_FolderManager as FolderManager
 else:
-    from ..WebtoonScraper import Webtoon as wt
-    from ..WebtoonScraper.FolderManager import FolderManager
+    from ..WebtoonScraper import B_Webtoon as wt
+    from ..WebtoonScraper.A_FolderManager import FolderManager
 
 
 def skip_by_KeyboadInterrupt(func):
     try:
         func()
     except KeyboardInterrupt:
         print('Interrupted.')
```

