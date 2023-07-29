# Comparing `tmp/hyd-0.1.6.tar.gz` & `tmp/hyd-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyd-0.1.6.tar", max compression
+gzip compressed data, was "hyd-0.1.7.tar", max compression
```

## Comparing `hyd-0.1.6.tar` & `hyd-0.1.7.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1063 2022-12-07 14:08:19.737464 hyd-0.1.6/LICENSE
--rw-r--r--   0        0        0      103 2022-12-07 14:08:19.737576 hyd-0.1.6/README.md
--rw-r--r--   0        0        0     4534 2023-07-28 18:45:13.440783 hyd-0.1.6/hyd/HaukursYouTubeDownloader.py
--rw-r--r--   0        0        0      457 2023-07-28 18:51:46.885389 hyd-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      657 1970-01-01 00:00:00.000000 hyd-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1063 2022-12-07 14:08:19.737464 hyd-0.1.7/LICENSE
+-rw-r--r--   0        0        0      103 2022-12-07 14:08:19.737576 hyd-0.1.7/README.md
+-rw-r--r--   0        0        0     4551 2023-07-29 10:24:38.090893 hyd-0.1.7/hyd/HaukursYouTubeDownloader.py
+-rw-r--r--   0        0        0      457 2023-07-29 10:24:53.266224 hyd-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      657 1970-01-01 00:00:00.000000 hyd-0.1.7/PKG-INFO
```

### Comparing `hyd-0.1.6/LICENSE` & `hyd-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `hyd-0.1.6/hyd/HaukursYouTubeDownloader.py` & `hyd-0.1.7/hyd/HaukursYouTubeDownloader.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,14 +47,15 @@
                 font=("UbuntuMono", 13),
                 bg="#910000",
                 fg="#111111",
                 border=False,
                 activebackground="#750000",
                 command=lambda: download(link.get(), True))
 
+
     # Window attribute locations and dimensions
     linkInputBox.place(relx=0.5, rely=0.45, anchor=CENTER)
     likeTextLabel.place(relx=0.87, rely=0.45, anchor=CENTER)
     downloadButtonMP4.place(relx=0.37, rely=0.7, anchor=CENTER)
     downloadButtonMP3.place(relx=0.63, rely=0.7, anchor=CENTER)
 
 
@@ -75,15 +76,15 @@
             if os.path.exists(f"{path}/{fixedTitle}.mp4") and mp3IsClicked:
                 print("Mp3IsClicked is true; downloading converting mp4 download to mp3 download...")
                 video = VideoFileClip(f"{path}/{fixedTitle}.mp4")
                 os.remove(f"{path}/{fixedTitle}.mp4")
                 video.audio.write_audiofile(f"{path}/{fixedTitle}.mp3")
                 mp3IsClicked = False  
             endTime = time()
-            print(f"Download success! Final Time was {endTime-startTime,3}")        
+            print(f"Download success! Final Time was {round(endTime-startTime,3)} seconds ")        
             popup = Tk()
             popup.title("Download Success!")
             popup.geometry("350x125")
             popup.resizable(False, False)
             popup.configure(bg="#222222")
             popupLabel = Label(popup, text=f"Successfuly downloaded video at \n{path}.\nTotal time taken: {round(endTime-startTime,3)} seconds", fg="#EDEDED", bg="#222222")
             popupLabel.place(relx=0.5, rely=0.25, anchor=CENTER)
```

### Comparing `hyd-0.1.6/PKG-INFO` & `hyd-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyd
-Version: 0.1.6
+Version: 0.1.7
 Summary: A basic python youtube downloader made using tkinter, moviepy and pytube.
 License: MIT
 Author: haukurlogi
 Author-email: haukurlogi2008@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

