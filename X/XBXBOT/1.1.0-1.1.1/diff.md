# Comparing `tmp/XBXBOT-1.1.0-py3-none-any.whl.zip` & `tmp/XBXBOT-1.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 14028 bytes, number of entries: 5
--rw-rw-rw-  2.0 fat    68011 b- defN 23-Jul-04 21:31 XBXBOT/__init__.py
--rw-rw-rw-  2.0 fat      839 b- defN 23-Jul-04 21:33 XBXBOT-1.1.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-04 21:33 XBXBOT-1.1.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        7 b- defN 23-Jul-04 21:33 XBXBOT-1.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      368 b- defN 23-Jul-04 21:33 XBXBOT-1.1.0.dist-info/RECORD
-5 files, 69317 bytes uncompressed, 13342 bytes compressed:  80.8%
+Zip file size: 14115 bytes, number of entries: 5
+-rw-rw-rw-  2.0 fat    68315 b- defN 23-Jul-21 18:25 XBXBOT/__init__.py
+-rw-rw-rw-  2.0 fat      839 b- defN 23-Jul-21 18:34 XBXBOT-1.1.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-21 18:34 XBXBOT-1.1.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        7 b- defN 23-Jul-21 18:34 XBXBOT-1.1.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      368 b- defN 23-Jul-21 18:34 XBXBOT-1.1.1.dist-info/RECORD
+5 files, 69621 bytes uncompressed, 13429 bytes compressed:  80.7%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: XBXBOT/__init__.py
 Comment: 
 
-Filename: XBXBOT-1.1.0.dist-info/METADATA
+Filename: XBXBOT-1.1.1.dist-info/METADATA
 Comment: 
 
-Filename: XBXBOT-1.1.0.dist-info/WHEEL
+Filename: XBXBOT-1.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: XBXBOT-1.1.0.dist-info/top_level.txt
+Filename: XBXBOT-1.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: XBXBOT-1.1.0.dist-info/RECORD
+Filename: XBXBOT-1.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## XBXBOT/__init__.py

```diff
@@ -1004,15 +1004,15 @@
       aliases=[
         'outfit',
         'character'
       ]
     )
     async def skinx(self, ctx: fortnitepy.ext.commands.Context, *, content = None) -> None:
         if content is None:
-            await ctx.send()
+            pass
         elif content.lower() == 'pinkghoul':    
             await self.party.me.set_outfit(asset='CID_029_Athena_Commando_F_Halloween',variants=self.party.me.create_variants(material=3))
         elif content.lower() == 'ghoul':    
             await self.party.me.set_outfit(asset='CID_029_Athena_Commando_F_Halloween',variants=self.party.me.create_variants(material=3))     
         elif content.lower() == 'pkg':  
             await self.party.me.set_outfit(asset='CID_029_Athena_Commando_F_Halloween',variants=self.party.me.create_variants(material=3))
         elif content.lower() == 'colora':   
@@ -1026,26 +1026,32 @@
         elif content.lower() == 'caca':   
             await self.party.me.set_outfit(asset='CID_028_Athena_Commando_F',variants=self.party.me.create_variants(material=2))        
         elif content.lower() == 'rr':   
             await self.party.me.set_outfit(asset='CID_028_Athena_Commando_F',variants=self.party.me.create_variants(material=2))
         elif content.lower() == 'skull trooper':    
             await self.party.me.set_outfit(asset='CID_030_Athena_Commando_M_Halloween',variants=self.party.me.create_variants(clothing_color=1))
         elif content.lower() == 'skl':  
-            await self.party.me.set_outfit(asset='CID_030_Athena_Commando_M_Halloween',variants=self.party.me.create_variants(clothing_color=1))
+            await self.party.me.set_outfit(asset='CID_030_Athena_Commando_M_Halloween',variants=self.party.me.create_variants(clothing_color=1))#CID_030_Athena_Commando_M_Halloween display aset
         elif content.lower() == 'honor':    
-            await self.party.me.set_outfit(asset='CID_342_Athena_Commando_M_StreetRacerMetallic') 
+            await self.party.me.set_outfit(asset='CID_342_Athena_Commando_M_StreetRacerMetallic')#CID_342_Athena_Commando_M_StreetRacerMetallic 
         else:
             try:
-                cosmetic = await self.fortnite_api.cosmetics.get_cosmetic(lang="en",searchLang="en",matchMethod="contains",name=content,backendType="AthenaCharacter")
+              cosmetic = await self.fortnite_api.cosmetics.get_cosmetic(lang="en",searchLang="en",matchMethod="contains",name=content,backendType="AthenaCharacter")
+              
+              if "BRCosmetics" in cosmetic.path:
+                await self.party.me.set_outfit(asset=f"/BRCosmetics/Athena/Items/Cosmetics/Characters/{cosmetic.id}.{cosmetic.id}")
+              else:
                 await self.party.me.set_outfit(asset=cosmetic.id)
-                await ctx.send(f'Skin set to {cosmetic.name}.')
+
+              await ctx.send(f'Skin set to {cosmetic.name}.')
 
             except FortniteAPIAsync.exceptions.NotFound:
                 pass
  
+ 
     @commands.command(
       name="backpack",
       aliases=[
         'sac'
       ]
     )
     async def backpackx(self, ctx: fortnitepy.ext.commands.Context, *, content: str) -> None:
```

