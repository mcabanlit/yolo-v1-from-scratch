# YOLO v1 Implementation from Scratch
 
This repository contains an implementation of YOLO v1 found on [Youtube](https://www.youtube.com/watch?v=n9_XyCGr-MI). The dataset (_PascalVOC_YOLO_) for this implementation can be found in [Kaggle](https://www.kaggle.com/datasets/734b7bcb7ef13a045cbdd007a3c19874c2586ed0b02b4afc86126e89d00af8d2)

## Architecture
The architecture for this implementation was based on the paper by Joseph Redmon, Santosh Divvala, Ross Girshick, and Ali Farhadi entitled: You Only Look Once:Unified, Real-Time Object Detection.
![image](https://user-images.githubusercontent.com/102983286/177241855-521291c9-c4af-4c1e-94fe-48f475511284.png)
Our detection network has 24 convolutional layers followed by 2 fully connected layers. Alternating 1 × 1 convolutional layers reduce the features space from preceding layers. We pretrain the convolutional layers on the ImageNet classification task at half the resolution (224 × 224 input image) and then double the resolution for detection (Redmon et al., 2016). 

## Loss Function
The loss function of YOLO v1.

![image](https://user-images.githubusercontent.com/102983286/179166150-3b7480e4-3882-40b5-b12f-a973757147ef.png)
(Redmon et al., 2016) 

## Resources
A video discussion of the code starting from the architecture can be found in this [link](https://drive.google.com/file/d/1vAVuVDqcsFAvn8jQwHO9u_jUh4LBEGDi/view?usp=sharing).

## References
Redmon, J., Divvala, S., Girshick, R., &amp; Farhadi, A. (2016). You Only Look Once:Unified, Real-Time Object Detection. https://doi.org/https://arxiv.org/pdf/1506.02640.pdf 

Persson, A.. (2020). YOLOv1 from Scratch. Youtube. Retrieved July 5, 2022, from https://www.youtube.com/watch?v=n9_XyCGr-MI. 
