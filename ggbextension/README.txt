This module defines a directive, `ggb`.  It takes a single, required
argument, a geogebra tube ID::

    .. ggb:: 1264951

The referenced geogebra applet will be embedded into HTML output.  

There are 4 necessary parameters "width" and "height" are the applet width and height, "img" and "imgwidth" are the location of an image file to be put in place of the applet into pdf output and the image width of that image.
"img" should be relative to the _build/latex folder.

There is an optional parameter "zoom_drag" (default setting: false) to control whether the applet image can be dragged and zoomed by the use by the user.

.. ggb:: 1264951
    :width: 846
    :height: 664
    :img: ../../_static/hi_logo.jpg
    :imgwidth: 4cm
    :zoom_drag: true 

Installation
============
python(3) setup.py build
sudo python(3) setup.py install  OR  python(3) setup.py install --user
