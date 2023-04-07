# Comparing `tmp/fish_audio_preprocess-0.1.9.tar.gz` & `tmp/fish_audio_preprocess-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fish_audio_preprocess-0.1.9.tar", max compression
+gzip compressed data, was "fish_audio_preprocess-0.2.0.tar", max compression
```

## Comparing `fish_audio_preprocess-0.1.9.tar` & `fish_audio_preprocess-0.2.0.tar`

### file list

```diff
@@ -1,22 +1,20 @@
--rw-r--r--   0        0        0    11344 2023-01-06 00:07:08.214784 fish_audio_preprocess-0.1.9/LICENSE
--rw-r--r--   0        0        0        0 2023-01-06 00:28:50.280789 fish_audio_preprocess-0.1.9/fish_audio_preprocess/__init__.py
--rw-r--r--   0        0        0      821 2023-02-14 07:54:46.680287 fish_audio_preprocess-0.1.9/fish_audio_preprocess/cli/__main__.py
--rw-r--r--   0        0        0     2479 2023-02-14 02:35:56.301360 fish_audio_preprocess-0.1.9/fish_audio_preprocess/cli/convert_to_wav.py
--rw-r--r--   0        0        0     3128 2023-02-14 02:35:56.301360 fish_audio_preprocess-0.1.9/fish_audio_preprocess/cli/frequency.py
--rw-r--r--   0        0        0     3089 2023-02-14 02:37:35.377657 fish_audio_preprocess-0.1.9/fish_audio_preprocess/cli/length.py
--rw-r--r--   0        0        0     2960 2023-02-14 02:35:56.301360 fish_audio_preprocess-0.1.9/fish_audio_preprocess/cli/loudness_norm.py
--rw-r--r--   0        0        0     4175 2023-01-09 04:43:12.400784 fish_audio_preprocess-0.1.9/fish_audio_preprocess/cli/separate_audio.py
--rw-r--r--   0        0        0     3729 2023-02-14 02:35:56.301360 fish_audio_preprocess-0.1.9/fish_audio_preprocess/cli/slice_audio.py
--rw-r--r--   0        0        0      176 2023-02-03 07:43:54.404072 fish_audio_preprocess-0.1.9/fish_audio_preprocess/cli/so_vits_svc/__init__.py
--rw-r--r--   0        0        0     3630 2023-02-14 02:37:35.413657 fish_audio_preprocess-0.1.9/fish_audio_preprocess/cli/so_vits_svc/preprocess.py
--rw-r--r--   0        0        0      638 2023-02-03 07:46:26.761161 fish_audio_preprocess-0.1.9/fish_audio_preprocess/cli/to_ipa.py
--rw-r--r--   0        0        0  9504952 2023-02-03 07:46:26.809162 fish_audio_preprocess-0.1.9/fish_audio_preprocess/utils/cedict_ts.u8
--rw-r--r--   0        0        0     1783 2023-02-14 02:35:56.301360 fish_audio_preprocess-0.1.9/fish_audio_preprocess/utils/file.py
--rw-r--r--   0        0        0     1821 2023-02-14 02:35:56.301360 fish_audio_preprocess-0.1.9/fish_audio_preprocess/utils/loudness_norm.py
--rw-r--r--   0        0        0     1438 2023-02-03 07:46:26.809162 fish_audio_preprocess-0.1.9/fish_audio_preprocess/utils/polyphonic.yaml
--rw-r--r--   0        0        0     4158 2023-02-14 02:35:56.301360 fish_audio_preprocess-0.1.9/fish_audio_preprocess/utils/separate_audio.py
--rw-r--r--   0        0        0     3844 2023-02-14 07:58:31.001279 fish_audio_preprocess-0.1.9/fish_audio_preprocess/utils/slice_audio.py
--rw-r--r--   0        0        0     4476 2023-02-14 02:37:35.397657 fish_audio_preprocess-0.1.9/fish_audio_preprocess/utils/to_ipa.py
--rw-r--r--   0        0        0     1052 2023-02-14 07:58:36.441303 fish_audio_preprocess-0.1.9/pyproject.toml
--rw-r--r--   0        0        0     1356 1970-01-01 00:00:00.000000 fish_audio_preprocess-0.1.9/setup.py
--rw-r--r--   0        0        0     1207 1970-01-01 00:00:00.000000 fish_audio_preprocess-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0    11344 2023-01-06 00:07:08.214784 fish_audio_preprocess-0.2.0/LICENSE
+-rw-r--r--   0        0        0        0 2023-01-06 00:28:50.280789 fish_audio_preprocess-0.2.0/fish_audio_preprocess/__init__.py
+-rw-r--r--   0        0        0      812 2023-04-07 15:48:03.774064 fish_audio_preprocess-0.2.0/fish_audio_preprocess/cli/__main__.py
+-rw-r--r--   0        0        0     2616 2023-04-07 15:48:03.654063 fish_audio_preprocess-0.2.0/fish_audio_preprocess/cli/convert_to_wav.py
+-rw-r--r--   0        0        0     3220 2023-02-15 00:17:07.529910 fish_audio_preprocess-0.2.0/fish_audio_preprocess/cli/frequency.py
+-rw-r--r--   0        0        0     3287 2023-02-15 00:02:34.687587 fish_audio_preprocess-0.2.0/fish_audio_preprocess/cli/length.py
+-rw-r--r--   0        0        0     3097 2023-04-07 15:48:03.650063 fish_audio_preprocess-0.2.0/fish_audio_preprocess/cli/loudness_norm.py
+-rw-r--r--   0        0        0     3203 2023-04-07 15:51:03.378957 fish_audio_preprocess-0.2.0/fish_audio_preprocess/cli/resample.py
+-rw-r--r--   0        0        0     4312 2023-04-07 15:48:03.674063 fish_audio_preprocess-0.2.0/fish_audio_preprocess/cli/separate_audio.py
+-rw-r--r--   0        0        0     3866 2023-04-07 15:48:03.658063 fish_audio_preprocess-0.2.0/fish_audio_preprocess/cli/slice_audio.py
+-rw-r--r--   0        0        0      638 2023-02-03 07:46:26.761161 fish_audio_preprocess-0.2.0/fish_audio_preprocess/cli/to_ipa.py
+-rw-r--r--   0        0        0  9504952 2023-02-03 07:46:26.809162 fish_audio_preprocess-0.2.0/fish_audio_preprocess/utils/cedict_ts.u8
+-rw-r--r--   0        0        0     1783 2023-02-14 02:35:56.301360 fish_audio_preprocess-0.2.0/fish_audio_preprocess/utils/file.py
+-rw-r--r--   0        0        0     1821 2023-02-14 02:35:56.301360 fish_audio_preprocess-0.2.0/fish_audio_preprocess/utils/loudness_norm.py
+-rw-r--r--   0        0        0     1438 2023-02-03 07:46:26.809162 fish_audio_preprocess-0.2.0/fish_audio_preprocess/utils/polyphonic.yaml
+-rw-r--r--   0        0        0     4158 2023-02-14 02:35:56.301360 fish_audio_preprocess-0.2.0/fish_audio_preprocess/utils/separate_audio.py
+-rw-r--r--   0        0        0     3869 2023-02-21 19:58:52.805912 fish_audio_preprocess-0.2.0/fish_audio_preprocess/utils/slice_audio.py
+-rw-r--r--   0        0        0     4476 2023-02-14 02:37:35.397657 fish_audio_preprocess-0.2.0/fish_audio_preprocess/utils/to_ipa.py
+-rw-r--r--   0        0        0     1052 2023-04-07 15:38:21.463154 fish_audio_preprocess-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1207 1970-01-01 00:00:00.000000 fish_audio_preprocess-0.2.0/PKG-INFO
```

### Comparing `fish_audio_preprocess-0.1.9/LICENSE` & `fish_audio_preprocess-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fish_audio_preprocess-0.1.9/fish_audio_preprocess/cli/__main__.py` & `fish_audio_preprocess-0.2.0/fish_audio_preprocess/cli/__main__.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 import richuru
 from loguru import logger
 
 from .convert_to_wav import to_wav
 from .frequency import frequency
 from .length import length
 from .loudness_norm import loudness_norm
