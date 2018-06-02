# wine_tensorflow

This project presents a notebook that uses a neural network devised to predict the rating from a taster by considering as inputs their reviews and the wine variety.

The code is based on the one presented in https://github.com/sararob/keras-wine-model.
However, with modifications: Keras is only used for pre-processing and TensorFlow is used to train and test the model.

The architecture is also slightly different: L2 regularization and dropout are used and more processing units are used in the final layer of the network (after the concatenation prodecure), whilst the loss function used is cross-entropy instead of MSE, since we tackle the problem as a classification one. The ratings are in one-hot encoding format.

## Requirements
* Python >= 2.7
* NumPy >= 1.9
* TensorFlow >= 1.7.0
* ScikitLearn >= 0.19.1
