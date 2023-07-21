# Comparing `tmp/AshCrypt-2.0.8.tar.gz` & `tmp/AshCrypt-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/AshCrypt-2.0.8.tar", last modified: Fri Jul 21 15:01:51 2023, max compression
+gzip compressed data, was "dist/AshCrypt-3.0.0.tar", last modified: Fri Jul 21 20:36:38 2023, max compression
```

## Comparing `AshCrypt-2.0.8.tar` & `AshCrypt-3.0.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:01:51.000000 AshCrypt-2.0.8/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:01:51.000000 AshCrypt-2.0.8/AshCrypt/
--rw-r--r--   0 runner    (1001) docker     (123)    38210 2023-07-21 15:01:40.000000 AshCrypt-2.0.8/AshCrypt/AshCryptGUI.py
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-21 15:01:40.000000 AshCrypt-2.0.8/AshCrypt/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-21 15:01:40.000000 AshCrypt-2.0.8/AshCrypt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6560 2023-07-21 15:01:40.000000 AshCrypt-2.0.8/AshCrypt/clicrypt.py
--rw-r--r--   0 runner    (1001) docker     (123)     7145 2023-07-21 15:01:40.000000 AshCrypt-2.0.8/AshCrypt/crypt.py
--rw-r--r--   0 runner    (1001) docker     (123)     8681 2023-07-21 15:01:40.000000 AshCrypt-2.0.8/AshCrypt/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-07-21 15:01:40.000000 AshCrypt-2.0.8/AshCrypt/filecrypt.py
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-21 15:01:40.000000 AshCrypt-2.0.8/AshCrypt/qr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-07-21 15:01:40.000000 AshCrypt-2.0.8/AshCrypt/textcrypt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:01:51.000000 AshCrypt-2.0.8/AshCrypt/unittests/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-21 15:01:40.000000 AshCrypt-2.0.8/AshCrypt/unittests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3263 2023-07-21 15:01:40.000000 AshCrypt-2.0.8/AshCrypt/unittests/unittest_crypt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:01:51.000000 AshCrypt-2.0.8/AshCrypt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-07-21 15:01:51.000000 AshCrypt-2.0.8/AshCrypt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-21 15:01:51.000000 AshCrypt-2.0.8/AshCrypt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 15:01:51.000000 AshCrypt-2.0.8/AshCrypt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-21 15:01:51.000000 AshCrypt-2.0.8/AshCrypt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-21 15:01:51.000000 AshCrypt-2.0.8/AshCrypt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-07-21 15:01:51.000000 AshCrypt-2.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    21164 2023-07-21 15:01:40.000000 AshCrypt-2.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 15:01:51.000000 AshCrypt-2.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-07-21 15:01:40.000000 AshCrypt-2.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:36:38.000000 AshCrypt-3.0.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:36:38.000000 AshCrypt-3.0.0/AshCrypt/
+-rw-r--r--   0 runner    (1001) docker     (123)    38210 2023-07-21 20:36:28.000000 AshCrypt-3.0.0/AshCrypt/AshCryptGUI.py
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-21 20:36:28.000000 AshCrypt-3.0.0/AshCrypt/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-21 20:36:28.000000 AshCrypt-3.0.0/AshCrypt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6583 2023-07-21 20:36:28.000000 AshCrypt-3.0.0/AshCrypt/clicrypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7145 2023-07-21 20:36:28.000000 AshCrypt-3.0.0/AshCrypt/crypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8681 2023-07-21 20:36:28.000000 AshCrypt-3.0.0/AshCrypt/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-07-21 20:36:28.000000 AshCrypt-3.0.0/AshCrypt/filecrypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-21 20:36:28.000000 AshCrypt-3.0.0/AshCrypt/qr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-07-21 20:36:28.000000 AshCrypt-3.0.0/AshCrypt/textcrypt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:36:38.000000 AshCrypt-3.0.0/AshCrypt/unittests/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-21 20:36:28.000000 AshCrypt-3.0.0/AshCrypt/unittests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3263 2023-07-21 20:36:28.000000 AshCrypt-3.0.0/AshCrypt/unittests/unittest_crypt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:36:38.000000 AshCrypt-3.0.0/AshCrypt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-07-21 20:36:38.000000 AshCrypt-3.0.0/AshCrypt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-21 20:36:38.000000 AshCrypt-3.0.0/AshCrypt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 20:36:38.000000 AshCrypt-3.0.0/AshCrypt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-21 20:36:38.000000 AshCrypt-3.0.0/AshCrypt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-21 20:36:38.000000 AshCrypt-3.0.0/AshCrypt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-07-21 20:36:38.000000 AshCrypt-3.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    21244 2023-07-21 20:36:28.000000 AshCrypt-3.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 20:36:38.000000 AshCrypt-3.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-07-21 20:36:28.000000 AshCrypt-3.0.0/setup.py
```

### Comparing `AshCrypt-2.0.8/AshCrypt/AshCryptGUI.py` & `AshCrypt-3.0.0/AshCrypt/AshCryptGUI.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-2.0.8/AshCrypt/clicrypt.py` & `AshCrypt-3.0.0/AshCrypt/clicrypt.py`

 * *Files 4% similar despite different names*

```diff
@@ -160,15 +160,15 @@
 
 def file_dec():
     keysetup()
     while file_decFlag:
         print()
         global key
         pre = input(
-            "Running file decryption mode , press the known commands or 'Enter' to continue.. : ")
+            "Running file decryption mode..\nPress the known commands or 'Enter' to continue.. : ")
         print()
         input_wrap(pre)
         if pre == '':
             print("You can use the commands AFTER entering the file name.. ")
             filename = input('Enter full file name to be Decrypted : ')
             target = af.CryptFile(filename, key)
             a = target.decrypt()
