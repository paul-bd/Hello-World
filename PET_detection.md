---
title: Detection and Segmentation in a large cohort of DLBCL
subtitle: 18F-FDG
---

## Objective 
Aim of the present study is to evaluate the performance of a deep convolutional neural networks to detect and segment PET abnormalities in a large population of DLBCL.

## Material & Methods
[Proprocessing](https://github.com/paul-bd/GAINED_repo/blob/master/GAINED_load_and_resample.ipynb) to a 128x128x256 tensor of 4mm3 voxel
 
Dataset included two multi centric trials from the LYSA. Data is not publicly available.
Models were trained using the nnunet library and can be found at this [link](https://github.com/paul-bd/petct_segmentation) : 

## Results per patient
BLUE BOUNDING BOXES are False Negatives 
RED BOUNDING BOXES are False Positives
![Img1](img/detection/11011101021002.jpg)
![Img1](img/detection/11011101021008.jpg)
![Img2](img/detection/11011101021014.jpg)

## Source Code : 
 - [Models](https://github.com/paul-bd/petct_segmentation/models)
 - [Figures](https://github.com/paul-bd/petct_segmentation/figure)
