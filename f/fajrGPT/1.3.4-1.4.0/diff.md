# Comparing `tmp/fajrGPT-1.3.4.tar.gz` & `tmp/fajrGPT-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fajrGPT-1.3.4.tar", last modified: Thu Jul  6 15:24:24 2023, max compression
+gzip compressed data, was "fajrGPT-1.4.0.tar", last modified: Sat Jul 22 20:01:52 2023, max compression
```

## Comparing `fajrGPT-1.3.4.tar` & `fajrGPT-1.4.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-07-06 15:24:24.048401 fajrGPT-1.3.4/
--rw-r--r--   0 malek8     (501) staff       (20)     1062 2023-05-15 07:44:33.000000 fajrGPT-1.3.4/LICENSE
--rw-r--r--   0 malek8     (501) staff       (20)     2946 2023-07-06 15:24:24.048261 fajrGPT-1.3.4/PKG-INFO
--rw-r--r--   0 malek8     (501) staff       (20)     2283 2023-06-12 00:59:24.000000 fajrGPT-1.3.4/README.md
-drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-07-06 15:24:24.047282 fajrGPT-1.3.4/fajrGPT/
--rw-r--r--   0 malek8     (501) staff       (20)        0 2023-06-12 01:14:16.000000 fajrGPT-1.3.4/fajrGPT/__init__.py
--rw-r--r--   0 malek8     (501) staff       (20)     1400 2023-07-03 14:08:35.000000 fajrGPT-1.3.4/fajrGPT/quran_metadata.py
--rw-r--r--   0 malek8     (501) staff       (20)    13300 2023-07-06 15:23:08.000000 fajrGPT-1.3.4/fajrGPT/wake.py
-drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-07-06 15:24:24.048104 fajrGPT-1.3.4/fajrGPT.egg-info/
--rw-r--r--   0 malek8     (501) staff       (20)     2946 2023-07-06 15:24:24.000000 fajrGPT-1.3.4/fajrGPT.egg-info/PKG-INFO
--rw-r--r--   0 malek8     (501) staff       (20)      276 2023-07-06 15:24:24.000000 fajrGPT-1.3.4/fajrGPT.egg-info/SOURCES.txt
--rw-r--r--   0 malek8     (501) staff       (20)        1 2023-07-06 15:24:24.000000 fajrGPT-1.3.4/fajrGPT.egg-info/dependency_links.txt
--rw-r--r--   0 malek8     (501) staff       (20)       46 2023-07-06 15:24:24.000000 fajrGPT-1.3.4/fajrGPT.egg-info/entry_points.txt
--rw-r--r--   0 malek8     (501) staff       (20)       54 2023-07-06 15:24:24.000000 fajrGPT-1.3.4/fajrGPT.egg-info/requires.txt
--rw-r--r--   0 malek8     (501) staff       (20)        8 2023-07-06 15:24:24.000000 fajrGPT-1.3.4/fajrGPT.egg-info/top_level.txt
--rw-r--r--   0 malek8     (501) staff       (20)       38 2023-07-06 15:24:24.048440 fajrGPT-1.3.4/setup.cfg
--rw-r--r--   0 malek8     (501) staff       (20)     1129 2023-07-06 15:22:39.000000 fajrGPT-1.3.4/setup.py
+drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-07-22 20:01:52.617955 fajrGPT-1.4.0/
+-rw-r--r--   0 malek8     (501) staff       (20)     1062 2023-05-15 07:44:33.000000 fajrGPT-1.4.0/LICENSE
+-rw-r--r--   0 malek8     (501) staff       (20)     2946 2023-07-22 20:01:52.617698 fajrGPT-1.4.0/PKG-INFO
+-rw-r--r--   0 malek8     (501) staff       (20)     2283 2023-06-12 00:59:24.000000 fajrGPT-1.4.0/README.md
+drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-07-22 20:01:52.615480 fajrGPT-1.4.0/fajrGPT/
+-rw-r--r--   0 malek8     (501) staff       (20)        0 2023-06-12 01:14:16.000000 fajrGPT-1.4.0/fajrGPT/__init__.py
+-rw-r--r--   0 malek8     (501) staff       (20)     1400 2023-07-03 14:08:35.000000 fajrGPT-1.4.0/fajrGPT/quran_metadata.py
+-rw-r--r--   0 malek8     (501) staff       (20)    17026 2023-07-22 19:27:14.000000 fajrGPT-1.4.0/fajrGPT/wake.py
+drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-07-22 20:01:52.617421 fajrGPT-1.4.0/fajrGPT.egg-info/
+-rw-r--r--   0 malek8     (501) staff       (20)     2946 2023-07-22 20:01:52.000000 fajrGPT-1.4.0/fajrGPT.egg-info/PKG-INFO
+-rw-r--r--   0 malek8     (501) staff       (20)      276 2023-07-22 20:01:52.000000 fajrGPT-1.4.0/fajrGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 malek8     (501) staff       (20)        1 2023-07-22 20:01:52.000000 fajrGPT-1.4.0/fajrGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 malek8     (501) staff       (20)       46 2023-07-22 20:01:52.000000 fajrGPT-1.4.0/fajrGPT.egg-info/entry_points.txt
+-rw-r--r--   0 malek8     (501) staff       (20)       54 2023-07-22 20:01:52.000000 fajrGPT-1.4.0/fajrGPT.egg-info/requires.txt
+-rw-r--r--   0 malek8     (501) staff       (20)        8 2023-07-22 20:01:52.000000 fajrGPT-1.4.0/fajrGPT.egg-info/top_level.txt
+-rw-r--r--   0 malek8     (501) staff       (20)       38 2023-07-22 20:01:52.618137 fajrGPT-1.4.0/setup.cfg
+-rw-r--r--   0 malek8     (501) staff       (20)     1129 2023-07-22 19:57:46.000000 fajrGPT-1.4.0/setup.py
```

### Comparing `fajrGPT-1.3.4/LICENSE` & `fajrGPT-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fajrGPT-1.3.4/PKG-INFO` & `fajrGPT-1.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fajrGPT
-Version: 1.3.4
+Version: 1.4.0
 Summary: A Python application to assist in waking up for Fajr prayer by providing 3 interactive verses/explanations from the Quran + ChatGPT explanations accompanied by a soothing Islamic prayer fade-in and fade-out audio file from YouTube.
 Home-page: https://github.com/malekinho8/quran-wake-up
 Author: Malek Ibrahim
 Author-email: shmeek8@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fajrGPT-1.3.4/README.md` & `fajrGPT-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `fajrGPT-1.3.4/fajrGPT/quran_metadata.py` & `fajrGPT-1.4.0/fajrGPT/quran_metadata.py`

 * *Files identical despite different names*

