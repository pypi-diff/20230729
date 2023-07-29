# Comparing `tmp/langful-0.39-py3-none-any.whl.zip` & `tmp/langful-0.40-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 5636 bytes, number of entries: 7
+Zip file size: 5289 bytes, number of entries: 7
 -rw-rw-rw-  2.0 fat      166 b- defN 23-Jul-06 06:25 langful/__init__.py
--rw-rw-rw-  2.0 fat    10313 b- defN 23-Jul-23 16:32 langful/lang.py
--rw-rw-rw-  2.0 fat     1066 b- defN 23-Jul-23 16:50 langful-0.39.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     3050 b- defN 23-Jul-23 16:50 langful-0.39.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-23 16:50 langful-0.39.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 23-Jul-23 16:50 langful-0.39.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      528 b- defN 23-Jul-23 16:50 langful-0.39.dist-info/RECORD
-7 files, 15223 bytes uncompressed, 4706 bytes compressed:  69.1%
+-rw-rw-rw-  2.0 fat     8206 b- defN 23-Jul-29 14:22 langful/lang.py
+-rw-rw-rw-  2.0 fat     1066 b- defN 23-Jul-29 16:22 langful-0.40.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     2984 b- defN 23-Jul-29 16:22 langful-0.40.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-29 16:22 langful-0.40.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 23-Jul-29 16:22 langful-0.40.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      527 b- defN 23-Jul-29 16:22 langful-0.40.dist-info/RECORD
+7 files, 13049 bytes uncompressed, 4359 bytes compressed:  66.6%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: langful/__init__.py
 Comment: 
 
 Filename: langful/lang.py
 Comment: 
 
-Filename: langful-0.39.dist-info/LICENSE
+Filename: langful-0.40.dist-info/LICENSE
 Comment: 
 
-Filename: langful-0.39.dist-info/METADATA
+Filename: langful-0.40.dist-info/METADATA
 Comment: 
 
-Filename: langful-0.39.dist-info/WHEEL
+Filename: langful-0.40.dist-info/WHEEL
 Comment: 
 
-Filename: langful-0.39.dist-info/top_level.txt
+Filename: langful-0.40.dist-info/top_level.txt
 Comment: 
 
-Filename: langful-0.39.dist-info/RECORD
+Filename: langful-0.40.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## langful/lang.py