@@ -181,30 +181,30 @@
                 print(
                     f'The file named : "{filename}" does not exists , try specifying the whole sys path')
             if a == 0:
                 print(
                     'Error in the decryption process. Check if the the file is distorted or it might just be '
                     'decrypted already')
             if a == 4:
-                print('Unknown Error has occurred\n')
+                print('Unknown Error has occurred ( system related ) \n')
             if a == 5:
                 print('ERROR : Key is Not 256-bit')
             if a == 6:
                 print('ERROR : File is already decrypted')
             elif a == 7:
                 print('ERROR : Given a directory instead of a file')
 
 
 def file_enc():
     keysetup()
     while file_encFlag:
         print()
         global key
         pre = input(
-            "Running file encryption mode, press the known commands or 'Enter' to continue.. : ")
+            "Running file encryption mode..\nPress the known commands or 'Enter' to continue.. : ")
         print()
         input_wrap(pre)
         if pre == '':
             print("You can use the commands AFTER entering the file name.. ")
             filename = input('Enter full file name to be Encrypted : ')
             target = af.CryptFile(filename, key)
             a = target.encrypt()
```

### Comparing `AshCrypt-2.0.8/AshCrypt/crypt.py` & `AshCrypt-3.0.0/AshCrypt/crypt.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-2.0.8/AshCrypt/database.py` & `AshCrypt-3.0.0/AshCrypt/database.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-2.0.8/AshCrypt/filecrypt.py` & `AshCrypt-3.0.0/AshCrypt/filecrypt.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-2.0.8/AshCrypt/textcrypt.py` & `AshCrypt-3.0.0/AshCrypt/textcrypt.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-2.0.8/AshCrypt/unittests/unittest_crypt.py` & `AshCrypt-3.0.0/AshCrypt/unittests/unittest_crypt.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-2.0.8/AshCrypt.egg-info/PKG-INFO` & `AshCrypt-3.0.0/AshCrypt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AshCrypt
-Version: 2.0.8
+Version: 3.0.0
 Summary: Comprehensive AES-256 Cryptography App & library equipped with files & text handling modules along with a database module to store encrypted content.
 Home-page: https://github.com/AshGw/AES-256.git
 Author: Ashref Gwader
 Author-email: AshrefGw@proton.me
 License: UNKNOWN
 Description: # Cryptography App &  Library : AES-256
         ##  Objective ##