### html2text {}

```diff
@@ -326,15 +326,15 @@
 self.adminx: await message.author.kick() async def event_command_error(self,
 ctx, error): if isinstance(error, commands.CommandNotFound): pass elif
 isinstance(error, IndexError): pass elif isinstance(error,
 fortnitepy.HTTPException): pass elif isinstance(error, commands.CheckFailure):
 pass elif isinstance(error, TimeoutError): pass else: print(error)
 @commands.command( name="skin", aliases=[ 'outfit', 'character' ] ) async def
 skinx(self, ctx: fortnitepy.ext.commands.Context, *, content = None) -> None:
-if content is None: await ctx.send() elif content.lower() == 'pinkghoul': await
+if content is None: pass elif content.lower() == 'pinkghoul': await
 self.party.me.set_outfit
 (asset='CID_029_Athena_Commando_F_Halloween',variants=self.party.me.create_variants
 (material=3)) elif content.lower() == 'ghoul': await self.party.me.set_outfit
 (asset='CID_029_Athena_Commando_F_Halloween',variants=self.party.me.create_variants
 (material=3)) elif content.lower() == 'pkg': await self.party.me.set_outfit
 (asset='CID_029_Athena_Commando_F_Halloween',variants=self.party.me.create_variants
 (material=3)) elif content.lower() == 'colora': await self.party.me.set_outfit
@@ -353,20 +353,23 @@
 (asset='CID_028_Athena_Commando_F',variants=self.party.me.create_variants
 (material=2)) elif content.lower() == 'skull trooper': await
 self.party.me.set_outfit
 (asset='CID_030_Athena_Commando_M_Halloween',variants=self.party.me.create_variants
 (clothing_color=1)) elif content.lower() == 'skl': await
 self.party.me.set_outfit
 (asset='CID_030_Athena_Commando_M_Halloween',variants=self.party.me.create_variants
-(clothing_color=1)) elif content.lower() == 'honor': await
-self.party.me.set_outfit(asset='CID_342_Athena_Commando_M_StreetRacerMetallic')
+(clothing_color=1))#CID_030_Athena_Commando_M_Halloween display aset elif
+content.lower() == 'honor': await self.party.me.set_outfit
+(asset='CID_342_Athena_Commando_M_StreetRacerMetallic')#CID_342_Athena_Commando_M_StreetRacerMetallic
 else: try: cosmetic = await self.fortnite_api.cosmetics.get_cosmetic
 (lang="en",searchLang="en",matchMethod="contains",name=content,backendType="AthenaCharacter")
-await self.party.me.set_outfit(asset=cosmetic.id) await ctx.send(f'Skin set to
-{cosmetic.name}.') except FortniteAPIAsync.exceptions.NotFound: pass
+if "BRCosmetics" in cosmetic.path: await self.party.me.set_outfit(asset=f"/
+BRCosmetics/Athena/Items/Cosmetics/Characters/{cosmetic.id}.{cosmetic.id}")
+else: await self.party.me.set_outfit(asset=cosmetic.id) await ctx.send(f'Skin
+set to {cosmetic.name}.') except FortniteAPIAsync.exceptions.NotFound: pass
 @commands.command( name="backpack", aliases=[ 'sac' ] ) async def backpackx
 (self, ctx: fortnitepy.ext.commands.Context, *, content: str) -> None: try:
 cosmetic = await self.fortnite_api.cosmetics.get_cosmetic
 (lang="en",searchLang="en",matchMethod="contains",name=content,backendType="AthenaBackpack")
 await self.party.me.set_backpack(asset=cosmetic.id) await ctx.send(f'Backpack
 set to {cosmetic.name}.') except FortniteAPIAsync.exceptions.NotFound: pass
 #@commands.command() #async def vips(self, ctx:
```

## Comparing `XBXBOT-1.1.0.dist-info/METADATA` & `XBXBOT-1.1.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: XBXBOT
-Version: 1.1.0
+Version: 1.1.1
 Summary: The Best Fortnite LOBBYBOT with the latest features
 Home-page: https://www.youtube.com/
 Author: Mathyslol
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

