# Semantic Segmentation
### Introduction
The pixels of a road in images using a Fully Convolutional Network (FCN). The FCN is trained on KITTI data set.

### Approach

#### Architecture
The intelligence in the pre-trained network VGG-16 is used in the FCN by replacing the fully connected layer with a 1 X 1 convolution in order to preserve the spatial information. The 1 X 1 convolution output is upsampled using Transpose Convolution to construct the output. Skip Connections are used to prevent the degradation problem.
### Setup
##### Frameworks and Packages
Make sure you have the following is installed:
 - [Python 3](https://www.python.org/)
 - [TensorFlow](https://www.tensorflow.org/)
 - [NumPy](http://www.numpy.org/)
 - [SciPy](https://www.scipy.org/)
##### Dataset
Download the [Kitti Road dataset](http://www.cvlibs.net/datasets/kitti/eval_road.php) from [here](http://www.cvlibs.net/download.php?file=data_road.zip).  Extract the dataset in the `data` folder.  This will create the folder `data_road` with all the training a test images.

##### Run
Run the following command to run the project:
```
python main.py
```

##### Results
The results can be found in the `runs` folder