```

### Comparing `AshCrypt-2.0.8/PKG-INFO` & `AshCrypt-3.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AshCrypt
-Version: 2.0.8
+Version: 3.0.0
 Summary: Comprehensive AES-256 Cryptography App & library equipped with files & text handling modules along with a database module to store encrypted content.
 Home-page: https://github.com/AshGw/AES-256.git
 Author: Ashref Gwader
 Author-email: AshrefGw@proton.me
 License: UNKNOWN
 Description: # Cryptography App &  Library : AES-256
         ##  Objective ##
```

### Comparing `AshCrypt-2.0.8/README.md` & `AshCrypt-3.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -15,16 +15,15 @@
 <br>Fully-fledged application that integrates all the modules in the library merging them into a unified and powerful software solution for developers and for people with no programming knowledge whatsoever
 <br>check [GUI](https://github.com/AshGw/AES-256#AshCryptGUI) header for more info.
 
 **Library :** 
 <br>A simple, secure, and developer-oriented library for
 encryption and decryption with AES-256 (CBC) . 
 <br>The core of the library is the module `crypt`
-It offers an intuitive interface, seamless integration with precompiled 
-functions, and top security measures to safeguard
+It offers cryptographic capabilities and top security measures to safeguard
 sensitive data,  providing a hassle-free experience when dealing with cryptographic libraries.
 <br>View [Features](https://github.com/AshGw/AES-256#features) Header for more details.
 
 
 
 
 
@@ -85,15 +84,15 @@
 sudo apt-get install curl
 ```
 2) If you're running a lightweight python version it might not include `tkinter` in the standard library so run
 ```bash
 sudo apt-get update
 sudo apt-get install python3-tk 
 ```
-3) If you're running `python 3.6` or older then you might need to install `dataclasses`
+3) If you're running `python 3.6` or older, then you might need to install `dataclasses`
 ```
 pip install dataclasses
 ```
 <br>Now if none of this works you might just use the docker image for this purpose, so check this [directory](Docker-build)
 </details>
 
 **After the library is installed** 
@@ -178,45 +177,45 @@
 - HMAC : 256 bit hashed using SHA512
 - Generates a random 128 bit Initialization Vector (IV) each time for the Cipher
 - PKCS7 message padding
 ### Other Features :
 These focus on ease of use: 
 - No need to manipulate the input to fit, it accepts strings or bytes you can pass them right away
 - You can get a string or a bytes representation of either the encryption or the decryption result
-- In `crypt` module the key is flexible it doesn't have to be 256 bit long, it can actually be of any length but that's up to you to ensure it's security, or leave it as is and use the key generation function to get secure and random keys ( although in `textcrypt` and `filecrypt` you have to use a 256 bit long key )
+- In `crypt` module the key is flexible it doesn't have to be 256 bit long, it can actually be of any length but that's up to you to ensure its security, or leave it as is and use the key generation function to get secure and random keys ( although in `textcrypt` and `filecrypt` you have to use a 256 bit long key )
 - Encrypting to a string has URL-safe string representation 
 ### Regarding KDFs
 Note that bcrypt is intentionally slow and computationally expensive, enhancing protection against brute-force attacks. The number of iterations, including salt and pepper, increases derivation time to strike a balance between security and performance. Use a suitable value based on your machine's capabilities and desired security level.
 <br>Im using 50 just to demonstrate the process and make it quick.
 <br>The bare minimum is 50, the max is 100 000, choose somewhere in between.
 <br>In my use case 50 takes around 0.5 secs while using the maximum number of iterations takes around 11 minutes to derive the keys and finish the cryptographic operations at hand.
-<br>You can check how it works by checking this [Jupyter Notebook](demo/demo.ipynb) demo file
+<br>You can check how it works by checking this [Jupyter Notebook](demo/performance-check.ipynb) demo file
 ## AshCryptGUI ##
-The GUI as mentioned above is a full, application , you can use it to encrypt files , texts , keep track of files by storing them on demand to a main database , also on demand it can keep track of the keys used for cryptographic operations.
+The GUI as mentioned above is a fully functional application , you can use it to encrypt files , texts , keep track of files by storing them on demand to a main database , also on demand it can keep track of the keys used for cryptographic operations.
 ### Usage ###
-1) Set the main key up. If you don't have one , press on the button `generate` to generate a secure safe key ready for use. 
+1) Set the main key up. If you don't have one , press on the button `generate` to generate a secure safe key ready for use. Then insert it in the `MAINKEY` entry
 2) Now you're able to encrypt files or text (text is limited to 200 characters max)
 ####  Text : 
 - You can insert some text in the entry right below the `TEXT ENCRYPTION` label.<br>The given text will be encrypted and you can choose if you want to have that text displayed as a qr code, a qr image will pop on the screen and you'll be able to scan it using your phone.
-- Insert some encrypted text below the `TEXT DECRYPTION` label.<br>The Given text will be decrypted and you'd have the option to display the "plaintext" as a qr code to be scanned by other devices.
+- Insert some encrypted text below the `TEXT DECRYPTION` label.<br>The given text will be decrypted and you'd have the option to display the "plaintext" as a qr code to be scanned by other devices.
 <br>If the text cannot be decrypted it will display itself , so you might as well use this to display the key you're using as a qr code 
 
 #### Files
 - Under the `FILE PATH` label enter the file name (if it's in the current working directory) or submit the whole file path , the file can be of any type, click on `ENCRYPT FILE` Button to encrypt the given file , if the encryption turned out to be successful , you'll see a success message along with a `added .crypt extention to the file` message if the encryption wasn't successful you'll see an error message specifying the problem.<br>Note that you cannot re-encrypt a file that  has `.crypt` as extention.
-- The file name should be changed by now to `filename + '.crypt'` , if the file has .crypt extention you can go ahead and decrypt it , if the same key is used for both enc/dec operations then the result should be `success` + `removed .crypt extention` from the file.
+- The file name should be changed by now to `filename + '.crypt'` , if the file has .crypt extension you can go ahead and decrypt it , if the same key is used for both enc/dec operations then the result should be `success` + `removed .crypt extention` from the file.
 #### Database
 - Now you have some encrypted/decrypted files but you want to keep them stored somewhere safe, this is where the main database comes in , where you need to store your files + their content + reference to the key used for their encryption/decryption. you can specify your database by 
 1) Specify the actual path where you want your database to be 
 2) Give it a name, it must be a valid file name that ends with `.db` .<br>
-If the database doesn't exist then a database with the name you've given will be created and automatically connected to.<br>If the given database already exists then it will automatically be connected.
-3) Did I mention the keys database ? well if you give a database it will also create a keys database with the same name as the database you chose plus `Keys` added to its name. This database holds the actual keys and the reference to these keys.
+If the database doesn't exist then a database with the name you've given will be created and automatically connected to.<br>If the given database already exists then it will automatically connect.
+3) Did I mention the keys' database ? well if you give a database it will also create a keys database with the same name as the database you chose plus `Keys` added to its name. This database holds the actual keys and the reference to these keys.
 <br>The only common piece of data that the two separate databases have in common are the key reference values.  
 
-**Note** : If your main database gets compromised , then the attacker wouldnt have anything useful , they can never know the actual key from the reference key so no problem with that if it only contains encrypted content BUT NEVER EVER GET YOUR KEYS DATABASE COMPROMISED ! 
-<br>If anyone gets hold of your main database they would only see some encrypted content and some key refrence that is actually 100% independent of the actual key used for encryption so they have nothing , but if they get hold of the keys database they can look for matching refs and use the matching key to decrypt that binary encrypted data to its actual format.
+**Note** : If your main database gets compromised , then the attacker wouldnt have anything useful , they can never know the actual key from the reference key so no problem with that if it only contains encrypted content BUT NEVER GET YOUR KEYS DATABASE EXPOSED ! 
+<br>If anyone gets hold of your main database they would only see some encrypted content and some key reference that is actually 100% independent of the actual key used for encryption so they have nothing , but if they get hold of the keys database they can look for matching refs and use the matching key to decrypt that binary encrypted data to its actual format.
 That's why I made two different databases not two tables within a single database. 
 <br> So you keep your keys database safe and secure.
 
 
 **Info** Both databases have the same table called `Classified` that has 4 columns <br>`ID` which is auto generated & incremented for each piece of data that gets inserted<br>
 `Name` that holds the filename in both databases , although in the keys database if you haven't specified any file to operate on and keep selecting keys the keys name will be `STANDALONE` 
 <br>`Contnet` in the main db that holds the entire content of the given file, in keys db that holds the actual 256 bit long encryption key.
@@ -234,65 +233,65 @@
 
 
 ## filecrypt ## 
 If you want to encrypt a file :
 1) Follow the steps above to set the key up.
 2) Create an instance of the class CryptFiles and pass 2 arguments, the first one being the target file and the second argument being the key :
 ```python
-instance1 = CryptFile('target.txt', key)
+my_instance = CryptFile('target.txt', key)
 ```
 ```python
-instance1 = CryptFile('testDataBase.db', key)
+my_instance = CryptFile('testDataBase.db', key)
 ```
 The file can be of anything : image`.png`, movie `.mp4`,`.sqlite`  etc..
 <br>It doesn't have to just be of `.txt` extension ,can be of anything really.  
 <br>**Note** : 
-If the file is not in the working directroy you can specify the whole path: 
+If the file is not in the working directory you can specify the whole path: 
 <br>**For windows**
 ```python
 target = CryptFile('C:\\Users\\offic\\MyProjects\\SomeOtherfolder\\myfile.txt',key) 
 ```
 <br>**On Mac and Linux :**
 ```python
 target = CryptFile('/User/Desktop/MyProjects/SomeOtherfolder/myfile.txt',key)
 ```
 3) Apply either the encryption or decryption functions to that instance :
 ```python
-instance1 = CryptFile('qrv10.png',key)
-instance1.encrypt()
+my_instance = CryptFile('qrv10.png',key)
+my_instance.encrypt()
 ```
-you can apply `print()` on `instance1.encrypt()`to check the result :
+you can apply `print()` on `my_instance.encrypt()`to check the result :
 <br> 1 : File successfully encrypted/decrypted + added/removed .crypt extension 
 <br> 2 : File is empty
 <br> 3 : File doesn't exist
 <br> 4 : Unknown Error usually a system related one 
 <br> 5 : Key is denied for cryptographic use
 <br> 6 : File is already encrypted/decrypted
 <br> 7 : File is not a file it's a directory
 <br> 0 : Error in enc/dec probable file distortion, tampering or wrong key
 ```python
-instance1.encrypt()
+my_instance.encrypt()
 ```
 ```python
-instance1.decrypt()
+my_instance.decrypt()
 ```
 
 That's it, if you follow the steps above then everything should work just fine.
 ## textcrypt ## 
 Same steps above just the naming is different, and keep in mind both accept either strings or bytes 
 ```python
-instance1 = Crypt('Hello Wold !',key)
+my_instance = Crypt('Hello Wold !',key)
 ```
 ```python
-instance1.encrypt()[1]
+my_instance.encrypt()[1]
 ```
 ```python
-instance1.decrypt()[1]
+my_instance.decrypt()[1]
 ```
-The result simply returns a tuple so index `[0]` is going to be the confirmation if it's 1 then it worked, else some Error has occured.
+The result simply returns a tuple so index `[0]` is going to be the confirmation if it's 1 then it worked, else some Error has occurred.
 <br>Index `[1]` contains the encrypted/decrypted content that's it very simple.
 
 **Note**:
 <br>Unlike the `crypt` module where if you try to decrypt a non-encrypted message you get all kinds of errors.
 
 in `filecrypt` & `textcrypt` it's simpler if you attempt to decrypt an non-encrypted message then you'll get the same message back along with an integer in this case `0` for failure.
 <br>`1`'s for success.
@@ -308,44 +307,45 @@
 To support efficient content management, I have integrated this database module to enable the storage and retrieval of encrypted content in a safe and secure manner using an sqlite3 database
 
 Ensuring that the encrypted data remains organized and readily accessible to anyone with the right key. Any content going in must be encrypted with a key that you must keep off grid.
 
 **Note** that in `database.py` I'm using `dataclasses` module which was introduced in `python 3.7`, so make sure to install it if you have an older version.
 
 ### Usage ## 
-In the module I'm providing built-in functions to make it easier to perform usual queries on Sqlite tables , by default it creates a table `Classified` with two deafult columns :
+In the module I'm providing built-in functions to make it easier to perform usual queries on Sqlite tables , by default it creates a table `Classified` with two default columns :
 
 **content** : This can be a single character or a whole movie in binary, that depends on your specific needs.
 
-**key** : This key column wasn't indeed meant to store a key itself but rather store a reference to the actual key. The key itself should be stored somewhere else safe and secure preferrably off-grid and completely seprerate from any vulnerable devices, you can even write it down on a piece of paper if you want , just make sure to rotate your keys from time to time.
+**key** : This key column wasn't indeed meant to store a key itself but rather store a reference to the actual key. The key itself should be stored somewhere else safe and secure preferably off-grid and completely separate from any vulnerable devices on you can have it on a separate database stored safely away, you can even write it down on a piece of paper if you want , just make sure to rotate your keys from time to time.
 
 1) Create a connection to the database :
 ```python
 connect = Database('test.db')
 ```
 This would automatically set the default table name to `Classifed` if no arguments are passed to the other class functions then they would all be working on the default table name , if you want to set your default table name instead of `Classified` you can pass your table name as the second argument : 
 ```python
 connect = Database('test.db','MyDefaultTable')
 ```
 2) create/add the table to the database :
 ```python
 connect.addtable()
 ```
 Added the default table that's been set to the database,  if you want to pass an argument to the function that would create another table of your choice
+
 3) Set a reference to the key not the key itself : 
 ```python
  key = '#5482A'
 ```
-4) Use the connection to perform various tasks
-The content can be anything post encryption in its Bytes or String format
+4) Use the connection to perform various tasks <br>
+The content can be anything post encryption bytes or string format
 ```python
 content='Some Encrypted Content'
 connect.insert(content=content,key='#1E89JO', optional_table_name=None)
 ```
-If the optional table name is None then it will insert into the default table , else it would insert into the table you specify
+If the optional table name is `None` then it will insert into the default table , else it would insert into the table you specify
 
 
 5) You can check the tables you have , it returns a generator object, yields the result of each element so you must run a for loop over it
 ```python
 for e in connect.show_tables():
         print(e)
 ```
@@ -354,24 +354,24 @@
 print(connect.size) # Size of the Database in MB 
 ```
 
 6) Check the module itself so you can run through all the available methods.
 <br>The methods available perform the usual operations like insertion, deletion , updating the database and more..
 
 
-7) to run more complex queries I've dedicated a query function that takes in *queries and returns the result fetched 
+7) to run more complex queries I've dedicated a query function that takes in `*queries` and returns the result fetched 
 ```python
 query = 'SELECT COUNT(*) AS cc ,content FROM Classified WHERE key = "#5482A" ORDER BY cc DESC '
 print(connect.query(query))
 ```
 The result fetched should look like this : 
  ```python
 [{'query 0': ['SUCCESS', [(1, 'some encrypted content of bytes or strings')]]}]
 ```
-If some error has occurred while doing a query like : 
+If some error has occurred while querying like : 
 ```python
 query = 'SELECT COUNT(*) AS cc ,content FROM DoesntExist WHERE key = "#5482A" ORDER BY cc DESC '
 ```
 The result fetched should look similar to this : 
 ```python
 [{'query 0': ('FAILURE', 'no such table: DoesntExist')}]
 ```
```

### Comparing `AshCrypt-2.0.8/setup.py` & `AshCrypt-3.0.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup , find_packages
 
 with open('AshCrypt/README.md','r') as f:
     readme = f.read()
 
 setup(
     name='AshCrypt',
-    version='2.0.8',
+    version='3.0.0',
     author='Ashref Gwader',
     author_email='AshrefGw@proton.me',
     python_requires='>=3.7',
     description="Comprehensive AES-256 Cryptography App & library equipped with files & text handling modules along with"
                 " a database module to store encrypted content.",
     long_description_content_type='text/markdown',
     long_description=readme,
```

