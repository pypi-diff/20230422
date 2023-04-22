# Comparing `tmp/elevenlabslib-0.4.2.tar.gz` & `tmp/elevenlabslib-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elevenlabslib-0.4.2.tar", last modified: Tue Apr 11 21:11:05 2023, max compression
+gzip compressed data, was "elevenlabslib-0.4.3.tar", last modified: Sat Apr 22 11:36:30 2023, max compression
```

## Comparing `elevenlabslib-0.4.2.tar` & `elevenlabslib-0.4.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 21:11:05.285869 elevenlabslib-0.4.2/
--rw-rw-rw-   0        0        0     1091 2023-02-17 22:48:32.000000 elevenlabslib-0.4.2/LICENSE
--rw-rw-rw-   0        0        0     2484 2023-04-11 21:11:05.285869 elevenlabslib-0.4.2/PKG-INFO
--rw-rw-rw-   0        0        0     1905 2023-03-20 00:23:33.000000 elevenlabslib-0.4.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-11 21:11:05.271868 elevenlabslib-0.4.2/elevenlabslib/
--rw-rw-rw-   0        0        0     3858 2023-03-18 16:40:33.000000 elevenlabslib-0.4.2/elevenlabslib/ElevenLabsHistoryItem.py
--rw-rw-rw-   0        0        0     2635 2023-03-18 16:40:43.000000 elevenlabslib-0.4.2/elevenlabslib/ElevenLabsSample.py
--rw-rw-rw-   0        0        0    14203 2023-03-25 13:50:30.000000 elevenlabslib-0.4.2/elevenlabslib/ElevenLabsUser.py
--rw-rw-rw-   0        0        0    31721 2023-04-11 21:06:56.000000 elevenlabslib-0.4.2/elevenlabslib/ElevenLabsVoice.py
--rw-rw-rw-   0        0        0      445 2023-03-25 13:50:30.000000 elevenlabslib-0.4.2/elevenlabslib/__init__.py
--rw-rw-rw-   0        0        0     5624 2023-03-30 11:08:35.000000 elevenlabslib-0.4.2/elevenlabslib/helpers.py
-drwxrwxrwx   0        0        0        0 2023-04-11 21:11:05.284868 elevenlabslib-0.4.2/elevenlabslib.egg-info/
--rw-rw-rw-   0        0        0     2484 2023-04-11 21:11:05.000000 elevenlabslib-0.4.2/elevenlabslib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      405 2023-04-11 21:11:05.000000 elevenlabslib-0.4.2/elevenlabslib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 21:11:05.000000 elevenlabslib-0.4.2/elevenlabslib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-04-11 21:11:05.000000 elevenlabslib-0.4.2/elevenlabslib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-04-11 21:11:05.000000 elevenlabslib-0.4.2/elevenlabslib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      777 2023-04-11 21:08:00.000000 elevenlabslib-0.4.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-11 21:11:05.285869 elevenlabslib-0.4.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-22 11:36:30.732367 elevenlabslib-0.4.3/
+-rw-rw-rw-   0        0        0     1091 2023-02-17 22:48:32.000000 elevenlabslib-0.4.3/LICENSE
+-rw-rw-rw-   0        0        0     2484 2023-04-22 11:36:30.732367 elevenlabslib-0.4.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1905 2023-03-20 00:23:33.000000 elevenlabslib-0.4.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-22 11:36:30.717367 elevenlabslib-0.4.3/elevenlabslib/
+-rw-rw-rw-   0        0        0     3858 2023-03-18 16:40:33.000000 elevenlabslib-0.4.3/elevenlabslib/ElevenLabsHistoryItem.py
+-rw-rw-rw-   0        0        0     2635 2023-03-18 16:40:43.000000 elevenlabslib-0.4.3/elevenlabslib/ElevenLabsSample.py
+-rw-rw-rw-   0        0        0    14203 2023-03-25 13:50:30.000000 elevenlabslib-0.4.3/elevenlabslib/ElevenLabsUser.py
+-rw-rw-rw-   0        0        0    31268 2023-04-22 11:34:15.000000 elevenlabslib-0.4.3/elevenlabslib/ElevenLabsVoice.py
+-rw-rw-rw-   0        0        0      445 2023-03-25 13:50:30.000000 elevenlabslib-0.4.3/elevenlabslib/__init__.py
+-rw-rw-rw-   0        0        0     5624 2023-03-30 11:08:35.000000 elevenlabslib-0.4.3/elevenlabslib/helpers.py
+drwxrwxrwx   0        0        0        0 2023-04-22 11:36:30.731368 elevenlabslib-0.4.3/elevenlabslib.egg-info/
+-rw-rw-rw-   0        0        0     2484 2023-04-22 11:36:30.000000 elevenlabslib-0.4.3/elevenlabslib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      405 2023-04-22 11:36:30.000000 elevenlabslib-0.4.3/elevenlabslib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-22 11:36:30.000000 elevenlabslib-0.4.3/elevenlabslib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-04-22 11:36:30.000000 elevenlabslib-0.4.3/elevenlabslib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-04-22 11:36:30.000000 elevenlabslib-0.4.3/elevenlabslib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      777 2023-04-22 11:36:14.000000 elevenlabslib-0.4.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-22 11:36:30.733366 elevenlabslib-0.4.3/setup.cfg
```

### Comparing `elevenlabslib-0.4.2/LICENSE` & `elevenlabslib-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `elevenlabslib-0.4.2/PKG-INFO` & `elevenlabslib-0.4.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elevenlabslib
-Version: 0.4.2
+Version: 0.4.3
 Summary: Complete python wrapper for the elevenlabs API
 Author-email: lugia19 <lugia19@lugia19.com>
 Project-URL: Homepage, https://github.com/lugia19/elevenlabslib
 Project-URL: Bug Tracker, https://github.com/lugia19/elevenlabslib
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `elevenlabslib-0.4.2/README.md` & `elevenlabslib-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `elevenlabslib-0.4.2/elevenlabslib/ElevenLabsHistoryItem.py` & `elevenlabslib-0.4.3/elevenlabslib/ElevenLabsHistoryItem.py`

 * *Files identical despite different names*

