# FashionMNIST
Temporal Convolutional Network for Classification on FashionMNIST


Traditionally, Time Series prediction in deep learning has been associated with Recurrent Neural Networks (RNNs) and its variants like LSTMs and GRUs due to their ability to capture temporal dependencies in sequential data. But recently researchers have been implementing convolutional approaches for complex sequential problems to achieve better performance. TCNs provide a consolidated model by combining the characteristics of CNNs and RNNs to capture all levels of information. Like RNNs, TCNs take a sequence of any length and map it to an output sequence of the same length and causal convolutions are introduced in the architecture to prohibit information “leakage” from future to past.

The dataset used in this project is the FashionMNIST, containing a total of 70,000 grayscale images of articles from Zalando, an e-commerce company. There are 60,000 images in the training set and 10,000 images in test set, and each image as 784 pixels. Each training and test have 10 labels, which are the class labels for the experiment. Each row contains a image. The first column depicts the class label and the remaining columns correspond to the pixel numbers i.e. 784 in total, each having a value between 1 to 255 depicting the darkness of the pixel in grayscale.

The two main characteristics of Temporal Neural network (TCN) are: first a 1D Fully Convoluted Network(FCN) where each hidden layer is the same length as the input layer; which makes the length of input layer equal to the output layer. And secondly causal convolutions, which have an output at time T that is convolved only the taking the elements from time T and its previous layers. FCN is used along with dilated convolutions which are similar to causal convolutions but can operate with exponentially large receptive field. The dataset will be modified for this experiment by converting the input type from image to sequential data which will then be fed into TCN model. For optimization of the algorithm, image augmentation will be used.

For setting up the environment for this project python, keras and tensorflow are used. Hyper-parameters that be plan to use for this project : Learning rate, Mini-Batch Size, Number of Epochs.
Parameters: Activation function, structure of neural network, optimization technique.
Performance metrics that will be used in this project are truth table, accuracy, confusion matrix.
