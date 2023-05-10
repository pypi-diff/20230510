# Comparing `tmp/pyunitx-0.9.2.tar.gz` & `tmp/pyunitx-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyunitx-0.9.2.tar", max compression
+gzip compressed data, was "pyunitx-0.9.3.tar", max compression
```

## Comparing `pyunitx-0.9.2.tar` & `pyunitx-0.9.3.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0    35147 2020-02-18 03:57:45.408000 pyunitx-0.9.2/LICENSE
--rw-r--r--   0        0        0     7778 2022-11-04 02:41:39.775835 pyunitx-0.9.2/README.md
--rw-r--r--   0        0        0      913 2022-12-24 07:53:24.853930 pyunitx-0.9.2/pyproject.toml
--rw-r--r--   0        0        0     1190 2022-10-21 06:17:34.189312 pyunitx-0.9.2/pyunitx/__init__.py
--rw-r--r--   0        0        0    34055 2022-12-24 07:46:34.409674 pyunitx-0.9.2/pyunitx/_api.py
--rw-r--r--   0        0        0      573 2022-10-02 00:10:39.992516 pyunitx-0.9.2/pyunitx/_exceptions.py
--rw-r--r--   0        0        0     3926 2022-11-08 23:55:37.626803 pyunitx-0.9.2/pyunitx/angle.py
--rw-r--r--   0        0        0      708 2022-10-29 05:43:33.532704 pyunitx-0.9.2/pyunitx/area.py
--rw-r--r--   0        0        0      744 2022-10-21 06:17:34.217312 pyunitx-0.9.2/pyunitx/capacitance.py
--rw-r--r--   0        0        0     1076 2022-10-29 05:43:33.832707 pyunitx-0.9.2/pyunitx/charge.py
--rw-r--r--   0        0        0     5187 2022-10-21 06:17:34.217312 pyunitx-0.9.2/pyunitx/constants.py
--rw-r--r--   0        0        0      482 2022-10-29 05:43:33.476703 pyunitx-0.9.2/pyunitx/current.py
--rw-r--r--   0        0        0     3380 2022-12-24 07:42:04.814804 pyunitx-0.9.2/pyunitx/data.py
--rw-r--r--   0        0        0     1567 2022-11-08 22:26:58.600988 pyunitx-0.9.2/pyunitx/derived.py
--rw-r--r--   0        0        0     2130 2022-11-04 05:45:10.694594 pyunitx-0.9.2/pyunitx/energy.py
--rw-r--r--   0        0        0     1134 2022-11-04 05:45:10.694594 pyunitx-0.9.2/pyunitx/force.py
--rw-r--r--   0        0        0      833 2022-10-29 05:43:33.668705 pyunitx-0.9.2/pyunitx/frequency.py
--rw-r--r--   0        0        0      676 2022-10-21 06:17:34.233313 pyunitx-0.9.2/pyunitx/inductance.py
--rw-r--r--   0        0        0     1498 2022-10-29 05:43:33.960709 pyunitx-0.9.2/pyunitx/length.py
--rw-r--r--   0        0        0      566 2022-10-21 06:17:34.233313 pyunitx-0.9.2/pyunitx/luminosity.py
--rw-r--r--   0        0        0      730 2022-10-21 06:17:34.245313 pyunitx-0.9.2/pyunitx/magneticflux.py
--rw-r--r--   0        0        0      687 2022-10-21 06:17:34.245313 pyunitx-0.9.2/pyunitx/magneticfluxdensity.py
--rw-r--r--   0        0        0     2292 2022-10-29 05:29:18.433484 pyunitx-0.9.2/pyunitx/mass.py
--rw-r--r--   0        0        0      861 2022-10-29 05:43:33.916708 pyunitx-0.9.2/pyunitx/mole.py
--rw-r--r--   0        0        0     1368 2022-11-04 05:45:10.714594 pyunitx-0.9.2/pyunitx/power.py
--rw-r--r--   0        0        0     1106 2022-11-04 05:45:10.714594 pyunitx-0.9.2/pyunitx/pressure.py
--rw-r--r--   0        0        0     5228 2022-10-29 19:26:58.315868 pyunitx-0.9.2/pyunitx/resistance.py
--rw-r--r--   0        0        0     1313 2022-11-02 07:04:08.384199 pyunitx-0.9.2/pyunitx/resistor.py
--rw-r--r--   0        0        0     3706 2022-10-29 05:18:08.458380 pyunitx-0.9.2/pyunitx/temperature.py
--rw-r--r--   0        0        0     2839 2022-10-29 02:15:44.326331 pyunitx-0.9.2/pyunitx/time.py
--rw-r--r--   0        0        0     2334 2022-11-04 05:45:10.714594 pyunitx-0.9.2/pyunitx/uconvert.py
--rw-r--r--   0        0        0      592 2022-10-29 05:18:08.262376 pyunitx-0.9.2/pyunitx/voltage.py
--rw-r--r--   0        0        0     2816 2022-11-04 05:45:10.722594 pyunitx-0.9.2/pyunitx/volume.py
--rw-r--r--   0        0        0     8912 1970-01-01 00:00:00.000000 pyunitx-0.9.2/setup.py
--rw-r--r--   0        0        0     8486 1970-01-01 00:00:00.000000 pyunitx-0.9.2/PKG-INFO
+-rw-r--r--   0        0        0    35147 2020-02-18 03:57:45.408000 pyunitx-0.9.3/LICENSE
+-rw-r--r--   0        0        0     7778 2022-11-04 02:41:39.775835 pyunitx-0.9.3/README.md
+-rw-r--r--   0        0        0      913 2022-12-29 00:01:20.680631 pyunitx-0.9.3/pyproject.toml
+-rw-r--r--   0        0        0     1190 2022-10-21 06:17:34.189312 pyunitx-0.9.3/pyunitx/__init__.py
+-rw-r--r--   0        0        0    34831 2022-12-29 00:00:25.091970 pyunitx-0.9.3/pyunitx/_api.py
+-rw-r--r--   0        0        0      573 2022-10-02 00:10:39.992516 pyunitx-0.9.3/pyunitx/_exceptions.py
+-rw-r--r--   0        0        0     3926 2022-11-08 23:55:37.626803 pyunitx-0.9.3/pyunitx/angle.py
+-rw-r--r--   0        0        0      708 2022-10-29 05:43:33.532704 pyunitx-0.9.3/pyunitx/area.py
+-rw-r--r--   0        0        0      744 2022-10-21 06:17:34.217312 pyunitx-0.9.3/pyunitx/capacitance.py
+-rw-r--r--   0        0        0     1076 2022-10-29 05:43:33.832707 pyunitx-0.9.3/pyunitx/charge.py
+-rw-r--r--   0        0        0     5187 2022-10-21 06:17:34.217312 pyunitx-0.9.3/pyunitx/constants.py
+-rw-r--r--   0        0        0      482 2022-10-29 05:43:33.476703 pyunitx-0.9.3/pyunitx/current.py
+-rw-r--r--   0        0        0     3380 2022-12-24 07:42:04.814804 pyunitx-0.9.3/pyunitx/data.py
+-rw-r--r--   0        0        0     1567 2022-11-08 22:26:58.600988 pyunitx-0.9.3/pyunitx/derived.py
+-rw-r--r--   0        0        0     2130 2022-11-04 05:45:10.694594 pyunitx-0.9.3/pyunitx/energy.py
+-rw-r--r--   0        0        0     1134 2022-11-04 05:45:10.694594 pyunitx-0.9.3/pyunitx/force.py
+-rw-r--r--   0        0        0      833 2022-10-29 05:43:33.668705 pyunitx-0.9.3/pyunitx/frequency.py
+-rw-r--r--   0        0        0      676 2022-10-21 06:17:34.233313 pyunitx-0.9.3/pyunitx/inductance.py
+-rw-r--r--   0        0        0     1498 2022-10-29 05:43:33.960709 pyunitx-0.9.3/pyunitx/length.py
+-rw-r--r--   0        0        0      566 2022-10-21 06:17:34.233313 pyunitx-0.9.3/pyunitx/luminosity.py
+-rw-r--r--   0        0        0      730 2022-10-21 06:17:34.245313 pyunitx-0.9.3/pyunitx/magneticflux.py
+-rw-r--r--   0        0        0      687 2022-10-21 06:17:34.245313 pyunitx-0.9.3/pyunitx/magneticfluxdensity.py
+-rw-r--r--   0        0        0     2292 2022-10-29 05:29:18.433484 pyunitx-0.9.3/pyunitx/mass.py
+-rw-r--r--   0        0        0      861 2022-10-29 05:43:33.916708 pyunitx-0.9.3/pyunitx/mole.py
+-rw-r--r--   0        0        0     1368 2022-11-04 05:45:10.714594 pyunitx-0.9.3/pyunitx/power.py
+-rw-r--r--   0        0        0     1106 2022-11-04 05:45:10.714594 pyunitx-0.9.3/pyunitx/pressure.py
+-rw-r--r--   0        0        0     5228 2022-10-29 19:26:58.315868 pyunitx-0.9.3/pyunitx/resistance.py
+-rw-r--r--   0        0        0     1313 2022-11-02 07:04:08.384199 pyunitx-0.9.3/pyunitx/resistor.py
+-rw-r--r--   0        0        0     3706 2022-10-29 05:18:08.458380 pyunitx-0.9.3/pyunitx/temperature.py
+-rw-r--r--   0        0        0     2839 2022-10-29 02:15:44.326331 pyunitx-0.9.3/pyunitx/time.py
+-rw-r--r--   0        0        0     2334 2022-11-04 05:45:10.714594 pyunitx-0.9.3/pyunitx/uconvert.py
+-rw-r--r--   0        0        0      592 2022-10-29 05:18:08.262376 pyunitx-0.9.3/pyunitx/voltage.py
+-rw-r--r--   0        0        0     2816 2022-11-04 05:45:10.722594 pyunitx-0.9.3/pyunitx/volume.py
+-rw-r--r--   0        0        0     8912 1970-01-01 00:00:00.000000 pyunitx-0.9.3/setup.py
+-rw-r--r--   0        0        0     8486 1970-01-01 00:00:00.000000 pyunitx-0.9.3/PKG-INFO
```

### Comparing `pyunitx-0.9.2/LICENSE` & `pyunitx-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyunitx-0.9.2/README.md` & `pyunitx-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `pyunitx-0.9.2/pyproject.toml` & `pyunitx-0.9.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyunitx"
-version = "0.9.2"
+version = "0.9.3"
 description = "First-class manipulation of physical quantities"
 authors = ["Nick Thurmes <nthurmes@gmail.com>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.7"
```

