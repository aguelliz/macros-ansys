The macros in this folder simulate the the dispersion curves of a square honeycomb (either beam elements or solid elements) to find the existence of bandgaps.

First, open Ansys, make sure that the Ansys directory is the same directory where the macros are stored (file>change directory). 

You can also change the jobname (file>change the jobname). 

Now, write in the command line "main". This will run the macros: geom, matandmesh, and loop.

You will obtain the dispersion curve, you can also write "*status, F" to obtain the list of eigenfrequencies of each datapoint and each mode.

Variables: L = length of the beam, d = height of the section of the beam, nmodes = number of modes, np = number of iterations/datapoints per 
direction in the brillouin zone. The depth of he section is 1, the results are the same independently of the thickness.

Main -> runs Geom,  matandmesh, and loop.
Geom -> Generates the geometry
matandmesh -> Assigns the material type and creates the mesh
Loop -> Creates the Bloch boundary conditions, and solves the modal analysis for every datapoint in the brillouin zone
singlemode -> Creates the bloch boundary condition solves the modal analysis for a single datapoint in the brillouin zone 