+from .resample import resample
 from .separate_audio import separate
 from .slice_audio import slice_audio
-from .so_vits_svc import so_vits_svc
 from .to_ipa import to_ipa
 
 
 @click.group()
 @click.option("--debug/--no-debug", default=False)
 def cli(debug: bool):
     """An audio preprocessing CLI."""
@@ -26,14 +26,14 @@
 cli.add_command(length)
 cli.add_command(frequency)
 
 cli.add_command(to_wav)
 cli.add_command(separate)
 cli.add_command(loudness_norm)
 cli.add_command(slice_audio)
+cli.add_command(resample)
 
-cli.add_command(so_vits_svc)
 cli.add_command(to_ipa)
 
 
 if __name__ == "__main__":
     to_wav()
```

### Comparing `fish_audio_preprocess-0.1.9/fish_audio_preprocess/cli/convert_to_wav.py` & `fish_audio_preprocess-0.2.0/fish_audio_preprocess/cli/convert_to_wav.py`

 * *Files 11% similar despite different names*

```diff
@@ -36,14 +36,19 @@
     overwrite: bool,
     clean: bool,
     segment: int,
 ):
     """Converts all audio and video files in input_dir to wav files in output_dir."""
 
     input_dir, output_dir = Path(input_dir), Path(output_dir)
