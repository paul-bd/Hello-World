---
title: Detection
subtitle: 18F-FDG
---
#MIP
## Material & Methods
Dataset was splitted into a training (373 patients), a validation (92 patients) and a testing (93 patients) cohort
A U-net was trained with a custom loss function taking into accound the spectral hierarchy of PET images

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

## Results in the validation cohort of 92 patients
Detection / Segmentation
![Img1](img/detection/results/Results_m.jpg)


Distribution of DSC 
![Img1](img/detection/results/DSC_distrib_m.jpg)


Distribution of MTV 
![Img1](img/detection/results/modified_predictionsMTV_scatter.jpg)
