# **Fastai : Convolutional Neural Networks**

The [**CNN**](https://github.com/ThinamXx/Fastai/blob/main/12.%20Convolutional%20Neural%20Networks/CNN.ipynb) notebook contains all the dependencies required to understand **Convolutional Neural Networks**. **Convolutions** are just a type of matrix multiplication with two constraints on the weight matrix: some elements are always zero and some elements are tied or forced to always have the same value. 

**Note:**
- 📑[**Convolutional Neural Networks**](https://nbviewer.jupyter.org/github/ThinamXx/Fastai/blob/main/12.%20Convolutional%20Neural%20Networks/CNN.ipynb) 

**Feature Engineering**
- Feature Engineering is the process of creating a new transformations of the input data in order to make it easier to model. I have presented the implementation of Feature Engineering and Mapping a Convolutional Kernel using Fastai and PyTorch here in the snapshot. 

![Image](https://github.com/ThinamXx/300Days__MachineLearningDeepLearning/blob/main/Images/Day%20249.PNG)

**Channels and Features**
- Channels and Features are largely used interchangeably and refer to the size of the second axis of a weight matrix which is the number of activations per grid cell after a convolution. Channels refer to the input data i.e colors or activations inside the network. Using a stride 2 convolution often increases the number of Features at the same time because the number of activations in the activation map decrease by the factor of 4. A channel is a single basic color in an image. For a regular full color images, there are three channels : red, green and blue. Kernels passed to convolutions need to be rank 4 tensors. 

**Strides and Padding**
- If we add a kernel of size ks by ks with ks an odd number then the necessary padding on each side to keep the same shape is ks//2. The general formula for each dimension is (n + 2\*padding - kernel size) // stride + 1.

![Image](https://github.com/ThinamXx/300Days__MachineLearningDeepLearning/blob/main/Images/Day%20251.PNG)

**Receptive Fields**
- The Receptive Field is the area of an image that is involved in the calculation of a layer. In the deeper layers of network, we have semantically rich features, corresponding to larger Receptive Fields. 

**1 Cycle Training**
- 1 Cycle Training is a combination of warmup and annealing. Warmup is the one where learning rate grows from the minimum value to the maximum value and Annealing is the one where it decreases back to the minimum value. 

**Convolutional Neural Networks**
- Convolutions are just a type of matrix multiplication with two constraints on the weight matrix: some elements are always zero and some elements are tied or forced to always have the same value. Batch Normalization adds some extra randomness to the training process. Larger batches have gradients that are more accurate since they are calculated from more data. But larger batch size means fewer batches per epoch which means fewer opportunities for the model to update weights.

![Image](https://github.com/ThinamXx/300Days__MachineLearningDeepLearning/blob/main/Images/Day%20252.PNG)
![Image](https://github.com/ThinamXx/300Days__MachineLearningDeepLearning/blob/main/Images/Day%20253.PNG)
