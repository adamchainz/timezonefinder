
Changelog
=========

**Note:** not mentioned versions only contain small and irrelevant changes (e.g. in the readme, setup.py...).
I am new to all this, so I am often missing small things which are not really new features worth mentioning.


1.5.1 (2016-04-18)
------------------

* added python 2.7 support:
    Therefore I had to change the tests a little bit (some operations were not supported). This only affects output.
    I also had to replace one part of the algorithms to prevent overflow in Python 2.7


1.5.0 (2016-04-12)
------------------

* automatically using optimized algorithms now (when numba is installed)
* added TimezoneFinder.using_numba() function to check if the import worked


1.4.0 (2016-04-07)
------------------

* Added the ``file_converter.py`` to the repository: It converts the .csv from pytzwhere to another ``.csv`` and this one into the used ``.bin``.
    Especially the shortcut computation and the boundary storage in there save a lot of reading and computation time, when deciding which timezone the coordinates are in.
    It will help to keep the package up to date, even when the timezone data should change in the future.

