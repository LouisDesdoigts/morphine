# morphine - derivatives from poppy
![](https://github.com/benjaminpope/morphine/workflows/integration/badge.svg)
[![Licence](http://img.shields.io/badge/license-GPLv3-blue.svg?style=flat)](http://www.gnu.org/licenses/gpl-3.0.html)

## Contributors

morphine hacks - Benjamin Pope

poppy base code - POPPY code by Marshall Perrin, Joseph Long, Ewan Douglas, Neil Zimmerman, Anand Sivaramakrishnan, Shannon Osborne, Kyle Douglass, Maciek Grochowicz, Phillip Springer, & Ted Corcovilos, with additional contributions from Remi Soummer, Kyle Van Gorkom, Jonathan Fraine, Christine Slocum, Roman Yurchak, and others on the Astropy team.

## Installation

Clone with 

`git clone https://github.com/benjaminpope/morphine`

and run

`python setup.py install`

## About Poppy

POPPY (**P**\ hysical **O**\ ptics **P**\ ropagation in **Py**\ thon) is a Python package that simulates physical optical propagation including diffraction. It implements a flexible framework for modeling Fraunhofer and Fresnel diffraction and point spread function formation, particularly in the context of astronomical telescopes.

POPPY was developed as part of a simulation package for the James Webb Space Telescope, but is more broadly applicable to many kinds of imaging simulations. It is not, however, a substitute for high fidelity optical design software such as Zemax or Code V, but rather is intended as a lightweight alternative for cases for which diffractive rather than geometric optics is the topic of interest, and which require portability between platforms or ease of scripting.

For documentation, see http://poppy-optics.readthedocs.io/