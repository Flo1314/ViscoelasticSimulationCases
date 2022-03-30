# ViscoelasticSimulationCases
This repository is used to store different Openfoam/Rheotool cases for viscoelastic simulations.  
The implementations are compatible with Openfoam V7 and Rheotool of70.

**This branch** defines the 2D Newtonian 4:1 contraction with symmetric bottom BC.

## Directory structure
`0/`  
* p - defines the unit of p, its initial field values and boundary conditions  
* tau - defines the unit of tau, its initial field values and boundary conditions
* theta - defines the unit of theta, its initial field values and boundary conditions  
* U - defines the unit of U, its initial field values and boundary conditions

`constant/`  
* constitutiveProperties - units dimensions and values of rho, eta, etaP and  lambda and a stabilization method for coulping  

`system/`  
* blockMeshDict - defines the whole mesh and boundary conditions for different patches  
* controlDict - defines startTime, endTime, etc.  
* fvSchemes - defines FV discretization schemes (ddt Schemes, grad Schemes, div schemes, interpolation schemes etc.)  
* fvSolution - defines system solvers (including maxiteration, tolerance), preconditioner and coupling algorithms

## Usefull commands
`./Allrun` - starts the whole simulation at once  
`./Allclean` - removes all (from ./Allrun generated) data, to get a clean repository again  
`paraFoam` - opens results in paraview  
`foamToVTK` - generates VTK-files to easily store or share the data after computation  

*all commands to be called from the toplevel directory
