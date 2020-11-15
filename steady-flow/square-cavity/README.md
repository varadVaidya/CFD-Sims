# Steady Flow in a Square Cavity

The velocity profile in the square cavity can be written as:  
  
![vel-image](https://latex.codecogs.com/png.latex?%5Cfrac%7Bd%20u%7D%7Bd%20x%7D%20&plus;%20%5Cfrac%7Bd%20v%7D%7Bd%20y%7D%20%3D%200)

This is simulated in OpenFoam (v7), with the dimension for the cavity are 1 x 1 m and the lid is driven along positve x with velocity 1 m/s
The cells size is 50*50 and the block is one cell thick.

The commands for this are:

    foamCleanTutorials
    foamCleanPolyMesh

    blockMesh
    checkMesh

    simpleFoam > log.simpleFoam

    paraFoam



# Results
## For Reynolds Number of 200
  
The velocity profile develops as:
  
![vel-profile](results/Re-200/velocity.gif?raw=True)  
  
The final velocity profile is:  
  
![final-vel](results/Re-200/velocity-profile.png?raw=True)  
  
The final pressure profile develops as:
  
![final-pressure](results/Re-200/pressure-profile.png)  
  
## For Reynolds Number of 1000
The velocity profile develops as:
  
![vel-profile](results/Re-1000/velocity.gif?raw=True)  
  
The final velocity profile is:  
  
![final-vel](results/Re-1000/velocity-profile.png?raw=True)  
  
The final pressure profile develops as:  
  
![final-pressure](results/Re-1000/pressure-profile.png)  
