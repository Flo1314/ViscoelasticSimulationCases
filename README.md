# ViscoelasticSimulationCases
This repository is used to store different Openfoam/Rheotool cases for viscoelastic simulations.

The current base case is the 2D Newtonian 4:1 contraction.

0/ contains the initial flow variables and field data
constant/ contains (constitutive) properties such as the values for rho, eta and lambda
system/ contians the mesh, timestep size, endtimestep, FV discretization schemes and solvers

Use ./Allrun to start the whole simulation at once.
Use ./Allclean, to remove all (from ./Allrun generated) data, to get a clean repository again.
Use paraFoam to view the results in paraview.
Use foamToVTK to generate VTK data files to store or share the data after computation.

