# Comparing `tmp/selenium-recaptcha-solver-1.8.3.tar.gz` & `tmp/selenium-recaptcha-solver-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "selenium-recaptcha-solver-1.8.3.tar", last modified: Mon Jun 19 11:30:09 2023, max compression
+gzip compressed data, was "selenium-recaptcha-solver-1.9.0.tar", last modified: Sun Jul  9 16:51:38 2023, max compression
```

## Comparing `selenium-recaptcha-solver-1.8.3.tar` & `selenium-recaptcha-solver-1.9.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 11:30:09.397650 selenium-recaptcha-solver-1.8.3/
--rw-rw-rw-   0        0        0     1095 2023-01-08 17:39:18.000000 selenium-recaptcha-solver-1.8.3/LICENSE
--rw-rw-rw-   0        0        0     3375 2023-06-19 11:30:09.397650 selenium-recaptcha-solver-1.8.3/PKG-INFO
--rw-rw-rw-   0        0        0     2949 2023-05-22 08:12:23.000000 selenium-recaptcha-solver-1.8.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-19 11:30:09.390397 selenium-recaptcha-solver-1.8.3/selenium_recaptcha_solver/
--rw-rw-rw-   0        0        0      170 2023-02-21 21:45:09.000000 selenium-recaptcha-solver-1.8.3/selenium_recaptcha_solver/__init__.py
--rw-rw-rw-   0        0        0      971 2023-04-12 10:28:50.000000 selenium-recaptcha-solver-1.8.3/selenium_recaptcha_solver/delay_config.py
--rw-rw-rw-   0        0        0       48 2023-01-08 17:39:18.000000 selenium-recaptcha-solver-1.8.3/selenium_recaptcha_solver/exceptions.py
--rw-rw-rw-   0        0        0     7838 2023-06-19 11:19:34.000000 selenium-recaptcha-solver-1.8.3/selenium_recaptcha_solver/services.py
--rw-rw-rw-   0        0        0     8889 2023-06-04 18:41:48.000000 selenium-recaptcha-solver-1.8.3/selenium_recaptcha_solver/solver.py
-drwxrwxrwx   0        0        0        0 2023-06-19 11:30:09.394645 selenium-recaptcha-solver-1.8.3/selenium_recaptcha_solver.egg-info/
--rw-rw-rw-   0        0        0     3375 2023-06-19 11:30:09.000000 selenium-recaptcha-solver-1.8.3/selenium_recaptcha_solver.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      482 2023-06-19 11:30:09.000000 selenium-recaptcha-solver-1.8.3/selenium_recaptcha_solver.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 11:30:09.000000 selenium-recaptcha-solver-1.8.3/selenium_recaptcha_solver.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       80 2023-06-19 11:30:09.000000 selenium-recaptcha-solver-1.8.3/selenium_recaptcha_solver.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2023-06-19 11:30:09.000000 selenium-recaptcha-solver-1.8.3/selenium_recaptcha_solver.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-19 11:30:09.397650 selenium-recaptcha-solver-1.8.3/setup.cfg
--rw-rw-rw-   0        0        0      769 2023-06-19 11:28:41.000000 selenium-recaptcha-solver-1.8.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-19 11:30:09.395651 selenium-recaptcha-solver-1.8.3/tests/
--rw-rw-rw-   0        0        0     1220 2023-06-19 11:24:15.000000 selenium-recaptcha-solver-1.8.3/tests/test_api.py
+drwxrwxrwx   0        0        0        0 2023-07-09 16:51:38.393985 selenium-recaptcha-solver-1.9.0/
+-rw-rw-rw-   0        0        0     1095 2023-01-08 17:39:18.000000 selenium-recaptcha-solver-1.9.0/LICENSE
+-rw-rw-rw-   0        0        0     3375 2023-07-09 16:51:38.393985 selenium-recaptcha-solver-1.9.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2949 2023-05-22 08:12:23.000000 selenium-recaptcha-solver-1.9.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-09 16:51:38.386983 selenium-recaptcha-solver-1.9.0/selenium_recaptcha_solver/
+-rw-rw-rw-   0        0        0      170 2023-02-21 21:45:09.000000 selenium-recaptcha-solver-1.9.0/selenium_recaptcha_solver/__init__.py
+-rw-rw-rw-   0        0        0      971 2023-04-12 10:28:50.000000 selenium-recaptcha-solver-1.9.0/selenium_recaptcha_solver/delay_config.py
+-rw-rw-rw-   0        0        0       48 2023-01-08 17:39:18.000000 selenium-recaptcha-solver-1.9.0/selenium_recaptcha_solver/exceptions.py
+-rw-rw-rw-   0        0        0     1649 2023-07-05 09:44:56.000000 selenium-recaptcha-solver-1.9.0/selenium_recaptcha_solver/services.py
+-rw-rw-rw-   0        0        0     9177 2023-07-06 10:33:47.000000 selenium-recaptcha-solver-1.9.0/selenium_recaptcha_solver/solver.py
+drwxrwxrwx   0        0        0        0 2023-07-09 16:51:38.390983 selenium-recaptcha-solver-1.9.0/selenium_recaptcha_solver.egg-info/
+-rw-rw-rw-   0        0        0     3375 2023-07-09 16:51:38.000000 selenium-recaptcha-solver-1.9.0/selenium_recaptcha_solver.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      482 2023-07-09 16:51:38.000000 selenium-recaptcha-solver-1.9.0/selenium_recaptcha_solver.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-09 16:51:38.000000 selenium-recaptcha-solver-1.9.0/selenium_recaptcha_solver.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       80 2023-07-09 16:51:38.000000 selenium-recaptcha-solver-1.9.0/selenium_recaptcha_solver.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2023-07-09 16:51:38.000000 selenium-recaptcha-solver-1.9.0/selenium_recaptcha_solver.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-09 16:51:38.394985 selenium-recaptcha-solver-1.9.0/setup.cfg
+-rw-rw-rw-   0        0        0      769 2023-07-09 16:51:08.000000 selenium-recaptcha-solver-1.9.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-09 16:51:38.391985 selenium-recaptcha-solver-1.9.0/tests/
+-rw-rw-rw-   0        0        0     1220 2023-07-09 06:57:49.000000 selenium-recaptcha-solver-1.9.0/tests/test_api.py
```

### Comparing `selenium-recaptcha-solver-1.8.3/LICENSE` & `selenium-recaptcha-solver-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `selenium-recaptcha-solver-1.8.3/PKG-INFO` & `selenium-recaptcha-solver-1.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: selenium-recaptcha-solver
-Version: 1.8.3
+Version: 1.9.0
 Home-page: https://github.com/thicccat688/selenium-recaptcha-solver
 Download-URL: https://pypi.org/project/selenium-recaptcha-solver
 Author: Tomás Perestrelo
 Author-email: tomasperestrelo21@gmail.com
 License: MIT
 Keywords: python,captcha,speech recognition,selenium,web automation
 Description-Content-Type: text/markdown
```

