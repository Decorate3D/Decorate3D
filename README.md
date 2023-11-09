# Decorate3D: Text-Driven High-Quality Texture Generation for Mesh Decoration in the Wild

<p align="center"><img src="docs/static/teaser/teaser.jpg" width="100%"/></p>

## Introduction
This paper presents Decorate3D, a versatile and user-friendly method for the creation and editing of 3D objects using images. Decorate3D models a real-world object of interest by neural radiance field (NeRF) and decomposes the NeRF representation into an explicit mesh representation, a view-dependent texture, and a diffuse UV texture. Subsequently, users can either manually edit the UV or provide a prompt for the automatic generation of a new 3D-consistent texture. To achieve high-quality 3D texture generation, we propose a structure-aware score distillation sampling method to optimize a neural UV texture based on user-defined text and empower an image diffusion model with 3D-consistent generation capability. Furthermore, we introduce a few-view resampling training method and utilize a super-resolution model to obtain refined high-resolution UV textures (2048$\times$2048) for 3D texturing. Extensive experiments collectively validate the superior performance of Decorate3D in retexturing real-world 3D objects. Project page: https://decorate3d.github.io/Decorate3D/. 

## Dataset
The collected datasets for our experiments can be accessed via the link [Google Driver](https://drive.google.com/file/d/1yF6LNoQejkzMcc0vG_VyS4UEag4J-ODN/view?usp=sharing). It consists of images, mesh and UV texture from 14 real-world objects. 

## Results

We provide some sample results in the path ``docs/samples/'', which include 4 textured mesh, and  360-view videos shown in our project page.

## Code 

It is easy to reproduce the paper. Here are some references that may help. 
- 3D scene reconstruction with NeRF (extracting Mesh & UV): [NeuS](https://github.com/Totoro97/NeuS)
- Depth condition diffusion model: [Diffusion](https://huggingface.co/stabilityai/stable-diffusion-2-depth)
- SDS sample code for 3D: [Threestudio](https://github.com/threestudio-project/threestudio)

For more details, please refer to the paper. 

## Citation

```
@inproceedings{guo2023decorate3d,
    title={Decorate3D: Text-Driven High-Quality Texture Generation for Mesh Decoration in the Wild},
    author={Guo, Yanhui and Zuo, Xinxin and Dai, Peng and Lu, Juwei and Wu, Xiaolin and Cheng, Li and Yan, Youliang and Xu, Songcen and Wu, Xiaofei},
    booktitle={Thirty-seventh Conference on Neural Information Processing Systems (NeurIPS)},
    year={2023},
}
```