### Comparing `fajrGPT-1.3.4/fajrGPT/wake.py` & `fajrGPT-1.4.0/fajrGPT/wake.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,16 +4,18 @@
 import youtube_dl
 import pygame
 from pydub import AudioSegment
 from threading import Thread
 from fajrGPT.quran_metadata import quran_chapter_to_verse
 import time
 import subprocess
+import requests
 import openai
 import random
+import tempfile
 from tqdm import tqdm
 from Quran_Module import Project_Quran
 
 openai.api_key = os.getenv("OPENAI_API_KEY")
 COMPLETIONS_MODEL = "gpt-3.5-turbo"
 
 @click.command()
@@ -38,23 +40,83 @@
     # Play audio with fade-in effect on a separate thread
     play_audio_thread = Thread(target=play_audio, args=(f'{output}.mp3',))
     play_audio_thread.start()
 
     # display a name of Allah
     get_name_of_allah_and_explanation(names_flag)
 
-    # display the quran verses
-    get_verses_and_explanations(countdown_seconds)
+    # stop the misharay audio once the user has finished reading the name of Allah on a separate thread
+    stop_audio(5)
+
+    # select the quran verses
+    versesQM, verses = select_quran_verse()
+
+    # print the verses selected
+    print(f'\n\nQuran Verses Selected:\n')
+    for verse in verses:
+        print(f'{verse}')
+    
+    # play the audio of the quran verses
+    play_audio_thread = Thread(target=play_quran_verses_audio, args=(verses,0.5))
+    play_audio_thread.start()
+
+    # get the explanations of the quran verses
+    get_explanations(versesQM, verses, countdown_seconds)
 
     # stop the audio once the user has completed reading the verses
     stop_audio()
 
     # return back to the main thread
     play_audio_thread.join()
 
