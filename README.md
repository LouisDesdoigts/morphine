# morphine - derivatives from poppy
[![integration](https://github.com/benjaminpope/morphine/actions/workflows/github-workflow.yml/badge.svg)](https://github.com/benjaminpope/morphine/actions/workflows/github-workflow.yml)
[![License](https://img.shields.io/badge/License-BSD%203--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)
[![PyPI version](https://badge.fury.io/py/morphine-optics.svg)](https://badge.fury.io/py/morphine-optics)
[![arXiv](http://img.shields.io/badge/arXiv-2011.09780-blue.svg?style=flat)](http://arxiv.org/abs/2011.09780)

## About morphine

The main hindrance to directly imaging exoplanets comes from optical aberrations that produce speckles that can be difficult to distinguish from real planets. 

The technology underlying deep learning - automatic differentiation or 'autodiff' - allows us to take derivatives by the chain rule of arbitrary numerical simulations, for example finding the kernel phase transfer matrix as the Jacobian of Fourier visibilities with respect to the phase of incoming light. This can be used for kernel phase calibration ([arXiv:2011.09780](https://arxiv.org/abs/2011.09780)), as well as for phase retrieval and optical design in highly nonlinear regimes ([arXiv:](https://arxiv.org/abs/2107.00952)). 

By rewriting the popular optical simulation package '[poppy](https://github.com/mperrin/poppy)' using the autodiff library [Google Jax](https://github.com/google/jax), we present 'morphine', a powerful new open source tool for optics and data analysis.

## Contributors

morphine - [Benjamin Pope](https://github.com/benjaminpope), [Louis Desdoigts](https://github.com/LouisDesdoigts), [Alison Wong](https://github.com/alipwong)

poppy base code - POPPY code by Marshall Perrin, Joseph Long, Ewan Douglas, Neil Zimmerman, Anand Sivaramakrishnan, Shannon Osborne, Kyle Douglass, Maciek Grochowicz, Phillip Springer, & Ted Corcovilos, with additional contributions from Remi Soummer, Kyle Van Gorkom, Jonathan Fraine, Christine Slocum, Roman Yurchak, and others on the Astropy team.

## Installation

The easiest way to install is from pip as 

`pip install morphine-optics`

Clone with 

`git clone https://github.com/benjaminpope/morphine`

and run

`python setup.py install`

## Talks

Fizeau Hackathon introduction: [slides](https://benjaminpope.github.io/talks/fizeau/fizeau.html) and [recording](https://sites.google.com/uci.edu/virtualmaskinghackathon/recordings?authuser=0).

## Citation

We would love it if you use `morphine` in a paper! If you do, please cite

```BibTeX
@ARTICLE{2021ApJ...907...40P,
       author = {{Pope}, Benjamin J.~S. and {Pueyo}, Laurent and {Xin}, Yinzi and {Tuthill}, Peter G.},
        title = "{Kernel Phase and Coronagraphy with Automatic Differentiation}",
      journal = {\apj},
     keywords = {Direct imaging, Astronomy data analysis, Optical interferometry, Coronagraphic imaging, Astronomical simulations, 387, 1858, 1168, 313, 1857, Astrophysics - Instrumentation and Methods for Astrophysics},
         year = 2021,
        month = jan,
       volume = {907},
       number = {1},
          eid = {40},
        pages = {40},
          doi = {10.3847/1538-4357/abcb00},
archivePrefix = {arXiv},
       eprint = {2011.09780},
 primaryClass = {astro-ph.IM},
       adsurl = {https://ui.adsabs.harvard.edu/abs/2021ApJ...907...40P},
      adsnote = {Provided by the SAO/NASA Astrophysics Data System}
}

```

and 

```BibTeX
@ARTICLE{2021arXiv210700952W,
       author = {{Wong}, Alison and {Pope}, Benjamin and {Desdoigts}, Louis and {Tuthill}, Peter and {Norris}, Barnaby and {Betters}, Chris},
        title = "{Phase Retrieval and Design with Automatic Differentiation}",
      journal = {arXiv e-prints},
     keywords = {Astrophysics - Instrumentation and Methods for Astrophysics},
         year = 2021,
        month = jul,
          eid = {arXiv:2107.00952},
        pages = {arXiv:2107.00952},
archivePrefix = {arXiv},
       eprint = {2107.00952},
 primaryClass = {astro-ph.IM},
       adsurl = {https://ui.adsabs.harvard.edu/abs/2021arXiv210700952W},
      adsnote = {Provided by the SAO/NASA Astrophysics Data System}
}
```

## About poppy

POPPY (**P**\ hysical **O**\ ptics **P**\ ropagation in **Py**\ thon) is a Python package that simulates physical optical propagation including diffraction. It implements a flexible framework for modeling Fraunhofer and Fresnel diffraction and point spread function formation, particularly in the context of astronomical telescopes.

POPPY was developed as part of a simulation package for the James Webb Space Telescope, but is more broadly applicable to many kinds of imaging simulations. It is not, however, a substitute for high fidelity optical design software such as Zemax or Code V, but rather is intended as a lightweight alternative for cases for which diffractive rather than geometric optics is the topic of interest, and which require portability between platforms or ease of scripting.

For documentation, see http://poppy-optics.readthedocs.io/