+
+    if input_dir == output_dir and clean:
+        logger.error("You are trying to clean the input directory, aborting")
+        return
+
     make_dirs(output_dir, clean)
 
     files = list_files(
         input_dir, extensions=VIDEO_EXTENSIONS | AUDIO_EXTENSIONS, recursive=recursive
     )
     logger.info(f"Found {len(files)} files, converting to wav")
```

### Comparing `fish_audio_preprocess-0.1.9/fish_audio_preprocess/cli/frequency.py` & `fish_audio_preprocess-0.2.0/fish_audio_preprocess/cli/frequency.py`

 * *Files 13% similar despite different names*

```diff
@@ -19,15 +19,19 @@
     Returns:
         Counter: A counter of the notes
     """
 
     import librosa
     import parselmouth as pm
 
-    pitch_ac = pm.Sound(str(file)).to_pitch_ac()
+    pitch_ac = pm.Sound(str(file)).to_pitch_ac(
+        voicing_threshold=0.6,
+        pitch_floor=40.0,
+        pitch_ceiling=1600.0,
+    )
     f0 = pitch_ac.selected_array["frequency"]
 
     counter = Counter()
     for i in f0:
         if np.isinf(i) or np.isnan(i) or i == 0:
             continue
```

### Comparing `fish_audio_preprocess-0.1.9/fish_audio_preprocess/cli/length.py` & `fish_audio_preprocess-0.2.0/fish_audio_preprocess/cli/length.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 from pathlib import Path
+from typing import Optional
 
 import click
 from loguru import logger
 from tqdm import tqdm
 
 from fish_audio_preprocess.utils.file import AUDIO_EXTENSIONS, list_files
 
 
 @click.command()
 @click.argument("input_dir", type=click.Path(exists=True, file_okay=False))
 @click.option("--recursive/--no-recursive", default=True, help="Search recursively")
 @click.option(
     "--visualize/--no-visualize", default=False, help="Visualize the distribution"
 )
-@click.option("-l", "--long-threshold", default=20, help="Threshold for long files")
-@click.option("-s", "--short-threshold", default=2, help="Threshold for short files")
+@click.option("-l", "--long-threshold", default=None, help="Threshold for long files")
+@click.option("-s", "--short-threshold", default=None, help="Threshold for short files")
 def length(
     input_dir: str,
     recursive: bool,
     visualize: bool,
-    long_threshold: int,
-    short_threshold: int,
+    long_threshold: Optional[int],
+    short_threshold: Optional[int],
 ):
     """
     Get the length of all audio files in a directory
     """
 
     import soundfile as sf
     from matplotlib import pyplot as plt
@@ -49,32 +50,38 @@
     total_duration = sum(i[2] for i in infos)
     avg_duration = total_duration / len(infos)
     logger.info(f"Total duration: {total_duration / 3600:.2f} hours")
     logger.info(f"Average duration: {avg_duration:.2f} seconds")
     logger.info(f"Max duration: {max(i[2] for i in infos):.2f} seconds")
     logger.info(f"Min duration: {min(i[2] for i in infos):.2f} seconds")
 
-    # Too Long or Too Short
-    long_files = [i for i in infos if i[2] > long_threshold]
-    short_files = [i for i in infos if i[2] < short_threshold]
-    # sort by duration
-    if long_files:
-        long_files = sorted(long_files, key=lambda x: x[2], reverse=True)
-        logger.warning(
-            f"Found {len(long_files)} files longer than {long_threshold} seconds"
-        )
-        for i in [f"{i[3]}: {i[2]:.2f}" for i in long_files]:
-            logger.warning(f"    {i}")
-    if short_files:
-        short_files = sorted(short_files, key=lambda x: x[2], reverse=False)
-        logger.warning(
-            f"Found {len(short_files)} files shorter than {short_threshold} seconds"
-        )
-        for i in [f"{i[3]}: {i[2]:.2f}" for i in short_files]:
-            logger.warning(f"    {i}")
+    # Too Long
+    if long_threshold is not None:
+        long_files = [i for i in infos if i[2] > long_threshold]
+
+        # sort by duration
+        if long_files:
+            long_files = sorted(long_files, key=lambda x: x[2], reverse=True)
+            logger.warning(
+                f"Found {len(long_files)} files longer than {long_threshold} seconds"
+            )
+            for i in [f"{i[3]}: {i[2]:.2f}" for i in long_files]:
+                logger.warning(f"    {i}")
+
+    # Too Short
+    if short_threshold is not None:
+        short_files = [i for i in infos if i[2] < short_threshold]
+
+        if short_files:
+            short_files = sorted(short_files, key=lambda x: x[2], reverse=False)
+            logger.warning(
+                f"Found {len(short_files)} files shorter than {short_threshold} seconds"
+            )
+            for i in [f"{i[3]}: {i[2]:.2f}" for i in short_files]:
+                logger.warning(f"    {i}")
 
     # Sample Rate
     total_samplerate = sum(i[1] for i in infos)
     avg_samplerate = total_samplerate / len(infos)
     logger.info(f"Average samplerate: {avg_samplerate:.2f}")
 
     if not visualize:
```

### Comparing `fish_audio_preprocess-0.1.9/fish_audio_preprocess/cli/loudness_norm.py` & `fish_audio_preprocess-0.2.0/fish_audio_preprocess/cli/loudness_norm.py`

 * *Files 9% similar despite different names*

```diff
@@ -59,14 +59,19 @@
     num_workers: int,
 ):
     """Perform loudness normalization (ITU-R BS.1770-4) on audio files."""
 
     from fish_audio_preprocess.utils.loudness_norm import loudness_norm_file
 
     input_dir, output_dir = Path(input_dir), Path(output_dir)
+
+    if input_dir == output_dir and clean:
+        logger.error("You are trying to clean the input directory, aborting")
+        return
+
     make_dirs(output_dir, clean)
 
     files = list_files(input_dir, extensions=AUDIO_EXTENSIONS, recursive=recursive)
     logger.info(f"Found {len(files)} files, normalizing loudness")
 
     skipped = 0
```

### Comparing `fish_audio_preprocess-0.1.9/fish_audio_preprocess/cli/separate_audio.py` & `fish_audio_preprocess-0.2.0/fish_audio_preprocess/cli/separate_audio.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,14 +100,19 @@
     num_workers_per_gpu: int,
 ):
     """
     Separates audio in input_dir using model and saves to output_dir.
     """
 
     input_dir, output_dir = Path(input_dir), Path(output_dir)
+
+    if input_dir == output_dir and clean:
+        logger.error("You are trying to clean the input directory, aborting")
+        return
+
     make_dirs(output_dir, clean)
 
     base_args = (
         input_dir,
         output_dir,
         recursive,
         overwrite,
```

### Comparing `fish_audio_preprocess-0.1.9/fish_audio_preprocess/cli/slice_audio.py` & `fish_audio_preprocess-0.2.0/fish_audio_preprocess/cli/slice_audio.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,14 +83,19 @@
     hop_length: int,
 ):
     """Slice audio files into smaller chunks by silence."""
 
     from fish_audio_preprocess.utils.slice_audio import slice_audio_file
 
     input_dir, output_dir = Path(input_dir), Path(output_dir)
+
+    if input_dir == output_dir and clean:
+        logger.error("You are trying to clean the input directory, aborting")
+        return
+
     make_dirs(output_dir, clean)
 
     files = list_files(input_dir, extensions=AUDIO_EXTENSIONS, recursive=recursive)
     logger.info(f"Found {len(files)} files, processing...")
 
     skipped = 0
```

### Comparing `fish_audio_preprocess-0.1.9/fish_audio_preprocess/cli/to_ipa.py` & `fish_audio_preprocess-0.2.0/fish_audio_preprocess/cli/to_ipa.py`

 * *Files identical despite different names*

### Comparing `fish_audio_preprocess-0.1.9/fish_audio_preprocess/utils/cedict_ts.u8` & `fish_audio_preprocess-0.2.0/fish_audio_preprocess/utils/cedict_ts.u8`

 * *Files identical despite different names*

### Comparing `fish_audio_preprocess-0.1.9/fish_audio_preprocess/utils/file.py` & `fish_audio_preprocess-0.2.0/fish_audio_preprocess/utils/file.py`

 * *Files identical despite different names*

### Comparing `fish_audio_preprocess-0.1.9/fish_audio_preprocess/utils/loudness_norm.py` & `fish_audio_preprocess-0.2.0/fish_audio_preprocess/utils/loudness_norm.py`

 * *Files identical despite different names*

### Comparing `fish_audio_preprocess-0.1.9/fish_audio_preprocess/utils/polyphonic.yaml` & `fish_audio_preprocess-0.2.0/fish_audio_preprocess/utils/polyphonic.yaml`

 * *Files identical despite different names*

### Comparing `fish_audio_preprocess-0.1.9/fish_audio_preprocess/utils/separate_audio.py` & `fish_audio_preprocess-0.2.0/fish_audio_preprocess/utils/separate_audio.py`

 * *Files identical despite different names*

### Comparing `fish_audio_preprocess-0.1.9/fish_audio_preprocess/utils/slice_audio.py` & `fish_audio_preprocess-0.2.0/fish_audio_preprocess/utils/slice_audio.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,15 +115,15 @@
         frame_length: frame_length of librosa.effects.split
         hop_length: hop_length of librosa.effects.split
     """
 
     output_dir = Path(output_dir)
     output_dir.mkdir(parents=True, exist_ok=True)
 