+def play_quran_verses_audio(verses,transition_time=0.5):
+    # convert verses to urls
+    urls = [quran_verse_to_mp3_url(verse) for verse in verses]
+
+    # download the verse audio
+    file_paths = [download_file_and_sleep(url,0.5) for url in urls]
+
+    # concatenate the audio files into one
+    combined_audio_file_name = combine_audio_from_files(file_paths)
+
+    # delete the temporary files
+    for file_path in file_paths:
+        os.remove(file_path)
+
+    # play the audio of the combined quaran verses
+    play_audio(combined_audio_file_name, transition_time)
+
+def combine_audio_from_files(file_paths):
+    # combine the audio files
+    combined_audio = AudioSegment.empty()
+    for file_path in file_paths:
+        combined_audio += AudioSegment.from_mp3(file_path)
+
+    # create a temporary file to store the combined audio
+    temp_file = tempfile.NamedTemporaryFile(suffix='.mp3', delete=False)
+
+    # export the combined audio to the temporary file
+    combined_audio.export(temp_file.name, format='mp3')
+
+    # return the path to the temporary file
+    return temp_file.name
+
+def quran_verse_to_mp3_url(verse):
+    # get the chapter and verse number
+    chapter, verse_number = verse.split(':')
+
+    # convert the numbers to the correct string format
+    chapter = chapter.zfill(3)
+    verse_number = verse_number.zfill(3)
+
+    # get the url of the mp3 file
+    url = f'https://islamicstudies.info/quran/afasy/audio/{chapter}{verse_number}.mp3'
+
+    return url
+
 def convert_to_seconds(time_str):
     # Get the number and the time unit (h/m/s)
     number = float(time_str[:-1])
     unit = time_str[-1].lower()
 
     # Convert to seconds
     if unit == "h":
@@ -150,23 +212,18 @@
         # Get the explanation of the name of Allah
         explanation = query_gpt(prompt)
 
         # print the name of the Allah and the explanation in a nice format
         print(f'\n\n\n\n ---------------- NAME OF ALLAH ---------------- \n')
         print(f'---------------- {name_of_allah_arabic}: {name_of_allah_transliteration} - {name_of_allah_english} ---------------- \n\n')
         print(f'Explanation: {explanation}\n\n\n\n')
-        print(f'When you are ready to begin, press ENTER (wait 10 seconds).')
+        print(f'When you are ready to begin, press ENTER.')
         input()
-        time.sleep(10)
-
-def get_verses_and_explanations(countdown_seconds):
-    # Get the verses
-    verses_Quran_Module, verses  = select_quran_verse()
-    # print(f"Verse 1:\n{verses}")
 
+def get_explanations(verses_Quran_Module,verses,countdown_seconds):
     # Depending on the length of the countdown, select the number of verses to display
     if countdown_seconds < 3600: # less than 1 hour
         verses_Quran_Module = verses_Quran_Module[0:1] # only display the first verse
         verses = verses[0:1]
     elif countdown_seconds > 3600 and countdown_seconds < 7200: # between 1 and 2 hours
         verses_Quran_Module = verses_Quran_Module[0:2] # only display the first two verses
         verses = verses[0:2]