### Comparing `selenium-recaptcha-solver-1.8.3/README.md` & `selenium-recaptcha-solver-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `selenium-recaptcha-solver-1.8.3/selenium_recaptcha_solver/delay_config.py` & `selenium-recaptcha-solver-1.9.0/selenium_recaptcha_solver/delay_config.py`

 * *Files identical despite different names*

### Comparing `selenium-recaptcha-solver-1.8.3/selenium_recaptcha_solver/solver.py` & `selenium-recaptcha-solver-1.9.0/selenium_recaptcha_solver/solver.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from selenium.webdriver.common.by import By
 from selenium.webdriver.support import expected_conditions as ec
 from selenium.webdriver.remote.webelement import WebElement
 from selenium.webdriver.chrome.webdriver import WebDriver
 from selenium.webdriver.support.ui import WebDriverWait
 from selenium.common.exceptions import TimeoutException
 from pydub import AudioSegment
-from typing import Union, Optional
+from typing import Optional
 import speech_recognition as sr
 import tempfile
 import requests
 import random
 import uuid
 import time
 import os
@@ -23,27 +23,30 @@
 
 
 class RecaptchaSolver:
     def __init__(
             self,
             driver: WebDriver,
             service: Service = DEFAULT_SERVICE,
+            service_language: str = 'en-US',
             delay_config: Optional[DelayConfig] = None,
     ):
         """
         :param driver: Selenium web driver to use to solve the captcha
         :param service: service to use for speech recognition (defaults to ``GoogleService``).
             See the ``services`` module for available services.
+        :param service_language: Language to use when recognizing speech to solve reCAPTCHA challenge (en-US by default for American English recognition)
         :param delay_config: if set, use the given configuration for delays between UI interactions.
             See :class:`DelayConfig`, and also :class:`StandardDelayConfig`, which provides a standard implementation that should work in many cases.
         """
 
         self._driver = driver
         self._service = service
         self._delay_config = delay_config
+        self._language = service_language
 
         # Initialise speech recognition API object
         self._recognizer = sr.Recognizer()
 
     def click_recaptcha_v2(self, iframe: WebElement, by_selector: Optional[str] = None) -> None:
         """
         Click the "I'm not a robot" checkbox and then solve a reCAPTCHA v2 challenge.
@@ -52,24 +55,24 @@
 
         :param iframe: web element for inline frame of reCAPTCHA to solve
         :param by_selector: By selector to use to find the iframe, if ``iframe`` is a string
         :raises selenium.common.exceptions.TimeoutException: if a timeout occurred while waiting
         """
 
         if isinstance(iframe, str):
