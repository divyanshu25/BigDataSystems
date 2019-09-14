# BigDataSystems

#Dataset Preparation
You are asked to use at least two different image datasets for your K-class classification task, and K >= 10.
  - (i) Color rich and object rich images like photos of people and buildings together, such as CIFAR-10 (https://www.cs.toronto.edu/~kriz/cifar.html). If you choose K>10, then extract K classes of images from ImageNet (https://github.com/tensorflow/models/tree/master/tutorials/image/imagenet), or Kaggle (https://www.kaggle.com/), or your favorite photo collections or from our own photo collections.
  - (ii) At minimum, you should have 10 images per class. Hint: Most laptop computers can handle training of CNN classifiers on 1000 images easily.

# Problem 2.1 Hand-on Experience with Deep Learning Framework for Building a K-class Image Classifier
Requirement.
  - (1) Choose your favorite deep learning framework, say TensorFlow. After download TensorFlow at https://www.tensorflow.org. Following the instruction to install it on your laptop or desktop computer: https://www.tensorflow.org/install/install_linux#ValidateYourInstallation. There are several options to install TensorFlow on machines without GPU card(s). For example, installing Tensorflow on virtualenv will isolate your Tensorflow’s python environment.
      , a high-level neural networks API, written in
 this homework as it is capable of running on top of TensorFlow, CNTK, or
 Theano.
   
  - (2) Using 80% of the images as the training dataset (say 20 pictures of cat and 20 pictures of dog) and 20% (5 pictures of cat and 5 pictures of dog) as the test dataset.
  - (3) You are asked to show how TensorFlow was used to train a K-class classification model, from input to training in CNN layers, to the output of the trained K-class model, including the storage size of the model in MB, the training accuracy and training time.
  - (4) Then you use your testing images to test your K-class CNN classifier trained by TensorFlow and report the average test accuracy and test time.
  - (5) Outlier Test Scenario. When performing testing on your K-class CNN classifier you have trained, in addition to use the test dataset from the same collection, you are asked to perform an outlier test by creating 10 or more images that do not belong to the K class classification task. For example, if you choose dog and cat as your binary classification task, then create 10 photos of your favorite actor/actress, or favorite cars). Perform outlier test on your classifiers and report your results in a table titled outlier test. Also include 5 examples of your outlier test set.
  - (6) Choose 3 new datasets from the public domain. Using TensorFlow to produce another 3 K-class CNN classifier. Measure the training and testing accuracy and time.
Hint: Here are some example datasets.
MNIST dataset. http://yann.lecun.com/exdb/mnist/.
USPS dataset. https://www.kaggle.com/bistaumanga/usps-dataset
Traffic Sign Recognition. https://www.kaggle.com/c/traffic-sign-recognition LISA dataset: http://cvrr.ucsd.edu/LISA/lisa-traffic-sign-dataset.html p2-trafficsigns. https://github.com/ vxy10/p2-TrafficSigns
The face database. https://www.cl.cam.ac.uk/research/dtg/attarchive/facedatabase.html
You can also find most of them at http://yanzhaowu.me/GTDLBench/datasets/.
Deliverable:
  - (1) provide URL of your open source code package and dataset download.
  - (2) Screen shots of your execution process/environments
  - (3) Input Analysis: Use a table to report your training configuration
parameters:
    -  theinputdataset(size,resolution,storagesizeinKBorMBperimage,
storage size of dataset in MB or GB).
    -  chooseandshow2sampleimagesperclassforallKclassesineach
of the four datasets.
 
    -  the training v.s. testing data split ratio and size used in your CNN training. (Hint: If you use 1000 images with 8:2 training v.s. testing ratio, then 800 for training and 200 for testing.)
    -  Youareaskedtorecordthedefaultneuralnetwork(NN)model,such as LeNet, ResNet, DenseNet, and the default NN structures (e.g., CNN with at least 2~5 convolutional layers), and the default hyper- parameters, such as neuron size, the number of weight filters and size, the min-batch size, #epochs/#iterations (convergence), in a table for the 4 configurations you use to train your 4 CNN classifiers for performing the same classification task.
    - e. Youareaskedtoreportthedefaulterrorthresholdusedinthe TensorFlow default configuration for convergence.
  - (4) Output Analysis: Report the performance comparison and analysis of your K-class CNN classifier:
    -  Youareaskedtoprovideatable(ideallyinanexcelfile,butnot
required) to compare the 4 CNN classifiers (each is trained from one of the 4 datasets in terms of training time, training accuracy, testing time and testing accuracy.
    - YouareaskedtorecordthetrainedmodelsizeinMBforthe4 classifiers in the above table.
    -  You are asked to add the test accuracy and time for your outliner dataset in requirement (5) by testing using all 4 CNN classifiers.
    - Youareaskedtomakeatleastthreeobservationsfromyour experimental comparison of the 4 CNN classifiers.
