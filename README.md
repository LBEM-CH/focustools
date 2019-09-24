# FOCUS TOOLS
Python utilities supporting the [FOCUS package](http://focus-em.org) and cryo-EM data processing in general.

__FOCUS TOOLS__ offers Python functions and scripts for performing common tasks in cryogenic electron microscopy (cryo-EM) data processing such as postprocessing 3D maps, filtering, masking, computing FSC curves, cropping/padding in real and Fourier space, CTF correction, among others. Some of the scripts and functions contained here were developed to support the FOCUS package. Others were written for the developer's own studies or mere convenience, and are made available here in the hope they can be useful to someone else.

The I/O of MRC files (with or without compression) is based on the [MRCZ library](https://github.com/em-MRCZ/python-mrcz).

Where possible, tasks are accelerated by the [NumExpr](https://github.com/pydata/numexpr) engine.

## Installation
__FOCUS TOOLS__ can be installed from [PyPI](http://pypi.org) using `pip`:

`sudo pip install focustools`

If not using `sudo`, it will be installed locally in the user `HOME`. In this case, make sure you have the following location in your `PATH` environment variable in order to be able to call the scripts directly:
`~/.local/bin/`

## Contents

Please see the [release notes](RELEASE_NOTES.md).

## Usage

Once installed, the scripts can be called directly from your shell, for example:

`focus.postprocess half1.mrc half2.mrc --angpix 0.639 --automask --auto_bfac -1,-1 --mtf data_mtf_k2_300kv.star --out postprocessed`

Use the `--help` flag to obtain a comprehensive list of options to the desired script, e.g.

`focus.postprocess --help`

### Tutorials

For more details, see our [Jupyter notebook](http://jupyter.org/install) tutorials below:

* [`focus.postprocess`](tutorial/tutorial_postprocess.ipynb)
* [`focus.mrcz`](tutorial/tutorial_mrcz.ipynb)

## Citing

If __FOCUS TOOLS__ in general is useful in your work, please cite:
* Biyani, N., Righetto, R.D., McLeod, R., Caujolle-Bert, D., Castano-Diez, D., Goldie, K.N., Stahlberg, H., 2017. _Focus: The interface between data collection and data processing in cryo-EM_. J. Struct. Biol. 198, 124–133. https://doi.org/10.1016/j.jsb.2017.03.007

If `focus.postprocess` is useful in your work, please cite:
* Righetto, R.D., Biyani, N., Kowal, J., Chami, M., Stahlberg, H., 2019. _Retrieving high-resolution information from disordered 2D crystals by single-particle cryo-EM_. Nat. Commun. 10, 1722. https://doi.org/10.1038/s41467-019-09661-5

If `focus.mrcz` or the [MRCZ library](https://github.com/em-MRCZ/python-mrcz) are useful in your work, please cite:
* McLeod, R.A., Diogo Righetto, R., Stewart, A., Stahlberg, H., 2018. _MRCZ – A file format for cryo-TEM data with fast compression_. J. Struct. Biol. 201, 252–257. https://doi.org/10.1016/j.jsb.2017.11.012

## Reporting bugs & Troubleshooting

Please use the [issue tracker](https://github.com/C-CINA/focustools/issues) to report bugs or ask for help, suggest features, etc.

## Authors
__FOCUS TOOLS__ was initially developed by [Ricardo Righetto](https://github.com/rdrighetto/) at the [Stahlberg lab](http://c-cina.org).  
The `FCC()` function was written by Robert A. McLeod.

