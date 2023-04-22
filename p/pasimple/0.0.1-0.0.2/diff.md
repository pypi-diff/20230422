# Comparing `tmp/pasimple-0.0.1.tar.gz` & `tmp/pasimple-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pasimple-0.0.1.tar", last modified: Sat Apr  2 13:46:01 2022, max compression
+gzip compressed data, was "pasimple-0.0.2.tar", last modified: Sat Apr 22 00:05:40 2023, max compression
```

## Comparing `pasimple-0.0.1.tar` & `pasimple-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 henrik    (1000) henrik    (1000)        0 2022-04-02 13:46:01.285380 pasimple-0.0.1/
--rw-r--r--   0 henrik    (1000) henrik    (1000)     1052 2022-01-21 18:02:01.000000 pasimple-0.0.1/LICENSE
--rw-r--r--   0 henrik    (1000) henrik    (1000)     9923 2022-04-02 13:46:01.285380 pasimple-0.0.1/PKG-INFO
--rw-r--r--   0 henrik    (1000) henrik    (1000)     9470 2022-04-02 13:01:37.000000 pasimple-0.0.1/README.md
-drwxr-xr-x   0 henrik    (1000) henrik    (1000)        0 2022-04-02 13:46:01.285380 pasimple-0.0.1/pasimple/
--rw-r--r--   0 henrik    (1000) henrik    (1000)     3388 2022-02-06 21:13:14.000000 pasimple-0.0.1/pasimple/__init__.py
--rw-r--r--   0 henrik    (1000) henrik    (1000)       98 2022-01-30 12:51:01.000000 pasimple-0.0.1/pasimple/exceptions.py
--rw-r--r--   0 henrik    (1000) henrik    (1000)     6965 2022-02-02 20:00:58.000000 pasimple-0.0.1/pasimple/pa_simple.py
-drwxr-xr-x   0 henrik    (1000) henrik    (1000)        0 2022-04-02 13:46:01.285380 pasimple-0.0.1/pasimple.egg-info/
--rw-r--r--   0 henrik    (1000) henrik    (1000)     9923 2022-04-02 13:46:00.000000 pasimple-0.0.1/pasimple.egg-info/PKG-INFO
--rw-r--r--   0 henrik    (1000) henrik    (1000)      236 2022-04-02 13:46:01.000000 pasimple-0.0.1/pasimple.egg-info/SOURCES.txt
--rw-r--r--   0 henrik    (1000) henrik    (1000)        1 2022-04-02 13:46:00.000000 pasimple-0.0.1/pasimple.egg-info/dependency_links.txt
--rw-r--r--   0 henrik    (1000) henrik    (1000)        9 2022-04-02 13:46:01.000000 pasimple-0.0.1/pasimple.egg-info/top_level.txt
--rw-r--r--   0 henrik    (1000) henrik    (1000)       93 2021-06-09 15:21:06.000000 pasimple-0.0.1/pyproject.toml
--rw-r--r--   0 henrik    (1000) henrik    (1000)      568 2022-04-02 13:46:01.285380 pasimple-0.0.1/setup.cfg
+drwxr-xr-x   0 henrik    (1000) henrik    (1000)        0 2023-04-22 00:05:40.725994 pasimple-0.0.2/
+-rw-r--r--   0 henrik    (1000) henrik    (1000)     1052 2023-04-21 16:57:18.000000 pasimple-0.0.2/LICENSE
+-rw-r--r--   0 henrik    (1000) henrik    (1000)    11934 2023-04-22 00:05:40.726994 pasimple-0.0.2/PKG-INFO
+-rw-r--r--   0 henrik    (1000) henrik    (1000)    11480 2023-04-21 23:52:14.000000 pasimple-0.0.2/README.md
+drwxr-xr-x   0 henrik    (1000) henrik    (1000)        0 2023-04-22 00:05:40.725994 pasimple-0.0.2/pasimple/
+-rw-r--r--   0 henrik    (1000) henrik    (1000)     3388 2023-04-21 16:57:18.000000 pasimple-0.0.2/pasimple/__init__.py
+-rw-r--r--   0 henrik    (1000) henrik    (1000)       98 2023-04-21 16:57:18.000000 pasimple-0.0.2/pasimple/exceptions.py
+-rw-r--r--   0 henrik    (1000) henrik    (1000)     7989 2023-04-21 23:47:51.000000 pasimple-0.0.2/pasimple/pa_simple.py
+drwxr-xr-x   0 henrik    (1000) henrik    (1000)        0 2023-04-22 00:05:40.725994 pasimple-0.0.2/pasimple.egg-info/
+-rw-r--r--   0 henrik    (1000) henrik    (1000)    11934 2023-04-22 00:05:40.000000 pasimple-0.0.2/pasimple.egg-info/PKG-INFO
+-rw-r--r--   0 henrik    (1000) henrik    (1000)      236 2023-04-22 00:05:40.000000 pasimple-0.0.2/pasimple.egg-info/SOURCES.txt
+-rw-r--r--   0 henrik    (1000) henrik    (1000)        1 2023-04-22 00:05:40.000000 pasimple-0.0.2/pasimple.egg-info/dependency_links.txt
+-rw-r--r--   0 henrik    (1000) henrik    (1000)        9 2023-04-22 00:05:40.000000 pasimple-0.0.2/pasimple.egg-info/top_level.txt
+-rw-r--r--   0 henrik    (1000) henrik    (1000)       93 2023-04-21 16:57:18.000000 pasimple-0.0.2/pyproject.toml
+-rw-r--r--   0 henrik    (1000) henrik    (1000)      570 2023-04-22 00:05:40.726994 pasimple-0.0.2/setup.cfg
```

### Comparing `pasimple-0.0.1/LICENSE` & `pasimple-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pasimple-0.0.1/PKG-INFO` & `pasimple-0.0.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: pasimple
-Version: 0.0.1
-Summary: PulseAudio "simple API" wrapper. Play/record audio via PulseAudio/PipeWire.
+Version: 0.0.2
+Summary: Play/record audio via PulseAudio/PipeWire. A PulseAudio "simple API" wrapper.
 Home-page: https://github.com/henrikschnor/pasimple
 Author: Henrik Schnor
 Author-email: hschnor@mailbox.org
 License: MIT
 Keywords: pulseaudio,pulse,pipewire,audio,recording,playback,play
 Platform: posix
 Classifier: Programming Language :: Python :: 3
