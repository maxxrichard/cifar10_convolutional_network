# CIFAR-10 dataset using Convolutional Neural Network
This repository contains the implementation of convolutional neural network in analysing the CIFAR-10 dataset.

## Packages
This project is implemented in python. The following python-based packages are used:

* **tensorflow** : It is an open-source platform for machine learning and deep learning. It has a comprehensive, flexible ecosystem of tools, libraries and community resources that lets developers easily build and deploy ML/DL-powered applications. It offers building and training DL models easily using intuitive high-level APIs like Keras with eager execution, which makes for immediate model iteration and easy debugging. In this project, it is used to build a fully functional convolutional network and analyse the dataset. [More Information](https://www.tensorflow.org/)

* **pickle** : It implements binary protocols for serializing and de-serializing a Python object structure. It is the process whereby a Python object hierarchy is converted into a byte stream, and 'unpickling' is the inverse operation, whereby a byte stream is converted back into an object hierarchy. In this project, the CIFAR-10 dataset is already pickled by using cPickle. So, this package is used to unpickle the dataset. [More Information](https://docs.python.org/3/library/pickle.html)

* **numpy** : It is the fundamental package for scientific computing with python. It offers comprehensive mathematical functions, random number generators, linear algebra routines, Fourier transforms, and more. It provides powerful N-dimensional array, which is fast and versatile in the vectorisation, indexing, and broadcasting concepts for computing. In this project, the NumPy array is used to store the preprocessed dataset and perform mathematical operations. [More Information](https://numpy.org/)

* **matplotlib** : It is a comprehensive library for creating static, animated, and interactive visualisations in python. It also offers 3D interactive plotting which can be zoomed, panned and updated. In this project, it is used for plotting images from the data. [More Information](https://matplotlib.org/index.html)

## Dataset
A fully-functional convolutional neural network is used to analyse this problem for which a labelled data is required to train the model.

The CIFAR-10 dataset has been used, which is a very famous dataset for image recognition. The CIFAR-10 dataset consists of 60000 32x32 colour images in 10 classes, with 6000 images per class.  The training images and testing images are divided into 50000 and 10000, respectively. The dataset is divided into five training batches and one test batch, each with 10000 images. The test batch contains exactly 1000 randomly-selected images from each class. The training batches contain the remaining images in random order, but some training batches may contain more images from one class than another. Between them, the training batches contain exactly 5000 images from each class. The dataset can be downloaded from [here](https://www.cs.toronto.edu/~kriz/cifar.html). 

The archive contains the files data_batch_1, data_batch_2, ..., data_batch_5, as well as test_batch. Each of these files is a Python 'pickled' object which is produced with cPickle. Each of the batch files contains a dictionary with the following elements:
* data - a 10000x3072 numpy array of uint8s. Each row of the array stores a 32x32 colour image. The first 1024 entries contain the red channel values, the next 1024 the green, and the final 1024 the blue. The image is stored in row-major order, so that the first 32 entries of the array are the red channel values of the first row of the image.
* labels - a list of 10000 numbers in the range 0-9. The number at index i indicates the label of the ith image in the array data.

The dataset contains another file, called batches.meta. It too contains a Python dictionary object. It has the following entries:
* label_names - a 10-element list which gives meaningful names to the numeric labels in the labels array described above. For example, label_names[0] == "airplane", label_names[1] == "automobile", etc.

The sample image of the first two rows is shown below by using the matplotlib package.
<img src="img/img1.png" width="100">
<img src="img/img2.png">
