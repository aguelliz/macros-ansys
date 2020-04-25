The macros in this folder simulate the nonlinear process of calculating the buckling of a shell-based beam.

The fundamental steps of simulating the buckling are the following: 
-	Preload the beam
-	Obtain the modes
-	Deform the beam with the shape of one of the eigenmodes and a factor f
-	Finally, solve the nonlinear problem of compressing the imperfect beam.

First, open Ansys, make sure that the Ansys directory is the same directory where the macros are stored (file>change directory). 

Now, write in the command line main. This will run the macros, geom, mesh, boundary, and Slinear.

After this observe the modes. Write down the maximum deformation (DMX) of the mode shape you will use to model the nonlinear problem (usually the first mode). 

Save as jobname.db (file>save as jobname.db), and change the filename (file>change jobname..) let’s name it file2.

Run nonlinear analysis, by writing nonlinear in the command line. Compute f as imperfection/DMX, imperfection is usually in the order of hundredths of the length.

Extract the buckling force. 

Main -> runs Geom, Mesh, Boundary and Slinear
Geom -> Generates the geometry
Mesh -> Creates the mesh
Boundary -> Creates the boundary conditions. 
Slinear -> Eigenmode extraction
nonlinear -> Nonlinear analysis