### Comparing `elevenlabslib-0.4.2/elevenlabslib/ElevenLabsSample.py` & `elevenlabslib-0.4.3/elevenlabslib/ElevenLabsSample.py`

 * *Files identical despite different names*

### Comparing `elevenlabslib-0.4.2/elevenlabslib/ElevenLabsUser.py` & `elevenlabslib-0.4.3/elevenlabslib/ElevenLabsUser.py`

 * *Files identical despite different names*

### Comparing `elevenlabslib-0.4.2/elevenlabslib/ElevenLabsVoice.py` & `elevenlabslib-0.4.3/elevenlabslib/ElevenLabsVoice.py`

 * *Files 3% similar despite different names*

```diff
@@ -307,23 +307,24 @@
         self._linkedUser = newUser
 
     @property
     def voiceID(self):
         return self._voiceID
 
 
-
+_defaultDType = "float32"
 class _AudioChunkStreamer:
     def __init__(self,portaudioDeviceID:int = None,onPlaybackStart:Callable=lambda: None, onPlaybackEnd:Callable=lambda: None):
         self._q = queue.Queue()
         self._bytesFile = io.BytesIO()
         self._bytesSoundFile: Optional[sf.SoundFile] = None  # Needs to be created later.
         self._bytesLock = threading.Lock()
         self._onPlaybackStart = onPlaybackStart
         self._onPlaybackEnd = onPlaybackEnd
+        self._frameSize = 0
 
         if portaudioDeviceID is None:
             portaudioDeviceID = sd.default.device
 
         self._deviceID = portaudioDeviceID
 
         self._events: dict[str, threading.Event] = {
@@ -352,44 +353,35 @@
             logging.debug("Waiting for header event...")
             self._events["headerReadyEvent"].wait()
             logging.debug("Header maybe ready?")
             try:
                 with self._bytesLock:
                     self._bytesSoundFile = sf.SoundFile(self._bytesFile)
                     logging.debug("File created (" + str(self._bytesFile.tell()) + " bytes read).")
+                    self._frameSize = self._bytesSoundFile.channels * sf._ffi.sizeof(self._bytesSoundFile._check_dtype(_defaultDType))
                     self._events["soundFileReadyEvent"].set()
                     break
             except sf.LibsndfileError:
                 self._bytesFile.seek(0)
                 dataBytes = self._bytesFile.read()
                 self._bytesFile.seek(0)
                 logging.debug("Error creating the soundfile with " + str(len(dataBytes)) + " bytes of data. Let's clear the headerReady event.")
                 self._events["headerReadyEvent"].clear()
                 self._events["soundFileReadyEvent"].set()
 
         stream = sd.RawOutputStream(
             samplerate=self._bytesSoundFile.samplerate, blocksize=_playbackBlockSize,
-            device=self._deviceID, channels=self._bytesSoundFile.channels, dtype='float32',
+            device=self._deviceID, channels=self._bytesSoundFile.channels, dtype=_defaultDType,
             callback=self._stream_playback_callback, finished_callback=self._events["playbackFinishedEvent"].set)
         logging.debug("Starting playback...")
         with stream:
-            #This timeout is actually irrelevant now because I'm making the queue infinite size.
-            #timeout = _playbackBlockSize * _playbackBufferSizeInBlocks / self._bytesSoundFile.samplerate
-
-            # Since I can't find any way to get the buffer size from soundfile,
-            # we will just assume the first read operation gives back a complete chunk
-            # and use that to check later reads. This SHOULD be accurate. Hopefully.
-            # Maybe there's like a weird edge case or something, hopefully not.
-            likelyReadChunkSize = -1
             while True:
-                data = self._insert_into_queue_from_download_thread()
-                if likelyReadChunkSize == -1:
-                    likelyReadChunkSize = len(data)
-                if len(data) >= likelyReadChunkSize:
-                    #logging.debug("Putting " + str(len(data)) + " bytes in queue.")
+                data = self._get_data_from_download_thread()
+                if len(data) == _playbackBlockSize*self._frameSize:
+                    logging.debug("Putting " + str(len(data)) + " bytes in queue.")
                     self._q.put(data)
                 else:
                     logging.debug("Got back less data than expected, check if we're at the end...")
                     with self._bytesLock:
                         # This needs to use bytes rather than frames left, as sometimes the number of frames left is wrong.
                         curPos = self._bytesFile.tell()
                         endPos = self._bytesFile.seek(0, os.SEEK_END)
@@ -399,15 +391,15 @@
                             if data != b"":
                                 logging.debug("Still some data left, writing it...")
                                 #logging.debug("Putting " + str(len(data)) +
                                 #              " bytes in queue.")
                                 self._q.put(data)
                             break
                         else:
-                            print("We're not at the end. Wait for more data.")
+                            logging.critical("We're not at the end, yet we recieved less data than expected. THIS SHOULD NOT HAPPEN.")
             logging.debug("While loop done.")
             self._events["playbackFinishedEvent"].wait()  # Wait until playback is finished
             self._onPlaybackEnd()
             logging.debug(stream.active)
         logging.debug("Stream done.")
         return
 
@@ -450,20 +442,14 @@
         logging.debug("Download finished - " + str(totalLength) + ".")
         self._events["downloadDoneEvent"].set()
         self._events["blockDataAvailable"].set()  # Ensure that the other thread knows data is available
         return
 
     def _stream_playback_callback(self, outdata, frames, timeData, status):
         assert frames == _playbackBlockSize
-        if status.output_underflow:
-            logging.error('Output underflow: increase blocksize?')
-            #raise sd.CallbackAbort
-        #assert not status
-
-        #Underflow can happen when two streams are started at once and it doesn't seem to do anything bad so I'm just ignoring it.
 
         while True:
             try:
                 readData = self._q.get_nowait()
                 if len(readData) == 0 and not self._events["downloadDoneEvent"].is_set():
                     logging.debug("An empty item got into the queue. Skip it.")
                     continue
@@ -476,15 +462,15 @@
                     # This should NEVER happen, as the getdownloaddata function handles waiting for new data to come in. ABORT.
                     logging.debug("Missing data but download isn't over. What the fuck?")
                     raise sd.CallbackAbort
         #We've read an item from the queue.
 
         if not self._events["playbackStartFired"].is_set(): #Ensure the callback only fires once.
             self._events["playbackStartFired"].set()
-            print("Firing onPlaybackStart...")
+            logging.debug("Firing onPlaybackStart...")
             self._onPlaybackStart()
 
         # Last read chunk was smaller than it should've been. It's either EOF or that stupid soundFile bug.
         if 0 < len(readData) < len(outdata):
             logging.debug("Data read smaller than it should've been.")
             logging.debug("Read " + str(len(readData)) + " bytes but expected " + str(len(outdata)) + ", padding...")
 
@@ -503,43 +489,46 @@
                     raise sd.CallbackStop
                 else:
                     logging.debug("...Read no data but the download isn't over, what the fuck? Panic. Just send silence.")
                     outdata[len(readData):] = b'\x00' * (len(outdata) - len(readData))
         else:
             outdata[:] = readData
     #THIS FUNCTION ASSUMES YOU'VE GIVEN THE THREAD THE LOCK.
-    def _soundFile_read_and_fix(self, dataToRead:int=-1, dtype="float32"):
+    def _soundFile_read_and_fix(self, dataToRead:int=-1, dtype=_defaultDType):
         readData = self._bytesSoundFile.buffer_read(dataToRead, dtype=dtype)
-        if len(readData) == 0:
-            logging.debug("No data read.")
-            logging.debug("Frame counter must be outdated, recreating soundfile...")
-            self._bytesFile.seek(0)
-            newSF = sf.SoundFile(self._bytesFile)
-            newSF.seek(self._bytesSoundFile.tell())
-            self._bytesSoundFile = newSF
-            readData = self._bytesSoundFile.buffer_read(dataToRead, dtype=dtype)
-            logging.debug("Now read " + str(len(readData)) + " bytes. I sure fucking hope that number isn't zero.")
+        logging.debug(f"Expected {dataToRead*self._frameSize} bytes, got back {len(readData)}")
+        if len(readData) < dataToRead * self._frameSize:
+            logging.debug("Insufficient data read.")
+            curPos = self._bytesFile.tell()
+            endPos = self._bytesFile.seek(0, os.SEEK_END)
+            if curPos != endPos:
+                logging.debug("We're not at the end of the file. Check if we're out of frames.")
+                logging.debug("Recreating soundfile...")
+                self._bytesFile.seek(0)
+                newSF = sf.SoundFile(self._bytesFile, mode="r")
+                newSF.seek(self._bytesSoundFile.tell() - int(len(readData) / self._frameSize))
+                if newSF.frames > self._bytesSoundFile.frames:
+                    logging.debug("Frame counter was outdated.")
+                    self._bytesSoundFile = newSF
+                    readData = self._bytesSoundFile.buffer_read(dataToRead, dtype=dtype)
+                    logging.debug("Now read " + str(len(readData)) +
+                          " bytes. I sure hope that number isn't zero.")
         return readData
 
-    def _insert_into_queue_from_download_thread(self) -> bytes:
+    def _get_data_from_download_thread(self) -> bytes:
         self._events["blockDataAvailable"].wait()  # Wait until a block of data is available.
         self._bytesLock.acquire()
         try:
             readData = self._soundFile_read_and_fix(_playbackBlockSize)
-        except AssertionError as e:
-            logging.debug("Exception in buffer_read (likely not enough data left), read what is available...")
-            try:
-                readData = self._soundFile_read_and_fix()
-            except AssertionError as en:
-                logging.debug("Mismatch in the number of frames read.")
-                logging.debug("This only seems to be an issue when it happens with files that have ID3v2 tags.")
-                logging.debug("Ignore it and return empty.")
-                readData = b""
+        except AssertionError as en:
+            logging.debug("Mismatch in the number of frames read.")
+            logging.debug("This only seems to be an issue when it happens with files that have ID3v2 tags.")
+            logging.debug("Ignore it and return empty.")
+            readData = b""
 
-        #logging.debug("Checking remaining bytes...")
         currentPos = self._bytesFile.tell()
         self._bytesFile.seek(0, os.SEEK_END)
         endPos = self._bytesFile.tell()
         #logging.debug("Remaining file length: " + str(endPos - currentPos) + "\n")
         self._bytesFile.seek(currentPos)
         remainingBytes = endPos - currentPos
```

### Comparing `elevenlabslib-0.4.2/elevenlabslib/helpers.py` & `elevenlabslib-0.4.3/elevenlabslib/helpers.py`

 * *Files identical despite different names*

### Comparing `elevenlabslib-0.4.2/elevenlabslib.egg-info/PKG-INFO` & `elevenlabslib-0.4.3/elevenlabslib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elevenlabslib
-Version: 0.4.2
+Version: 0.4.3
 Summary: Complete python wrapper for the elevenlabs API
 Author-email: lugia19 <lugia19@lugia19.com>
 Project-URL: Homepage, https://github.com/lugia19/elevenlabslib
 Project-URL: Bug Tracker, https://github.com/lugia19/elevenlabslib
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `elevenlabslib-0.4.2/pyproject.toml` & `elevenlabslib-0.4.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0",
             "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "elevenlabslib"
-version = "0.4.2"
+version = "0.4.3"
 authors = [
   { name="lugia19", email="lugia19@lugia19.com" },
 ]
 description = "Complete python wrapper for the elevenlabs API"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies=[
```

