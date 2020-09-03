# Geo-FEM Matlab Finite Element routines for 2D poromechanics

This is a set of matlab routines for 2D (plane-strain & axi-symmetric) Finite Element analysis for laplacian, diffusion, elastic & coupled problems, used during the Computational Geomechanics class.

© All rights reserved. ECOLE POLYTECHNIQUE FEDERALE DE LAUSANNE, Switzerland, Geo-Energy Lab, 2015-2020

authors:
Brice Lecampion

See the LICENSE.TXT file for more details.

Weak form operators currently coded:
- Elasticity: stiffness,  pre stress field , boundary loads
- Laplacian
- Mass matrix
- poroelastic Coupling operator 

Problem type currently coded up:
- 2D steady-state flow : confined and unconfined
- 2D transient flow (confined)
- 2D plane-strain elasticity, poroelasticity
- 2D axi-symmetry

Available Element type:
- Linear triangular Element (2D) : Tri3 (for flow and elasticity), Tri6 (for elasticity, poroelasticity)


For mesh generation, either ones directly script it in matlab (for simple geometries), or use available matlab libraries e.g. MESH2D - Delaunay-based unstructured mesh-generation 
(https://ch.mathworks.com/matlabcentral/fileexchange/25555-mesh2d-delaunay-based-unstructured-mesh-generation)

Short description of the different classes 

Element classes - contain the B-matrices, isoparametric mapping etc.

  + ElementTri3
 
+ ElementTri6
