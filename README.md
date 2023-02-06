# Data Sets For Our Study On Automatic Annotation Of New Objects

These data sets have been created for a project concerning continuous learning for object detection tasks on a homogeneous background. One main goal in this study was the automatic annotation of new objects including bounding box coordinates (see reference below). The two data sets presented here have been used for evaluating our approach. The first data set includes objects on a white background; all images have been taken and manually annoteted by our team. The second is a subset of the [iCubWorld data set](https://robotology.github.io/iCubWorld); the annotations provided here are created by us.

## Fruits Data Set

This data set consists of five different artificial fruits and vegetables (tomato, onion, apricot, cucumber, banana) on a white background. Approximately half of the images contain a single object, the rest contains a mix of different objects. Image sizes are 708x531 and 576x432 resp. 531x708 and 432x576. The images have been manually annotated using the tool [LabelImg](https://github.com/heartexlabs/labelImg). The data is split into training and validation data sets (approximately 90% resp. 10% of the images). Additionally, we created a test data set with 100 images of size 800x600. Each image of the test data set contains exactly one object on a white background. This data set consists of 20 classes (5 images for each class), including the training objects as well as new objects (e.g. other fruits and vegetables, pliers, measuring tape).

## iCubWorld Data Set

The original [iCubWorld data set](https://robotology.github.io/iCubWorld) contains more than 400k images of 20 different classes, including annotations for object detection. Due to automatic generation of the image annotations in the context of a human-robot-interaction, the original bounding box information is not optimal in many cases. For this reason, we created our own ground truth annotations for a subset of 659 images of seven object classes (mug, pencil case, ring binder, soap dispenser, soda bottle, squeezer, sunglasses) with 83-105 images per class and split this into training and validation data set (90% resp. 10% of the images). The test set is different subset of 82 images containing all 20 object classes. The annotation files for this manually labeled subset can be found here.


## Reference
If you use this data set, please cite our paper:
```
@misc{10.48550/arxiv.2206.00280,
  title = {Automatic Bounding Box Annotation with Small Training Data Sets for Industrial Manufacturing},
  author = {Gei{\ss}, Manuela and Wagner, Raphael and Baresch, Martin and Steiner, Josef and Zwick, Michael},
  doi = {10.48550/ARXIV.2206.00280},
  url = {https://arxiv.org/abs/2206.00280}, 
  keywords = {Computer Vision and Pattern Recognition (cs.CV), Machine Learning (stat.ML), FOS: Computer and information sciences, FOS: Computer and information sciences},  
  publisher = {arXiv},  
  year = {2022},  
  copyright = {Creative Commons Attribution 4.0 International}
}
```

More background information on our project can be found here:
```
@InProceedings{10.1007/978-3-031-14343-4_22,
author={Gei{\ss}, Manuela and Baresch, Martin and Chasparis, Georgios and Schweiger, Edwin and Teringl, Nico and Zwick, Michael},
title={Fast and Automatic Object Registration for Human-Robot Collaboration in Industrial Manufacturing},
booktitle={Database and Expert Systems Applications - DEXA 2022 Workshops},
year={2022},
publisher={Springer International Publishing},
address={Cham},
pages={232--242},
isbn={978-3-031-14343-4}
}
```