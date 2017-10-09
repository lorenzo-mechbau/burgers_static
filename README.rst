

==============
Burgers Static
==============

Short synopsis of the example.

Building the example
====================

The fortran version of the example can be configured and built with CMake::

  cd ~/opencmiss/build/examples/
  git clone https://github.com/OpenCMISS-Examples/burgers_static.git
  cd burgers_static/
  cmake -DOpenCMISSLibs_DIR=~/opencmiss/install/  ~/opencmiss/src/examples/burgers_static/
  make

Running the example
===================

Fortran version::

  cd src/fortran/
  .burgers_static_fortran

Python version::

  source /opencmiss/install/virtaul_environments/oclibs_venv_py27_release/bin/activate
  cd src/python/
  python burgers_static.py

The results can be visualised by running `visualise.com <./src/fortran/visualise.com>`_ with the `Cmgui visualiser <http://physiomeproject.org/software/opencmiss/cmgui/download>`_.

Prerequisites
=============

There are no additional input files required for this example as it is self-contained.

License
=======

License applicable to this example is described in `LICENSE <./LICENSE>`_.
