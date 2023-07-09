# Comparing `tmp/doubledate-0.0.8.tar.gz` & `tmp/doubledate-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "doubledate-0.0.8.tar", last modified: Mon Jan 17 20:51:56 2022, max compression
+gzip compressed data, was "doubledate-0.0.9.tar", last modified: Wed Apr  6 22:24:50 2022, max compression
```

## Comparing `doubledate-0.0.8.tar` & `doubledate-0.0.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 dschenck   (501) staff       (20)        0 2022-01-17 20:51:56.579725 doubledate-0.0.8/
--rw-r--r--   0 dschenck   (501) staff       (20)      732 2022-01-17 20:51:56.579517 doubledate-0.0.8/PKG-INFO
--rw-r--r--   0 dschenck   (501) staff       (20)      259 2022-01-14 08:50:25.000000 doubledate-0.0.8/README.md
-drwxr-xr-x   0 dschenck   (501) staff       (20)        0 2022-01-17 20:51:56.577480 doubledate-0.0.8/doubledate/
--rw-r--r--   0 dschenck   (501) staff       (20)      595 2022-01-17 16:03:31.000000 doubledate-0.0.8/doubledate/__init__.py
--rw-r--r--   0 dschenck   (501) staff       (20)    45605 2022-01-17 16:36:15.000000 doubledate-0.0.8/doubledate/calendar.py
--rw-r--r--   0 dschenck   (501) staff       (20)      485 2022-01-14 16:04:10.000000 doubledate-0.0.8/doubledate/constants.py
--rw-r--r--   0 dschenck   (501) staff       (20)    36420 2022-01-15 15:48:36.000000 doubledate-0.0.8/doubledate/utils.py
-drwxr-xr-x   0 dschenck   (501) staff       (20)        0 2022-01-17 20:51:56.578413 doubledate-0.0.8/doubledate.egg-info/
--rw-r--r--   0 dschenck   (501) staff       (20)      732 2022-01-17 20:51:56.000000 doubledate-0.0.8/doubledate.egg-info/PKG-INFO
--rw-r--r--   0 dschenck   (501) staff       (20)      338 2022-01-17 20:51:56.000000 doubledate-0.0.8/doubledate.egg-info/SOURCES.txt
--rw-r--r--   0 dschenck   (501) staff       (20)        1 2022-01-17 20:51:56.000000 doubledate-0.0.8/doubledate.egg-info/dependency_links.txt
--rw-r--r--   0 dschenck   (501) staff       (20)       33 2022-01-17 20:51:56.000000 doubledate-0.0.8/doubledate.egg-info/requires.txt
--rw-r--r--   0 dschenck   (501) staff       (20)       17 2022-01-17 20:51:56.000000 doubledate-0.0.8/doubledate.egg-info/top_level.txt
--rw-r--r--   0 dschenck   (501) staff       (20)       38 2022-01-17 20:51:56.579781 doubledate-0.0.8/setup.cfg
--rw-r--r--   0 dschenck   (501) staff       (20)      687 2022-01-14 08:49:28.000000 doubledate-0.0.8/setup.py
-drwxr-xr-x   0 dschenck   (501) staff       (20)        0 2022-01-17 20:51:56.579080 doubledate-0.0.8/tests/
--rw-r--r--   0 dschenck   (501) staff       (20)        0 2021-11-11 12:53:05.000000 doubledate-0.0.8/tests/__init__.py
--rw-r--r--   0 dschenck   (501) staff       (20)    18580 2022-01-17 20:41:43.000000 doubledate-0.0.8/tests/test_calendar.py
--rw-r--r--   0 dschenck   (501) staff       (20)    16384 2021-12-05 17:13:16.000000 doubledate-0.0.8/tests/test_utils.py
+drwxr-xr-x   0 dschenck   (501) staff       (20)        0 2022-04-06 22:24:50.530995 doubledate-0.0.9/
+-rw-r--r--   0 dschenck   (501) staff       (20)      732 2022-04-06 22:24:50.530779 doubledate-0.0.9/PKG-INFO
+-rw-r--r--   0 dschenck   (501) staff       (20)      259 2022-01-14 08:50:25.000000 doubledate-0.0.9/README.md
+drwxr-xr-x   0 dschenck   (501) staff       (20)        0 2022-04-06 22:24:50.529470 doubledate-0.0.9/doubledate/
+-rw-r--r--   0 dschenck   (501) staff       (20)      595 2022-01-17 16:03:31.000000 doubledate-0.0.9/doubledate/__init__.py
+-rw-r--r--   0 dschenck   (501) staff       (20)    47193 2022-04-06 22:01:49.000000 doubledate-0.0.9/doubledate/calendar.py
+-rw-r--r--   0 dschenck   (501) staff       (20)      485 2022-01-14 16:04:10.000000 doubledate-0.0.9/doubledate/constants.py
+-rw-r--r--   0 dschenck   (501) staff       (20)    36420 2022-01-15 15:48:36.000000 doubledate-0.0.9/doubledate/utils.py
+drwxr-xr-x   0 dschenck   (501) staff       (20)        0 2022-04-06 22:24:50.530116 doubledate-0.0.9/doubledate.egg-info/
+-rw-r--r--   0 dschenck   (501) staff       (20)      732 2022-04-06 22:24:50.000000 doubledate-0.0.9/doubledate.egg-info/PKG-INFO
+-rw-r--r--   0 dschenck   (501) staff       (20)      338 2022-04-06 22:24:50.000000 doubledate-0.0.9/doubledate.egg-info/SOURCES.txt
+-rw-r--r--   0 dschenck   (501) staff       (20)        1 2022-04-06 22:24:50.000000 doubledate-0.0.9/doubledate.egg-info/dependency_links.txt
+-rw-r--r--   0 dschenck   (501) staff       (20)       33 2022-04-06 22:24:50.000000 doubledate-0.0.9/doubledate.egg-info/requires.txt
+-rw-r--r--   0 dschenck   (501) staff       (20)       17 2022-04-06 22:24:50.000000 doubledate-0.0.9/doubledate.egg-info/top_level.txt
+-rw-r--r--   0 dschenck   (501) staff       (20)       38 2022-04-06 22:24:50.531051 doubledate-0.0.9/setup.cfg
+-rw-r--r--   0 dschenck   (501) staff       (20)      687 2022-04-06 22:24:48.000000 doubledate-0.0.9/setup.py
+drwxr-xr-x   0 dschenck   (501) staff       (20)        0 2022-04-06 22:24:50.530482 doubledate-0.0.9/tests/
+-rw-r--r--   0 dschenck   (501) staff       (20)        0 2021-11-11 12:53:05.000000 doubledate-0.0.9/tests/__init__.py
+-rw-r--r--   0 dschenck   (501) staff       (20)    18583 2022-04-06 21:31:45.000000 doubledate-0.0.9/tests/test_calendar.py
+-rw-r--r--   0 dschenck   (501) staff       (20)    16384 2021-12-05 17:13:16.000000 doubledate-0.0.9/tests/test_utils.py
```

### Comparing `doubledate-0.0.8/PKG-INFO` & `doubledate-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doubledate
-Version: 0.0.8
+Version: 0.0.9
 Summary: A calendar wrapper
 Home-page: https://github.com/dschenck/doubledate
 Author: david.schenck@outlook.com
 Author-email: david.schenck@outlook.com
 License: UNKNOWN
 Description: [![Documentation Status](https://readthedocs.org/projects/doubledate/badge/?version=latest)](https://doubledate.readthedocs.io/en/latest/?badge=latest)
```

### Comparing `doubledate-0.0.8/doubledate/__init__.py` & `doubledate-0.0.9/doubledate/__init__.py`

 * *Files identical despite different names*

### Comparing `doubledate-0.0.8/doubledate/calendar.py` & `doubledate-0.0.9/doubledate/calendar.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,26 +5,35 @@
 import doubledate.utils as utils
 import doubledate.constants as constants
 
 
 class BD:
     """
     Business day
+
+    Parameters
+    ----------
+    index : int
+        day of the frequency
+    frequency : str
+        one of 'D','W','M','Q','H' or 'Y'
+    base : 0 (default), 1
+        whether to consider the index 1-based or 0-based 
     """
 
     def __init__(self, index: int, frequency: str = "M", *, base: int = 0):
         if not isinstance(index, int):
             raise TypeError(
                 f"Expected index to be an integer, received {type(index).__name__}"
             )
         self.index = index
 
-        if frequency not in ["W", "M", "Q", "H", "Y"]:
+        if frequency not in ["D", "W", "M", "Q", "H", "Y"]:
             raise ValueError(
-                f"Expected frequency to be one of 'W','M','Q','H' or 'Y', received '{frequency}'"
+                f"Expected frequency to be one of 'D','W','M','Q','H' or 'Y', received '{frequency}'"
             )
         self.frequency = frequency
 
         if base not in (0, 1):
             raise ValueError(f"Expected base to be one of 0 or 1, received {base}")
         self.base = base
 
@@ -49,14 +58,17 @@
             handling policy for periods the n'th business day is not defined
 
         Returns
         -------
         Calendar
             Calendar containing the n'th business day each frequency
         """
+        if self.frequency == "D":
+            return calendar
+
         dates = []
         for subcal in calendar.resample(self.frequency):
             try:
                 dates.append(subcal[self.index - self.base])
             except Exception as e:
                 if onerror == "raise":
                     raise e
@@ -786,30 +798,30 @@
         Parameters
         ----------
         grouper : str, callable
             the criterion to group dates by
 
         Returns
         -------
-        :class:`doubledate.calendar.Grouper`
+        :class:`doubledate.calendar.Collection`
             Collection of calendars    
 
         Example
         -------
         Group dates by month
 
         >>> calendar = Calendar(dates)
         >>> calendar.groupby("M")
-        <doubledate.Grouper at 0x7fd0fa52c2e0>
+        <doubledate.Collection at 0x7fd0fa52c2e0>
 
         Group dates in half months
 
         >>> calendar = Calendar(dates)
         >>> calendar.groupby(lambda date: (date.year, date.month, date.day < 15))
-        <doubledate.Grouper at 0x7fd0fa52c2e0>
+        <doubledate.Collection at 0x7fd0fa52c2e0>
 
         """
         if isinstance(grouper, str):
             if grouper == "W":
                 return self.groupby(lambda date: (date.year, date.isocalendar()[1]))
             elif grouper == "M":
                 return self.groupby(lambda date: (date.year, date.month))
@@ -823,15 +835,15 @@
                 f"Expected one of 'W', 'M', 'Q', 'H' or 'Y'; '{grouper}' given"
             )
 
         if callable(grouper):
             calendars = collections.defaultdict(lambda: [])
             for date in self:
                 calendars[grouper(date)].append(date)
-            return Grouper([Calendar(dates) for dates in calendars.values()])
+            return Collection([Calendar(dates) for dates in calendars.values()])
 
         raise ValueError(f"Expected string or function, received '{grouper}'")
 
     def resample(self, grouper):
         """
         Alias for :class:`doubledate.Calendar.groupby`
         """
@@ -858,31 +870,31 @@
         starting : BD
             the business day on which to split (with side :code:`left`)
         ending : BD
             the business day on which to split (with side :code:`right`)
 
         Returns
         -------
-        Grouper
+        Collection
             The collection of calendars each starting or ending 
             on the given business day
 
         Example
         -------
         Split the calendar on the 10th business day each month
 
         >>> from doubledate import BD
         >>> calendar = Calendar(dates)
         >>> calendar.split(BD(10, "M"))
-        <doubledate.Grouper at 0x7fd0fa52c2e0>
+        <doubledate.Collection at 0x7fd0fa52c2e0>
 
         Split the calendar on the penultimate day each quarter
 
         >>> calendar.split(BD(-2, "Y"))
-        <doubledate.Grouper at 0x7fd0fa52c2e0>
+        <doubledate.Collection at 0x7fd0fa52c2e0>
 
         See also
         --------
         Calendar.groupby
             Split the calendar on a criteria
         
         """
@@ -902,15 +914,15 @@
         calendars = collections.defaultdict(lambda: [])
         for date in self:
             try:
                 calendars[splitdays.asof(date, side)].append(date)
             except:
                 pass
 
-        return Grouper([Calendar(calendar) for calendar in calendars.values()])
+        return Collection([Calendar(calendar) for calendar in calendars.values()])
 
     def fa(self, date: datetime.date, default=constants.RAISE) -> datetime.date:
         """
         Returns the first date strictly after ("first-after", or "fa")
 
         Parameters
         ----------
@@ -1309,27 +1321,64 @@
         for i in range(self.index(date), len(self)):
             if self.__dates__[i].year == date.year:
                 continue
             return self.__dates__[i - 1]
         return self.__dates__[i]
 
 
-class Grouper:
+class Collection:
     """
-    Collection of calendars
+    Collection of calendars. 
+
+    Collections are normally generated from splitting a Calendar in several periods 
+    via resampling or grouping
+
+    Example
+    -------
+    .. code-block::
+
+        >>> import datetime
+        >>> import doubledate as dtwo
+
+        >>> holidays = [
+        ...     datetime.date(2022, 1, 17), 
+        ...     datetime.date(2022, 5, 30), 
+        ...     datetime.date(2022, 6, 4), 
+        ...     datetime.date(2022, 9, 5), 
+        ...     datetime.date(2022, 11, 11), 
+        ...     datetime.date(2022, 12, 24),
+        ...     datetime.date(2022, 12, 26)
+        ... ]
+
+        >>> calendar = dtwo.Calendar(holidays).inverse().weekdays()
+        >>> calendar
+        <doubledate.Calendar>
+
+        >>> calendar.resample("M") #split the calendar by month
+        <doubledate.Collection>
+
+        >>> calendar.resample("M").nth(10, base=1) #get the 10th business day each month
+        <doubledate.Calendar>
+
     """
 
     def __init__(self, calendars):
+        """
+        Parameters
+        ----------
+        calendars : iterable
+            list of Calendar instances
+        """
         if not all([isinstance(calendar, Calendar) for calendar in calendars]):
             raise TypeError("Expected a list of calendar objects")
         self.calendars = list(calendars)
 
     def first(self, onerror="raise") -> Calendar:
         """
-        Returns a calendar with the first date each period
+        Returns a calendar with the first date each period in the collection
 
         Allowed values for the onerror parameter: 
             - 'skip' to skip empty calendars
             - 'raise' to raise an error
 
         Parameters
         ----------
@@ -1340,15 +1389,15 @@
         -------
         Calendar
         """
         return self.apply(lambda period: period[0], onerror=onerror).combine()
 
     def last(self, onerror="raise") -> Calendar:
         """
-        Returns a calendar with the last date each period
+        Returns a calendar with the last date each period in the collection
 
         Allowed values for the onerror parameter: 
             - 'skip' to skip empty calendars
             - 'raise' to raise an error
 
         Parameters
         ----------
@@ -1359,15 +1408,15 @@
         -------
         Calendar
         """
         return self.apply(lambda period: period[-1], onerror=onerror).combine()
 
     def nth(self, index, *, base=0, onerror="raise") -> Calendar:
         """
-        Returns a calendar with the nth date each period
+        Returns a calendar with the nth date each period from the collection
         
         Allowed values for the onerror parameter: 
             - 'skip' to skip periods where the n'th business day is not defined
             - 'first' to fallback to the first date in the period when the n'th 
               business day is not defined
             - 'last' to fallback to the last date in the period when the n'th 
               business day is not defined
@@ -1458,15 +1507,15 @@
 
     def apply(self, func, onerror="raise"):
         """
         Applies a function to each calendar
 
         Returns
         -------
-        Grouper
+        Collection
         """
         if not callable(func):
             raise ValueError("Expected func to be a callable function")
 
         dates = []
         for calendar in self.calendars:
             try:
@@ -1495,48 +1544,52 @@
             elif isinstance(value, Calendar):
                 pass
             else:
                 raise ValueError(
                     "mapped values must be a datetime, a list thereof or a Calendar"
                 )
 
-        return Grouper(dates)
+        return Collection(dates)
 
     def combine(self):
         """
-        Combines the calendars back in one
+        Combines the calendars of the collection back into a 
+        single Calendar object
 
         Returns
         -------
         Calendar
         """
         return Calendar([]).union(*self.calendars)
 
     def filter(self, func):
         """
-        Filters out calendars
+        Filters out calendars from the collection
 
         Parameters
         ----------
         func : callable
             filtering function
 
         Returns
         -------
-        Grouper
+        Collection
         """
         if not callable(func):
             raise ValueError("Expected func to be a callable function")
-        return Grouper([cal for cal in self.calendars if func(cal)])
+        return Collection([cal for cal in self.calendars if func(cal)])
 
     def __len__(self):
         """
         Returns the number of calendars
 
         Returns
         -------
         int
         """
         return len(self.calendars)
 
     def __iter__(self):
+        """
+        Iterate over each calendar in the collection
+        """
         return iter(self.calendars)
```

### Comparing `doubledate-0.0.8/doubledate/utils.py` & `doubledate-0.0.9/doubledate/utils.py`

 * *Files identical despite different names*

### Comparing `doubledate-0.0.8/doubledate.egg-info/PKG-INFO` & `doubledate-0.0.9/doubledate.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doubledate
-Version: 0.0.8
+Version: 0.0.9
 Summary: A calendar wrapper
 Home-page: https://github.com/dschenck/doubledate
 Author: david.schenck@outlook.com
 Author-email: david.schenck@outlook.com
 License: UNKNOWN
 Description: [![Documentation Status](https://readthedocs.org/projects/doubledate/badge/?version=latest)](https://doubledate.readthedocs.io/en/latest/?badge=latest)
```

### Comparing `doubledate-0.0.8/setup.py` & `doubledate-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="doubledate",
-    version="0.0.8",
+    version="0.0.9",
     author="david.schenck@outlook.com",
     author_email="david.schenck@outlook.com",
     description="A calendar wrapper",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/dschenck/doubledate",
     packages=setuptools.find_packages(),
```

### Comparing `doubledate-0.0.8/tests/test_calendar.py` & `doubledate-0.0.9/tests/test_calendar.py`

 * *Files 0% similar despite different names*

```diff
@@ -523,15 +523,15 @@
         calendar = Calendar(
             [datetime.date(2022, 1, 17), datetime.date(2022, 2, 14)]
         ).inverse(datetime.date(2022, 1, 17), datetime.date(2022, 12, 31))
 
         assert calendar[0] == datetime.date(2022, 1, 18)
 
 
-class TestGrouper(unittest.TestCase):
+class TestCollection(unittest.TestCase):
     def test_index(self):
         cals = load().groupby("M")
 
         self.assertTrue(datetime.date(2014, 12, 16) in cals)
 
         self.assertFalse(datetime.date(2014, 12, 25) in cals)
```

### Comparing `doubledate-0.0.8/tests/test_utils.py` & `doubledate-0.0.9/tests/test_utils.py`

 * *Files identical despite different names*

