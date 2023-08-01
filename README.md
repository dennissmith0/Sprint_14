# Sprint_14: Neural Networks Foundations

# Architect
We began this assignment by loading a subset of the QuickDraw dataset, containing doodles from 10 categories. The dataset was divided into X (the features) and y (the labels). We preprocessed the data by normalizing the pixel values in X to fall within the range of 0 to 1.

Next, we built a sequential neural network model using Keras. This model included three hidden layers with 500, 250, and 100 nodes, all using the ReLU activation function. The output layer used the softmax activation function and was designed to have one neuron for each class in our data.

We compiled the model with the SGD optimizer and the sparse categorical cross-entropy loss function, then trained it for 20 epochs. Upon examining the training and validation losses and accuracies, we identified signs of overfitting in our model.

In the final part of the assignment, we experimented with changing the model's optimizer to Adam and discussed the potential impact of changing the activation function from ReLU to sigmoid. We explored the effects of these changes on the model's performance and learning outcomes.

# Train

We experimented with various hyperparameters to optimize a neural network model for a multi-class classification problem using the QuickDraw-10 dataset. We created a function to build and compile the model, which had one hidden layer with 250 nodes and an output layer with 10 nodes. We then conducted a series of experiments to assess the impact of input data normalization, batch size, learning rate, and optimizer type on the model's performance. We used TensorBoard to visualize the training process and results. Based on these experiments, we identified the best performing model configuration.

# Tune

We optimized a neural network to classify hand-drawn images from the QuickDraw-10 dataset. We loaded and normalized the data, defined a customizable model architecture, and set a range for various hyperparameters. We then used Keras Tuner's Bayesian Optimization to find the optimal hyperparameters. Bayesian Optimization builds a probability model of the objective function to intelligently suggest promising hyperparameters, resulting in an efficient search process. We trained and evaluated models using these parameters, aiming to find the best-performing model configuration.

# Deploy