@@ -25,15 +25,15 @@
 - A running PulseAudio/PipeWire server
 
 There's a good chance your Linux distribution comes with PulseAudio or PipeWire preinstalled.
 
 
 ## Installation
 
-```
+```sh
 pip3 install pasimple
 ```
 
 
 ## Quick start
 
 There are two simple convenience functions for recording/playing audio to/from a `.wav` file:
@@ -49,15 +49,15 @@
 ```
 
 Both functions block until all audio has been recorded/played. The default encoding used by `record_wav` is `PA_SAMPLE_S24LE`, mono, 41kHz. The function `play_wav` can only recognize files encoded in one of the following formats: `PA_SAMPLE_U8`, `PA_SAMPLE_S16LE`, `PA_SAMPLE_S24LE`, `PA_SAMPLE_S32LE`. For more complex use cases, scroll down to the "Documentation" section.
 
 
 ### Recording
 
-A more extensive example for recording audio can be found in [examples/record.py](examples/record.py):
+A more extensive example for recording audio can be found in [examples/record.py](https://github.com/henrikschnor/pasimple/blob/master/examples/record.py):
 
 ```python
 import wave
 import pasimple
 
 # Audio attributes for the recording
 FORMAT = pasimple.PA_SAMPLE_S32LE
@@ -82,15 +82,15 @@
 The recording starts as soon as the `PaSimple` object is created and audio data is buffered internally. Calls to `read` can retrieve the raw audio data, specifying the number of bytes to read as an argument. The function will block until the requested number of bytes is available. When done recording, the `PaSimple` object's audio stream should be closed with a call to `close()`. Alternatively, it can be used with python's context manager (the `with` statement in the example above).
 
 Finally, the data is written to a `.wav` file. We specify the audio format again, so that a correct `.wav` file header can be written.
 
 
 ### Playing
 
-An example for playing audio can be found in [examples/play.py](examples/play.py):
+An example for playing audio can be found in [examples/play.py](https://github.com/henrikschnor/pasimple/blob/master/examples/play.py):
 
 ```python
 import wave
 import pasimple
 
 # Read a .wav file with its attributes
 with wave.open('recording.wav', 'rb') as wave_file:
@@ -104,14 +104,19 @@
     pa.write(audio_data)
     pa.drain()
 ```
 
 To play a `.wav` file, we basically do the recording steps in reverse. First, we read the audio encoding together with the raw audio data from the file. When creating the `PaSimple` object, this time, we're opening a playback stream and specify the format of the audio we're going to play. It's then as simple as passing the raw audio data to the `write` function. Finally, we call `drain` to make sure all audio has played before closing the stream by leaving the `with` context.
 
 
+### Streaming
+
+An annotated example of how to stream audio from/to a source/sink can be found in [examples/echo.py](https://github.com/henrikschnor/pasimple/blob/master/examples/echo.py)
+
+
 ## Documentation
 
 This sections describes all constants/functions/classes available in the `pasimple` module.
 
 ### Constants
 
 **Stream directions**
@@ -175,23 +180,28 @@
 Records a `.wav` file via PulseAudio and blocks until all audio data has been recorded. The following formats are supported: `PA_SAMPLE_U8`, `PA_SAMPLE_S16LE`, `PA_SAMPLE_S24LE`, `PA_SAMPLE_S32LE`. Throws a `wave.Error` if the `.wav` file cannot be written or a `PaSimpleError` if the audio data cannot be recorded.
 
 
 ### PaSimple
 
 An instance of `PaSimple` represents an audio stream for playing or recording audio via PulseAudio. On error, all functions throw a `PaSimpleError`.
 
-**PaSimple**(`direction`, `format`, `channels`, `rate`, `app_name='python'`, `stream_name=None`, `server_name=None`, `device_name=None`):
+**PaSimple**(`direction`, `format`, `channels`, `rate`, `app_name='python'`, `stream_name=None`, `server_name=None`, `device_name=None`, `maxlength=-1`, `tlength=-1`, `prebuf=-1`, `minreq=-1`, `fragsize=-1`):
 - `direction`: Either `PA_STREAM_PLAYBACK` or `PA_STREAM_RECORD`.
 - `format`: The audio encoding (one of `PA_SAMPLE_*`) for this stream.
 - `channels`: Integer specifying the number of channels (1=mono, 2=stereo).
 - `rate`: Integer specifying the sample rate in Hz.
 - `app_name`: String specifying the name of the application that will be registered in PulseAudio.
 - `stream_name`: `None` (use `app_name`) or a string specifying the name of this stream that will be registered in PulseAudio.
-- `server_name`: `None` (use default) or a string specifying a PulseAudio server name.
-- `device_name`: `None` (use default) or a string specifying a specific PulseAudio device for recording or playback.
+- `server_name`: `None` (default) or a string specifying a PulseAudio server name.
+- `device_name`: `None` (default) or a string specifying a specific PulseAudio device for recording or playback.
+- `maxlength`: `-1` (default: max supported) or an integer specifying the buffer size limit in bytes.
+- `tlength`: `-1` (default: about 2s) or an integer specifying how many bytes to keep in the playback buffer.
+- `prebuf`: `-1` (use `tlength`) or an integer specifying how many bytes to buffer before starting playback.
+- `minreq`: `-1` (default: about 2s) or an integer specifying the minimum size of chunks for refilling the playback buffer in bytes.
+- `fragsize`: `-1` (default: about 2s) or an integer specifying the size of recording chunks in bytes.
 
 Initialize a PulseAudio simple API stream for playing or recording audio data.
 
 
 **close()**
 
 Close the underlying stream and free resources.
@@ -240,7 +250,41 @@
 
 
 **get_latency()**
 
 Returns the record/playback latency reported by PulseAudio in microseconds.
 
 
+### PulseAudio error codes
+
+This list of PulseAudio internal error codes has been [taken from here](https://gitlab.freedesktop.org/pulseaudio/pulseaudio/-/blob/master/src/pulse/def.h#L471).
+
+| Error code | Description |
+| --- | --- |
+| 0 | No error |
+| 1 | Access failure |
+| 2 | Unknown command |
+| 3 | Invalid argument |
+| 4 | Entity exists |
+| 5 | No such entity |
+| 6 | Connection refused |
+| 7 | Protocol error |
+| 8 | Timeout |
+| 9 | No authentication key |
+| 10 | Internal error |
+| 11 | Connection terminated |
+| 12 | Entity killed |
+| 13 | Invalid server |
+| 14 | Module initialization failed |
+| 15 | Bad state |
+| 16 | No data |
+| 17 | Incompatible protocol version |
+| 18 | Data too large |
+| 19 | Operation not supported |
+| 20 | The error code was unknown to the client |
+| 21 | Extension does not exist |
+| 22 | Obsolete functionality |
+| 23 | Missing implementation |
+| 24 | The caller forked without calling execve() and tried to reuse the context |
+| 25 | An IO error happened |
+| 26 | Device or resource busy |
+| 27 | Not really an error but the first invalid error code |
```

### Comparing `pasimple-0.0.1/README.md` & `pasimple-0.0.2/pasimple.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+Metadata-Version: 2.1
+Name: pasimple
+Version: 0.0.2
+Summary: Play/record audio via PulseAudio/PipeWire. A PulseAudio "simple API" wrapper.
+Home-page: https://github.com/henrikschnor/pasimple
+Author: Henrik Schnor
+Author-email: hschnor@mailbox.org
+License: MIT
+Keywords: pulseaudio,pulse,pipewire,audio,recording,playback,play
+Platform: posix
+Classifier: Programming Language :: Python :: 3
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # pulseaudio-simple
 
 A python wrapper for the [pulseaudio simple API](https://www.freedesktop.org/software/pulseaudio/doxygen/simple.html). Supports playing and recording audio via PulseAudio and PipeWire.
 
 This library is feature-complete, so there won't be much ongoing activity in this repository. Reported bugs will be fixed. PRs for improvements are always welcome.
 
 
@@ -11,15 +25,15 @@
 - A running PulseAudio/PipeWire server
 
 There's a good chance your Linux distribution comes with PulseAudio or PipeWire preinstalled.
 
 
 ## Installation
 
-```
+```sh
 pip3 install pasimple
 ```
 
 
 ## Quick start
 
 There are two simple convenience functions for recording/playing audio to/from a `.wav` file:
@@ -35,15 +49,15 @@
 ```
 
 Both functions block until all audio has been recorded/played. The default encoding used by `record_wav` is `PA_SAMPLE_S24LE`, mono, 41kHz. The function `play_wav` can only recognize files encoded in one of the following formats: `PA_SAMPLE_U8`, `PA_SAMPLE_S16LE`, `PA_SAMPLE_S24LE`, `PA_SAMPLE_S32LE`. For more complex use cases, scroll down to the "Documentation" section.
 
 
 ### Recording
 
-A more extensive example for recording audio can be found in [examples/record.py](examples/record.py):
+A more extensive example for recording audio can be found in [examples/record.py](https://github.com/henrikschnor/pasimple/blob/master/examples/record.py):
 
 ```python
 import wave
 import pasimple
 
 # Audio attributes for the recording
 FORMAT = pasimple.PA_SAMPLE_S32LE
@@ -68,15 +82,15 @@
 The recording starts as soon as the `PaSimple` object is created and audio data is buffered internally. Calls to `read` can retrieve the raw audio data, specifying the number of bytes to read as an argument. The function will block until the requested number of bytes is available. When done recording, the `PaSimple` object's audio stream should be closed with a call to `close()`. Alternatively, it can be used with python's context manager (the `with` statement in the example above).
 
 Finally, the data is written to a `.wav` file. We specify the audio format again, so that a correct `.wav` file header can be written.
 
 
 ### Playing
 
-An example for playing audio can be found in [examples/play.py](examples/play.py):
+An example for playing audio can be found in [examples/play.py](https://github.com/henrikschnor/pasimple/blob/master/examples/play.py):
 
 ```python
 import wave
 import pasimple
 
 # Read a .wav file with its attributes
 with wave.open('recording.wav', 'rb') as wave_file:
@@ -90,14 +104,19 @@
     pa.write(audio_data)
     pa.drain()
 ```
 
 To play a `.wav` file, we basically do the recording steps in reverse. First, we read the audio encoding together with the raw audio data from the file. When creating the `PaSimple` object, this time, we're opening a playback stream and specify the format of the audio we're going to play. It's then as simple as passing the raw audio data to the `write` function. Finally, we call `drain` to make sure all audio has played before closing the stream by leaving the `with` context.
 
 
+### Streaming
+
+An annotated example of how to stream audio from/to a source/sink can be found in [examples/echo.py](https://github.com/henrikschnor/pasimple/blob/master/examples/echo.py)
+
+
 ## Documentation
 
 This sections describes all constants/functions/classes available in the `pasimple` module.
 
 ### Constants
 
 **Stream directions**
@@ -161,23 +180,28 @@
 Records a `.wav` file via PulseAudio and blocks until all audio data has been recorded. The following formats are supported: `PA_SAMPLE_U8`, `PA_SAMPLE_S16LE`, `PA_SAMPLE_S24LE`, `PA_SAMPLE_S32LE`. Throws a `wave.Error` if the `.wav` file cannot be written or a `PaSimpleError` if the audio data cannot be recorded.
 
 
 ### PaSimple
 
 An instance of `PaSimple` represents an audio stream for playing or recording audio via PulseAudio. On error, all functions throw a `PaSimpleError`.
 
-**PaSimple**(`direction`, `format`, `channels`, `rate`, `app_name='python'`, `stream_name=None`, `server_name=None`, `device_name=None`):
+**PaSimple**(`direction`, `format`, `channels`, `rate`, `app_name='python'`, `stream_name=None`, `server_name=None`, `device_name=None`, `maxlength=-1`, `tlength=-1`, `prebuf=-1`, `minreq=-1`, `fragsize=-1`):
 - `direction`: Either `PA_STREAM_PLAYBACK` or `PA_STREAM_RECORD`.
 - `format`: The audio encoding (one of `PA_SAMPLE_*`) for this stream.
 - `channels`: Integer specifying the number of channels (1=mono, 2=stereo).
 - `rate`: Integer specifying the sample rate in Hz.
 - `app_name`: String specifying the name of the application that will be registered in PulseAudio.
 - `stream_name`: `None` (use `app_name`) or a string specifying the name of this stream that will be registered in PulseAudio.
-- `server_name`: `None` (use default) or a string specifying a PulseAudio server name.
-- `device_name`: `None` (use default) or a string specifying a specific PulseAudio device for recording or playback.
+- `server_name`: `None` (default) or a string specifying a PulseAudio server name.
+- `device_name`: `None` (default) or a string specifying a specific PulseAudio device for recording or playback.
+- `maxlength`: `-1` (default: max supported) or an integer specifying the buffer size limit in bytes.
+- `tlength`: `-1` (default: about 2s) or an integer specifying how many bytes to keep in the playback buffer.
+- `prebuf`: `-1` (use `tlength`) or an integer specifying how many bytes to buffer before starting playback.
+- `minreq`: `-1` (default: about 2s) or an integer specifying the minimum size of chunks for refilling the playback buffer in bytes.
+- `fragsize`: `-1` (default: about 2s) or an integer specifying the size of recording chunks in bytes.
 
 Initialize a PulseAudio simple API stream for playing or recording audio data.
 
 
 **close()**
 
 Close the underlying stream and free resources.
@@ -224,7 +248,43 @@
 
 Discards any data in the record/playback buffers.
 
 
 **get_latency()**
 
 Returns the record/playback latency reported by PulseAudio in microseconds.
+
+
+### PulseAudio error codes
+
+This list of PulseAudio internal error codes has been [taken from here](https://gitlab.freedesktop.org/pulseaudio/pulseaudio/-/blob/master/src/pulse/def.h#L471).
+
+| Error code | Description |
+| --- | --- |
+| 0 | No error |
+| 1 | Access failure |
+| 2 | Unknown command |
+| 3 | Invalid argument |
+| 4 | Entity exists |
+| 5 | No such entity |
+| 6 | Connection refused |
+| 7 | Protocol error |
+| 8 | Timeout |
+| 9 | No authentication key |
+| 10 | Internal error |
+| 11 | Connection terminated |
+| 12 | Entity killed |
+| 13 | Invalid server |
+| 14 | Module initialization failed |
+| 15 | Bad state |
+| 16 | No data |
+| 17 | Incompatible protocol version |
+| 18 | Data too large |
+| 19 | Operation not supported |
+| 20 | The error code was unknown to the client |
+| 21 | Extension does not exist |
+| 22 | Obsolete functionality |
+| 23 | Missing implementation |
+| 24 | The caller forked without calling execve() and tried to reuse the context |
+| 25 | An IO error happened |
+| 26 | Device or resource busy |
+| 27 | Not really an error but the first invalid error code |
```

### Comparing `pasimple-0.0.1/pasimple/__init__.py` & `pasimple-0.0.2/pasimple/__init__.py`

 * *Files identical despite different names*

### Comparing `pasimple-0.0.1/pasimple/pa_simple.py` & `pasimple-0.0.2/pasimple/pa_simple.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 _libpulse_simple = None
 def get_libpulse_simple():
     global _libpulse_simple
     if _libpulse_simple is None:
         try:
             _libpulse_simple = ctypes.CDLL('libpulse-simple.so.0')
             _libpulse_simple.pa_simple_new.restype = ctypes.c_void_p
-            _libpulse_simple.pa_simple_get_latency = ctypes.c_ulonglong
+            _libpulse_simple.pa_simple_get_latency.restype = ctypes.c_uint64
         except OSError as err:
             raise PaSimpleError(f'{type(err)}: {err}')
     return _libpulse_simple
 
 
 class pa_sample_spec(ctypes.Structure):
     """Struct describing the audio encoding for the pulse server"""
@@ -23,50 +23,72 @@
     _fields_ = [
         ('format', ctypes.c_int),
         ('rate', ctypes.c_uint32),
         ('channels', ctypes.c_uint8)
     ]
 
 
+class pa_buffer_attr(ctypes.Structure):
+    """Struct describing playback and record buffer metrics"""
+
+    _fields_ = [
+        ('maxlength', ctypes.c_uint32),
+        ('tlength', ctypes.c_uint32),
+        ('prebuf', ctypes.c_uint32),
+        ('minreq', ctypes.c_uint32),
+        ('fragsize', ctypes.c_uint32),
+    ]
+
+
 class PaSimple:
-    def __init__(self, direction, format, channels, rate, app_name='python', stream_name=None, server_name=None, device_name=None):
+    def __init__(self, direction, format, channels, rate, app_name='python',
+                 stream_name=None, server_name=None, device_name=None,
+                 maxlength=-1, tlength=-1, prebuf=-1, minreq=-1, fragsize=-1):
         """Initialize a pulseaudio simple API stream.
 
         direction: either PA_STREAM_PLAYBACK or PA_STREAM_RECORD
         format: one of the PA_SAMPLE_* formats
         channels: integer specifying the number of channels
         rate: integer specifying the sample rate
         app_name: string specifying the name of the application
         stream_name: None (use app_name) or string specifying a name for this stream
         server_name: None (use default) or string specifying a pulseaudio server name
         device_name: None (use default) or string specifying a pulseaudio device
+
+        Buffer-related options are in units of bytes:
+        maxlength: integer buffer size limit, or -1 (default: max supported)
+        tlength: keep this many bytes in playback buffer, or -1 (default: about 2s)
+        prebuf: buffer this many bytes before starting playback, or -1 (default: ==tlength)
+        minreq: refill playback buffer in chunks at least this big, or -1 (default: about 2s)
+        fragsize: receive recorded audio in chunks of this size, or -1 (default: about 2s)
         """
 
         # Save audio encoding properties
         self._direction = direction
         self._format = format
         self._channels = channels
         self._rate = rate
 
         # If no stream_name is specified, use the app_name
         if stream_name is None:
             stream_name = app_name
 
         # Prepare arguments for initializing a pulseaudio stream
         sample_spec = pa_sample_spec(format, rate, channels)
+        buffer_attr = pa_buffer_attr(maxlength, tlength, prebuf, minreq, fragsize)
         arg_server_name = ctypes.c_char_p(server_name.encode()) if server_name is not None else None
         arg_app_name = ctypes.c_char_p(app_name.encode())
         arg_device_name = ctypes.c_char_p(device_name.encode()) if device_name is not None else None
         arg_stream_name = ctypes.c_char_p(stream_name.encode())
         error = ctypes.c_int(0)
 
         # Initialize the stream.
         # Keep track of the underlying stream's state to avoid double frees
         self._stream_alive = False
-        self._stream = get_libpulse_simple().pa_simple_new(arg_server_name, arg_app_name, direction, arg_device_name, arg_stream_name, ctypes.byref(sample_spec), None, None, ctypes.byref(error))
+        self._stream = get_libpulse_simple().pa_simple_new(arg_server_name, arg_app_name, direction, arg_device_name, arg_stream_name, ctypes.byref(sample_spec), None, ctypes.byref(buffer_attr), ctypes.byref(error))
         if self._stream is None:
             raise PaSimpleError(f'Error while creating stream: {error.value}')
         self._stream_alive = True
 
 
     def close(self):
         """Close the underlying stream and free resources"""
@@ -126,15 +148,15 @@
         
         rec_buffer = bytearray(num_bytes)
         rec_buffer_ptr = ctypes.c_char * num_bytes
         error = ctypes.c_int(0)
         ok = get_libpulse_simple().pa_simple_read(ctypes.c_void_p(self._stream), rec_buffer_ptr.from_buffer(rec_buffer), num_bytes, ctypes.byref(error))
         if ok != 0:
             raise PaSimpleError(f'Could not record audio, error code: {error.value}')
-        return rec_buffer
+        return bytes(rec_buffer)
 
 
     def write(self, data):
         """Play audio via the PulseAudio server.
 
         PA_STREAM_PLAYBACK must be used during initialization.
         Encoding of `data` must match the one specified in the constructor.
@@ -181,10 +203,10 @@
         """Get the record/playback latency reported by PulseAudio in microseconds"""
 
         if not self._stream_alive:
             raise PaSimpleError('Cannot perform operation on closed stream')
         
         error = ctypes.c_int(0)
         latency = get_libpulse_simple().pa_simple_get_latency(ctypes.c_void_p(self._stream), ctypes.byref(error))
-        if error != 0:
+        if error.value != 0:
             raise PaSimpleError(f'Could not get latency, error code: {error.value}')
-        return latency.value
+        return latency
```

### Comparing `pasimple-0.0.1/pasimple.egg-info/PKG-INFO` & `pasimple-0.0.2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: pasimple
-Version: 0.0.1
-Summary: PulseAudio "simple API" wrapper. Play/record audio via PulseAudio/PipeWire.
-Home-page: https://github.com/henrikschnor/pasimple
-Author: Henrik Schnor
-Author-email: hschnor@mailbox.org
-License: MIT
-Keywords: pulseaudio,pulse,pipewire,audio,recording,playback,play
-Platform: posix
-Classifier: Programming Language :: Python :: 3
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # pulseaudio-simple
 
 A python wrapper for the [pulseaudio simple API](https://www.freedesktop.org/software/pulseaudio/doxygen/simple.html). Supports playing and recording audio via PulseAudio and PipeWire.
 
 This library is feature-complete, so there won't be much ongoing activity in this repository. Reported bugs will be fixed. PRs for improvements are always welcome.
 
 
@@ -25,15 +11,15 @@
 - A running PulseAudio/PipeWire server
 
 There's a good chance your Linux distribution comes with PulseAudio or PipeWire preinstalled.
 
 
 ## Installation
 
-```
+```sh
 pip3 install pasimple
 ```
 
 
 ## Quick start
 
 There are two simple convenience functions for recording/playing audio to/from a `.wav` file:
@@ -49,15 +35,15 @@
 ```
 
 Both functions block until all audio has been recorded/played. The default encoding used by `record_wav` is `PA_SAMPLE_S24LE`, mono, 41kHz. The function `play_wav` can only recognize files encoded in one of the following formats: `PA_SAMPLE_U8`, `PA_SAMPLE_S16LE`, `PA_SAMPLE_S24LE`, `PA_SAMPLE_S32LE`. For more complex use cases, scroll down to the "Documentation" section.
 
 
 ### Recording
 
-A more extensive example for recording audio can be found in [examples/record.py](examples/record.py):
+A more extensive example for recording audio can be found in [examples/record.py](https://github.com/henrikschnor/pasimple/blob/master/examples/record.py):
 
 ```python
 import wave
 import pasimple
 
 # Audio attributes for the recording
 FORMAT = pasimple.PA_SAMPLE_S32LE
@@ -82,15 +68,15 @@
 The recording starts as soon as the `PaSimple` object is created and audio data is buffered internally. Calls to `read` can retrieve the raw audio data, specifying the number of bytes to read as an argument. The function will block until the requested number of bytes is available. When done recording, the `PaSimple` object's audio stream should be closed with a call to `close()`. Alternatively, it can be used with python's context manager (the `with` statement in the example above).
 
 Finally, the data is written to a `.wav` file. We specify the audio format again, so that a correct `.wav` file header can be written.
 
 
 ### Playing
 
-An example for playing audio can be found in [examples/play.py](examples/play.py):
+An example for playing audio can be found in [examples/play.py](https://github.com/henrikschnor/pasimple/blob/master/examples/play.py):
 
 ```python
 import wave
 import pasimple
 
 # Read a .wav file with its attributes
 with wave.open('recording.wav', 'rb') as wave_file:
@@ -104,14 +90,19 @@
     pa.write(audio_data)
     pa.drain()
 ```
 
 To play a `.wav` file, we basically do the recording steps in reverse. First, we read the audio encoding together with the raw audio data from the file. When creating the `PaSimple` object, this time, we're opening a playback stream and specify the format of the audio we're going to play. It's then as simple as passing the raw audio data to the `write` function. Finally, we call `drain` to make sure all audio has played before closing the stream by leaving the `with` context.
 
 
+### Streaming
+
+An annotated example of how to stream audio from/to a source/sink can be found in [examples/echo.py](https://github.com/henrikschnor/pasimple/blob/master/examples/echo.py)
+
+
 ## Documentation
 
 This sections describes all constants/functions/classes available in the `pasimple` module.
 
 ### Constants
 
 **Stream directions**
@@ -175,23 +166,28 @@
 Records a `.wav` file via PulseAudio and blocks until all audio data has been recorded. The following formats are supported: `PA_SAMPLE_U8`, `PA_SAMPLE_S16LE`, `PA_SAMPLE_S24LE`, `PA_SAMPLE_S32LE`. Throws a `wave.Error` if the `.wav` file cannot be written or a `PaSimpleError` if the audio data cannot be recorded.
 
 
 ### PaSimple
 
 An instance of `PaSimple` represents an audio stream for playing or recording audio via PulseAudio. On error, all functions throw a `PaSimpleError`.
 
-**PaSimple**(`direction`, `format`, `channels`, `rate`, `app_name='python'`, `stream_name=None`, `server_name=None`, `device_name=None`):
+**PaSimple**(`direction`, `format`, `channels`, `rate`, `app_name='python'`, `stream_name=None`, `server_name=None`, `device_name=None`, `maxlength=-1`, `tlength=-1`, `prebuf=-1`, `minreq=-1`, `fragsize=-1`):
 - `direction`: Either `PA_STREAM_PLAYBACK` or `PA_STREAM_RECORD`.
 - `format`: The audio encoding (one of `PA_SAMPLE_*`) for this stream.
 - `channels`: Integer specifying the number of channels (1=mono, 2=stereo).
 - `rate`: Integer specifying the sample rate in Hz.
 - `app_name`: String specifying the name of the application that will be registered in PulseAudio.
 - `stream_name`: `None` (use `app_name`) or a string specifying the name of this stream that will be registered in PulseAudio.
-- `server_name`: `None` (use default) or a string specifying a PulseAudio server name.
-- `device_name`: `None` (use default) or a string specifying a specific PulseAudio device for recording or playback.
+- `server_name`: `None` (default) or a string specifying a PulseAudio server name.
+- `device_name`: `None` (default) or a string specifying a specific PulseAudio device for recording or playback.
+- `maxlength`: `-1` (default: max supported) or an integer specifying the buffer size limit in bytes.
+- `tlength`: `-1` (default: about 2s) or an integer specifying how many bytes to keep in the playback buffer.
+- `prebuf`: `-1` (use `tlength`) or an integer specifying how many bytes to buffer before starting playback.
+- `minreq`: `-1` (default: about 2s) or an integer specifying the minimum size of chunks for refilling the playback buffer in bytes.
+- `fragsize`: `-1` (default: about 2s) or an integer specifying the size of recording chunks in bytes.
 
 Initialize a PulseAudio simple API stream for playing or recording audio data.
 
 
 **close()**
 
 Close the underlying stream and free resources.
@@ -240,7 +236,41 @@
 
 
 **get_latency()**
 
 Returns the record/playback latency reported by PulseAudio in microseconds.
 
 
+### PulseAudio error codes
+
+This list of PulseAudio internal error codes has been [taken from here](https://gitlab.freedesktop.org/pulseaudio/pulseaudio/-/blob/master/src/pulse/def.h#L471).
+
+| Error code | Description |
+| --- | --- |
+| 0 | No error |
+| 1 | Access failure |
+| 2 | Unknown command |
+| 3 | Invalid argument |
+| 4 | Entity exists |
+| 5 | No such entity |
+| 6 | Connection refused |
+| 7 | Protocol error |
+| 8 | Timeout |
+| 9 | No authentication key |
+| 10 | Internal error |
+| 11 | Connection terminated |
+| 12 | Entity killed |
+| 13 | Invalid server |
+| 14 | Module initialization failed |
+| 15 | Bad state |
+| 16 | No data |
+| 17 | Incompatible protocol version |
+| 18 | Data too large |
+| 19 | Operation not supported |
+| 20 | The error code was unknown to the client |
+| 21 | Extension does not exist |
+| 22 | Obsolete functionality |
+| 23 | Missing implementation |
+| 24 | The caller forked without calling execve() and tried to reuse the context |
+| 25 | An IO error happened |
+| 26 | Device or resource busy |
+| 27 | Not really an error but the first invalid error code |
```

### Comparing `pasimple-0.0.1/setup.cfg` & `pasimple-0.0.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [metadata]
 name = pasimple
-version = 0.0.1
+version = 0.0.2
 author = Henrik Schnor
 author_email = hschnor@mailbox.org
 url = https://github.com/henrikschnor/pasimple
-description = PulseAudio "simple API" wrapper. Play/record audio via PulseAudio/PipeWire.
+description = Play/record audio via PulseAudio/PipeWire. A PulseAudio "simple API" wrapper.
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = pulseaudio, pulse, pipewire, audio, recording, playback, play
 license = MIT
 license_file = LICENSE
 platform = posix
 classifiers =
```

