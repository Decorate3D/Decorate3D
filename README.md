# Decorate3D: Text-Driven High-Quality Texture Generation for Mesh Decoration in the Wild

<p align="center"><img src="docs/static/teaser/teaser.jpg" width="100%"/></p>

## Introduction

This paper introduces Decorate3D, a flexible and easy-to-use tool to create \& edit 3D objects from images. Given multi-view photos of an object of interest, our approach starts with a textured mesh 3D reconstruction of the object, followed by either manual editing, or text-to-3D texture automatic generation of textures that align with the mesh. Decorate3D decomposes the Neural Radiance Field into an explicit mesh representation and a view-dependent texture, allowing for flexible decoration. One key contribution of Decorate3D is paving the way to text-driven 3D high-quality texture generation, which has remained an unresolved problem. To tackle this challenge, we propose a structure-aware score distillation sampling method to optimize a UV neural texture based on user-defined text and empower an image diffusion model with 3D-consistent generation capability. Furthermore, we introduce a few-view resampling training method and utilize a super-resolution model to obtain high-quality UV textures (2048x2048) for 3D texturing. 
Extensive experiments collectively validate the superior performance of Decorate3D in decorating real-world 3D objects.  

## Code Coming Soon!
