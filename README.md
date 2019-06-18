# Single Shot Detector (SSD) wrapper ROS
By [Or Tslil](https://github.com/ortslil64), [Tal Feiner](https://github.com/TalFeiner)

## Introduction
This work uses an implementation of [1], forked from the repository (https://github.com/balancap/SSD-Tensorflow).
SSD is an unified framework for object detection with a single network. The intuition behaynd SSD is a multiple convolution
operation with different shapes and sizes, each for different abstract (depth) of the network.
![alt text](images/ssd2.png)
> SSD architecture [1].

The output of such architechture is an array of possible object, each one with its predicted class, location in the image and abounding box.
The loss function of SSD is a combination of a catagorical crossentropy and a mean square error (MSE) of the predicted location and bounding of each object.

## Installation
Dependencies:

* install tensorflow (gpu is recomended)
* install opencv (pip install opencv-python --user)
* Clone the repository
* unzip `ssd_300_vgg.ckpt` file under the `model` folder. 
## Examples




## References
[1] Liu W, Anguelov D, Erhan D, Szegedy C, Reed S, Fu CY, Berg AC. Ssd: Single shot multibox detector. InEuropean conference on computer vision 2016 Oct 8 (pp. 21-37). Springer, Cham.
