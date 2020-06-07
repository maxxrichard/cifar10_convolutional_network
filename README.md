# CIFAR-10 dataset using Convolutional Neural Network
This repository contains the implementation of convolutional neural network in analysing the CIFAR-10 dataset.

## Packages
This project is implemented in python. The following python-based packages are used:

* **tensorflow** : It is an open-source platform for machine learning and deep learning. It has a comprehensive, flexible ecosystem of tools, libraries and community resources that lets developers easily build and deploy ML/DL-powered applications. It offers building and training DL models easily using intuitive high-level APIs like Keras with eager execution, which makes for immediate model iteration and easy debugging. In this project, it is used to build a fully functional convolutional network and analyse the dataset. [More Information](https://www.tensorflow.org/)

* **pickle** : It implements binary protocols for serializing and de-serializing a Python object structure. It is the process whereby a Python object hierarchy is converted into a byte stream, and 'unpickling' is the inverse operation, whereby a byte stream is converted back into an object hierarchy. In this project, the CIFAR-10 dataset is already pickled by using cPickle. So, this package is used to unpickle the dataset. [More Information](https://docs.python.org/3/library/pickle.html)

* **numpy** : It is the fundamental package for scientific computing with python. It offers comprehensive mathematical functions, random number generators, linear algebra routines, Fourier transforms, and more. It provides powerful N-dimensional array, which is fast and versatile in the vectorisation, indexing, and broadcasting concepts for computing. In this project, the NumPy array is used to store the preprocessed dataset and perform mathematical operations. [More Information](https://numpy.org/)

* **matplotlib** : It is a comprehensive library for creating static, animated, and interactive visualisations in python. It also offers 3D interactive plotting which can be zoomed, panned and updated. In this project, it is used for plotting images from the data. [More Information](https://matplotlib.org/index.html)
