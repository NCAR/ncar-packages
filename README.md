# ncar-packages

This *Git* repository contains the *Spack package* repository **ncar.hpcd**,
which provides NCAR-specific package recipes for packages that, for various
reasons, we do not want to upstream (or haven't yet) to the Spack builtin
repository. Examples of such packages include:

1. `ncarcompilers` - NCAR HPC compiler wrappers
2. `netcdf` - metapackage that bundles separate NetCDF components together

## Installation

You'll probably want to install these packages into a Spack clone as part of a
[spacklot]() cluster installation, in which case you would set the following
variables in the cluster's `main.cfg`:

- `SPACKLOT_URL_PACKAGES_NCAR`: URL of this repo on GitHub
- `SPACKLOT_ROOT_PACKAGES_NCAR`: path on system in which you want this repo to
   exist after cloning (e.g., `$SPACKLOT_ROOT_DEPLOYMENT/packages/ncar`)
- `SPACKLOT_BRANCH_PACKAGES_NCAR`: optionally specify a particular branch (or
  commit) of this repo to use
