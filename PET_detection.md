---
title: Detection and Segmentation in a large cohort of DLBCL
subtitle: 18F-FDG
---

## Objective 
Aim of the present study is to evaluate the performance of a deep convolutional neural networks to detect and segment PET abnormalities in a large population of DLBCL.

## Material & Methods
[Proprocessing](https://github.com/paul-bd/GAINED_repo/blob/master/GAINED_load_and_resample.ipynb) to a 128x128x256 tensor of 4mm3 voxel
 
Dataset was splitted into a training (373 patients), a validation (92 patients) and a testing (93 patients) cohort
A U-net was trained with a custom loss function taking into accound the spectral hierarchy of PET images.

Main metrics were 
 - For the detection task : Sensitivity, PPV at the lesion levels. Sensitivity, Specificity, PPV, NPV at the voxel level
 - For the segmentation task : the Dice similarity coefficient (DSC)
 
## Results per patient
BLUE BOUNDING BOXES are False Negatives 
RED BOUNDING BOXES are False Positives
![Img1](img/detection/11011101021002.jpg)
![Img1](img/detection/11011101021008.jpg)
![Img2](img/detection/11011101021014.jpg)
![Img2](img/detection/11011101031003.jpg)
![Img2](img/detection/11011101051009.jpg)
![Img2](img/detection/11011101051015.jpg)
![Img2](img/detection/11011101051026.jpg)
![Img2](img/detection/11011101061010.jpg)

## Results in the validation cohort of 90 patients
Main results at the lesion / Voxel level

![Img3](img/detection/results/Results_m.jpg)


Distribution of DSC 

![Img4](img/detection/results/DSC_distrib_m.jpg)


Scatter plot of MTV predicted / MTV ground truth

![Img5](img/detection/results/modified_predictionsMTV_scatter.jpg)

## Source Code : 
 - [GAINED Proprocessing](https://github.com/paul-bd/GAINED_repo/blob/master/GAINED_load_and_resample.ipynb) 
 - [Analysis of predictions](https://github.com/paul-bd/GAINED_repo/blob/master/check_preds.ipynb)
