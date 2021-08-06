# **Fastai : Collaborative Filtering**

The [**Collaborative Filtering**](https://github.com/ThinamXx/Fastai/blob/main/7.%20Collaborative%20Filtering/CollaborativeFiltering.ipynb) notebook contains all the dependencies required to build a **Recommendation System**. It presents how gradient descent can learn intrinsic factors or biases about items from a history of ratings which then gives information about the data. 

**Note:**
- 📑[**Collaborative Filtering**](https://nbviewer.jupyter.org/github/ThinamXx/Fastai/blob/main/7.%20Collaborative%20Filtering/CollaborativeFiltering.ipynb)

**Loading the Data**
- I will use the subset of [**MovieLens**](https://grouplens.org/datasets/movielens/) dataset. The entire dataset contains tens of millions of movie rankings i.e a combination of a movie ID, a user ID and a numeric rating. The mathematical operation of multiplying the elements of two vectors together and then summing up the result is called **Dot Product**. I have presented the implementation of Initializing Dataset and Creating DataLoaders using Fastai and PyTorch here in the snapshot.

![Image](https://github.com/ThinamXx/300Days__MachineLearningDeepLearning/blob/main/Images/Day%20219.PNG)

**Embedding**
- The special layer that indexes into a vector using an integer but has its derivative calculated in such a way that it is identical to what it would have been if it had done a matrix multiplication with a one hot encoded vector is called **Embedding**. Multiplying by a one hot encoded matrix using the computational shortcut that it can be implemented by simply indexing directly. The thing that multiply the one hot encoded matrix is called the **Embedding Matrix**. 

**Weight Decay Regularization**
- **Weight Decay** consists of adding sum of the squared weights to the loss function. The idea is that the larger the coefficients are, the sharper the canyons will be in the loss function.

![Image](https://github.com/ThinamXx/300Days__MachineLearningDeepLearning/blob/main/Images/Day%20221a.PNG)
![Image](https://github.com/ThinamXx/300Days__MachineLearningDeepLearning/blob/main/Images/Day%20221b.PNG)

