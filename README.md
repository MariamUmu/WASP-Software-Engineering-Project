# WASP-Software-Engineering-Project
This repository is created by Mariam Taha &amp; Aso Bozorgpanah to do WASP Software Engineering Project

Machine Learning and Deep Learning by different libraries
#Regression This notebook introduced a few techniques to handle a regression problem.
Mean Squared Error (MSE) is a common loss function used for regression problems (different loss functions are used for classification problems). Similarly, evaluation metrics used for regression differ from classification. A common regression metric is Mean Absolute Error (MAE). When numeric input data features have values with different ranges, each feature should be scaled independently to the same range. If there is not much training data, one technique is to prefer a small network with few hidden layers to avoid overfitting. Early stopping is a useful technique to prevent overfitting.

'''Demonstrate overfitting''' The simplest way to prevent overfitting is to start with a small model: A model with a small number of learn-able parameters (which is determined by the number of layers and the number of units per layer). In deep learning, the number of learn-able parameters in a model is often referred to as the model's "capacity".
Indeed, deep learning models tend to be good at fitting to the training data, but the real challenge is generalization, not fitting.
On the other hand, if the network has limited memorization resources, it will not be able to learn the mapping as easily. To minimize its loss, it will have to learn compressed representations that have more predictive power. At the same time, if you make your model too small, it will have difficulty fitting to the training data. There is a balance between "too much capacity" and "not enough capacity".
Intuitively, a model with more parameters will have more "memorization capacity" and therefore will be able to easily learn a perfect dictionary-like mapping between training samples and their targets, a mapping without any generalization power, but this would be useless when making predictions on previously unseen data
Unfortunately, there is no magical formula to determine the right size or architecture of your model (in terms of the number of layers, or the right size for each layer). You will have to experiment using a series of different architectures.
To find an appropriate model size, it's best to start with relatively few layers and parameters, then begin increasing the size of the layers or adding new layers until you see diminishing returns on the validation loss.
Some information about trending the training and validation losses This is apparent if you plot and compare the validation metrics to the training metrics.
It's normal for there to be a small difference. If both metrics are moving in the same direction, everything is fine. If the validation metric begins to stagnate while the training metric continues to improve, you are probably close to overfitting. If the validation metric is going in the wrong direction, the model is clearly overfitting.
here are the most common ways to prevent overfitting in neural networks:
Get more training data. Reduce the capacity of the network. Add weight regularization. Add dropout. Two important approaches not covered in this guide are:
data-augmentation batch normalization Remember that each method can help on its own, but often combining them can be even more effective. 

######Project structure
This project is composed of two major files:

/Regression.ipynb: this file contains all the source code to train  and build our ML model with some test functions
/tests/test_Regression.ipynb: this file contains  source code to testing too
If you have any questions or improvements about this work, feel free to open an issue.

