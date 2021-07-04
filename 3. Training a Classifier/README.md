# **Fastai : Training a Classifier**

The [**DigitClassifier**](https://github.com/ThinamXx/Fastai/blob/main/3.%20Training%20a%20Classifier/DigitClassifier.ipynb) notebook contains all the dependencies required for **Image Classification** project from scratch.  

**Getting the Data**
- I will download a sample of MNIST.

**Pixel Similarity**
- I will get the average of pixel values for each groups of 3 and 7. I will create a tensor containing all the 3s stacked together. I have presented the simple implementation of Pixels and Computer Vision using Fastai here in the snapshot.

![Image](https://github.com/ThinamXx/300Days__MachineLearningDeepLearning/blob/main/Images/Day%20198.PNG)

**L1 and L2 Norm**
- Taking the mean of absolute value of differences is called Mean Absolute Difference or L1 Norm. Taking the mean of square of differences and then taking the square root is called Root Mean Squared Error or L2 Norm. I have presented the simple implementation of Arrays and Tensors, L1 and L2 Norm using Fastai here in the snapshot.

![Image](https://github.com/ThinamXx/300Days__MachineLearningDeepLearning/blob/main/Images/Day%20199.PNG)

**Stochastic Gradient Descent**
- The steps of **Gradient Descent** process are: 
  - Step 1: Initialize the Parameters
  - Step 2: Calculate the Predictions
  - Step 3: Calculate the Loss
  - Step 4: Calculate the Gradients
  - Step 5: Step the Weights
  - Step 6: Repeat the Process
  - Step 7: Stop
 
 ![Image](https://github.com/ThinamXx/300Days__MachineLearningDeepLearning/blob/main/Images/Day%20201.PNG)

**Accuracy and Loss Function**
- The key difference between metric such as accuracy and loss function is that the loss is to drive automated learning and the metric is to drive human understanding. The loss must be a function with meaningful derivative and metrics focuses on performance of the model. The function weights\*pixels is not flexible. I will initialize a random number to intercept as well. In Neural Networks the equation y=w\*x+b, w is called the weights and the b is called the bias. Together the weights and bias make up the parameters. The Sigmoid function always outputs a number between 0 and 1. I have presented the implementation of Loss Function and Sigmoid using Fastai and PyTorch here in the snapshot.

![Image](https://github.com/ThinamXx/300Days__MachineLearningDeepLearning/blob/main/Images/Day%20203.PNG)
