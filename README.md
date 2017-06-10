Business Card
=============

Example:

<div>
    <img src="images/front.png" alt-="front side business card" width="200px"/>
    <img src="images/back.png" alt-="back side business card" width="200px"/>
</div>

How this business card was designed, is explained in [this blog post](https://olivierpieters.be/blog/2017/02/11/designing-a-business-card-in-latex).

Requirements
------------

* Recent TeX installation (tested on a 2017 one)
* XeLaTeX
* [Font Awesome](https://github.com/xdanaux/fontawesome-latex)
* [Fira Sans](https://github.com/mozilla/Fira)

It is also possible to use [this Docker container](https://hub.docker.com/r/accupara/business-cards/):

```shell
docker run \
    --rm -it \
    -v `pwd`:/tmp/src accupara/business-cards \
    /bin/bash -c 'cd /tmp/src/src ; xelatex front.tex;'
```

Building Documents
------------------

Build the front and back sides with XeLaTeX:

```shell
xelatex src/front.tex
xelatex src/back.tex
```

SVG Files
---------

LaTeX is not equipped to handle SVG files directly. A conversion to a PDF file is needed. This can be done using an external tool such as Inkscape:

```shell
inkscape --without-gui --export-area-drawing --file=logo.svg --export-pdf=logo.pdf
```

License
-------

GNU GPLv3. See LICENSE file.

© 2017 Olivier Pieters
