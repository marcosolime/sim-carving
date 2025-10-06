# 3D Volume Reconstruction from Cylindrical Ray Casting

This project demonstrates a simple 3D reconstruction technique using **ray casting** around an object, inspired by photo-thermoelectric (PTE) imaging concepts. Rays are generated from a cylindrical distribution around the target (a cube) and cast inward. Each ray has a binary transmission value:  
- **1 (transmitted)** means the ray passes through without hitting the object.  
- **0 (blocked)** means the ray intersects the cube, and the corresponding voxels along the ray’s interior path are marked as filled.  

The algorithm reconstructs the 3D volume by progressively filling the grid with information inferred from blocked rays. The result is saved as a `.npy` file for further visualization and analysis.

![3D Reconstruction Visualization](reconstruction_example.png)