### Comparing `pyunitx-0.9.2/pyunitx/__init__.py` & `pyunitx-0.9.3/pyunitx/__init__.py`

 * *Files identical despite different names*

### Comparing `pyunitx-0.9.2/pyunitx/_api.py` & `pyunitx-0.9.3/pyunitx/_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -748,14 +748,31 @@
 
     def __str__(self):
         return f"{self.value} {self.abbreviation}"
 
     def __repr__(self):
         return str(self)
 
+    def __format__(self, format_spec):
+        """Format this measurement similar to a float.
+
+        :param format_spec: The format specification, in a restricted subset of
+            the python `string formatting mini-language. \
+            <https://docs.python.org/3/library/string.html#format-specification-mini-language>`_
+            Currently only supports ``.[precision]g`` to round to the specified
+            number of significant figures.
+        """
+        if not format_spec:
+            return str(self)
+        match = re.fullmatch(r"\.(\d+)[gG]", format_spec)
+        if match:
+            precision = int(match.group(1))
+            return f"{self.sig_figs(precision).value} {self.abbreviation}"
+        raise ValueError("Invalid format specification")
+
     def is_dimension(self, dim: DimensionBase) -> bool:
         """Check if this unit is of the given dimension.
 
         Most useful for checking whether two measurements can be reasonably
         compared with ``.equivalent_to`` or converted into the other.
 
         :param dim: The dimension to check against.
```

### Comparing `pyunitx-0.9.2/pyunitx/_exceptions.py` & `pyunitx-0.9.3/pyunitx/_exceptions.py`

 * *Files identical despite different names*

### Comparing `pyunitx-0.9.2/pyunitx/angle.py` & `pyunitx-0.9.3/pyunitx/angle.py`

 * *Files identical despite different names*

### Comparing `pyunitx-0.9.2/pyunitx/area.py` & `pyunitx-0.9.3/pyunitx/area.py`

 * *Files identical despite different names*

### Comparing `pyunitx-0.9.2/pyunitx/capacitance.py` & `pyunitx-0.9.3/pyunitx/capacitance.py`

 * *Files identical despite different names*

### Comparing `pyunitx-0.9.2/pyunitx/charge.py` & `pyunitx-0.9.3/pyunitx/charge.py`

 * *Files identical despite different names*

### Comparing `pyunitx-0.9.2/pyunitx/constants.py` & `pyunitx-0.9.3/pyunitx/constants.py`

 * *Files identical despite different names*

### Comparing `pyunitx-0.9.2/pyunitx/data.py` & `pyunitx-0.9.3/pyunitx/data.py`

 * *Files identical despite different names*

### Comparing `pyunitx-0.9.2/pyunitx/derived.py` & `pyunitx-0.9.3/pyunitx/derived.py`

 * *Files identical despite different names*

### Comparing `pyunitx-0.9.2/pyunitx/energy.py` & `pyunitx-0.9.3/pyunitx/energy.py`

 * *Files identical despite different names*

### Comparing `pyunitx-0.9.2/pyunitx/force.py` & `pyunitx-0.9.3/pyunitx/force.py`

 * *Files identical despite different names*

### Comparing `pyunitx-0.9.2/pyunitx/frequency.py` & `pyunitx-0.9.3/pyunitx/frequency.py`

 * *Files identical despite different names*

### Comparing `pyunitx-0.9.2/pyunitx/inductance.py` & `pyunitx-0.9.3/pyunitx/inductance.py`

 * *Files identical despite different names*

### Comparing `pyunitx-0.9.2/pyunitx/length.py` & `pyunitx-0.9.3/pyunitx/length.py`

 * *Files identical despite different names*

### Comparing `pyunitx-0.9.2/pyunitx/luminosity.py` & `pyunitx-0.9.3/pyunitx/luminosity.py`

 * *Files identical despite different names*

### Comparing `pyunitx-0.9.2/pyunitx/magneticflux.py` & `pyunitx-0.9.3/pyunitx/magneticflux.py`

 * *Files identical despite different names*

### Comparing `pyunitx-0.9.2/pyunitx/magneticfluxdensity.py` & `pyunitx-0.9.3/pyunitx/magneticfluxdensity.py`

 * *Files identical despite different names*

### Comparing `pyunitx-0.9.2/pyunitx/mass.py` & `pyunitx-0.9.3/pyunitx/mass.py`

 * *Files identical despite different names*

### Comparing `pyunitx-0.9.2/pyunitx/mole.py` & `pyunitx-0.9.3/pyunitx/mole.py`

 * *Files identical despite different names*

### Comparing `pyunitx-0.9.2/pyunitx/power.py` & `pyunitx-0.9.3/pyunitx/power.py`

 * *Files identical despite different names*

### Comparing `pyunitx-0.9.2/pyunitx/pressure.py` & `pyunitx-0.9.3/pyunitx/pressure.py`

 * *Files identical despite different names*

### Comparing `pyunitx-0.9.2/pyunitx/resistance.py` & `pyunitx-0.9.3/pyunitx/resistance.py`

 * *Files identical despite different names*

### Comparing `pyunitx-0.9.2/pyunitx/resistor.py` & `pyunitx-0.9.3/pyunitx/resistor.py`

 * *Files identical despite different names*

### Comparing `pyunitx-0.9.2/pyunitx/temperature.py` & `pyunitx-0.9.3/pyunitx/temperature.py`

 * *Files identical despite different names*

### Comparing `pyunitx-0.9.2/pyunitx/time.py` & `pyunitx-0.9.3/pyunitx/time.py`

 * *Files identical despite different names*

### Comparing `pyunitx-0.9.2/pyunitx/uconvert.py` & `pyunitx-0.9.3/pyunitx/uconvert.py`

 * *Files identical despite different names*

### Comparing `pyunitx-0.9.2/pyunitx/voltage.py` & `pyunitx-0.9.3/pyunitx/voltage.py`

 * *Files identical despite different names*

### Comparing `pyunitx-0.9.2/pyunitx/volume.py` & `pyunitx-0.9.3/pyunitx/volume.py`

 * *Files identical despite different names*

### Comparing `pyunitx-0.9.2/setup.py` & `pyunitx-0.9.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 entry_points = \
 {'console_scripts': ['resistor = pyunitx.resistor:main',
                      'uconvert = pyunitx.uconvert:main']}
 
 setup_kwargs = {
     'name': 'pyunitx',
-    'version': '0.9.2',
+    'version': '0.9.3',
     'description': 'First-class manipulation of physical quantities',
     'long_description': '# pyunitx\n\n[![Coverage Status](https://coveralls.io/repos/github/the-nick-of-time/units/badge.svg?branch=main)](https://coveralls.io/github/the-nick-of-time/units?branch=main)\n[![Documentation Status](https://readthedocs.org/projects/pyunitx/badge/?version=latest)](https://pyunitx.readthedocs.io/en/latest/?badge=latest)\n\nWhen doing calculations using physical measurements, it\'s all too easy to forget to account for\nunits. This can result in problems when you find you\'ve been adding kilograms to newtons and\nyour calculation is off by a factor of ten.\n\nThis library uses the standard\nlibrary [decimal.Decimal](https://docs.python.org/3/library/decimal.html) for all calculations\nto avoid most floating-point calculation pitfalls. Values given for units are automatically\nconverted so you can enter any value that constructor can take. Functionally, this means that\nfloat notation should be given as strings rather than float literals.\n\n## Illustrative Examples\n\nQ. How many meters does light travel in a millisecond?\n\n```pycon\n>>> from pyunitx.time import seconds\n>>> from pyunitx.constants import c\n>>> (c * seconds("1e-3")).sig_figs(5)\n2.9979E+5 m\n\n```\n\nQ. What is that in feet?\n\n```pycon\n>>> from pyunitx.time import seconds\n>>> from pyunitx.constants import c\n>>> (c * seconds("1e-3")).to_feet().sig_figs(5)\n9.8357E+5 ft\n\n```\n\nQ. How fast is someone on the equator moving around the center of the earth?\n\n```pycon\n>>> from pyunitx.time import days\n>>> from pyunitx.constants import earth_radius\n>>> from math import pi\n>>> circumference = 2 * pi * earth_radius\n>>> (circumference / days(1)).to_meters_per_second().sig_figs(3)\n464 m s^-1\n\n```\n\nQ. How fast is the earth orbiting the sun?\n\n```pycon\n>>> from pyunitx.time import julian_years\n>>> from pyunitx.length import au\n>>> from math import pi\n>>> circumference = 2 * pi * au(1)\n>>> (circumference / julian_years(1)).to_kilometers_per_hour().sig_figs(3)\n1.07E+5 km hr^-1\n\n```\n\nQ. What\'s the mass of air in one of your car tires, if the inner radius is 6 inches, the outer\nradius is 12.5 inches, the width is 8 inches, and it\'s filled to 42 psi?[^1]\n\n[^1]: No, I don\'t write homework problems. Why do you ask?\n\n```pycon\n>>> from pyunitx.length import inches\n>>> from pyunitx.pressure import psi\n>>> from pyunitx.constants import R, air_molar_mass\n>>> from pyunitx.temperature import celsius, celsius_to_kelvin_absolute\n>>> from math import pi\n>>> volume = (pi * inches(8) * (inches("12.5") ** 2 - inches(6) ** 2)).to_meters_cubed()\n>>> pressure = psi(42).to_pascals()\n>>> temperature = celsius_to_kelvin_absolute(celsius(25))\n>>> mols = pressure * volume / (R * temperature)\n>>> mass = mols * air_molar_mass\n>>> mass.to_pounds_mass().sig_figs(3)\n0.369 lbm\n\n```\n\nAll constants like `R` are defined in SI base units so you will need to convert your units, but\nas you can see, that task is easy. It\'s just a matter of calling `.to_<other unit>()`. You can\nconvert from any unit to another that measures the same dimension this way. If you\'re going to a\ncomposite unit that hasn\'t been explicitly declared with a name, this is still possible, and the\nlibrary will create a converter for you - you just need to get the name right. The name format\nis as intuitive as possible, as you can see with the above examples.\n\nA name is made of the names of the base units, suffixed with `_squared`, `_cubed`, etc. to\nrelate the size of the exponent and prefixed by `per_` if the exponent is negative. Units with\nnegative exponents are made singular[^2] to follow how you would say it.\n\n[^2]: Naively; it\'s done by just stripping off a trailing \'s\' if there is one.\n\nSome examples of the most complicated possible situations will be illustrative.\n\n```pycon\n>>> from pyunitx.constants import gas_constant, stefan_boltzmann\n>>> print(gas_constant.to_feet_pounds_per_mole_per_rankine().sig_figs(4))\n3.407 ft^2 slug mol^-1 °R^-1 s^-2\n\n>>> print(stefan_boltzmann.to_horsepower_per_feet_squared_per_rankine_to_the_fourth().sig_figs(5))\n3.7013E-10 slug s^-3 °R^-4\n\n```\n\nYou will notice that the output will have all units broken down to their bases. It is guaranteed\nto be equivalent.\n\nNow what happens if a calculation results in a predefined unit, like how newtons times meters\nequals joules?\n\n```pycon\n>>> from pyunitx.voltage import volts\n>>> from pyunitx.resistance import ohms\n>>> print(volts(2) / ohms(100))\n0.02 A\n\n```\n\nCalculations check their result against all the units that have been specially defined to find a\nmatch. However, if you end up with a result that could be broken into some product of complex\nunits (like newton-seconds) this library will *not* do that for you and instead display it in\nits basest components. This is because the number of possible options is large and it\'s not\npossible to figure out what you want.\n\nThis library predefines all the SI units and dimensions, as well as a bunch of US Customary\nunits, but what if that\'s not enough? You might want to model some other quantity, like cash\nflow in your budget.\n\n```pycon\n>>> from pyunitx import make_dimension, make_unit\n>>> from pyunitx.time import days\n>>> Money = make_dimension(\'Money\')\n>>> dollars = make_unit(name="dollars", abbrev="$", dimension=Money, scale=1)\n>>> euros = make_unit(name="euros", abbrev="€", dimension=Money, scale="0.98019")\n>>> (dollars(150) / days(7)).to_euros_per_year().sig_figs(6)\n7984.80 € yr^-1\n\n```\n\nFor more examples, including derived units, see the definitions in the package, like\n[energy](https://github.com/the-nick-of-time/units/blob/main/pyunitx/energy.py) or\n[time](https://github.com/the-nick-of-time/units/blob/main/pyunitx/time.py).\n\n## `uconvert`\n\nThis package also comes with a command-line tool to perform unit conversions between any\npredefined units.\n\nQ. What\'s the conversion factor between kilowatts and foot-pounds per second?\n\n```shell\n$ uconvert 1 kW ft.lb/s\n737.562 ft^2 slug s^-3\n```\n\nQ. What\'s my cat\'s weight in pounds, rounded to 3 significant figures?\n\n```shell\n$ uconvert -f 3 4.9 kg lbm\n10.8 lbm\n```\n\n## Resistor color code converter\n\nIn the `resistance` module there is a function to construct a resistance from a color code.\n\nQ. What\'s the value of a resistor reading "orange, violet, red, silver"?\n\n```pycon\n>>> from pyunitx.resistance import from_color\n>>> from_color("OVRS")\n3700 Ω\n\n```\n\nQ. I want to know the tolerance on that same resistor.\n\n```pycon\n>>> from pyunitx.resistance import from_color\n>>> from_color("OVRS", include_tol=True)\n(3700 Ω, 370.0 Ω)\n\n```\n\nQ. What\'s the full specification of a six-band resistor reading "green, blue, blue, orange,\nbrown, red"?\n\n```pycon\n>>> from pyunitx.resistance import from_color\n>>> from_color("EUUOBR", include_coeff=True)\n(566000 Ω, 5660.00 Ω, 28.30000 m^2 kg K^-1 A^-2 s^-3)\n\n```\n\nNote: that last quantity is ohms per kelvin. As above, it gets decomposed into its base units\ndue to not being a named derived unit.\n\nFor the mapping between letter and color,\nsee [the documentation](https://pyunitx.readthedocs.io/complex.html#resistance). Because the\nstarting letter of the colors are not unique (black, brown, and blue, as well as green, gray,\nand gold) the letter chosen to represent it isn\'t perfectly intuitive. If you want your code to\nbe more readable, all the colors are defined in an enum that you can use directly.\n\n```pycon\n>>> from pyunitx.resistance import from_color, Color\n>>> from_color([Color.ORANGE, Color.VIOLET, Color.RED, Color.SILVER], include_tol=True)\n(3700 Ω, 370.0 Ω)\n\n```\n\nThere is also a companion command-line tool that outputs its values in a human-readable format.\nIt is installed as `resistor` alongside `uconvert`.\n\n```shell\n$ resistor -c euuobr\n566 kΩ + 28.3 Ω/K ± 5.66 kΩ\n```\n\nThe full documentation can be found at [ReadTheDocs](https://pyunitx.readthedocs.io/en/latest/).\n',
     'author': 'Nick Thurmes',
     'author_email': 'nthurmes@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `pyunitx-0.9.2/PKG-INFO` & `pyunitx-0.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyunitx
-Version: 0.9.2
+Version: 0.9.3
 Summary: First-class manipulation of physical quantities
 License: GPL-3.0-or-later
 Author: Nick Thurmes
 Author-email: nthurmes@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
```