```diff
@@ -3,47 +3,26 @@
 """
 
 import json
 import os
 
 __all__ = [ "to_json" , "to_lang" , "getdefaultlocale" , "lang" ]
 
-def to_json( lang_file : str ) -> dict :
-    """
-    .lang -> .json
-    """
-    import re
+def to_json( text : str ) -> dict[ str , str ] :
+    from re import split
     ret = {}
-    for line in lang_file.split( "\n" ) :
-        text = re.split( "([^#^=^\\s]+|)(\\s+=\\s+|\\s+=|=\\s+|=|)([^#^\\n]+|)" , line )
-        index = 0
-        for value in text :
-            if "=" in value :
-                ret[ "".join( text[ :index ] ) ] = "".join( text[ index + 1 : ] )
-                break
-            index += 1
-    return ret
-
-def to_lang( dict_file : dict ) -> str :
-    """
-    .json -> .lang
-    """
-    ret = ""
-    for key , value in dict_file.items() :
-        ret += f"{ key } = { value }\n"
+    for line in text.split( "\n" ) :
+        try :
+            ret.update( dict( [ split( "\s=\s" , line.split( "#" )[ 0 ] , 1 ) ] ) )
+        except ValueError :
+            continue
     return ret
 
-def to_list( args : str | list ) -> list :
-    """
-    only use it in this file don't add it in __all__ list
-    """
-    if isinstance( args , list ) :
-        return args
-    else :
-        return [ args ]
+def to_lang( text : dict ) -> str :
+    return "\n".join( [ ' = '.join( item ) for item in list( text.items() ) ] )
 
 def getdefaultlocale() -> str :
     """
     getdefaultlocale will deprecated so use this
     """
     from locale import getlocale
     from sys import platform
@@ -53,143 +32,100 @@
             from locale import windows_locale
             code = windows_locale.get( int( code , 0 ) )
     else :
         code = getlocale()[ 0 ]
     return code.replace( "-" , "_" ).lower()
 
 class lang :
-    """
-    # lang
-    """
 
-    @property
-    def locales( self ) -> list :
-        """
-        locales
-        """
-        return list( self.types.keys() )
+    locale_system = getdefaultlocale()
+    __slots__ = [ "locale_default" , "locale_use" , "languages" , "path" , "configs" , "types" ]
 
     @property
     def locale( self ) -> str :
-        """
-        choose locale
-        """
-        for locale in [ self.use_locale , self.system_locale , self.default_locale ] :
+        for locale in [ self.locale_use , self.locale_system , self.locale_default ] :
             if locale and locale in self.locales :
                 return locale
-        raise KeyError( f"no such locale '{ self.system_locale }' or '{ self.default_locale }'" )
+        raise KeyError( f"no such locale '{ self.locale_system }' or '{ self.locale_default }'" )
 
     @property
-    def language( self ) -> dict :
-        """
-        get now language
-        """
+    def locales( self ) -> list[ str ] :
+        return list( self.types.keys() )
+
+    @property
+    def language( self ) -> dict[ str , str ] :
         return self.lang_get( self.locale )
 
     @property
-    def lang( self ) -> dict :
-        """
-        same to language function
-        """
+    def lang( self ) -> dict[ str , str ] :
         return self.language
 
     @property
-    def langs( self ) -> dict :
-        """
-        same to languages variable
-        """
+    def langs( self ) -> dict[ str , str ] :
         return self.languages
 
-    @property
-    def type( self ) -> str :
-        """
-        get type, ".json" or ".lang"
-        """
-        return self.types[ self.locale ]
-
     def __getitem__( self , key ) -> str :
-        """
-        get the value in language variable
-        """
         return self.get( key )
 
     def __setitem__( self , key , value ) -> None :
-        """
-        set the value in languages[ locale ]
-        """
         self.set( key , value )
 
     def __delitem__( self , key ) -> None :
-        """
-        remove the value in languages[ locale ]
-        """
         self.remove( key )
 
-    def __call__( self ) -> None :
-        """
-        init function
-        """
-        self.init()
-
     def __str__( self ) -> str :
-        """
-        to string
-        """
-        return json.dumps( self.languages , indent = 4 , ensure_ascii = False , separators = self.separators )
+        return json.dumps( self.languages , indent = 4 , ensure_ascii = False , separators = self.configs[ "separators" ] )
 
     def __len__( self ) -> int :
-        """
-        how many item in language variable
-        """
         return len( self.language )
 
     def __bool__( self ) -> bool :
-        """
-        is system locale in languages dictionary
-        """
-        return self.system_locale in self.languages
+        return self.locale_system in self.languages
 
-    def __init__( self , lang_dir : str | dict = "lang" , default_locale : str = "en_us" , json_first : bool = True ) -> None :
-        """
-        lang_dir: lang files dir, if use dict to set that to a dictionary or False
-        default_locale: default locale
-        json_first: is load json file first
+    def __call__( self ) -> None :
+        self.init()
+
+    def __init__( self , path : str | dict = "lang" , locale_default : str = "en_us" , json_first : bool = True ) -> None :
         """
-        self.system_locale = getdefaultlocale()
-        self.default_locale = default_locale
-        self.separators = [ " ," , ": " ]
-        self.json_first = json_first
-        self.replace_letter = "%"
-        self.lang_dir = lang_dir
-        self.use_locale = None
-        self.is_file = False
+        path: lang files dir, if use dict to set that to a dictionary or False
+        locale_default: default locale
+        load: is load json file first
+        """
+        self.configs = { "separators" : [ " ," , ": " ] , "replace" : "%" , "load" : json_first , "file" : False }
+        self.locale_default = locale_default
+        self.locale_use = None
         self.languages = {}
+        self.path = path
         self.types = {}
         self.init()
 
+    def config( self , key : str , value : str ) -> None :
+        if key in self.configs :
+            self.configs[ key ] = value
+        else :
+            raise KeyError( f"'{ key }' not in configs" )
+
     def init( self ) :
-        """
-        init
-        """
-        if isinstance( self.lang_dir , str ) :
-            self.init_file( self.lang_dir )
-        elif isinstance( self.lang_dir , dict ) :
-            self.init_dict( self.lang_dir )
+        if isinstance( self.path , str ) :
+            self.init_file( self.path )
+        elif isinstance( self.path , dict ) :
+            self.init_dict( self.path )
 
     def init_file( self , path ) -> None :
         """
         init by a directory
         """
-        self.is_file = True
-        if not os.path.exists( path ) :
-            raise FileNotFoundError( f"can't find '{ os.path.abspath( path ) }'" )
-        loads = [ [ ".lang" , ".json" ] , [ ".json" , ".lang" ] ][ self.json_first ]
+        loads = [ [ ".lang" , ".lang" ] , [ ".json" , ".lang" ] ][ self.configs[ "load" ] ]
+        self.configs[ "file" ] = True
+        self.language = {}
+        self.path = path
+        self.types = {}
         for lang_file in os.listdir( path ) :
             name , suffix = os.path.splitext( lang_file )
-            if ( suffix in loads ) and ( ( suffix == loads[ 0 ] ) or ( suffix not in self.locales ) ) :
+            if ( suffix in loads ) and ( ( suffix == loads[ 0 ] ) or ( name not in self.locales ) ) :
                 with open( os.path.join( path , lang_file ) , "r" , encoding = "utf-8" ) as file :
                     if suffix == ".json" :
                         try :
                             data = json.load( file )
                         except json.decoder.JSONDecodeError :
                             raise SyntaxError( "can't to load .json file" )
                     elif suffix == ".lang" :
@@ -199,138 +135,87 @@
                 self.languages[ name ] = data
                 self.types[ name ] = suffix
 
     def init_dict( self , language : dict = None ) -> None :
         """
         init by a dictionary, so cant't to save it to the file
         """
-        self.is_file = False
-        for key in language.keys() :
-            self.types[ key ] = ".json"
+        self.types = { key : ".json" for key in language.keys() }
+        self.configs[ "file" ] = False
         self.languages = language
-        self.lang_dir = language
+        self.path = language
 
     def to_dict( self ) :
-        """
-        set type to dict
-        """
-        self.types = { key : ".json" for key in self.types.keys() }
-        self.lang_dir = self.languages
-        self.is_file = False
+        self.types = { key : ".json" for key in self.languages.keys() }
+        self.configs[ "file" ] = False
+        self.path = self.languages
 
     def to_file( self , path ) :
-        """
-        set type to file
-        """
         if not os.path.exists( path ) :
             os.makedirs( path )
-        self.lang_dir = path
-        self.is_file = True
+        self.configs[ "file" ] = True
+        self.path = path
 
     def locale_get( self , locale : str = None ) -> str :
-        """
-        get locale, usually use in function
-        """
-        if locale :
-            return locale
-        else :
-            return self.locale
+        return locale if locale else self.locale
 
     def locale_set( self , locale : str = None  ) -> None :
-        """
-        if give a locale then set that, else reset it
-        """
         if locale and locale not in self.locales :
             raise KeyError( f"no such locale '{ locale }'" )
-        self.use_locale = locale
+        self.locale_use = locale
 
-    def lang_get( self , locale : str ) -> dict :
-        """
-        get a lang
-        """
-        return self.languages[ locale ]
+    def lang_get( self , locale : str ) -> dict[ str , str ] :
+        return self.languages[ self.locale_get( locale ) ]
 
     def lang_set( self , locale : str , value : dict = {} , suffix : str = ".json" ) -> None :
-        """
-        set a lang
-        """
+        locale = self.locale_get( locale )
         self.languages[ locale ] = value
         self.types[ locale ] = suffix
 
     def lang_remove( self , locale : str ) -> None :
-        """
-        remove a lang
-        """
+        locale = self.locale_get( locale )
         del self.languages[ locale ]
         del self.types[ locale ]
 
-    def lang_merge( self , to : str , locale : str = None , args : str | list = [] ) -> None :
-        """
-        merge to a locale
-        """
+    def lang_merge( self , to : str , locale : str = None , args : str | list[ str ] = [] ) -> None :
         self.lang_set( to , self.merge( locale , args ) )
 
     def get( self , key : str , locale : str = None ) -> str :
-        """
-        get the key by a locale dictionary
-        """
-        locale = self.locale_get( locale )
-        return self.languages[ locale ][ key ]
+        return self.languages[ self.locale_get( locale ) ][ key ]
 
     def set( self , key : str , value : str , locale : str = None ) -> None :
-        """
-        set a value by a locale dictionary
-        """
-        locale = self.locale_get( locale )
-        self.languages[ locale ][ key ] = value
+        self.languages[ self.locale_get( locale ) ][ key ] = value
 
     def remove( self , key : str , locale : str = None ) -> None :
-        """
-        remove a value by a locale dictionary
-        """
-        locale = self.locale_get( locale )
-        del self.languages[ locale ][ key ]
+        del self.languages[ self.locale_get( locale ) ][ key ]
 
-    def merge( self , locale : str = None , args : str | list = [] ) -> dict :
-        """
-        merge
-        """
-        args = to_list( args )
-        ret = self.lang_get( self.locale_get( locale ) )
+    def merge( self , locale : str = None , args : list[ str ] = [] ) -> dict[ str , str ] :
+        ret = self.lang_get( locale )
         for locale_key in args :
-            for key , value in self.lang_get( locale_key ).items() :
-                ret[ key ] = value
+            ret.update( self.lang_get( locale_key ) )
         return ret
 
-    def save( self ) -> dict :
-        """
-        save file when is_file variable is true
-        """
-        if self.is_file :
+    def save( self ) -> dict[ str , str ] :
+        if self.configs[ "file" ] :
             for key , value in self.languages.items() :
                 suffix = self.types[ key ]
-                with open( os.path.join( self.lang_dir , key + suffix ) , "w" , encoding = "utf-8" ) as file :
+                with open( os.path.join( self.path , key + suffix ) , "w" , encoding = "utf-8" ) as file :
                     if suffix == ".json" :
-                        json.dump( value , file , indent = 4 , separators = self.separators , ensure_ascii = False )
+                        json.dump( value , file , indent = 4 , separators = self.configs[ "separators" ] , ensure_ascii = False )
                     elif suffix == ".lang" :
                         file.write( to_lang( value ) )
         return self.languages
 
-    def replace( self , key : str = None , args : str | list  = None , locale : str = None ) -> str :
-        """
-        replace
-        """
-        replace_letter = self.replace_letter
-        locale = self.locale_get( locale )
-        args = to_list( args )
+    def replace( self , key : str = None , args : list[ str ] = None , locale : str = None ) -> str :
+        symbol = self.configs[ "replace" ]
         index = 0
         ret = ""
         for text in self.get( key , locale ) :
-            if text == replace_letter :
+            if text == symbol :
                 if len( ret ) and ret[ -1 ] == "\\" :
-                    ret = ret[ : -1 ] + replace_letter
+                    ret = ret[ : -1 ] + symbol
                 else :
                     ret += str( args[ index ] )
                     index += index < len( args ) - 1
             else :
                 ret += text
         return ret
```

