# 3D-Reconstruction
## SMERF

### Introduction

- 
- Google Deep Mind
- Streamable, multi-room NeRFs with cm-level detail

### Features

- Sweet spot between the speed of 3D Gaussian Splatting & the quality of Zip-NeRF
- Support mobile, laptop, desktop
- Comparison with 3DGS
  - way less artifacts
  - far more forgiving capture requirements
  - less floaters
  - can reproduce effects, e.g.  tiling textures on the floor, reflections on the screen (like those in NeRFs but cannot be achieved in 3DGS)
- can train on distorted fisheye & perspective photos as long as they're taken by the camera that's been placed in the same location
- allows texture editing with 2D software (PhotoShop, Firefly, etc.) thanks for Nuvo (provides neural fields for uv mapping)



### Limitations

- Requires extensively training



### Theory

- teacher model: Zip-NeRF; student model: SMERF



### Applications

- Google Maps, immersive view, used to explore interiors & exteriors in high fidelity



## 3D Gaussian Splatting (3DGS)

### Introduction

- Gaussian Splatting = Radiance Field - slower Neural Rendering part
- classical computer graphics + modern deep learning techniques

### Features

- has an explicit representation; represent the scene as a collection of gaussians (ellipsoidal splats)
- way faster than NeRFs
- better photorealistic effects than photogrammetry
- support 3D editing (select, move, delete, relight)



### Limitations

- 

### Theory

- use Spherical Harmonics to represent all view-dependent effects & lighting (glint, veneer, specularities)

### Applications



## NeRFs



### Limitations

- hard to edit: if turned into a mesh, the geometry & the uv maps are like disaster. Even simple texture editing is impossible. (Solved in Nuvo)



## Photogrammetry

### Introduction



### Features



### Limitations



### Theory



### Applications