@@ -187,24 +244,26 @@
             I want you to act as Sheikh Hamza Yusuf. You are an influential Islamic scholar, who has a profound understanding of the Qur'an, Hadith, and various branches of Islamic Jurisprudence. 
             You are deeply conversant with the various cultural, historical, and philosophical contexts of Islamic thought. You are committed to promoting peace, understanding, and the intellectual tradition of Islam. 
             I know that you are just an AI, but I don't want you to say that at the beginning, just emulate this description to the best of your ability. My first request is as follows:
 
             First please give some brief context about Chapter {chapter_number} from the Qur'an. Then, to the best of your ability, explain the meaning of the verse below. 
             I understand you are just an AI language model, but please remember I don't want you to state or acknowledge that, just try to interpret the possible meaning of the verse given. \n\n Verse: {verse_text} \n\n Explanation:
             """
+            explanation = query_gpt(prompt2)
         else:
+            concatenated_explanations = '\n\n'.join(explanations)
             prompt2 = f"""
             I want you to act as Sheikh Hamza Yusuf. You are an influential Islamic scholar, who has a profound understanding of the Qur'an, Hadith, and various branches of Islamic Jurisprudence. 
             You are deeply conversant with the various cultural, historical, and philosophical contexts of Islamic thought. You are committed to promoting peace, understanding, and the intellectual tradition of Islam. 
             I know that you are just an AI, but I don't want you to say that at the beginning, just emulate this description to the best of your ability. My first request is as follows:
 
             To the best of your ability, explain the meaning of the verse below. 
