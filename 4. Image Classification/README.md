# **Fastai : Image Classification**

The [**Image Classification**](https://github.com/ThinamXx/Fastai/blob/main/4.%20Image%20Classification/ImageClassification.ipynb) notebook contains all the dependencies for **Image Classification** such as getting image data ready for modeling i.e presizing and data block summary and for fitting the model i.e learning rate finder, unfreezing, discriminative learning rates, setting the number of epochs and using deeper architectures. It has explanations of cross entropy loss function as well.  

**Note:**
- 📑[**Image Classification**](https://nbviewer.jupyter.org/github/ThinamXx/Fastai/blob/main/4.%20Image%20Classification/ImageClassification.ipynb)

**Getting the Dataset:**
- I will download the [Pets](https://www.robots.ox.ac.uk/~vgg/data/pets/) dataset. The dataset provides images and annotations directories. The Pets dataset website tells that the annotations directory contains information about where the pets are rather than what they are. Since it is a Classification rather than Localization, I will ignore the annotations directory for now. 

**Initializing Datablock and Dataloaders:**
- I have used Resize as an item transform with a large size and RandomResizedCrop as a batch transform with a smaller size. RandomResizedCrop will be added if min scale parameter is passed in aug transforms function as was done in DataBlock call above. I have presented the implementation of Creating and Debugging Data Block and Data Loaders using Fastai and PyTorch here in the snapshot. 

![Image](https://github.com/ThinamXx/300Days__MachineLearningDeepLearning/blob/main/Images/Day%20208.PNG)

**Cross Entropy Loss:**
- Cross Entropy Loss is a loss function which works even when the dependent variable has more than two categories. It results faster and more reliable training. When we first take the Softmax and then the Log Likelihood of that, that combination is called Cross Entropy Loss.

**Softmax Activation Function:**
- The Softmax Activation Function is used in the final layer to ensure that the activations are all between 0 and 1 and that they sum to 1. Softmax is similar to the Sigmoid function. Softmax is the multicategory equivalent of Sigmoid.

**Exponential Function:**
- Exponential Function is defined as e\*\*x where e is a special number approximately equal to 2.718. It is the inverse of natural logarithm function. Exponential Function is always positive and increases very rapidly. I have presented the implementation of Softmax Function and Negative Log Likelihood using Fastai and PyTorch here in the snapshot.

![Image](https://github.com/ThinamXx/300Days__MachineLearningDeepLearning/blob/main/Images/Day%20209.PNG)

**Model Interpretation:**
- I have presented the implementation of Cross Entropy Loss, Confusion Matrix and Learning Rate Finder using Fastai and PyTorch here in the snapshot.

![Image](https://github.com/ThinamXx/300Days__MachineLearningDeepLearning/blob/main/Images/Day%20210.PNG)

**Unfreezing and Transfer Learning:**
- I have presented the implementation of Unfreezing and Transfer Learning and Discriminative Learning Rates using Fastai and PyTorch here in the snapshot. 

![Image](https://github.com/ThinamXx/300Days__MachineLearningDeepLearning/blob/main/Images/Day%20211.PNG)
