# AI-Image-Classifier
This repository contains the code for an image classification application built using pre-trained deep convolutional networks.

The image classifier is developed in two parts. In the first part, the code is implemented in a Jupyter notebook, where the necessary packages and modules are imported, and the data is preprocessed and augmented using torchvision transforms. A pretrained network, such as VGG16, is loaded and the parameters are frozen. A new feedforward network is defined as a classifier, and the parameters of the classifier are trained while keeping the parameters of the feature network static. The model is then tested on a separate test dataset, and the accuracy is measured.

In the second part, the code is converted into a command-line application. The train.py script allows users to train a new network on a dataset of images and save the model to a checkpoint. Users can choose from different architectures available in torchvision.models and set hyperparameters such as learning rate, number of hidden units, and training epochs. The training loss, validation loss, and validation accuracy are printed out during training. The predict.py script reads in an image and a checkpoint and predicts the most likely image class along with its associated probability. Users can also print out the top K classes and use the GPU for prediction.

The repository also includes a development notebook, which serves as a guide for implementing the image classifier, and a detailed project rubric that outlines the requirements and evaluation criteria.

Feel free to explore the code, experiment with different architectures and hyperparameters, and create your own image classifier!