-    audio, rate = sf.read(str(input_file))
+    audio, rate = librosa.load(str(input_file), sr=None, mono=True)
     for idx, sliced in enumerate(
         slice_audio(
             audio,
             rate,
             min_duration=min_duration,
             max_duration=max_duration,
             pad_silence=pad_silence,
```

### Comparing `fish_audio_preprocess-0.1.9/fish_audio_preprocess/utils/to_ipa.py` & `fish_audio_preprocess-0.2.0/fish_audio_preprocess/utils/to_ipa.py`

 * *Files identical despite different names*

### Comparing `fish_audio_preprocess-0.1.9/pyproject.toml` & `fish_audio_preprocess-0.2.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fish-audio-preprocess"
-version = "0.1.9"
+version = "0.2.0"
 description = "Preprocess audio data"
 authors = ["Lengyue <lengyue@lengyue.me>"]
 license = "Apache"
 
 packages = [{ include = "fish_audio_preprocess" }]
 
 [tool.poetry.dependencies]
```

### Comparing `fish_audio_preprocess-0.1.9/PKG-INFO` & `fish_audio_preprocess-0.2.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fish-audio-preprocess
-Version: 0.1.9
+Version: 0.2.0
 Summary: Preprocess audio data
 License: Apache
 Author: Lengyue
 Author-email: lengyue@lengyue.me
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

