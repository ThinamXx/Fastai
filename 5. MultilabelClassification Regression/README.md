# **Fastai : Multilabel Classification and Regression**

The [**Multilabel Classification**](https://github.com/ThinamXx/Fastai/blob/main/5.%20MultilabelClassification%20Regression/MultilabelClassification.ipynb) notebook contains all the dependencies required to understand **Multilabel Classification**. It contains the explanations of initializing **DataBlock** and **DataLoaders**. 

The [**Regression**](https://github.com/ThinamXx/Fastai/blob/main/5.%20MultilabelClassification%20Regression/Regression.ipynb) notebook contains all the dependencies required to understand **Image Regression**. 

**Note:**
- 📑[**Multilabel Classification**](https://github.com/ThinamXx/Fastai/blob/main/5.%20MultilabelClassification%20Regression/MultilabelClassification.ipynb)
- 📑[**Image Regression**](https://github.com/ThinamXx/Fastai/blob/main/5.%20MultilabelClassification%20Regression/Regression.ipynb)

**DataBlock and DataLoaders:**
- Dataset: A collection that returns a tuple of independent and dependent variable for a single item.
- DataLoader: An iterator that provides a stream of minibatches where each minibatch is a couple of a batch of independent variables and a batch of dependent variables.
- Datasets: An iterator that contains a training Dataset and a validation Dataset.
- DataLoaders: An object that contains a training DataLoader and a validation DataLoader.

![Image](https://github.com/ThinamXx/300Days__MachineLearningDeepLearning/blob/main/Images/Day%20213.PNG)

**Binary CrossEntropy**
- I will create a **Learner** which contains four things such as the model, a **DataLoaders** object, an **Optimizer** and the loss function to use. **F.binary_cross_entropy** and its module equivalent **nn.BCELoss** calculate cross entropy on a one hot encoded target but don't include the initial sigmoid. Normally, **F.binary_cross_entropy_with_logits** or **nn.BCEWithLogitsLoss** do both sigmoid and binary cross entropy in a single function. Similarly for single label dataset, **F.nll_loss** or **nn.NLLoss** for the version without initial softmax and **F.cross_entropy** or **nn.CrossEntropyLoss** for the version with initial softmax. 

![Image](https://github.com/ThinamXx/300Days__MachineLearningDeepLearning/blob/main/Images/Day%20214.PNG)

**Image Regression**
- I have presented the implementation of Initializing DataBlock and DataLoaders and Training Image Regression using Fastai and PyTorch here in the snapshot. 

![Image](https://github.com/ThinamXx/300Days__MachineLearningDeepLearning/blob/main/Images/Day%20216a.PNG)
![Image](https://github.com/ThinamXx/300Days__MachineLearningDeepLearning/blob/main/Images/Day%20216b.PNG)
