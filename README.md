

# An addition to the paper "Boosting Monocular Depth Estimation Models to High-Resolution via Content-Adaptive Multi-Resolution Merging" done with 2 approaches

> S. Mahdi H. Miangoleh\*, Sebastian Dille\*, Long Mai, Sylvain Paris, Yağız Aksoy.
> [Main pdf](http://yaksoy.github.io/papers/CVPR21-HighResDepth.pdf),
> [Supplementary pdf](http://yaksoy.github.io/papers/CVPR21-HighResDepth-Supp.pdf),
> [Project Page](http://yaksoy.github.io/highresdepth/).

[![video](./figures/video_thumbnail.jpg)](https://www.youtube.com/watch?v=lDeI17pHlqo)

## Approach 1
For each segmented region, the corresponding mode of the depth map region will be
the intensity of that region. This has worked considerably well for any kind of object in an image.
The edges of the objects in the result are defined, however, the background depth variation has been
neglected as only the mode of the entire background area is considered. 

## Approach 2
In approach 2, a simple bitwise AND operation is performed between the depth estimate and panoptic
segmentation that gives out a depth estimate with significant depth variance in the background but in
a layered manner. However, in most cases, each object in the foreground undergoes depth variation in
layers alongside the background. This has worked considerably well for any kind of background in
an image. 

##### Check out the results with detailed explantion in the [![report attached] (https://github.com/sharmithag/HiRes-BoostingMonocularDepth/blob/main/Final_Project_Report.pdf)
#### CREDITS:
[1]: https://github.com/intel-isl/MiDaS/tree/v2
[2]: https://github.com/aim-uofa/AdelaiDepth/tree/main/LeReS
[3]: https://github.com/KexianHust/Structure-Guided-Ranking-Loss
[4]: https://github.com/junyanz/pytorch-CycleGAN-and-pix2pix

