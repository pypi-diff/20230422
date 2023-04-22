# Comparing `tmp/deew-2.9.5.tar.gz` & `tmp/deew-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deew-2.9.5.tar", max compression
+gzip compressed data, was "deew-3.0.0.tar", max compression
```

## Comparing `deew-2.9.5.tar` & `deew-3.0.0.tar`

### file list

```diff
@@ -1,10 +1,9 @@
--rw-r--r--   0        0        0    44584 2022-11-24 23:47:57.870981 deew-2.9.5/deew/__main__.py
--rw-r--r--   0        0        0     1080 2022-11-24 23:47:57.870981 deew-2.9.5/deew/bitrates.py
--rw-r--r--   0        0        0     9112 2022-11-24 23:47:57.870981 deew-2.9.5/deew/logos.py
--rw-r--r--   0        0        0     2162 2022-11-24 23:47:57.870981 deew-2.9.5/deew/messages.py
--rw-r--r--   0        0        0     8288 2022-11-24 23:47:57.870981 deew-2.9.5/deew/xml_base.py
--rw-r--r--   0        0        0     1086 2022-11-24 23:47:57.870981 deew-2.9.5/LICENSE
--rw-r--r--   0        0        0      586 2022-11-24 23:47:57.886621 deew-2.9.5/pyproject.toml
--rw-r--r--   0        0        0    10422 2022-11-24 23:47:57.870981 deew-2.9.5/README.md
--rw-r--r--   0        0        0    11331 1970-01-01 00:00:00.000000 deew-2.9.5/setup.py
--rw-r--r--   0        0        0    11114 1970-01-01 00:00:00.000000 deew-2.9.5/PKG-INFO
+-rw-r--r--   0        0        0    46890 2023-04-22 13:55:31.689447 deew-3.0.0/deew/__main__.py
+-rw-r--r--   0        0        0     1125 2023-04-22 13:55:31.689447 deew-3.0.0/deew/bitrates.py
+-rw-r--r--   0        0        0     9112 2023-04-22 13:55:31.689447 deew-3.0.0/deew/logos.py
+-rw-r--r--   0        0        0     2450 2023-04-22 13:55:31.689447 deew-3.0.0/deew/messages.py
+-rw-r--r--   0        0        0    11603 2023-04-22 13:55:31.689447 deew-3.0.0/deew/xml_base.py
+-rw-r--r--   0        0        0     1086 2023-04-22 13:55:31.673805 deew-3.0.0/LICENSE
+-rw-r--r--   0        0        0      593 2023-04-22 13:55:31.689447 deew-3.0.0/pyproject.toml
+-rw-r--r--   0        0        0    10120 2023-04-22 13:55:31.673805 deew-3.0.0/README.md
+-rw-r--r--   0        0        0    10814 1970-01-01 00:00:00.000000 deew-3.0.0/PKG-INFO
```

### Comparing `deew-2.9.5/deew/__main__.py` & `deew-3.0.0/deew/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,18 +38,18 @@
 from unidecode import unidecode
 
 sys.path.append('.')
 
 from deew.bitrates import allowed_bitrates
 from deew.logos import logos
 from deew.messages import error_messages
-from deew.xml_base import xml_dd_ddp_base, xml_thd_base
+from deew.xml_base import xml_dd_ddp_base, xml_thd_base, xml_ac4_base
 
 prog_name = 'deew'
-prog_version = '2.9.5'
+prog_version = '3.0.0'
 
 simplens = SimpleNamespace()
 
 
 class RParse(argparse.ArgumentParser):
     def _print_message(self, message, file=None):
         if message:
