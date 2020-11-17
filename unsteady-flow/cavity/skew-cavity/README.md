# Unsteady Flow Simulation in Square Cavity 
Lid-Driven Square cavity actually has a steady state solution. So using the unsteady solver in OpenFoam the residual does converge to zero.\
  

For unsteady simulation the solver used is : `icoFoam`.\
icoFoam solves the incompressible laminar Navier-Stokes equations.
This is simulated in OpenFoam (v7), with the dimension for the cavity are 1 x 1 m and the lid is driven along positve x with velocity 1 m/s .\
The mesh created is non-uniform with more cells near the boundary to account for better near wall physics.

# Results
## For Re 400

The Residual Plot plotred by pyFoam is: The residual approaches 1e-6 and the simulation converges.
![residual](results/Re-400/residual.png)
The velocity profile develops as:
![vel-profile](results/Re-400/velocity.gif)

And the strean line plot is as:
![stream](results/Re-400/stream.gif)

## For Re 800

The Residual Plot plotred by pyFoam is: The residual approaches 1e-6 and the simulation converges.
![residual](results/Re-800/residual.png)
The velocity profile develops as:
![vel-profile](results/Re-800/velocity.gif)

And the strean line plot is as:
![stream](results/Re-800/stream.gif)
