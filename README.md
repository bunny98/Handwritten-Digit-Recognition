# Handwritten-Digit-Recognition
Handwritten character recognition is a combination of two fields namely image processing and pattern recognition. There are two approaches involved in Optical Character Recognition for hand written numbers which can be classified as structural approach and statistical approach. In structural approach, a character is identified on the basis of interrelationship and interconnection of various features whereas in statistical approach, data in generated based on input and is assigned to one of the n classes.
Since all handwritten aren’t the same, building a general recognition system which can identify a number which can identify a number with high accuracy is needed. Hence, such systems are developed keeping in mind maximum reliability and need for high performance. In particular, hand written digit recognition for isolated integral number is helpful wherever there is a need to process data without having to invest in manual labor, which saves time, resources and increases efficiency. Thus, it has found applications in various avenues like banking, data analysis, exam evaluation, accounting etc.
Hand written digit recognition can be divided in four stages:
i)	Acquisition of data.
ii)	Preprocessing the data
iii)	Extracting features
iv)	Classification
Preparing CNN Model:
    CNNs are a special type of neural networks.
    In CNN, Neural Networks receive an input, and transform it through a series of hidden layers. Each hidden layer is made up of a set of neurons, where each neuron is fully connected to all neurons in the previous layer. The last fully connected layer is called the output layer.
    CNN can be divided into two parts:
      i) feature learning part : Feature learning is typically done by combining two types of layers: Convolution layers and pooling layers.
      ii) Classification: It is then performed based on the learned features through dense layers.
    We will need the following python libraries to build our neural network.
    NumPy - To perform matrix/vector operations as we are working with Images.
    Matplotlib - To visualize what’s happening with our neural network model.
    Tensorflow, Keras - To create the neural network model with neurons, layers.
Training the Model:
    After creating the model, we need to compile the model for optimization and learning. Adam (gradient descent algorithm) as the optimizer and accuracy as our performance metric.
    After compiling the model, we need to fit the model with the MNIST dataset. Using model fit function. To analyse how our model gets trained with the dataset, we can use history object provided by Keras.
Testing the Model:
    In order to test the model, we can use some images from the testing dataset. These are taken from the testing dataset because these images are unknown to our model, so that we can test our model’s performance easily. 
    We will grab few images from those 10,000 test images and make predictions using model.predict_classes function which takes in the flattened raw pixel intensities of the test image.  
DATASETS
    The dataset used is the MNIST database of handwritten digits. It consists of a training set of 60,000 examples, and a test set of 10,000 examples. The digits have been size-normalized and centered in a fixed-size image. The images are of size 28*28 pixels. It is a good database for people who want to try learning techniques and pattern recognition methods on real-world data while spending minimal efforts on pre-processing and formatting.