-            WebDriverWait(self._driver, 150).until(
+            WebDriverWait(self._driver, 10).until(
                 ec.frame_to_be_available_and_switch_to_it((by_selector, iframe)))
 
         else:
             self._driver.switch_to.frame(iframe)
 
         checkbox = self._wait_for_element(
             by='id',
             locator='recaptcha-anchor',
-            timeout=150,
+            timeout=10,
         )
 
         self._js_click(checkbox)
 
         if checkbox.get_attribute('aria-checked') == 'true':
             return
 
@@ -88,15 +91,15 @@
 
     def solve_recaptcha_v2_challenge(self, iframe: WebElement) -> None:
         """
         Solve a reCAPTCHA v2 challenge that has already appeared.
 
         Call this method directly on web pages with the "invisible reCAPTCHA" badge. See <https://developers.google.com/recaptcha/docs/versions> for details of how this works.
 
-        :param iframe: web element for inline frame of reCAPTCHA to solve
+        :param iframe: Web element for inline frame of reCAPTCHA to solve
         :raises selenium.common.exceptions.TimeoutException: if a timeout occurred while waiting
         """
 
         self._driver.switch_to.frame(iframe)
 
         # If the captcha image audio is available, locate it. Otherwise, skip to the next line of code.
 
@@ -106,15 +109,15 @@
                 locator='//*[@id="recaptcha-audio-button"]',
                 timeout=1,
             ).click()
 
         except TimeoutException:
             pass
 
-        self._solve_audio_challenge()
+        self._solve_audio_challenge(self._language)
 
         # Locate verify button and click it via JavaScript
         verify_button = self._wait_for_element(
             by=By.ID,
             locator='recaptcha-verify-button',
             timeout=5,
         )
@@ -127,15 +130,15 @@
         try:
             self._wait_for_element(
                 by=By.XPATH,
                 locator='//div[normalize-space()="Multiple correct solutions required - please solve more."]',
                 timeout=1,
             )
 
-            self._solve_audio_challenge()
+            self._solve_audio_challenge(self._language)
 
             # Locate verify button again to avoid stale element reference and click it via JavaScript
             second_verify_button = self._wait_for_element(
                 by=By.ID,
                 locator='recaptcha-verify-button',
                 timeout=5,
             )
@@ -143,15 +146,15 @@
             self._js_click(second_verify_button)
 
         except TimeoutException:
             pass
 
         self._driver.switch_to.parent_frame()
 
-    def _solve_audio_challenge(self) -> None:
+    def _solve_audio_challenge(self, language: str) -> None:
         try:
             # Locate audio challenge download link
             download_link: WebElement = self._wait_for_element(
                 by=By.CLASS_NAME,
                 locator='rc-audiochallenge-tdownload-link',
                 timeout=10,
             )
@@ -183,15 +186,15 @@
         # Disable dynamic energy threshold to avoid failed reCAPTCHA audio transcription due to static noise
         self._recognizer.dynamic_energy_threshold = False
 
         with sr.AudioFile(wav_file) as source:
             audio = self._recognizer.listen(source)
 
             try:
-                recognized_text = self._service.recognize(self._recognizer, audio)
+                recognized_text = self._service.recognize(self._recognizer, audio, language)
 
             except sr.UnknownValueError:
                 raise RecaptchaException('Speech recognition API could not understand audio, try again')
 
         # Clean up all temporary files
         for path in tmp_files:
             if os.path.exists(path):
```

### Comparing `selenium-recaptcha-solver-1.8.3/selenium_recaptcha_solver.egg-info/PKG-INFO` & `selenium-recaptcha-solver-1.9.0/selenium_recaptcha_solver.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: selenium-recaptcha-solver
-Version: 1.8.3
+Version: 1.9.0
 Home-page: https://github.com/thicccat688/selenium-recaptcha-solver
 Download-URL: https://pypi.org/project/selenium-recaptcha-solver
 Author: Tomás Perestrelo
 Author-email: tomasperestrelo21@gmail.com
 License: MIT
 Keywords: python,captcha,speech recognition,selenium,web automation
 Description-Content-Type: text/markdown
```

### Comparing `selenium-recaptcha-solver-1.8.3/setup.py` & `selenium-recaptcha-solver-1.9.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='selenium-recaptcha-solver',
-    version='1.8.3',
+    version='1.9.0',
     license='MIT',
     author='Tomás Perestrelo',
     author_email='tomasperestrelo21@gmail.com',
     packages=find_packages(exclude=('tests*', 'testing*')),
     url='https://github.com/thicccat688/selenium-recaptcha-solver',
     download_url='https://pypi.org/project/selenium-recaptcha-solver',
     keywords='python, captcha, speech recognition, selenium, web automation',
```

### Comparing `selenium-recaptcha-solver-1.8.3/tests/test_api.py` & `selenium-recaptcha-solver-1.9.0/tests/test_api.py`

 * *Files identical despite different names*

