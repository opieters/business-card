Business Card
=============

Example:

<style>
img {
  border: 1px solid black; 
  max-width: 200px;
}
</style>
<div>
    <img src="images/front.png" alt-="front side business card"/>
    <img src="images/back.png" alt-="back side business card"/>
</div>

Requirements
------------

* Recent TeX installation (tested on a 2017 one)
* XeLaTeX
* [Font Awesome](https://github.com/xdanaux/fontawesome-latex)
* [Fira Sans](https://github.com/mozilla/Fira)

Building Documents
------------------

Build the front and back sides with XeLaTeX:

```shell
xelatex src/front.tex
xelatex src/back.tex
```

License
-------

GNU GPLv3. See LICENSE file.

© 2017 Olivier Pieters
