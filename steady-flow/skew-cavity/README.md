# Steady Flow in Skew Cavity
This contains numerial analysis for the skwed cavity at various angles.    \
The equation for the lid driven flow in a cavity is given by:
  
  ![vel-image](https://latex.codecogs.com/png.latex?%5Cfrac%7Bd%20u%7D%7Bd%20x%7D%20&plus;%20%5Cfrac%7Bd%20v%7D%7Bd%20y%7D%20%3D%200)


This is simulated in OpenFoam (v7), with the dimension for the cavity are 1 x 1 m and the lid is driven along positve x with velocity 1 m/s \
The cells size is 200*200 and the block is one cell thick.

The commands for this are:

    foamCleanTutorials
    foamCleanPolyMesh

    blockMesh
    checkMesh

    simpleFoam > log.simpleFoam

    paraFoam

For the residual to converge to zero. We have to change the default parameter in `laplacianSchemes` in `fvSchemes` to `Gass linear corrected` to account for the *non-orthogonality* of the mesh.\
This should also be acompained by changing `nNonOrthogonalCorrectors` to some non-zero value.

# Results
The results for various skew angles at various Reynold's numbers are in the directoies named after their skew angle.