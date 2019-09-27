# DL4NLP-2nd-Assignment
Multi Layer Perceptron Classifier (Autodiff) 

In this assignment we implement a logistic regression classifier for this [dataset] (https://www.kaggle.com/iarunava/imdb-movie-reviews-dataset) from scratch.

### Data prepration 
The dataset has test and train splits but for research purposes we used part of the training data as validation. So, after splitting we have the following parts:

  Train: 20000 
  Validation: 5000
  Test: 25000

We also used a feature vector with 2000 features for each of the sentences as a representation.

### Model parameters
The default model is multi-layer perceptron with one hidden layer (200 neurons) and sigmoid as activation function but you can easily add layers and change the activation function.

The model default hyper-parameters are set as follows but you can easily changed the parameters by passing them to the train function:
  Learning rate: 0.1
  Batch size: 20
  Number of epochs: 50
  
### How to use the code
Here is the view only [link](https://colab.research.google.com/drive/14V9vKUeBKfJow_PdlzdQrltsm5DxTwKz) to the colab notebook. Also, by clicking on the ".ipynb" file up there you can see the code and a runtime of it which I ran before.

First you need to make an instance of model class. Then you can set the train, validation, and test data. You can set the input and output shapes using the set_input_layer and set_output_layer methods respectively. After that, you can add any amount of layers with arbitrary neurons using add_layer methods. Finally, you can train the model using train method and giving the hyper-parameter accordingly. 

If you wish to change the activation function for a layer, first you need to implement the function and its derivative and then you can add it in the layer class.
