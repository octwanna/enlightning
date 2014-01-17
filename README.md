# Enlightning

Simulation software for numerically solving the Navier-Stokes equations using a Runge-Kutta method for the time derivative and a hybrid WENO and DRP scheme for the space derivative. This software was specifically developed to simulate the numerical acoustical propagation of thunder using the SAMRAI adaptive mesh refinement (AMR) library developed by Lawrence Livermore National Laboratory. Although it had/has a specific purpose for my research, it can also be used for simulating general nonlinear acoustics problems using very efficient AMR techniques and runs on top of MPI, making it very scalable to massively parallel machines.

## Notes

Refer to `README.txt` and `INSTALL.txt` for notes and instructions on installation. Also refer to the paper on the simulation in `paper/jr_dissertation.pdf`, the Matlab prototype of the model in `matlab/hybrid.m` and the OpenCL prototype of the model in `opencl/main.c`.

Enlightning relies upon the [zlib](http://www.zlib.net/)(v1.2.8), [HDF5](http://www.hdfgroup.org/HDF5/)(v1.8.7), MPI ([Open MPI](http://www.open-mpi.org)(v1.7.3) or [MPICH](http://www.mpich.org)), and [SAMRAI](https://computation-rnd.llnl.gov/SAMRAI/)(v3.1.0) software libraries.


## Example Simulation of a Mach Reflection
Output from example problem in `input.txt`:
![Screenshot](https://raw.github.com/jonrood/enlightning/master/media/mach_stem1.png)
![Screenshot](https://raw.github.com/jonrood/enlightning/master/media/mach_stem2.png)