@@ -101,15 +101,15 @@
                     default=None,
                     metavar='DIRECTORY',
                     help='[underline magenta]default:[/underline magenta] current directory\nspecifies output directory')
 parser.add_argument('-f', '--format',
                     type=str,
                     default='ddp',
                     help=
-'''[underline magenta]options:[/underline magenta] [bold color(231)]dd[/bold color(231)] / [bold color(231)]ddp[/bold color(231)] / [bold color(231)]thd[/bold color(231)]
+'''[underline magenta]options:[/underline magenta] [bold color(231)]dd[/bold color(231)] / [bold color(231)]ddp[/bold color(231)] / [bold color(231)]ac4[/bold color(231)] / [bold color(231)]thd[/bold color(231)]
 [underline magenta]default:[/underline magenta] [bold color(231)]ddp[/bold color(231)]''')
 parser.add_argument('-b', '--bitrate',
                     type=int,
                     default=None,
                     help=
 '''[underline magenta]options:[/underline magenta] run [green]-lb[/green]/[green]--list-bitrates[/green]
 [underline magenta]default:[/underline magenta] run [green]-c[/green]/[green]--config[/green]''')
@@ -262,14 +262,15 @@
     dd_1_0 = 128
     dd_2_0 = 256
     dd_5_1 = 640
     ddp_1_0 = 128
     ddp_2_0 = 256
     ddp_5_1 = 1024
     ddp_7_1 = 1536
+    ac4_2_0 = 320
 
 # You can toggle what sections you would like to see in the encoding summary
 [summary_sections]
     deew_info = true
     binaries = true
     input_info = true
     output_info = true
@@ -314,16 +315,16 @@
 
 
 def parse_version_string(inp: list) -> str:
     try:
         v = subprocess.run(inp, capture_output=True, encoding='utf-8').stdout
         v = v.split('\n')[0].split(' ')[2]
         v = v.replace(',', '').replace('-static', '')
-        if len(v) > 20:
-            v = f'{v[0:17]}...'
+        if len(v) > 30:
+            v = f'{v[0:27]}...'
     except Exception:
         v = "[red]couldn't parse"
     return v
 
 def convert_delay_to_ms(inp, compensate):
     if not inp.startswith(('-', '+')): print_exit('delay')
     inp = inp.replace(',', '.')
@@ -604,18 +605,18 @@
 
     aformat = args.format.lower()
     bitrate = args.bitrate
     downmix = args.downmix
     args.dialnorm = clamp(args.dialnorm, -31, 0)
     trackindex = max(0, args.track_index)
 
-    if aformat not in ['dd', 'ddp', 'thd']: print_exit('format')
+    if aformat not in ['dd', 'ddp', 'thd', 'ac4']: print_exit('format')
     if downmix and downmix not in [1, 2, 6]: print_exit('downmix')
     if downmix and aformat == 'thd': print_exit('thd_downmix')
-    if args.drc not in ['film_light', 'film_standard', 'music_light', 'music_standard', 'speech']: print_exit('drc')
+    if args.drc not in ['film_light', 'film_standard', 'music_light', 'music_standard', 'speech', 'none']: print_exit('drc')
     if not simplens.dee_is_exe and platform.system() == 'Linux' and aformat == 'thd': print_exit('linux_thd')
     if args.measure_only: aformat = 'ddp'
 
     filelist = []
     for f in args.input:
         if not os.path.exists(f): print_exit('path', f)
         if os.path.isdir(f):
@@ -656,31 +657,44 @@
             bit_depth = 24
         else:
             bit_depth = 32
 
     if channels not in [1, 2, 6, 8]: print_exit('channels')
     if downmix and downmix >= channels: print_exit('downmix_mismatch')
     if not downmix and aformat == 'dd' and channels == 8: downmix = 6
+    if aformat == 'ac4' and channels != 6: print_exit('ac4_input_channels')
+    if aformat == 'ac4': downmix = 2
+    if aformat == 'thd' and channels == 1: print_exit('thd_mono_input')
 
     downmix_config = 'off'
     if downmix:
         outchannels = downmix
         downmix_config = channel_number_to_name(outchannels)
     else:
         outchannels = channels
 
-    if outchannels in [1, 2]:
+    if outchannels in [1, 2] and aformat in ['dd', 'ddp']:
         if args.no_prompt:
             print('Consider using [bold cyan]qaac[/bold cyan] or [bold cyan]opus[/bold cyan] for \
 [bold yellow]mono[/bold yellow] and [bold yellow]stereo[/bold yellow] encoding.')
         else:
             continue_enc = Confirm.ask('Consider using [bold cyan]qaac[/bold cyan] or [bold cyan]opus[/bold cyan] for \
 [bold yellow]mono[/bold yellow] and [bold yellow]stereo[/bold yellow] encoding, are you sure you want to use [bold cyan]DEE[/bold cyan]?')
             if not continue_enc: sys.exit(1)
 
+    if outchannels == 2 and aformat == 'thd':
+        if args.no_prompt:
+            print('Consider using [bold cyan]FLAC[/bold cyan] for lossless \
+[bold yellow]mono[/bold yellow] and [bold yellow]stereo[/bold yellow] encoding.')
+        else:
+            continue_enc = Confirm.ask('Consider using [bold cyan]FLAC[/bold cyan] for lossless \
+[bold yellow]mono[/bold yellow] and [bold yellow]stereo[/bold yellow] encoding, are you sure you want to use [bold cyan]DEE[/bold cyan]?')
+            if not continue_enc: sys.exit(1)
+
+
     if args.dialnorm != 0:
         if args.no_prompt:
             print('Consider leaving the dialnorm value at 0 (auto), setting it manually can be dangerous.')
         else:
             continue_enc = Confirm.ask('Consider leaving the dialnorm value at 0 (auto), setting it manually can be dangerous, are you sure you want to do it?')
             if not continue_enc: sys.exit(1)
 
@@ -690,15 +704,15 @@
             bitrate = find_closest_allowed(bitrate, allowed_bitrates['dd_10'])
         elif outchannels == 2:
             if not bitrate: bitrate = config['default_bitrates']['dd_2_0']
             bitrate = find_closest_allowed(bitrate, allowed_bitrates['dd_20'])
         elif outchannels == 6:
             if not bitrate: bitrate = config['default_bitrates']['dd_5_1']
             bitrate = find_closest_allowed(bitrate, allowed_bitrates['dd_51'])
-    elif aformat == 'ddp':
+    if aformat == 'ddp':
         if outchannels == 1:
             if not bitrate: bitrate = config['default_bitrates']['ddp_1_0']
             bitrate = find_closest_allowed(bitrate, allowed_bitrates['ddp_10'])
         elif outchannels == 2:
             if not bitrate: bitrate = config['default_bitrates']['ddp_2_0']
             bitrate = find_closest_allowed(bitrate, allowed_bitrates['ddp_20'])
         elif outchannels == 6:
@@ -708,14 +722,17 @@
             if not bitrate: bitrate = config['default_bitrates']['ddp_7_1']
             if args.force_standard:
                 bitrate = find_closest_allowed(bitrate, allowed_bitrates['ddp_71_standard'])
             elif args.force_bluray:
                 bitrate = find_closest_allowed(bitrate, allowed_bitrates['ddp_71_bluray'])
             else:
                 bitrate = find_closest_allowed(bitrate, allowed_bitrates['ddp_71_combined'])
+    elif aformat == 'ac4':
+        if not bitrate: bitrate = config['default_bitrates']['ac4_2_0']
+        bitrate = find_closest_allowed(bitrate, allowed_bitrates['ac4_20'])
 
     if args.output:
         createdir(os.path.abspath(args.output))
         output = os.path.abspath(args.output)
     else:
         output = os.getcwd()
 
@@ -735,14 +752,23 @@
         if aformat == 'dd':
             xml_base['job_config']['filter']['audio']['pcm_to_ddp']['encoder_mode'] = 'dd'
         xml_base['job_config']['filter']['audio']['pcm_to_ddp']['downmix_config'] = downmix_config
         xml_base['job_config']['filter']['audio']['pcm_to_ddp']['data_rate'] = bitrate
         xml_base['job_config']['filter']['audio']['pcm_to_ddp']['drc']['line_mode_drc_profile'] = args.drc
         xml_base['job_config']['filter']['audio']['pcm_to_ddp']['drc']['rf_mode_drc_profile'] = args.drc
         xml_base['job_config']['filter']['audio']['pcm_to_ddp']['custom_dialnorm'] = args.dialnorm
+    elif aformat in ['ac4']:
+        xml_base = xmltodict.parse(xml_ac4_base)
+        xml_base['job_config']['output']['ac4']['storage']['local']['path'] = wpc(output, quote=True)
+        xml_base['job_config']['filter']['audio']['encode_to_ims_ac4']['data_rate'] = bitrate
+        xml_base['job_config']['filter']['audio']['encode_to_ims_ac4']['drc']['ddp_drc_profile'] = args.drc
+        xml_base['job_config']['filter']['audio']['encode_to_ims_ac4']['drc']['flat_panel_drc_profile'] = args.drc
+        xml_base['job_config']['filter']['audio']['encode_to_ims_ac4']['drc']['home_theatre_drc_profile'] = args.drc
+        xml_base['job_config']['filter']['audio']['encode_to_ims_ac4']['drc']['portable_hp_drc_profile'] = args.drc
+        xml_base['job_config']['filter']['audio']['encode_to_ims_ac4']['drc']['portable_spkr_drc_profile'] = args.drc
     elif aformat == 'thd':
         xml_base = xmltodict.parse(xml_thd_base)
         xml_base['job_config']['output']['mlp']['storage']['local']['path'] = wpc(output, quote=True)
         xml_base['job_config']['filter']['audio']['encode_to_dthd']['atmos_presentation']['drc_profile'] = args.drc
         xml_base['job_config']['filter']['audio']['encode_to_dthd']['presentation_8ch']['drc_profile'] = args.drc
         xml_base['job_config']['filter']['audio']['encode_to_dthd']['presentation_6ch']['drc_profile'] = args.drc
         xml_base['job_config']['filter']['audio']['encode_to_dthd']['presentation_2ch']['drc_profile'] = args.drc
@@ -779,15 +805,15 @@
             summary.add_row('[bold yellow]Input')
             summary.add_row('Channels', channel_number_to_name(channels))
             summary.add_row('Bit depth', str(bit_depth), end_section=True)
 
         if config['summary_sections']['output_info']:
             summary.add_row('[bold yellow]Output')
             summary.add_row('Format', 'TrueHD' if aformat == 'thd' else aformat.upper())
-            summary.add_row('Channels', channel_number_to_name(outchannels))
+            summary.add_row('Channels', 'immersive stereo' if aformat == 'ac4' else channel_number_to_name(outchannels))
             summary.add_row('Bitrate', 'N/A' if aformat == 'thd' else f'{str(bitrate)} kbps')
             summary.add_row('Dialnorm', 'auto (0)' if args.dialnorm == 0 else f'{str(args.dialnorm)} dB', end_section=True)
 
         if config['summary_sections']['other']:
             if args.delay:
                 delay_print, delay_xml, delay_mode = convert_delay_to_ms(args.delay, compensate=False)
             summary.add_row('[bold yellow]Other')
@@ -796,15 +822,15 @@
             summary.add_row('Delay', delay_print if args.delay else '0 ms or parsed from filename')
             summary.add_row('Temp path', config['temp_path'])
 
         print(summary)
         print()
 
     resample_value = ''
-    if aformat in ['dd', 'ddp'] and samplerate != 48000:
+    if aformat in ['dd', 'ddp', 'ac4'] and samplerate != 48000:
         bit_depth = 32
         resample_value = '48000'
     elif aformat == 'thd' and samplerate not in [48000, 96000]:
         bit_depth = 32
         if samplerate < 72000:
             resample_value = '48000'
         else:
@@ -929,20 +955,25 @@
                 xml['job_config']['output']['ec3']['file_name'] = basename(filelist[i], 'ec3', quote=True, stripdelay=True)
             if args.force_bluray:
                 xml['job_config']['output']['ec3']['file_name'] = basename(filelist[i], 'eb3', quote=True, stripdelay=True)
         elif aformat == 'dd':
             xml['job_config']['output']['ec3']['file_name'] = basename(filelist[i], 'ac3', quote=True, stripdelay=True)
             xml['job_config']['output']['ac3'] = xml['job_config']['output']['ec3']
             del xml['job_config']['output']['ec3']
+        elif aformat == 'ac4':
+            xml['job_config']['output']['ac4']['file_name'] = basename(filelist[i], 'ac4', quote=True, stripdelay=True)
         else:
             xml['job_config']['output']['mlp']['file_name'] = basename(filelist[i], 'thd', quote=True, stripdelay=True)
 
         if aformat in ['dd', 'ddp']:
             delay_print, delay_xml, delay_mode = convert_delay_to_ms(delay, compensate=True)
             xml['job_config']['filter']['audio']['pcm_to_ddp'][delay_mode] = delay_xml
+        elif aformat in ['ac4']:
+            delay_print, delay_xml, delay_mode = convert_delay_to_ms(delay, compensate=True)
+            xml['job_config']['filter']['audio']['encode_to_ims_ac4'][delay_mode] = delay_xml
         else:
             delay_print, delay_xml, delay_mode = convert_delay_to_ms(delay, compensate=False)
             xml['job_config']['filter']['audio']['encode_to_dthd'][delay_mode] = delay_xml
 
         save_xml(os.path.join(config['temp_path'], basename(filelist[i], 'xml', sanitize=True)), xml)
 
         settings.append([filelist[i], output, length_list[i], ffmpeg_args, dee_args, intermediate_exists, aformat])
```

### Comparing `deew-2.9.5/deew/bitrates.py` & `deew-3.0.0/deew/bitrates.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,8 +4,9 @@
     'dd_51': [224, 256, 320, 384, 448, 512, 576, 640],
     'ddp_10': [32, 40, 48, 56, 64, 72, 80, 88, 96, 104, 112, 120, 128, 144, 160, 176, 192, 200, 208, 216, 224, 232, 240, 248, 256, 272, 288, 304, 320, 336, 352, 368, 384, 400, 448, 512, 576, 640, 704, 768, 832, 896, 960, 1008, 1024],
     'ddp_20': [96, 104, 112, 120, 128, 144, 160, 176, 192, 200, 208, 216, 224, 232, 240, 248, 256, 272, 288, 304, 320, 336, 352, 368, 384, 400, 448, 512, 576, 640, 704, 768, 832, 896, 960, 1008, 1024],
     'ddp_51': [192, 200, 208, 216, 224, 232, 240, 248, 256, 272, 288, 304, 320, 336, 352, 368, 384, 400, 448, 512, 576, 640, 704, 768, 832, 896, 960, 1008, 1024],
     'ddp_71_standard': [384, 448, 576, 640, 704, 768, 832, 896, 960, 1008, 1024],
     'ddp_71_bluray': [768, 1024, 1280, 1536, 1664],
     'ddp_71_combined': [384, 448, 576, 640, 704, 768, 832, 896, 960, 1008, 1024, 1280, 1536, 1664],
+    'ac4_20': [64, 72, 114, 144, 256, 320],
 }
```

### Comparing `deew-2.9.5/deew/logos.py` & `deew-3.0.0/deew/logos.py`

 * *Files identical despite different names*

### Comparing `deew-2.9.5/deew/messages.py` & `deew-3.0.0/deew/messages.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 error_messages = {
-    'changelog'        : 'couldn\'t fetch changelog from GitHub.',
-    'delay'            : 'unsupported delay value.',
-    'wsl_path'         : 'WSL path conversion doesn\'t work with [bold yellow]🤠[/bold yellow].',
-    'create_dir'       : 'failed to create [bold yellow]🤠[/bold yellow].',
-    'format'           : '[bold yellow]-f[/bold yellow]/[bold yellow]--format[/bold yellow] can only be [bold yellow]dd[/bold yellow], [bold yellow]ddp[/bold yellow] or [bold yellow]thd[/bold yellow].',
-    'downmix'          : '[bold yellow]-dm[/bold yellow]/[bold yellow]--downmix[/bold yellow] can only be [bold yellow]1[/bold yellow], [bold yellow]2[/bold yellow] or [bold yellow]6[/bold yellow].',
-    'downmix_mismatch' : 'downmix value has to be lower than the number of input channels.',
-    'thd_downmix'      : '[bold yellow]-m[/bold yellow]/[bold yellow]--mix[/bold yellow] can only be used for [bold yellow]DD[/bold yellow]/[bold yellow]DDP[/bold yellow] encoding.',
-    'drc'              : 'allowed DRC values: [bold yellow]film_light[/bold yellow], [bold yellow]film_standard[/bold yellow], [bold yellow]music_light[/bold yellow], [bold yellow]music_standard[/bold yellow], [bold yellow]speech[/bold yellow].',
-    'linux_thd'        : 'Linux version of DEE does not support TrueHD encoding.',
-    'path'             : 'path [bold yellow]🤠[/bold yellow] does not exist.',
-    'ffprobe'          : 'input file couldn\'t be parsed by ffprobe, try to extract/remux it with ffmpeg or mkvmerge.',
-    'sample_mismatch'  : 'each input has to have the same sample rate:\n🤠',
-    'channel_mismatch' : 'each input has to have the same channel count:\n🤠',
-    'bitdepth_mismatch': 'each input has to have the same bit depth:\n🤠',
-    'channels'         : 'number of input channels can only be [bold yellow]1[/bold yellow], [bold yellow]2[/bold yellow], [bold yellow]6[/bold yellow] or [bold yellow]8[/bold yellow].',
-    'binary_exist'     : '[bold yellow]🤠[/bold yellow] does not exist.',
-    'config_key'       : 'the following keys are missing from your config file: 🤠.\nUpdate your config file.'
+    'changelog'         : 'couldn\'t fetch changelog from GitHub.',
+    'delay'             : 'unsupported delay value.',
+    'wsl_path'          : 'WSL path conversion doesn\'t work with [bold yellow]🤠[/bold yellow].',
+    'create_dir'        : 'failed to create [bold yellow]🤠[/bold yellow].',
+    'format'            : '[bold yellow]-f[/bold yellow]/[bold yellow]--format[/bold yellow] can only be [bold yellow]dd[/bold yellow], [bold yellow]ddp[/bold yellow] or [bold yellow]thd[/bold yellow].',
+    'downmix'           : '[bold yellow]-dm[/bold yellow]/[bold yellow]--downmix[/bold yellow] can only be [bold yellow]1[/bold yellow], [bold yellow]2[/bold yellow] or [bold yellow]6[/bold yellow].',
+    'downmix_mismatch'  : 'downmix value has to be lower than the number of input channels.',
+    'thd_downmix'       : '[bold yellow]-m[/bold yellow]/[bold yellow]--mix[/bold yellow] can only be used for [bold yellow]DD[/bold yellow]/[bold yellow]DDP[/bold yellow] encoding.',
+    'thd_mono_input'    : 'input channels for TrueHD encoding can only be [bold yellow]2[/bold yellow]/[bold yellow]6[/bold yellow]/[bold yellow]8[/bold yellow]. ',
+    'drc'               : 'allowed DRC values: [bold yellow]film_light[/bold yellow], [bold yellow]film_standard[/bold yellow], [bold yellow]music_light[/bold yellow], [bold yellow]music_standard[/bold yellow], [bold yellow]speech[/bold yellow].',
+    'linux_thd'         : 'Linux version of DEE does not support TrueHD encoding.',
+    'path'              : 'path [bold yellow]🤠[/bold yellow] does not exist.',
+    'ffprobe'           : 'input file couldn\'t be parsed by ffprobe, try to extract/remux it with ffmpeg or mkvmerge.',
+    'sample_mismatch'   : 'each input has to have the same sample rate:\n🤠',
+    'channel_mismatch'  : 'each input has to have the same channel count:\n🤠',
+    'bitdepth_mismatch' : 'each input has to have the same bit depth:\n🤠',
+    'channels'          : 'number of input channels can only be [bold yellow]1[/bold yellow], [bold yellow]2[/bold yellow], [bold yellow]6[/bold yellow] or [bold yellow]8[/bold yellow].',
+    'binary_exist'      : '[bold yellow]🤠[/bold yellow] does not exist.',
+    'config_key'        : 'the following keys are missing from your config file: 🤠.\nUpdate your config file.',
+    'ac4_input_channels': 'input channels for AC4 encoding can only be [bold yellow]6[/bold yellow].'
 }
```

### Comparing `deew-2.9.5/deew/xml_base.py` & `deew-3.0.0/deew/xml_base.py`

 * *Files 12% similar despite different names*

```diff
@@ -151,8 +151,75 @@
   </output>
   <misc>
     <temp_dir>
       <clean_temp>true</clean_temp>
       <path>-</path>
     </temp_dir>
   </misc>
+</job_config>'''
+
+xml_ac4_base = '''<?xml version="1.0"?>
+<job_config>
+  <input>
+    <audio>
+      <wav version="1">
+        <file_name>-</file_name>    <!-- string -->
+        <timecode_frame_rate>not_indicated</timecode_frame_rate>    <!-- One of: not_indicated, 23.976, 24, 25, 29.97, 30, 48, 50, 59.94, 60 -->
+        <offset>auto</offset>    <!-- string -->
+        <ffoa>auto</ffoa>    <!-- string -->
+        <storage>
+          <local>
+            <path>-</path>    <!-- string -->
+          </local>
+        </storage>
+      </wav>
+    </audio>
+  </input>
+  <filter>
+    <audio>
+      <encode_to_ims_ac4 version="1">
+        <timecode_frame_rate>not_indicated</timecode_frame_rate>    <!-- One of: not_indicated, 23.976, 24, 25, 29.97, 30, 48, 50, 59.94, 60 -->
+        <start>first_frame_of_action</start>    <!-- string -->
+        <end>end_of_file</end>    <!-- string -->
+        <time_base>file_position</time_base>    <!-- One of: file_position, embedded_timecode -->
+        <prepend_silence_duration>0</prepend_silence_duration>    <!-- string -->
+        <append_silence_duration>0</append_silence_duration>    <!-- string -->
+        <loudness>
+          <measure_only>
+            <metering_mode>1770-4</metering_mode>    <!-- One of: 1770-4, 1770-3, 1770-2, 1770-1, LeqA -->
+            <dialogue_intelligence>true</dialogue_intelligence>    <!-- boolean: true or false -->
+            <speech_threshold>15</speech_threshold>    <!-- integer: from 0 to 100 -->
+          </measure_only>
+        </loudness>
+        <data_rate>256</data_rate>    <!-- One of: 64, 72, 112, 144, 256, 320 -->
+        <ac4_frame_rate>native</ac4_frame_rate>    <!-- One of: native, 23.976, 24, 25, 29.97 -->
+        <ims_legacy_presentation>false</ims_legacy_presentation>    <!-- boolean: true or false -->
+        <iframe_interval>0</iframe_interval>    <!-- integer: from 0 to 1000 -->
+        <language>LANGUAGE</language>    <!-- For example "eng-US". Remove this parameter to leave language tag empty. -->
+        <encoding_profile>ims</encoding_profile>    <!-- One of: ims, ims_music -->
+        <drc>
+          <ddp_drc_profile>-</ddp_drc_profile>    <!-- One of: film_standard, film_light, music_standard, music_light, speech, none -->
+          <flat_panel_drc_profile>-</flat_panel_drc_profile>    <!-- One of: film_standard, film_light, music_standard, music_light, speech, none -->
+          <home_theatre_drc_profile>-</home_theatre_drc_profile>    <!-- One of: film_standard, film_light, music_standard, music_light, speech, none -->
+          <portable_hp_drc_profile>-</portable_hp_drc_profile>    <!-- One of: film_standard, film_light, music_standard, music_light, speech, none -->
+          <portable_spkr_drc_profile>-</portable_spkr_drc_profile>    <!-- One of: film_standard, film_light, music_standard, music_light, speech, none -->
+        </drc>
+      </encode_to_ims_ac4>
+    </audio>
+  </filter>
+  <output>
+    <ac4 version="1">
+      <file_name>-</file_name>    <!-- string -->
+      <storage>
+        <local>
+          <path>-</path>    <!-- string -->
+        </local>
+      </storage>
+    </ac4>
+  </output>
+  <misc>
+    <temp_dir>
+      <clean_temp>true</clean_temp>
+      <path>-</path>
+    </temp_dir>
+  </misc>
 </job_config>'''
```

### Comparing `deew-2.9.5/LICENSE` & `deew-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `deew-2.9.5/pyproject.toml` & `deew-3.0.0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "deew"
-version = "2.9.5"
+version = "3.0.0"
 readme = 'README.md'
 description = "Dolby Encoding Engine Wrapper"
 authors = ["pcroland <pcroland@protonmail.ch>"]
 license = "MIT"
 
 [tool.poetry.dependencies]
-python = "^3.7"
+python = ">=3.7,<3.12"
 packaging = "^21.3"
 platformdirs = "^2.5.2"
 requests = "^2.28.1"
 rich = "^12.5.1"
 toml = "^0.10.2"
 Unidecode = "^1.3.4"
 xmltodict = "^0.13.0"
```

### Comparing `deew-2.9.5/README.md` & `deew-3.0.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,13 @@
-[![builds](https://img.shields.io/github/workflow/status/pcroland/deew/Build%20and%20publish?logo=github&style=flat-square)](https://github.com/pcroland/deew/actions/workflows/build.yaml)
+[![builds](https://img.shields.io/github/actions/workflow/status/pcroland/deew/build.yaml?logo=github&style=flat-square)](https://github.com/pcroland/deew/actions/workflows/build.yaml)
 [![github_release](https://img.shields.io/github/v/release/pcroland/deew?logo=github&color=70920c&style=flat-square)](https://github.com/pcroland/deew/releases)
 [![pypi_release](https://img.shields.io/pypi/v/deew?label=PyPI&logo=pypi&logoColor=ffffff&color=70920c&style=flat-square)](https://pypi.org/project/deew)
 [![pypi_downloads](https://img.shields.io/pypi/dm/deew?color=70920c&logo=pypi&logoColor=white&style=flat-square)](https://pypi.org/project/deew)
 [![license](https://img.shields.io/github/license/pcroland/deew?color=blueviolet&style=flat-square)](https://github.com/pcroland/deew/blob/master/LICENSE)
 \
-[![telegram](https://img.shields.io/endpoint?color=1d93d2&style=flat-square&url=https://cadoth.net/tgmembercount%3Fchat_id=deew_support%26name=Discussion%2520and%2520Support)](https://t.me/deew_support)
 [![commits](https://img.shields.io/github/last-commit/pcroland/deew?color=355ab8&logo=github&style=flat-square)](https://github.com/pcroland/deew/commits/main)
 [![issues](https://img.shields.io/github/issues/pcroland/deew?color=355ab8&logo=github&style=flat-square)](https://github.com/pcroland/deew/issues)
 \
 [![name](https://img.shields.io/badge/platform-win%20%7C%20linux%20%7C%20osx-eeeeee?style=flat-square)](https://github.com/pcroland/deew)
 [![name](https://img.shields.io/pypi/pyversions/deew?logo=Python&logoColor=eeeeee&color=eeeeee&style=flat-square)](https://github.com/pcroland/deew)
 [![name](https://img.shields.io/badge/DEE-5.1.0--5.2.1-green?logoColor=white&logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAMCAYAAABr5z2BAAAA9ElEQVQokZXSzypFURQG8N89LsnEv1KGBp5CKU9wBygPIJ5AeYM7MjLAzMBAmRuYyszU3AOgG6GQpZ19OM69Tny1Wu39rVXfWt9qRcQaljCOUbygh3c/MYQJDOMZ9zhvYwEb+hG1n9aAmlaBkfzYwQo2cZUbqnGJdSxjP/eMiYi9+MRiRKjEWXzjpMZ1MnNUVORM1+R1ck6jrNa4qZJrD5irRFrUHW4aahRNJN7w2lTQpCBhBpN/VfBU4w5yTr53a1war0/BPK7zQW1lS0tsYxa7eMDcFxMRhxW7/ovjpOAUj9madMppabe/nHKyOvWkcXu4+AAd1Ju1TsOvFgAAAABJRU5ErkJggg==&color=eeeeee&style=flat-square)](https://customer.dolby.com/content-creation-and-delivery/dolby-encoding-engine-with-ac-4)
 <hr>
@@ -28,15 +27,15 @@
 - converts inputs to RF64 which DEE can use
   - bit depth, number of channels and other infos are parsed from the source
 - an XML file will be generated for each input based on the settings
 - the script utilizes thread pooling for batch encoding (see config)
 - supports WSL path conversion for the Windows version of DEE (see config)
 - in case of an invalid bitrate it will pick the closest allowed one
 - automatic sample rate conversion using ffmpeg's soxr resampler in case of an unsupported sample rate
-  - for DD/DDP unsupported rates will be converted to 48 kHz
+  - for DD/DDP/AC4 unsupported rates will be converted to 48 kHz
   - for TrueHD unsupported rates will be converted to 48 kHz if source sample rate is lower than 72 kHz, otherwise will be converted to 96 kHz
 - automatic channel swapping for 7.1 sources (DEE swaps Ls Rs with Lrs Rrs for some reason)
 - automatic dialnorm setting
 - automatically compensates for DEE's 256 sample delay (DD and DDP encoding)
 - checks if intermediate file is already created so you can encode different formats/bitrates using a single intermediate file, for example:\
   `deew -f dd -b 448 -i input -k`\
   `deew -f dd -b 640 -i input -k`\
@@ -44,15 +43,15 @@
 - works even with video inputs (first audio will be selected)
 - fancy terminal output using rich
 - versatile delay option that supports ms, s and also frame@fps formats
 - parsing delay from filenames
 
 # Requirements
 - Python *(you don't need it if you use a standalone build of deew)*
-- ffmpeg 5.1.2 or older *(they messed up something in w64/rf64 and new versions can't be used currently for DEE)*
+- ffmpeg
 - ffprobe
 - Dolby Encoding Engine
 
 # Dolby Encoding Engine installation
 - install [DEE](https://customer.dolby.com/content-creation-and-delivery/dolby-encoding-engine-with-ac-4) (if you use macOS, install [DME](https://customer.dolby.com/content-creation-and-delivery/dolby-media-encoder-with-ac-4))
   - for TrueHD encoding support you need the Windows version
   - if you use WSL1 use the Windows version for better performance
@@ -94,30 +93,30 @@
 PATH="/usr/local/bin/dee:$PATH"
 PATH="/usr/local/bin/ffmpeg:$PATH"
 ```
 
 # Usage
 ```
 ❯ deew -h
-deew 2.9.5
+deew 3.0.0
 
 USAGE: deew [-h] [-v] [-i [INPUT ...]] [-ti INDEX] [-o DIRECTORY] [-f FORMAT]
             [-b BITRATE] [-dm CHANNELS] [-d DELAY] [-r DRC] [-dn DIALNORM]
             [-in INSTANCES] [-k] [-mo] [-fs] [-fb] [-lb] [-la] [-np] [-pl]
             [-cl] [-c] [-gc]
 
 FLAGS:
   -h, --help                  show this help message.
   -v, --version               show version.
   -i, --input [INPUT ...]     audio file(s) or folder(s)
   -ti, --track-index INDEX    default: 0
                               select audio track index of input(s)
   -o, --output DIRECTORY      default: current directory
                               specifies output directory
-  -f, --format FORMAT         options: dd / ddp / thd
+  -f, --format FORMAT         options: dd / ddp / ac4 / thd
                               default: ddp
   -b, --bitrate BITRATE       options: run -lb/--list-bitrates
                               default: run -c/--config
   -dm, --downmix CHANNELS     options: 1 / 2 / 6
                               specifies downmix, only works for DD/DDP
                               DD will be automatically downmixed to 5.1 in case of a 7.1 source
   -d, --delay DELAY           examples: -5.1ms, +1,52s, -24@pal, +10@24000/1001
```

#### html2text {}

```diff
@@ -1,28 +1,25 @@
-[![builds](https://img.shields.io/github/workflow/status/pcroland/deew/
-Build%20and%20publish?logo=github&style=flat-square)](https://github.com/
-pcroland/deew/actions/workflows/build.yaml) [![github_release](https://
-img.shields.io/github/v/release/pcroland/
-deew?logo=github&color=70920c&style=flat-square)](https://github.com/pcroland/
-deew/releases) [![pypi_release](https://img.shields.io/pypi/v/
-deew?label=PyPI&logo=pypi&logoColor=ffffff&color=70920c&style=flat-square)]
-(https://pypi.org/project/deew) [![pypi_downloads](https://img.shields.io/pypi/
-dm/deew?color=70920c&logo=pypi&logoColor=white&style=flat-square)](https://
-pypi.org/project/deew) [![license](https://img.shields.io/github/license/
-pcroland/deew?color=blueviolet&style=flat-square)](https://github.com/pcroland/
-deew/blob/master/LICENSE) \ [![telegram](https://img.shields.io/
-endpoint?color=1d93d2&style=flat-square&url=https://cadoth.net/
-tgmembercount%3Fchat_id=deew_support%26name=Discussion%2520and%2520Support)]
-(https://t.me/deew_support) [![commits](https://img.shields.io/github/last-
-commit/pcroland/deew?color=355ab8&logo=github&style=flat-square)](https://
-github.com/pcroland/deew/commits/main) [![issues](https://img.shields.io/
-github/issues/pcroland/deew?color=355ab8&logo=github&style=flat-square)](https:
-//github.com/pcroland/deew/issues) \ [![name](https://img.shields.io/badge/
-platform-win%20%7C%20linux%20%7C%20osx-eeeeee?style=flat-square)](https://
-github.com/pcroland/deew) [![name](https://img.shields.io/pypi/pyversions/
+[![builds](https://img.shields.io/github/actions/workflow/status/pcroland/deew/
+build.yaml?logo=github&style=flat-square)](https://github.com/pcroland/deew/
+actions/workflows/build.yaml) [![github_release](https://img.shields.io/github/
+v/release/pcroland/deew?logo=github&color=70920c&style=flat-square)](https://
+github.com/pcroland/deew/releases) [![pypi_release](https://img.shields.io/
+pypi/v/deew?label=PyPI&logo=pypi&logoColor=ffffff&color=70920c&style=flat-
+square)](https://pypi.org/project/deew) [![pypi_downloads](https://
+img.shields.io/pypi/dm/deew?color=70920c&logo=pypi&logoColor=white&style=flat-
+square)](https://pypi.org/project/deew) [![license](https://img.shields.io/
+github/license/pcroland/deew?color=blueviolet&style=flat-square)](https://
+github.com/pcroland/deew/blob/master/LICENSE) \ [![commits](https://
+img.shields.io/github/last-commit/pcroland/
+deew?color=355ab8&logo=github&style=flat-square)](https://github.com/pcroland/
+deew/commits/main) [![issues](https://img.shields.io/github/issues/pcroland/
+deew?color=355ab8&logo=github&style=flat-square)](https://github.com/pcroland/
+deew/issues) \ [![name](https://img.shields.io/badge/platform-
+win%20%7C%20linux%20%7C%20osx-eeeeee?style=flat-square)](https://github.com/
+pcroland/deew) [![name](https://img.shields.io/pypi/pyversions/
 deew?logo=Python&logoColor=eeeeee&color=eeeeee&style=flat-square)](https://
 github.com/pcroland/deew) [![name](https://img.shields.io/badge/DEE-5.1.0--
 5.2.1-green?logoColor=white&logo=data:image/
 png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAMCAYAAABr5z2BAAAA9ElEQVQokZXSzypFURQG8N89LsnEv1KGBp5CKU9wBygPIJ5AeYM7MjLAzMBAmRuYyszU3AOgG6GQpZ19OM69Tny1Wu39rVXfWt9qRcQaljCOUbygh3c/
 MYQJDOMZ9zhvYwEb+hG1n9aAmlaBkfzYwQo2cZUbqnGJdSxjP/
 eMiYi9+MRiRKjEWXzjpMZ1MnNUVORM1+R1ck6jrNa4qZJrD5irRFrUHW4aahRNJN7w2lTQpCBhBpN/
 VfBU4w5yTr53a1war0/BPK7zQW1lS0tsYxa7eMDcFxMRhxW7/ovjpOAUj9madMppabe/
@@ -38,71 +35,70 @@
 in the background, giving you a proper CLI interface - converts inputs to RF64
 which DEE can use - bit depth, number of channels and other infos are parsed
 from the source - an XML file will be generated for each input based on the
 settings - the script utilizes thread pooling for batch encoding (see config) -
 supports WSL path conversion for the Windows version of DEE (see config) - in
 case of an invalid bitrate it will pick the closest allowed one - automatic
 sample rate conversion using ffmpeg's soxr resampler in case of an unsupported
-sample rate - for DD/DDP unsupported rates will be converted to 48 kHz - for
-TrueHD unsupported rates will be converted to 48 kHz if source sample rate is
-lower than 72 kHz, otherwise will be converted to 96 kHz - automatic channel
+sample rate - for DD/DDP/AC4 unsupported rates will be converted to 48 kHz -
+for TrueHD unsupported rates will be converted to 48 kHz if source sample rate
+is lower than 72 kHz, otherwise will be converted to 96 kHz - automatic channel
 swapping for 7.1 sources (DEE swaps Ls Rs with Lrs Rrs for some reason) -
 automatic dialnorm setting - automatically compensates for DEE's 256 sample
 delay (DD and DDP encoding) - checks if intermediate file is already created so
 you can encode different formats/bitrates using a single intermediate file, for
 example:\ `deew -f dd -b 448 -i input -k`\ `deew -f dd -b 640 -i input -k`\
 `deew -f ddp -i input` - works even with video inputs (first audio will be
 selected) - fancy terminal output using rich - versatile delay option that
 supports ms, s and also frame@fps formats - parsing delay from filenames #
 Requirements - Python *(you don't need it if you use a standalone build of
-deew)* - ffmpeg 5.1.2 or older *(they messed up something in w64/rf64 and new
-versions can't be used currently for DEE)* - ffprobe - Dolby Encoding Engine #
-Dolby Encoding Engine installation - install [DEE](https://customer.dolby.com/
-content-creation-and-delivery/dolby-encoding-engine-with-ac-4) (if you use
-macOS, install [DME](https://customer.dolby.com/content-creation-and-delivery/
-dolby-media-encoder-with-ac-4)) - for TrueHD encoding support you need the
-Windows version - if you use WSL1 use the Windows version for better
-performance - if you use the Windows version of DEE under Linux (and not from
-WSL) / macOS install `wine-binfmt` - place your `license.lic` file next to the
-DEE binary (`dee.exe` under Windows, `dee` under Linux/macOS) - if DEE throws
-`Failed to load library "...dll".` errors when you run deew install
-[VisualCppRedist AIO](https://github.com/abbodi1406/vcredist/releases) # deew
-installation ### with standalone build (Windows 8-11/Linux): - grab the latest
-build from: [https://github.com/pcroland/deew/releases](https://github.com/
-pcroland/deew/releases) - run with: `deew`\ *(run the binary from terminal,
-doubleclicking it won't work)* - on the first run it will create a config file,
-choose where you want to keep it - updating: grab the latest build from:
-[https://github.com/pcroland/deew/releases](https://github.com/pcroland/deew/
-releases) ### with Python environment (Windows/Linux/macOS): - install Python
-and pip if you don't have it already - run: `pip install deew` - run with:
-`deew` - on the first run it will create a config file - updating: `pip install
-deew --upgrade` # Setup system PATH variable If you don't want to use full
-paths for the binaries in your config or when you use them from CLI, I suggest
-to setup system PATH variables ### Windows: - open `cmd.exe` as administrator -
-run a `setx /m PATH "%PATH%;[location]"` command for each path that contains
-binaries\ *(replace* `[location]` *with the path)* - for example: ```bat setx /
-m PATH "%PATH%;C:\bin\dee" setx /m PATH "%PATH%;C:\bin\ffmpeg" ``` ### Linux/
-macOS: - add a `PATH="[location]:$PATH"` line in your `~/.bashrc` or `~/.zshrc`
-file for each path that contains a binary\ *(replace* `[location]` *with the
-path)* - for example: ```sh PATH="/usr/local/bin/dee:$PATH" PATH="/usr/local/
-bin/ffmpeg:$PATH" ``` # Usage ``` â¯ deew -h deew 2.9.5 USAGE: deew [-h] [-v]
-[-i [INPUT ...]] [-ti INDEX] [-o DIRECTORY] [-f FORMAT] [-b BITRATE] [-dm
-CHANNELS] [-d DELAY] [-r DRC] [-dn DIALNORM] [-in INSTANCES] [-k] [-mo] [-fs]
-[-fb] [-lb] [-la] [-np] [-pl] [-cl] [-c] [-gc] FLAGS: -h, --help show this help
-message. -v, --version show version. -i, --input [INPUT ...] audio file(s) or
-folder(s) -ti, --track-index INDEX default: 0 select audio track index of input
-(s) -o, --output DIRECTORY default: current directory specifies output
-directory -f, --format FORMAT options: dd / ddp / thd default: ddp -b, --
-bitrate BITRATE options: run -lb/--list-bitrates default: run -c/--config -dm,
---downmix CHANNELS options: 1 / 2 / 6 specifies downmix, only works for DD/DDP
-DD will be automatically downmixed to 5.1 in case of a 7.1 source -d, --delay
-DELAY examples: -5.1ms, +1,52s, -24@pal, +10@24000/1001 default: 0ms or parsed
-from filename specifies delay as ms, s or frame@FPS FPS can be a number,
-division or ntsc / pal you have to specify negative values as -d=-0ms -r, --drc
-DRC options: film_light / film_standard / music_light / music_standard / speech
+deew)* - ffmpeg - ffprobe - Dolby Encoding Engine # Dolby Encoding Engine
+installation - install [DEE](https://customer.dolby.com/content-creation-and-
+delivery/dolby-encoding-engine-with-ac-4) (if you use macOS, install [DME]
+(https://customer.dolby.com/content-creation-and-delivery/dolby-media-encoder-
+with-ac-4)) - for TrueHD encoding support you need the Windows version - if you
+use WSL1 use the Windows version for better performance - if you use the
+Windows version of DEE under Linux (and not from WSL) / macOS install `wine-
+binfmt` - place your `license.lic` file next to the DEE binary (`dee.exe` under
+Windows, `dee` under Linux/macOS) - if DEE throws `Failed to load library
+"...dll".` errors when you run deew install [VisualCppRedist AIO](https://
+github.com/abbodi1406/vcredist/releases) # deew installation ### with
+standalone build (Windows 8-11/Linux): - grab the latest build from: [https://
+github.com/pcroland/deew/releases](https://github.com/pcroland/deew/releases) -
+run with: `deew`\ *(run the binary from terminal, doubleclicking it won't
+work)* - on the first run it will create a config file, choose where you want
+to keep it - updating: grab the latest build from: [https://github.com/
+pcroland/deew/releases](https://github.com/pcroland/deew/releases) ### with
+Python environment (Windows/Linux/macOS): - install Python and pip if you don't
+have it already - run: `pip install deew` - run with: `deew` - on the first run
+it will create a config file - updating: `pip install deew --upgrade` # Setup
+system PATH variable If you don't want to use full paths for the binaries in
+your config or when you use them from CLI, I suggest to setup system PATH
+variables ### Windows: - open `cmd.exe` as administrator - run a `setx /m PATH
+"%PATH%;[location]"` command for each path that contains binaries\ *(replace* `
+[location]` *with the path)* - for example: ```bat setx /m PATH "%PATH%;C:
+\bin\dee" setx /m PATH "%PATH%;C:\bin\ffmpeg" ``` ### Linux/macOS: - add a
+`PATH="[location]:$PATH"` line in your `~/.bashrc` or `~/.zshrc` file for each
+path that contains a binary\ *(replace* `[location]` *with the path)* - for
+example: ```sh PATH="/usr/local/bin/dee:$PATH" PATH="/usr/local/bin/ffmpeg:
+$PATH" ``` # Usage ``` â¯ deew -h deew 3.0.0 USAGE: deew [-h] [-v] [-i [INPUT
+...]] [-ti INDEX] [-o DIRECTORY] [-f FORMAT] [-b BITRATE] [-dm CHANNELS] [-
+d DELAY] [-r DRC] [-dn DIALNORM] [-in INSTANCES] [-k] [-mo] [-fs] [-fb] [-lb]
+[-la] [-np] [-pl] [-cl] [-c] [-gc] FLAGS: -h, --help show this help message. -
+v, --version show version. -i, --input [INPUT ...] audio file(s) or folder(s) -
+ti, --track-index INDEX default: 0 select audio track index of input(s) -o, --
+output DIRECTORY default: current directory specifies output directory -f, --
+format FORMAT options: dd / ddp / ac4 / thd default: ddp -b, --bitrate BITRATE
+options: run -lb/--list-bitrates default: run -c/--config -dm, --downmix
+CHANNELS options: 1 / 2 / 6 specifies downmix, only works for DD/DDP DD will be
+automatically downmixed to 5.1 in case of a 7.1 source -d, --delay DELAY
+examples: -5.1ms, +1,52s, -24@pal, +10@24000/1001 default: 0ms or parsed from
+filename specifies delay as ms, s or frame@FPS FPS can be a number, division or
+ntsc / pal you have to specify negative values as -d=-0ms -r, --drc DRC
+options: film_light / film_standard / music_light / music_standard / speech
 default: music_light (this is the closest to the missing none preset) specifies
 drc profile -dn, --dialnorm DIALNORM options: between -31 and 0 (in case of 0
 DEE's measurement will be used) default: 0 applied dialnorm value between -in,
 --instances INSTANCES examples: 1, 4, 50% default: 50% specifies how many
 encodes can run at the same time 50% means 4 on a cpu with 8 threads one DEE
 can use 2 threads so 50% can utilize all threads (this option overrides the
 config's number) -k, --keeptemp keep temp files -mo, --measure-only kills DEE
```

### Comparing `deew-2.9.5/setup.py` & `deew-3.0.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,40 +1,198 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: deew
+Version: 3.0.0
+Summary: Dolby Encoding Engine Wrapper
+License: MIT
+Author: pcroland
+Author-email: pcroland@protonmail.ch
+Requires-Python: >=3.7,<3.12
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: Unidecode (>=1.3.4,<2.0.0)
+Requires-Dist: packaging (>=21.3,<22.0)
+Requires-Dist: platformdirs (>=2.5.2,<3.0.0)
+Requires-Dist: requests (>=2.28.1,<3.0.0)
+Requires-Dist: rich (>=12.5.1,<13.0.0)
+Requires-Dist: toml (>=0.10.2,<0.11.0)
+Requires-Dist: xmltodict (>=0.13.0,<0.14.0)
+Description-Content-Type: text/markdown
+
+[![builds](https://img.shields.io/github/actions/workflow/status/pcroland/deew/build.yaml?logo=github&style=flat-square)](https://github.com/pcroland/deew/actions/workflows/build.yaml)
+[![github_release](https://img.shields.io/github/v/release/pcroland/deew?logo=github&color=70920c&style=flat-square)](https://github.com/pcroland/deew/releases)
+[![pypi_release](https://img.shields.io/pypi/v/deew?label=PyPI&logo=pypi&logoColor=ffffff&color=70920c&style=flat-square)](https://pypi.org/project/deew)
+[![pypi_downloads](https://img.shields.io/pypi/dm/deew?color=70920c&logo=pypi&logoColor=white&style=flat-square)](https://pypi.org/project/deew)
+[![license](https://img.shields.io/github/license/pcroland/deew?color=blueviolet&style=flat-square)](https://github.com/pcroland/deew/blob/master/LICENSE)
+\
+[![commits](https://img.shields.io/github/last-commit/pcroland/deew?color=355ab8&logo=github&style=flat-square)](https://github.com/pcroland/deew/commits/main)
+[![issues](https://img.shields.io/github/issues/pcroland/deew?color=355ab8&logo=github&style=flat-square)](https://github.com/pcroland/deew/issues)
+\
+[![name](https://img.shields.io/badge/platform-win%20%7C%20linux%20%7C%20osx-eeeeee?style=flat-square)](https://github.com/pcroland/deew)
+[![name](https://img.shields.io/pypi/pyversions/deew?logo=Python&logoColor=eeeeee&color=eeeeee&style=flat-square)](https://github.com/pcroland/deew)
+[![name](https://img.shields.io/badge/DEE-5.1.0--5.2.1-green?logoColor=white&logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAMCAYAAABr5z2BAAAA9ElEQVQokZXSzypFURQG8N89LsnEv1KGBp5CKU9wBygPIJ5AeYM7MjLAzMBAmRuYyszU3AOgG6GQpZ19OM69Tny1Wu39rVXfWt9qRcQaljCOUbygh3c/MYQJDOMZ9zhvYwEb+hG1n9aAmlaBkfzYwQo2cZUbqnGJdSxjP/eMiYi9+MRiRKjEWXzjpMZ1MnNUVORM1+R1ck6jrNa4qZJrD5irRFrUHW4aahRNJN7w2lTQpCBhBpN/VfBU4w5yTr53a1war0/BPK7zQW1lS0tsYxa7eMDcFxMRhxW7/ovjpOAUj9madMppabe/nHKyOvWkcXu4+AAd1Ju1TsOvFgAAAABJRU5ErkJggg==&color=eeeeee&style=flat-square)](https://customer.dolby.com/content-creation-and-delivery/dolby-encoding-engine-with-ac-4)
+<hr>
+<p align="center"><img width="192" src="https://raw.githubusercontent.com/pcroland/deew/main/logo/logo.svg"><br>Dolby Encoding Engine Wrapper</p>
+
+
+<p align="center"><a href="https://github.com/pcroland/deew/blob/main/README.md">English readme</a>
+ • <a href="https://github.com/pcroland/deew/blob/main/README_hu.md">Magyar leírás</a></p>
+
+## DDP encoding has never been so easy!
+
+![img](https://telegra.ph/file/efd2a1d3519bdf87fca03.gif)
+<!---https://i.kek.sh/Mk3qQ0QGWUj.gif--->
+
+# Description
+- handles Dolby's XML input fuckery in the background, giving you a proper CLI interface
+- converts inputs to RF64 which DEE can use
+  - bit depth, number of channels and other infos are parsed from the source
+- an XML file will be generated for each input based on the settings
+- the script utilizes thread pooling for batch encoding (see config)
+- supports WSL path conversion for the Windows version of DEE (see config)
+- in case of an invalid bitrate it will pick the closest allowed one
+- automatic sample rate conversion using ffmpeg's soxr resampler in case of an unsupported sample rate
+  - for DD/DDP/AC4 unsupported rates will be converted to 48 kHz
+  - for TrueHD unsupported rates will be converted to 48 kHz if source sample rate is lower than 72 kHz, otherwise will be converted to 96 kHz
+- automatic channel swapping for 7.1 sources (DEE swaps Ls Rs with Lrs Rrs for some reason)
+- automatic dialnorm setting
+- automatically compensates for DEE's 256 sample delay (DD and DDP encoding)
+- checks if intermediate file is already created so you can encode different formats/bitrates using a single intermediate file, for example:\
+  `deew -f dd -b 448 -i input -k`\
+  `deew -f dd -b 640 -i input -k`\
+  `deew -f ddp -i input`
+- works even with video inputs (first audio will be selected)
+- fancy terminal output using rich
+- versatile delay option that supports ms, s and also frame@fps formats
+- parsing delay from filenames
+
+# Requirements
+- Python *(you don't need it if you use a standalone build of deew)*
+- ffmpeg
+- ffprobe
+- Dolby Encoding Engine
+
+# Dolby Encoding Engine installation
+- install [DEE](https://customer.dolby.com/content-creation-and-delivery/dolby-encoding-engine-with-ac-4) (if you use macOS, install [DME](https://customer.dolby.com/content-creation-and-delivery/dolby-media-encoder-with-ac-4))
+  - for TrueHD encoding support you need the Windows version
+  - if you use WSL1 use the Windows version for better performance
+  - if you use the Windows version of DEE under Linux (and not from WSL) / macOS install `wine-binfmt`
+- place your `license.lic` file next to the DEE binary (`dee.exe` under Windows, `dee` under Linux/macOS)
+- if DEE throws `Failed to load library "...dll".` errors when you run deew install [VisualCppRedist AIO](https://github.com/abbodi1406/vcredist/releases)
+
+# deew installation
+### with standalone build (Windows 8-11/Linux):
+- grab the latest build from: [https://github.com/pcroland/deew/releases](https://github.com/pcroland/deew/releases)
+- run with: `deew`\
+*(run the binary from terminal, doubleclicking it won't work)*
+- on the first run it will create a config file, choose where you want to keep it
+- updating: grab the latest build from: [https://github.com/pcroland/deew/releases](https://github.com/pcroland/deew/releases)
+
+### with Python environment (Windows/Linux/macOS):
+- install Python and pip if you don't have it already
+- run: `pip install deew`
+- run with: `deew`
+- on the first run it will create a config file
+- updating: `pip install deew --upgrade`
+
+# Setup system PATH variable
+If you don't want to use full paths for the binaries in your config or when you use them from CLI, I suggest to setup system PATH variables
+### Windows:
+- open `cmd.exe` as administrator
+- run a `setx /m PATH "%PATH%;[location]"` command for each path that contains binaries\
+  *(replace* `[location]` *with the path)*
+- for example:
+```bat
+setx /m PATH "%PATH%;C:\bin\dee"
+setx /m PATH "%PATH%;C:\bin\ffmpeg"
+```
+### Linux/macOS:
+- add a `PATH="[location]:$PATH"` line in your `~/.bashrc` or `~/.zshrc` file for each path that contains a binary\
+  *(replace* `[location]` *with the path)*
+- for example:
+```sh
+PATH="/usr/local/bin/dee:$PATH"
+PATH="/usr/local/bin/ffmpeg:$PATH"
+```
+
+# Usage
+```
+❯ deew -h
+deew 3.0.0
+
+USAGE: deew [-h] [-v] [-i [INPUT ...]] [-ti INDEX] [-o DIRECTORY] [-f FORMAT]
+            [-b BITRATE] [-dm CHANNELS] [-d DELAY] [-r DRC] [-dn DIALNORM]
+            [-in INSTANCES] [-k] [-mo] [-fs] [-fb] [-lb] [-la] [-np] [-pl]
+            [-cl] [-c] [-gc]
+
+FLAGS:
+  -h, --help                  show this help message.
+  -v, --version               show version.
+  -i, --input [INPUT ...]     audio file(s) or folder(s)
+  -ti, --track-index INDEX    default: 0
+                              select audio track index of input(s)
+  -o, --output DIRECTORY      default: current directory
+                              specifies output directory
+  -f, --format FORMAT         options: dd / ddp / ac4 / thd
+                              default: ddp
+  -b, --bitrate BITRATE       options: run -lb/--list-bitrates
+                              default: run -c/--config
+  -dm, --downmix CHANNELS     options: 1 / 2 / 6
+                              specifies downmix, only works for DD/DDP
+                              DD will be automatically downmixed to 5.1 in case of a 7.1 source
+  -d, --delay DELAY           examples: -5.1ms, +1,52s, -24@pal, +10@24000/1001
+                              default: 0ms or parsed from filename
+                              specifies delay as ms, s or frame@FPS
+                              FPS can be a number, division or ntsc / pal
+                              you have to specify negative values as -d=-0ms
+  -r, --drc DRC               options: film_light / film_standard / music_light / music_standard / speech
+                              default: music_light (this is the closest to the missing none preset)
+                              specifies drc profile
+  -dn, --dialnorm DIALNORM    options: between -31 and 0 (in case of 0 DEE's measurement will be used)
+                              default: 0
+                              applied dialnorm value between
+  -in, --instances INSTANCES  examples: 1, 4, 50%
+                              default: 50%
+                              specifies how many encodes can run at the same time
+                              50% means 4 on a cpu with 8 threads
+                              one DEE can use 2 threads so 50% can utilize all threads
+                              (this option overrides the config's number)
+  -k, --keeptemp              keep temp files
+  -mo, --measure-only         kills DEE when the dialnorm gets written to the progress bar
+                              this option overrides format with ddp
+  -fs, --force-standard       force standard profile for 7.1 DDP encoding (384-1024 kbps)
+  -fb, --force-bluray         force bluray profile for 7.1 DDP encoding (768-1664 kbps)
+  -lb, --list-bitrates        list bitrates that DEE can do for DD and DDP encoding
+  -la, --long-argument        print ffmpeg and DEE arguments for each input
+  -np, --no-prompt            disables prompt
+  -pl, --print-logos          show all logo variants you can set in the config
+  -cl, --changelog            show changelog
+  -c, --config                show config and config location(s)
+  -gc, --generate-config      generate a new config
+```
+# Examples
+`deew -i *thd`\
+encode DDP
+
+`deew -b 768 -i *flac`\
+encode DDP@768
+
+`deew -dm 2 -f dd -b 192 -i *.ec3`\
+encode DD@192 with stereo downmixing
+
+`deew -f dd -b 448 -t 4 -i S01`\
+encode DD@448 using 4 threads (input is a folder)
+
+`deew -f thd -i *w64`\
+encode TrueHD
+
+`deew -f dd -i *dts -k`\
+`deew -f ddp -i *dts`\
+encode multiple formats/bitrates while creating the temp file only once
 
-packages = \
-['deew']
+# Discussion and Support
+[https://t.me/deew_support](https://t.me/deew_support)
 
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['Unidecode>=1.3.4,<2.0.0',
- 'packaging>=21.3,<22.0',
- 'platformdirs>=2.5.2,<3.0.0',
- 'requests>=2.28.1,<3.0.0',
- 'rich>=12.5.1,<13.0.0',
- 'toml>=0.10.2,<0.11.0',
- 'xmltodict>=0.13.0,<0.14.0']
-
-entry_points = \
-{'console_scripts': ['deew = deew.__main__:main']}
-
-setup_kwargs = {
-    'name': 'deew',
-    'version': '2.9.5',
-    'description': 'Dolby Encoding Engine Wrapper',
-    'long_description': '[![builds](https://img.shields.io/github/workflow/status/pcroland/deew/Build%20and%20publish?logo=github&style=flat-square)](https://github.com/pcroland/deew/actions/workflows/build.yaml)\n[![github_release](https://img.shields.io/github/v/release/pcroland/deew?logo=github&color=70920c&style=flat-square)](https://github.com/pcroland/deew/releases)\n[![pypi_release](https://img.shields.io/pypi/v/deew?label=PyPI&logo=pypi&logoColor=ffffff&color=70920c&style=flat-square)](https://pypi.org/project/deew)\n[![pypi_downloads](https://img.shields.io/pypi/dm/deew?color=70920c&logo=pypi&logoColor=white&style=flat-square)](https://pypi.org/project/deew)\n[![license](https://img.shields.io/github/license/pcroland/deew?color=blueviolet&style=flat-square)](https://github.com/pcroland/deew/blob/master/LICENSE)\n\\\n[![telegram](https://img.shields.io/endpoint?color=1d93d2&style=flat-square&url=https://cadoth.net/tgmembercount%3Fchat_id=deew_support%26name=Discussion%2520and%2520Support)](https://t.me/deew_support)\n[![commits](https://img.shields.io/github/last-commit/pcroland/deew?color=355ab8&logo=github&style=flat-square)](https://github.com/pcroland/deew/commits/main)\n[![issues](https://img.shields.io/github/issues/pcroland/deew?color=355ab8&logo=github&style=flat-square)](https://github.com/pcroland/deew/issues)\n\\\n[![name](https://img.shields.io/badge/platform-win%20%7C%20linux%20%7C%20osx-eeeeee?style=flat-square)](https://github.com/pcroland/deew)\n[![name](https://img.shields.io/pypi/pyversions/deew?logo=Python&logoColor=eeeeee&color=eeeeee&style=flat-square)](https://github.com/pcroland/deew)\n[![name](https://img.shields.io/badge/DEE-5.1.0--5.2.1-green?logoColor=white&logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAMCAYAAABr5z2BAAAA9ElEQVQokZXSzypFURQG8N89LsnEv1KGBp5CKU9wBygPIJ5AeYM7MjLAzMBAmRuYyszU3AOgG6GQpZ19OM69Tny1Wu39rVXfWt9qRcQaljCOUbygh3c/MYQJDOMZ9zhvYwEb+hG1n9aAmlaBkfzYwQo2cZUbqnGJdSxjP/eMiYi9+MRiRKjEWXzjpMZ1MnNUVORM1+R1ck6jrNa4qZJrD5irRFrUHW4aahRNJN7w2lTQpCBhBpN/VfBU4w5yTr53a1war0/BPK7zQW1lS0tsYxa7eMDcFxMRhxW7/ovjpOAUj9madMppabe/nHKyOvWkcXu4+AAd1Ju1TsOvFgAAAABJRU5ErkJggg==&color=eeeeee&style=flat-square)](https://customer.dolby.com/content-creation-and-delivery/dolby-encoding-engine-with-ac-4)\n<hr>\n<p align="center"><img width="192" src="https://raw.githubusercontent.com/pcroland/deew/main/logo/logo.svg"><br>Dolby Encoding Engine Wrapper</p>\n\n\n<p align="center"><a href="https://github.com/pcroland/deew/blob/main/README.md">English readme</a>\n • <a href="https://github.com/pcroland/deew/blob/main/README_hu.md">Magyar leírás</a></p>\n\n## DDP encoding has never been so easy!\n\n![img](https://telegra.ph/file/efd2a1d3519bdf87fca03.gif)\n<!---https://i.kek.sh/Mk3qQ0QGWUj.gif--->\n\n# Description\n- handles Dolby\'s XML input fuckery in the background, giving you a proper CLI interface\n- converts inputs to RF64 which DEE can use\n  - bit depth, number of channels and other infos are parsed from the source\n- an XML file will be generated for each input based on the settings\n- the script utilizes thread pooling for batch encoding (see config)\n- supports WSL path conversion for the Windows version of DEE (see config)\n- in case of an invalid bitrate it will pick the closest allowed one\n- automatic sample rate conversion using ffmpeg\'s soxr resampler in case of an unsupported sample rate\n  - for DD/DDP unsupported rates will be converted to 48 kHz\n  - for TrueHD unsupported rates will be converted to 48 kHz if source sample rate is lower than 72 kHz, otherwise will be converted to 96 kHz\n- automatic channel swapping for 7.1 sources (DEE swaps Ls Rs with Lrs Rrs for some reason)\n- automatic dialnorm setting\n- automatically compensates for DEE\'s 256 sample delay (DD and DDP encoding)\n- checks if intermediate file is already created so you can encode different formats/bitrates using a single intermediate file, for example:\\\n  `deew -f dd -b 448 -i input -k`\\\n  `deew -f dd -b 640 -i input -k`\\\n  `deew -f ddp -i input`\n- works even with video inputs (first audio will be selected)\n- fancy terminal output using rich\n- versatile delay option that supports ms, s and also frame@fps formats\n- parsing delay from filenames\n\n# Requirements\n- Python *(you don\'t need it if you use a standalone build of deew)*\n- ffmpeg 5.1.2 or older *(they messed up something in w64/rf64 and new versions can\'t be used currently for DEE)*\n- ffprobe\n- Dolby Encoding Engine\n\n# Dolby Encoding Engine installation\n- install [DEE](https://customer.dolby.com/content-creation-and-delivery/dolby-encoding-engine-with-ac-4) (if you use macOS, install [DME](https://customer.dolby.com/content-creation-and-delivery/dolby-media-encoder-with-ac-4))\n  - for TrueHD encoding support you need the Windows version\n  - if you use WSL1 use the Windows version for better performance\n  - if you use the Windows version of DEE under Linux (and not from WSL) / macOS install `wine-binfmt`\n- place your `license.lic` file next to the DEE binary (`dee.exe` under Windows, `dee` under Linux/macOS)\n- if DEE throws `Failed to load library "...dll".` errors when you run deew install [VisualCppRedist AIO](https://github.com/abbodi1406/vcredist/releases)\n\n# deew installation\n### with standalone build (Windows 8-11/Linux):\n- grab the latest build from: [https://github.com/pcroland/deew/releases](https://github.com/pcroland/deew/releases)\n- run with: `deew`\\\n*(run the binary from terminal, doubleclicking it won\'t work)*\n- on the first run it will create a config file, choose where you want to keep it\n- updating: grab the latest build from: [https://github.com/pcroland/deew/releases](https://github.com/pcroland/deew/releases)\n\n### with Python environment (Windows/Linux/macOS):\n- install Python and pip if you don\'t have it already\n- run: `pip install deew`\n- run with: `deew`\n- on the first run it will create a config file\n- updating: `pip install deew --upgrade`\n\n# Setup system PATH variable\nIf you don\'t want to use full paths for the binaries in your config or when you use them from CLI, I suggest to setup system PATH variables\n### Windows:\n- open `cmd.exe` as administrator\n- run a `setx /m PATH "%PATH%;[location]"` command for each path that contains binaries\\\n  *(replace* `[location]` *with the path)*\n- for example:\n```bat\nsetx /m PATH "%PATH%;C:\\bin\\dee"\nsetx /m PATH "%PATH%;C:\\bin\\ffmpeg"\n```\n### Linux/macOS:\n- add a `PATH="[location]:$PATH"` line in your `~/.bashrc` or `~/.zshrc` file for each path that contains a binary\\\n  *(replace* `[location]` *with the path)*\n- for example:\n```sh\nPATH="/usr/local/bin/dee:$PATH"\nPATH="/usr/local/bin/ffmpeg:$PATH"\n```\n\n# Usage\n```\n❯ deew -h\ndeew 2.9.5\n\nUSAGE: deew [-h] [-v] [-i [INPUT ...]] [-ti INDEX] [-o DIRECTORY] [-f FORMAT]\n            [-b BITRATE] [-dm CHANNELS] [-d DELAY] [-r DRC] [-dn DIALNORM]\n            [-in INSTANCES] [-k] [-mo] [-fs] [-fb] [-lb] [-la] [-np] [-pl]\n            [-cl] [-c] [-gc]\n\nFLAGS:\n  -h, --help                  show this help message.\n  -v, --version               show version.\n  -i, --input [INPUT ...]     audio file(s) or folder(s)\n  -ti, --track-index INDEX    default: 0\n                              select audio track index of input(s)\n  -o, --output DIRECTORY      default: current directory\n                              specifies output directory\n  -f, --format FORMAT         options: dd / ddp / thd\n                              default: ddp\n  -b, --bitrate BITRATE       options: run -lb/--list-bitrates\n                              default: run -c/--config\n  -dm, --downmix CHANNELS     options: 1 / 2 / 6\n                              specifies downmix, only works for DD/DDP\n                              DD will be automatically downmixed to 5.1 in case of a 7.1 source\n  -d, --delay DELAY           examples: -5.1ms, +1,52s, -24@pal, +10@24000/1001\n                              default: 0ms or parsed from filename\n                              specifies delay as ms, s or frame@FPS\n                              FPS can be a number, division or ntsc / pal\n                              you have to specify negative values as -d=-0ms\n  -r, --drc DRC               options: film_light / film_standard / music_light / music_standard / speech\n                              default: music_light (this is the closest to the missing none preset)\n                              specifies drc profile\n  -dn, --dialnorm DIALNORM    options: between -31 and 0 (in case of 0 DEE\'s measurement will be used)\n                              default: 0\n                              applied dialnorm value between\n  -in, --instances INSTANCES  examples: 1, 4, 50%\n                              default: 50%\n                              specifies how many encodes can run at the same time\n                              50% means 4 on a cpu with 8 threads\n                              one DEE can use 2 threads so 50% can utilize all threads\n                              (this option overrides the config\'s number)\n  -k, --keeptemp              keep temp files\n  -mo, --measure-only         kills DEE when the dialnorm gets written to the progress bar\n                              this option overrides format with ddp\n  -fs, --force-standard       force standard profile for 7.1 DDP encoding (384-1024 kbps)\n  -fb, --force-bluray         force bluray profile for 7.1 DDP encoding (768-1664 kbps)\n  -lb, --list-bitrates        list bitrates that DEE can do for DD and DDP encoding\n  -la, --long-argument        print ffmpeg and DEE arguments for each input\n  -np, --no-prompt            disables prompt\n  -pl, --print-logos          show all logo variants you can set in the config\n  -cl, --changelog            show changelog\n  -c, --config                show config and config location(s)\n  -gc, --generate-config      generate a new config\n```\n# Examples\n`deew -i *thd`\\\nencode DDP\n\n`deew -b 768 -i *flac`\\\nencode DDP@768\n\n`deew -dm 2 -f dd -b 192 -i *.ec3`\\\nencode DD@192 with stereo downmixing\n\n`deew -f dd -b 448 -t 4 -i S01`\\\nencode DD@448 using 4 threads (input is a folder)\n\n`deew -f thd -i *w64`\\\nencode TrueHD\n\n`deew -f dd -i *dts -k`\\\n`deew -f ddp -i *dts`\\\nencode multiple formats/bitrates while creating the temp file only once\n\n# Discussion and Support\n[https://t.me/deew_support](https://t.me/deew_support)\n',
-    'author': 'pcroland',
-    'author_email': 'pcroland@protonmail.ch',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'None',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.7,<4.0',
-}
-
-
-setup(**setup_kwargs)
```

#### html2text {}

```diff
@@ -1,140 +1,130 @@
-# -*- coding: utf-8 -*- from setuptools import setup packages = \ ['deew']
-package_data = \ {'': ['*']} install_requires = \ ['Unidecode>=1.3.4,<2.0.0',
-'packaging>=21.3,<22.0', 'platformdirs>=2.5.2,<3.0.0',
-'requests>=2.28.1,<3.0.0', 'rich>=12.5.1,<13.0.0', 'toml>=0.10.2,<0.11.0',
-'xmltodict>=0.13.0,<0.14.0'] entry_points = \ {'console_scripts': ['deew =
-deew.__main__:main']} setup_kwargs = { 'name': 'deew', 'version': '2.9.5',
-'description': 'Dolby Encoding Engine Wrapper', 'long_description': '[![builds]
-(https://img.shields.io/github/workflow/status/pcroland/deew/
-Build%20and%20publish?logo=github&style=flat-square)](https://github.com/
-pcroland/deew/actions/workflows/build.yaml)\n[![github_release](https://
-img.shields.io/github/v/release/pcroland/
+Metadata-Version: 2.1 Name: deew Version: 3.0.0 Summary: Dolby Encoding Engine
+Wrapper License: MIT Author: pcroland Author-email: pcroland@protonmail.ch
+Requires-Python: >=3.7,<3.12 Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3 Classifier: Programming
+Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: Unidecode (>=1.3.4,<2.0.0) Requires-Dist: packaging
+(>=21.3,<22.0) Requires-Dist: platformdirs (>=2.5.2,<3.0.0) Requires-Dist:
+requests (>=2.28.1,<3.0.0) Requires-Dist: rich (>=12.5.1,<13.0.0) Requires-
+Dist: toml (>=0.10.2,<0.11.0) Requires-Dist: xmltodict (>=0.13.0,<0.14.0)
+Description-Content-Type: text/markdown [![builds](https://img.shields.io/
+github/actions/workflow/status/pcroland/deew/build.yaml?logo=github&style=flat-
+square)](https://github.com/pcroland/deew/actions/workflows/build.yaml) [!
+[github_release](https://img.shields.io/github/v/release/pcroland/
 deew?logo=github&color=70920c&style=flat-square)](https://github.com/pcroland/
-deew/releases)\n[![pypi_release](https://img.shields.io/pypi/v/
+deew/releases) [![pypi_release](https://img.shields.io/pypi/v/
 deew?label=PyPI&logo=pypi&logoColor=ffffff&color=70920c&style=flat-square)]
-(https://pypi.org/project/deew)\n[![pypi_downloads](https://img.shields.io/
-pypi/dm/deew?color=70920c&logo=pypi&logoColor=white&style=flat-square)](https:/
-/pypi.org/project/deew)\n[![license](https://img.shields.io/github/license/
+(https://pypi.org/project/deew) [![pypi_downloads](https://img.shields.io/pypi/
+dm/deew?color=70920c&logo=pypi&logoColor=white&style=flat-square)](https://
+pypi.org/project/deew) [![license](https://img.shields.io/github/license/
 pcroland/deew?color=blueviolet&style=flat-square)](https://github.com/pcroland/
-deew/blob/master/LICENSE)\n\\\n[![telegram](https://img.shields.io/
-endpoint?color=1d93d2&style=flat-square&url=https://cadoth.net/
-tgmembercount%3Fchat_id=deew_support%26name=Discussion%2520and%2520Support)]
-(https://t.me/deew_support)\n[![commits](https://img.shields.io/github/last-
+deew/blob/master/LICENSE) \ [![commits](https://img.shields.io/github/last-
 commit/pcroland/deew?color=355ab8&logo=github&style=flat-square)](https://
-github.com/pcroland/deew/commits/main)\n[![issues](https://img.shields.io/
+github.com/pcroland/deew/commits/main) [![issues](https://img.shields.io/
 github/issues/pcroland/deew?color=355ab8&logo=github&style=flat-square)](https:
-//github.com/pcroland/deew/issues)\n\\\n[![name](https://img.shields.io/badge/
+//github.com/pcroland/deew/issues) \ [![name](https://img.shields.io/badge/
 platform-win%20%7C%20linux%20%7C%20osx-eeeeee?style=flat-square)](https://
-github.com/pcroland/deew)\n[![name](https://img.shields.io/pypi/pyversions/
+github.com/pcroland/deew) [![name](https://img.shields.io/pypi/pyversions/
 deew?logo=Python&logoColor=eeeeee&color=eeeeee&style=flat-square)](https://
-github.com/pcroland/deew)\n[![name](https://img.shields.io/badge/DEE-5.1.0--
+github.com/pcroland/deew) [![name](https://img.shields.io/badge/DEE-5.1.0--
 5.2.1-green?logoColor=white&logo=data:image/
 png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAMCAYAAABr5z2BAAAA9ElEQVQokZXSzypFURQG8N89LsnEv1KGBp5CKU9wBygPIJ5AeYM7MjLAzMBAmRuYyszU3AOgG6GQpZ19OM69Tny1Wu39rVXfWt9qRcQaljCOUbygh3c/
 MYQJDOMZ9zhvYwEb+hG1n9aAmlaBkfzYwQo2cZUbqnGJdSxjP/
 eMiYi9+MRiRKjEWXzjpMZ1MnNUVORM1+R1ck6jrNa4qZJrD5irRFrUHW4aahRNJN7w2lTQpCBhBpN/
 VfBU4w5yTr53a1war0/BPK7zQW1lS0tsYxa7eMDcFxMRhxW7/ovjpOAUj9madMppabe/
 nHKyOvWkcXu4+AAd1Ju1TsOvFgAAAABJRU5ErkJggg==&color=eeeeee&style=flat-square)]
 (https://customer.dolby.com/content-creation-and-delivery/dolby-encoding-
-engine-with-ac-4)\n
+engine-with-ac-4)
 ===============================================================================
-\n
      [https://raw.githubusercontent.com/pcroland/deew/main/logo/logo.svg]
                          Dolby Encoding Engine Wrapper
-\n\n\n
-                     English_readme\n â¢ Magyar_leÃ­rÃ¡s
-\n\n## DDP encoding has never been so easy!\n\n![img](https://telegra.ph/file/
-efd2a1d3519bdf87fca03.gif)\n\n\n# Description\n- handles Dolby\'s XML input
-fuckery in the background, giving you a proper CLI interface\n- converts inputs
-to RF64 which DEE can use\n - bit depth, number of channels and other infos are
-parsed from the source\n- an XML file will be generated for each input based on
-the settings\n- the script utilizes thread pooling for batch encoding (see
-config)\n- supports WSL path conversion for the Windows version of DEE (see
-config)\n- in case of an invalid bitrate it will pick the closest allowed
-one\n- automatic sample rate conversion using ffmpeg\'s soxr resampler in case
-of an unsupported sample rate\n - for DD/DDP unsupported rates will be
-converted to 48 kHz\n - for TrueHD unsupported rates will be converted to 48
-kHz if source sample rate is lower than 72 kHz, otherwise will be converted to
-96 kHz\n- automatic channel swapping for 7.1 sources (DEE swaps Ls Rs with Lrs
-Rrs for some reason)\n- automatic dialnorm setting\n- automatically compensates
-for DEE\'s 256 sample delay (DD and DDP encoding)\n- checks if intermediate
-file is already created so you can encode different formats/bitrates using a
-single intermediate file, for example:\\\n `deew -f dd -b 448 -i input -k`\\\n
-`deew -f dd -b 640 -i input -k`\\\n `deew -f ddp -i input`\n- works even with
-video inputs (first audio will be selected)\n- fancy terminal output using
-rich\n- versatile delay option that supports ms, s and also frame@fps
-formats\n- parsing delay from filenames\n\n# Requirements\n- Python *(you
-don\'t need it if you use a standalone build of deew)*\n- ffmpeg 5.1.2 or older
-*(they messed up something in w64/rf64 and new versions can\'t be used
-currently for DEE)*\n- ffprobe\n- Dolby Encoding Engine\n\n# Dolby Encoding
-Engine installation\n- install [DEE](https://customer.dolby.com/content-
-creation-and-delivery/dolby-encoding-engine-with-ac-4) (if you use macOS,
-install [DME](https://customer.dolby.com/content-creation-and-delivery/dolby-
-media-encoder-with-ac-4))\n - for TrueHD encoding support you need the Windows
-version\n - if you use WSL1 use the Windows version for better performance\n -
-if you use the Windows version of DEE under Linux (and not from WSL) / macOS
-install `wine-binfmt`\n- place your `license.lic` file next to the DEE binary
-(`dee.exe` under Windows, `dee` under Linux/macOS)\n- if DEE throws `Failed to
-load library "...dll".` errors when you run deew install [VisualCppRedist AIO]
-(https://github.com/abbodi1406/vcredist/releases)\n\n# deew installation\n###
-with standalone build (Windows 8-11/Linux):\n- grab the latest build from:
-[https://github.com/pcroland/deew/releases](https://github.com/pcroland/deew/
-releases)\n- run with: `deew`\\\n*(run the binary from terminal, doubleclicking
-it won\'t work)*\n- on the first run it will create a config file, choose where
-you want to keep it\n- updating: grab the latest build from: [https://
-github.com/pcroland/deew/releases](https://github.com/pcroland/deew/
-releases)\n\n### with Python environment (Windows/Linux/macOS):\n- install
-Python and pip if you don\'t have it already\n- run: `pip install deew`\n- run
-with: `deew`\n- on the first run it will create a config file\n- updating: `pip
-install deew --upgrade`\n\n# Setup system PATH variable\nIf you don\'t want to
-use full paths for the binaries in your config or when you use them from CLI, I
-suggest to setup system PATH variables\n### Windows:\n- open `cmd.exe` as
-administrator\n- run a `setx /m PATH "%PATH%;[location]"` command for each path
-that contains binaries\\\n *(replace* `[location]` *with the path)*\n- for
-example:\n```bat\nsetx /m PATH "%PATH%;C:\\bin\\dee"\nsetx /m PATH "%PATH%;C:
-\\bin\\ffmpeg"\n```\n### Linux/macOS:\n- add a `PATH="[location]:$PATH"` line
-in your `~/.bashrc` or `~/.zshrc` file for each path that contains a binary\\\n
-*(replace* `[location]` *with the path)*\n- for example:\n```sh\nPATH="/usr/
-local/bin/dee:$PATH"\nPATH="/usr/local/bin/ffmpeg:$PATH"\n```\n\n#
-Usage\n```\nâ¯ deew -h\ndeew 2.9.5\n\nUSAGE: deew [-h] [-v] [-i [INPUT ...]]
-[-ti INDEX] [-o DIRECTORY] [-f FORMAT]\n [-b BITRATE] [-dm CHANNELS] [-d DELAY]
-[-r DRC] [-dn DIALNORM]\n [-in INSTANCES] [-k] [-mo] [-fs] [-fb] [-lb] [-la] [-
-np] [-pl]\n [-cl] [-c] [-gc]\n\nFLAGS:\n -h, --help show this help message.\n -
-v, --version show version.\n -i, --input [INPUT ...] audio file(s) or folder
-(s)\n -ti, --track-index INDEX default: 0\n select audio track index of input
-(s)\n -o, --output DIRECTORY default: current directory\n specifies output
-directory\n -f, --format FORMAT options: dd / ddp / thd\n default: ddp\n -b, --
-bitrate BITRATE options: run -lb/--list-bitrates\n default: run -c/--config\n -
-dm, --downmix CHANNELS options: 1 / 2 / 6\n specifies downmix, only works for
-DD/DDP\n DD will be automatically downmixed to 5.1 in case of a 7.1 source\n -
-d, --delay DELAY examples: -5.1ms, +1,52s, -24@pal, +10@24000/1001\n default:
-0ms or parsed from filename\n specifies delay as ms, s or frame@FPS\n FPS can
-be a number, division or ntsc / pal\n you have to specify negative values as -
-d=-0ms\n -r, --drc DRC options: film_light / film_standard / music_light /
-music_standard / speech\n default: music_light (this is the closest to the
-missing none preset)\n specifies drc profile\n -dn, --dialnorm DIALNORM
-options: between -31 and 0 (in case of 0 DEE\'s measurement will be used)\n
-default: 0\n applied dialnorm value between\n -in, --instances INSTANCES
-examples: 1, 4, 50%\n default: 50%\n specifies how many encodes can run at the
-same time\n 50% means 4 on a cpu with 8 threads\n one DEE can use 2 threads so
-50% can utilize all threads\n (this option overrides the config\'s number)\n -
-k, --keeptemp keep temp files\n -mo, --measure-only kills DEE when the dialnorm
-gets written to the progress bar\n this option overrides format with ddp\n -fs,
---force-standard force standard profile for 7.1 DDP encoding (384-1024 kbps)\n
--fb, --force-bluray force bluray profile for 7.1 DDP encoding (768-1664 kbps)\n
--lb, --list-bitrates list bitrates that DEE can do for DD and DDP encoding\n -
-la, --long-argument print ffmpeg and DEE arguments for each input\n -np, --no-
-prompt disables prompt\n -pl, --print-logos show all logo variants you can set
-in the config\n -cl, --changelog show changelog\n -c, --config show config and
-config location(s)\n -gc, --generate-config generate a new config\n```\n#
-Examples\n`deew -i *thd`\\\nencode DDP\n\n`deew -b 768 -i *flac`\\\nencode
-DDP@768\n\n`deew -dm 2 -f dd -b 192 -i *.ec3`\\\nencode DD@192 with stereo
-downmixing\n\n`deew -f dd -b 448 -t 4 -i S01`\\\nencode DD@448 using 4 threads
-(input is a folder)\n\n`deew -f thd -i *w64`\\\nencode TrueHD\n\n`deew -f dd -
-i *dts -k`\\\n`deew -f ddp -i *dts`\\\nencode multiple formats/bitrates while
-creating the temp file only once\n\n# Discussion and Support\n[https://t.me/
-deew_support](https://t.me/deew_support)\n', 'author': 'pcroland',
-'author_email': 'pcroland@protonmail.ch', 'maintainer': 'None',
-'maintainer_email': 'None', 'url': 'None', 'packages': packages,
-'package_data': package_data, 'install_requires': install_requires,
-'entry_points': entry_points, 'python_requires': '>=3.7,<4.0', } setup
-(**setup_kwargs)
+                      English_readme â¢ Magyar_leÃ­rÃ¡s
+## DDP encoding has never been so easy! ![img](https://telegra.ph/file/
+efd2a1d3519bdf87fca03.gif)  # Description - handles Dolby's XML input fuckery
+in the background, giving you a proper CLI interface - converts inputs to RF64
+which DEE can use - bit depth, number of channels and other infos are parsed
+from the source - an XML file will be generated for each input based on the
+settings - the script utilizes thread pooling for batch encoding (see config) -
+supports WSL path conversion for the Windows version of DEE (see config) - in
+case of an invalid bitrate it will pick the closest allowed one - automatic
+sample rate conversion using ffmpeg's soxr resampler in case of an unsupported
+sample rate - for DD/DDP/AC4 unsupported rates will be converted to 48 kHz -
+for TrueHD unsupported rates will be converted to 48 kHz if source sample rate
+is lower than 72 kHz, otherwise will be converted to 96 kHz - automatic channel
+swapping for 7.1 sources (DEE swaps Ls Rs with Lrs Rrs for some reason) -
+automatic dialnorm setting - automatically compensates for DEE's 256 sample
+delay (DD and DDP encoding) - checks if intermediate file is already created so
+you can encode different formats/bitrates using a single intermediate file, for
+example:\ `deew -f dd -b 448 -i input -k`\ `deew -f dd -b 640 -i input -k`\
+`deew -f ddp -i input` - works even with video inputs (first audio will be
+selected) - fancy terminal output using rich - versatile delay option that
+supports ms, s and also frame@fps formats - parsing delay from filenames #
+Requirements - Python *(you don't need it if you use a standalone build of
+deew)* - ffmpeg - ffprobe - Dolby Encoding Engine # Dolby Encoding Engine
+installation - install [DEE](https://customer.dolby.com/content-creation-and-
+delivery/dolby-encoding-engine-with-ac-4) (if you use macOS, install [DME]
+(https://customer.dolby.com/content-creation-and-delivery/dolby-media-encoder-
+with-ac-4)) - for TrueHD encoding support you need the Windows version - if you
+use WSL1 use the Windows version for better performance - if you use the
+Windows version of DEE under Linux (and not from WSL) / macOS install `wine-
+binfmt` - place your `license.lic` file next to the DEE binary (`dee.exe` under
+Windows, `dee` under Linux/macOS) - if DEE throws `Failed to load library
+"...dll".` errors when you run deew install [VisualCppRedist AIO](https://
+github.com/abbodi1406/vcredist/releases) # deew installation ### with
+standalone build (Windows 8-11/Linux): - grab the latest build from: [https://
+github.com/pcroland/deew/releases](https://github.com/pcroland/deew/releases) -
+run with: `deew`\ *(run the binary from terminal, doubleclicking it won't
+work)* - on the first run it will create a config file, choose where you want
+to keep it - updating: grab the latest build from: [https://github.com/
+pcroland/deew/releases](https://github.com/pcroland/deew/releases) ### with
+Python environment (Windows/Linux/macOS): - install Python and pip if you don't
+have it already - run: `pip install deew` - run with: `deew` - on the first run
+it will create a config file - updating: `pip install deew --upgrade` # Setup
+system PATH variable If you don't want to use full paths for the binaries in
+your config or when you use them from CLI, I suggest to setup system PATH
+variables ### Windows: - open `cmd.exe` as administrator - run a `setx /m PATH
+"%PATH%;[location]"` command for each path that contains binaries\ *(replace* `
+[location]` *with the path)* - for example: ```bat setx /m PATH "%PATH%;C:
+\bin\dee" setx /m PATH "%PATH%;C:\bin\ffmpeg" ``` ### Linux/macOS: - add a
+`PATH="[location]:$PATH"` line in your `~/.bashrc` or `~/.zshrc` file for each
+path that contains a binary\ *(replace* `[location]` *with the path)* - for
+example: ```sh PATH="/usr/local/bin/dee:$PATH" PATH="/usr/local/bin/ffmpeg:
+$PATH" ``` # Usage ``` â¯ deew -h deew 3.0.0 USAGE: deew [-h] [-v] [-i [INPUT
+...]] [-ti INDEX] [-o DIRECTORY] [-f FORMAT] [-b BITRATE] [-dm CHANNELS] [-
+d DELAY] [-r DRC] [-dn DIALNORM] [-in INSTANCES] [-k] [-mo] [-fs] [-fb] [-lb]
+[-la] [-np] [-pl] [-cl] [-c] [-gc] FLAGS: -h, --help show this help message. -
+v, --version show version. -i, --input [INPUT ...] audio file(s) or folder(s) -
+ti, --track-index INDEX default: 0 select audio track index of input(s) -o, --
+output DIRECTORY default: current directory specifies output directory -f, --
+format FORMAT options: dd / ddp / ac4 / thd default: ddp -b, --bitrate BITRATE
+options: run -lb/--list-bitrates default: run -c/--config -dm, --downmix
+CHANNELS options: 1 / 2 / 6 specifies downmix, only works for DD/DDP DD will be
+automatically downmixed to 5.1 in case of a 7.1 source -d, --delay DELAY
+examples: -5.1ms, +1,52s, -24@pal, +10@24000/1001 default: 0ms or parsed from
+filename specifies delay as ms, s or frame@FPS FPS can be a number, division or
+ntsc / pal you have to specify negative values as -d=-0ms -r, --drc DRC
+options: film_light / film_standard / music_light / music_standard / speech
+default: music_light (this is the closest to the missing none preset) specifies
+drc profile -dn, --dialnorm DIALNORM options: between -31 and 0 (in case of 0
+DEE's measurement will be used) default: 0 applied dialnorm value between -in,
+--instances INSTANCES examples: 1, 4, 50% default: 50% specifies how many
+encodes can run at the same time 50% means 4 on a cpu with 8 threads one DEE
+can use 2 threads so 50% can utilize all threads (this option overrides the
+config's number) -k, --keeptemp keep temp files -mo, --measure-only kills DEE
+when the dialnorm gets written to the progress bar this option overrides format
+with ddp -fs, --force-standard force standard profile for 7.1 DDP encoding
+(384-1024 kbps) -fb, --force-bluray force bluray profile for 7.1 DDP encoding
+(768-1664 kbps) -lb, --list-bitrates list bitrates that DEE can do for DD and
+DDP encoding -la, --long-argument print ffmpeg and DEE arguments for each input
+-np, --no-prompt disables prompt -pl, --print-logos show all logo variants you
+can set in the config -cl, --changelog show changelog -c, --config show config
+and config location(s) -gc, --generate-config generate a new config ``` #
+Examples `deew -i *thd`\ encode DDP `deew -b 768 -i *flac`\ encode DDP@768
+`deew -dm 2 -f dd -b 192 -i *.ec3`\ encode DD@192 with stereo downmixing `deew
+-f dd -b 448 -t 4 -i S01`\ encode DD@448 using 4 threads (input is a folder)
+`deew -f thd -i *w64`\ encode TrueHD `deew -f dd -i *dts -k`\ `deew -f ddp -
+i *dts`\ encode multiple formats/bitrates while creating the temp file only
+once # Discussion and Support [https://t.me/deew_support](https://t.me/
+deew_support)
```

