# FOCUS TOOLS
Python utilities supporting the FOCUS package and cryo-EM data processing in general.

FOCUS TOOLS offers Python functions and scripts for performing common tasks in cryogenic electron microscopy (cryo-EM) data processing such as postprocessing 3D maps, filtering, masking, computing FSC curves, cropping/padding in real and Fourier space, CTF correction, among others. Some of the tools contained here were developed to support the FOCUS package.

The I/O of MRC files is based on the [MRCZ library](https://github.com/em-MRCZ/python-mrcz).

Where possible, tasks are accelerated by the [NumExpr](https://github.com/pydata/numexpr) engine.

## Installation
FOCUS TOOLS can be installed from [PyPI](http://pypi.org) using `pip`:

`sudo pip install focustools`

If not using `sudo`, it will be installed locally in the user `HOME`. In this case, make sure you have the following location in your `PATH` environment variable:
`~/.local/bin/`

## Citing
If FOCUS TOOLS is useful in your work, please cite the following papers:

* Righetto, R.D., Biyani, N., Kowal, J., Chami, M., Stahlberg, H., 2019. _Retrieving high-resolution information from disordered 2D crystals by single-particle cryo-EM_. Nat. Commun. 10, 1722. https://doi.org/10.1038/s41467-019-09661-5
* Biyani, N., Righetto, R.D., McLeod, R., Caujolle-Bert, D., Castano-Diez, D., Goldie, K.N., Stahlberg, H., 2017. _Focus: The interface between data collection and data processing in cryo-EM_. J. Struct. Biol. 198, 124–133. https://doi.org/10.1016/j.jsb.2017.03.007

## Troubleshooting

Please use the [issue tracker](https://github.com/C-CINA/focustools/issues) to report bugs or ask for help.

## Authors
FOCUS TOOLS is developed by [Ricardo Righetto](https://github.com/rdrighetto/) at the [Stahlberg lab](http://c-cina.org) together with the [FOCUS package](http://focus-em.org).

