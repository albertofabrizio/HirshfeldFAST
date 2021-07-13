# HirshfeldFAST
Compute Classical and Dominant Hirshfeld Charges Given Density Predictions

## SPHERICAL ATOMS

Compute the spherical averaged density matrix (DM) of all the elements up to Ar @ HF level.

Usage:
`compute_DM.py [-h] [--atom ATM] [--basis BASE]`

optional arguments:
  -h, --help    show this help message and exit
  --atom ATM    The periodic table symbol for the atom.
  --basis BASE  The name of the basis set for the computation.


and project the DM onto a specified basis set. 

Usage:
`project.py [-h] --atom ATM --dm DMFILE --basis BASE --auxbasis AUXBASE [--isS] [--isfile]`

optional arguments:
  -h, --help          show this help message and exit
  --atom ATM          The periodic table symbol for the atom.
  --dm DMFILE         The path for the density matrix.
  --basis BASE        The name of the basis set (or path) used for the DM computation.
  --auxbasis AUXBASE  The name of the basis set for the projection.
  --isS               Whether or not using the overlap metric for projection.
  --isfile            Whether or not the auxbasis is the name of an external file to read [default: False].




