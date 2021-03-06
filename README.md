    Copyright (C) 2013-2016 Christian T. Jacobs.

    This file is part of PyQSO.

    PyQSO is free software: you can redistribute it and/or modify
    it under the terms of the GNU General Public License as published by
    the Free Software Foundation, either version 3 of the License, or
    (at your option) any later version.

    PyQSO is distributed in the hope that it will be useful,
    but WITHOUT ANY WARRANTY; without even the implied warranty of
    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
    GNU General Public License for more details.

    You should have received a copy of the GNU General Public License
    along with PyQSO.  If not, see <http://www.gnu.org/licenses/>.

PyQSO
=====

PyQSO is a contact logging tool for amateur radio operators.

[![Build Status](https://travis-ci.org/ctjacobs/pyqso.svg)](https://travis-ci.org/ctjacobs/pyqso)
[![Documentation Status](https://readthedocs.org/projects/pyqso/badge/?version=latest)](https://readthedocs.org/projects/pyqso/?badge=latest)

Installation and running
------------------------

Assuming that the current working directory is PyQSO's base directory (the directory that the Makefile is in), PyQSO can be installed via the terminal with the following command:

   `make install`

Note: 'sudo' may be needed for this. Once installed, the following command will run PyQSO:
   
   `pyqso`

Alternatively, PyQSO can be run (without installing) with:

   `python3 bin/pyqso`

from PyQSO's base directory.

Documentation
-------------

The PyQSO documentation is stored in the `docs` directory. It can be built with the following command:

   `make docs`

which will produce an HTML version of the documentation in `docs/build/html` that can be opened in a web browser.

Alternatively, a ready-built version of the PyQSO documentation can be found on [Read the Docs](http://pyqso.readthedocs.io/).

Dependencies
------------

PyQSO depends on the following Debian packages:

* gir1.2-gtk-3.0
* python3
* python3-gi-cairo (for log printing purposes)

The following extra packages are necessary to enable the grey line tool and the plotting of logbook statistics:

* python3-matplotlib (version 1.3.0 or later)
* python3-mpltoolkits.basemap
* python3-numpy
* libxcb-render0-dev
* python3-cairocffi

The following extra package is necessary to build the documentation:

* python3-sphinx

There currently does not exist a Python 3-compatible Debian package for [Hamlib](http://www.hamlib.org). This library must be built manually to enable Hamlib support.

Contact
-------

If you have any comments or questions about PyQSO, please send them via email to Christian Jacobs (2E0ICL) at <christian@christianjacobs.uk>.