-            I understand you are just an AI language model, but please remember I don't want you to state or acknowledge that, just try to emulate Sheikh Hamza Yusuf and interpret the possible meaning of the given verse. \n\n Verse: {verse_text} \n\n Explanation:
+            I understand you are just an AI language model, but please remember I don't want you to state or acknowledge that, just try to emulate Sheikh Hamza Yusuf and interpret the possible meaning of the given verse. \n\n Verse: {verse_text} \n\n Context: {concatenated_explanations} \n\n Explanation:
             """
-        explanation = query_gpt(prompt2)
+            explanation = query_gpt(prompt2)
         verse_texts.append(verse_text)
         explanations.append(explanation)
     
     # begin the interactive session
     for verse_text, explanation, verse in zip(verse_texts, explanations, verses):
         print(f'\n\n\n\n\n\n ------------------ FIRST VERSE ------------------') if verse == verses[0] else None
         print(f'\n\n{verse}:\n{verse_text} \n\n ------------------ \n\n When you are ready to see the explanaton, press Enter.')
@@ -215,14 +274,22 @@
         if verse != verses[-1]:
             print(f'{explanation} \n\n ------------------ \n\n When you are ready to proceed to the next verse, press Enter (20 second timer).')
         else:
             print(f'{explanation} \n\n ------------------ \n\n When you are ready to stop the alarm, press Enter (20 second timer).')
         time.sleep(20) # Wait for the user to press Enter, but not before 20 seconds have passed
         input() # wait for the user to press Enter
 
+def get_verses_and_explanations(countdown_seconds):
+    # Get the verses
+    verses_Quran_Module, verses  = select_quran_verse()
+    # print(f"Verse 1:\n{verses}")
+
+    # Get the explanations
+    get_explanations(verses_Quran_Module,verses,countdown_seconds)
+
 def select_quran_verse():
     # List of surah numbers
     surahs = list(quran_chapter_to_verse.keys())
 
     # Number of verses in each surah, this is just a placeholder
     # Please replace this with the actual number of verses in each surah
     verses_in_surah = list(quran_chapter_to_verse.values())
@@ -258,65 +325,105 @@
                 **COMPLETIONS_API_PARAMS
             )
 
     return response['choices'][0]['message']['content']
 
 def gradually_change_volume(start_volume, end_volume, duration):
     # Compute the number of steps and the change in volume per step
-    steps = duration
+    steps = int(duration * 100)  # Multiply by 100 to allow for hundredths of seconds
+    delay = 0.01  # Delay for each step
+
+    max_steps = 10000  # Maximum number of steps
+
+    # If steps are more than maximum, adjust steps and delay
+    if steps > max_steps:
+        steps = max_steps
+        delay = duration / max_steps
+
     delta_volume = (end_volume - start_volume) / steps
 
     # Set the initial volume
     pygame.mixer.music.set_volume(start_volume)
 
     # Gradually change the volume
     for i in range(steps):
-        # Wait for 1 second
-        time.sleep(1)
+        # Wait for the calculated delay
+        time.sleep(delay)
 
         # Change the volume
         new_volume = start_volume + i * delta_volume
         pygame.mixer.music.set_volume(new_volume)
 
         # If the stop_audio function has been called, break the loop
         if stop_audio_called:
             print("Stopping volume change due to stop_audio being called")
             break
 
-def play_audio(file_path):
+def play_audio(file_path_or_url, transition_time=900):
     global stop_audio_called
     stop_audio_called = False
+    file_path = ''
+
+    # Check if file_path_or_url is URL
+    if file_path_or_url.startswith('http'):
+        # Download the file and get the path
+        file_path = download_file(file_path_or_url)
+    else:
+        file_path = file_path_or_url
 
     # Initialize pygame mixer
     pygame.mixer.init()
 
     # Load the audio file
     pygame.mixer.music.load(file_path)
 
     # Start playing the audio with volume 0
     pygame.mixer.music.set_volume(0.0)
     pygame.mixer.music.play()
 
     # Gradually increase the volume over 15 minutes in a separate thread
-    gradually_change_volume(0.0, 1.0, 900)
+    gradually_change_volume(0.0, 1.0, transition_time)
 
     # Loop the audio until the stop_audio function is called
     while not stop_audio_called:
         if not pygame.mixer.music.get_busy():
             # The music has finished, restart it
             pygame.mixer.music.play()
-        time.sleep(1)    
+        time.sleep(1)
+
+    # Delete the file if it was downloaded
+    if file_path_or_url.startswith('http'):
+        os.remove(file_path)    
 
-def stop_audio():
+def stop_audio(transition_time=10):
     global stop_audio_called
     stop_audio_called = True # stop the audio in the other thread
     time.sleep(1)
     stop_audio_called = False # reset back to False to allow volume to decrease
-    gradually_change_volume(pygame.mixer.music.get_volume(), 0.0, 10)
+    gradually_change_volume(pygame.mixer.music.get_volume(), 0.0, transition_time)
 
     # Stop the audio completely
     stop_audio_called = True
     pygame.mixer.music.stop()
 
+def download_file(url):
+    """Download file from URL and return the path to the file"""
+    headers = {
+        'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/58.0.3029.110 Safari/537.3'
+    }
+    response = requests.get(url, headers=headers, stream=True)
+    file = tempfile.NamedTemporaryFile(delete=False)
+    file_path = file.name
+    with open(file_path, 'wb') as fd:
+        for chunk in response.iter_content(chunk_size=1024):
+            fd.write(chunk)
+    return file_path
+
+def download_file_and_sleep(url, time_to_sleep=0.5):
+    result = download_file(url)
+    time.sleep(time_to_sleep)
+    return result
+
+
 if __name__ == "__main__":
     main()
```

### Comparing `fajrGPT-1.3.4/fajrGPT.egg-info/PKG-INFO` & `fajrGPT-1.4.0/fajrGPT.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fajrGPT
-Version: 1.3.4
+Version: 1.4.0
 Summary: A Python application to assist in waking up for Fajr prayer by providing 3 interactive verses/explanations from the Quran + ChatGPT explanations accompanied by a soothing Islamic prayer fade-in and fade-out audio file from YouTube.
 Home-page: https://github.com/malekinho8/quran-wake-up
 Author: Malek Ibrahim
 Author-email: shmeek8@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fajrGPT-1.3.4/setup.py` & `fajrGPT-1.4.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="fajrGPT",
-    version="1.3.4",
+    version="1.4.0",
     author="Malek Ibrahim",
     author_email="shmeek8@gmail.com",
     description=("A Python application to assist in waking up for Fajr prayer "
                  "by providing 3 interactive verses/explanations from the Quran + ChatGPT explanations "
                  "accompanied by a soothing Islamic prayer fade-in and fade-out audio file from YouTube."),
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
```

