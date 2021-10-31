anonymize-slide
===============

This is [Benjamin Gilbert's anonymize-slide](https://github.com/bgilbert/anonymize-slide) program updated to run under python3.

**Please note that the updated code has not been tested with MRXS files**

This is a program to remove the slide label from whole-slide images in the
following formats:

 * Aperio SVS
 * Hamamatsu NDPI
 * 3DHISTECH MRXS

Slide files are modified **in place**, making this program both fast and
potentially destructive.  Do not run it on your only copy of a slide.

[Download](https://github.com/cornish/anonymize-slide-python3/releases)

Examples
--------

Delete the label from `slide.mrxs`:

    anonymize-slide.py slide.mrxs

Delete the label from all NDPI files in the current directory:

    anonymize-slide.py *.ndpi

Requirements
------------

 * Python 3.0+

Changes
-------

1. Basic update using 2to3
2. Updates for byte/str representation and methods
3. TiffFile class modified, because "file" no longer exists to inherit from

License
-------

This program is distributed under the [GNU General Public License, version
2](LICENSE).

No Warranty
-----------

This program is distributed in the hope that it will be useful, but WITHOUT
ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or
FITNESS FOR A PARTICULAR PURPOSE.  See the [license](COPYING) for more
details.
