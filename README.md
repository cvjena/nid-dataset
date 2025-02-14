# NID Dataset

This folder contains the NID dataset prepared for the evaluation
of insect detection and localization algorithms. If you use this dataset, please 
cite the corresponding paper:

D. Korsch, P. Bodesheim, G. Brehm, and J. Denzler.
Automated Visual Monitoring of Nocturnal Insects with Light-based Camera Traps.
CVPR Workshop on Fine-grained Visual Classification (CVPR-WS), 2022.

For more details visit the website of the dataset:
https://inf-cv.uni-jena.de/nid_dataset/

## Directory Information

- ``images/``
    This directory contains subdirectories named after the corresponding moth species and each subdirectory contains the sample images of that species

- ``images.txt``
    The filenames of the images relative to the images directory
    Each line contains a separate image.

- ``multi_boxes.json``
    Bounding box annotations for the insects in json format.
    For each image from images.txt, there is a list of objects and each object is specified by box coordinates (x0,y0) and (x1,y1) with ranges between 0 and 1 relative to the image size.

- ``tr_ID.txt``
    Proposed train-test-split for each image in images.txt. 
    Each line in tr_ID.txt corresponds to the image in the same line in images.txt. 
    A value of 0 means that this image is used for testing and a value of 1 means this image is used for training.
    

