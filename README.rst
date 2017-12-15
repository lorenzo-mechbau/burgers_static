

==============
Burgers Static
==============

Burgers equation is the simplified version of the Navier-Stokes equation (by dropping the pressure term). This equation can be investigated in one spatial dimension. 


Building the example
====================

The fortran version of the example can be configured and built with CMake::

  cd ~/opencmiss/build/examples/
  git clone https://github.com/OpenCMISS-Examples/burgers_static.git
  mkdir burgers_static-build
  cd burgers_static-build
  cmake -DOpenCMISSLibs_DIR=~/opencmiss/install/  ../burgers_static/
  make


Running the example
===================

Fortran version::

  cd src/fortran/
  .burgers_static_fortran

The results can be visualised by running `visualise.com <./src/fortran/visualise.com>`_ with the `Cmgui visualiser <http://physiomeproject.org/software/opencmiss/cmgui/download>`_.


Results
=======

For the static nonlinear newton iteration problem, with 4 elements on x(0-->1) with

u(x): u(0)=1, u(1)=0

Expected results:
0.80492
0.56704
0.29369

Exact solution:
0.80531
0.56763
0.29412


References
==========

Heinrich, J.C. and Pepper, D.W., 1999. Intermediate finite element method: fluid flow and heat transfer applications. (pg. 216)


Prerequisites
=============

There are no additional input files required for this example as it is self-contained.

License
=======

License applicable to this example is described in `LICENSE <./LICENSE>`_.
