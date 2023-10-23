---
name: Marching Cubes (Transvoxel Algorithm)
tools: [Mesh Generation, Computer Graphics]
image: ../images/transvoxel.png
description: Marching cubes is an algorithm to extract a mesh from a 3D scalar field. This project is an efficient implementation of this algorithm based on the Transvoxel Algorithm.
external_url:
---


# Marching Cubes (Transvoxel Algorithm)

The Marching Cubes algorithm is a computational method used to generate a three-dimensional surface mesh from volumetric data. It operates on a grid of voxels and identifies the intersections between the grid cells and an isosuraface. By examining the value of voxels and their neighbors, the algorithm determines the conficuration of triangles needed to approximate the shape of the isosurface. These triangles form a mesh which can be renered and visualized, allowing for the representation of complex three-dimensional structures from volumetric data.

<img src="../images/transvoxel.png" alt="preview" width="400"/>

This project was implemented as for the Game Graphics Course at UCSC, Winter 2022, instructed by Eric Lengyl. I originally implemented this in the provided Game Engine, but I extracted this as an standalone implementation of marching cubes to share on GitHub.

<p class="text-center">
{% include elements/button.html link="https://github.com/iambb5445/Marching-Cubes" text="Learn More" %}
</p>
