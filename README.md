# Undergraduate Thesis for Brandon Barker, University of Tennessee, Knoxville
Repo for work for my undergraduate senior thesis at the University of Tennessee, Knoxville.

A copy of my thesis in the university's open-access database can be found [here](https://trace.tennessee.edu/utk_chanhonoproj/).

For this project, I found analytic forms for the right and left eigenvectors
of the flux Jacobian of the Euler equations of hydrodynamics with an additional conservation law
for electrons. They are compatible with a tabulated equation of state suitable for simulations of core-collapse supernovae.
This allows us to perform characteristic slope limiting, which has been shown
to be more efficient than limiting directly on the conserved variables, without the need
for numerically diagonalizing the flux Jacobian.
This has been implemented in [thornado](https://github.com/endeve/thornado), and initial
1D tests have been performed, showing the superior performance of the characteristic limiter.
We hope that this work will improve the fidelity of CCSN simulations.

The work done here will be extended to include 2D tests and published soon after.

Example of a test Riemann problem showing the significant improvements of characteristic limiting: 
![plot](./characteristic_cw.png)