## Comparing `langful-0.39.dist-info/LICENSE` & `langful-0.40.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `langful-0.39.dist-info/METADATA` & `langful-0.40.dist-info/METADATA`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langful
-Version: 0.39
+Version: 0.40
 Summary: Help to localization
 Home-page: https://github.com/cueavy/langful
 Author: cueavyqwp
 Author-email: cueavyqwp@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -89,23 +89,23 @@
 then you can put file at there :
 
 * lang
 * * en_us.lang
 * * en_us.json
 * * zh_cn.lang
 * * zh_cn.json
+* * ...
 
 or use other directory name and set `langful.lang( "directory name" )`
 
 ### by dictionary
 
 ```python
 import langful
-lang = langful.lang( False )
-lang.init_dict( {
+lang = langful.lang( {
     "en_us" : {
         "hi" : "Hi" ,
         "welcome" : "Welcome"
     } ,
     "zh_cn" : {
         "hi" : "你好" ,
         "welcome" : "欢迎"
@@ -114,29 +114,27 @@
 ```
 
 ## function
 
 ### replace
 
 ```python
-lang = langful.lang( False )
-lang.init_dict( {
+lang = langful.lang( {
     "en_us" : {
         "test" : "%.%\%"
     }
 } )
 print( lang.replace( "test" , [ 33 , 3 ] ) )
 ```
 
 ### merge
 
 ```python
 import langful
-lang = langful.lang( False )
-lang.init_dict( {
+lang = langful.lang( {
     "en_us" : {
         "hi" : "Hi" ,
         "welcome" : "Welcome"
     } ,
     "zh_cn" : {
         "hi" : "你好"
     }
```

