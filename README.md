# Deep-Neural-Network-for-Urban-Sound-Classification
Sound is one of the vital informatics indicating activities, events and even safety issues. UrbanSound database library (https://urbansounddataset.weebly.com/index.html#welcome) is an open dataset source that offers several classes of sound data with audio files in each class. In this project, based on deep neural networks and using the UrbanSound database, the group aims to develop a framework to identify each sound class in urban areas accurately and improve classification performance. 

# Urban Sound Category
<img src="https://raw.githubusercontent.com/wbz596/img/master/Picture1.png?token=ALIMGIHQUY3WJGMCILH7DPC7IGTLO" width="50%" height="50%">

# Methods
1. Our idea is to apply multilayer neural network using Tensorflow in Python to classify each sound clip into a different category. 

2. To determine configuration parameters required by neural network model, such as the number of hidden layers, the number of hidden units in each layer, learning rate and training epochs, we do perform multiple runs and guide our hyperparameters search according to the performance of F measure.

3. Experiments show that two layers neural network with 60 hidden units in each layer works well for the 4 main classes of urban sound. For the 8 sub-classes, we use two layers neural network with 100 hidden units in each layer. 10000 training epochs and 0.01 learning rate can guarantee that a good convergence is reached within acceptable time. For non-linearity, we used tanh in the first hidden layer and sigmoid function in the second layer.
# Experiment
1. We used batch gradient descent optimizer, which means weight vectors are updated once after taking all samples into account. 

2. To do multiple runs, we randomly selected around 70% of the whole dataset as our training data for each run. The cost curve can be calculated for each ru
