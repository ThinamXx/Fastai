# **Fastai : Residual Networks**

- The [**ResNets**](https://github.com/ThinamXx/Fastai/blob/main/13.%20ResNets/ResNets.ipynb) notebook contains all the dependencies required to understand the implementation of skip connections which allow deeper models to be trained. **ResNet** is the pretrained model when using **Transfer Learning**. 

**Note:**
- 📑[**Residual Networks**](https://nbviewer.jupyter.org/github/ThinamXx/Fastai/blob/main/13.%20ResNets/ResNets.ipynb)

**Fully Convolutional Neural Networks**
- The idea in Fully Convolutional Networks is to take the average of activations across a convolutional grid. A Fully Convolutional Networks has a number of convolutional layers, some of which will be stride 2 convolutions at the end of which is an adaptive average pooling layer, a flatten layer to remove the unit axis and finally a linear layer.  Larger batches have gradients that are more accurate since they are calculated from more data. But larger batch size means fewer batches per epoch which means fewer opportunities for the model to update weights. I have presented the implementation of Preparing Data and Fully Convolutional Networks using Fastai and PyTorch here in the snapshot.

![Image](https://github.com/ThinamXx/300Days__MachineLearningDeepLearning/blob/main/Images/Day%20254.PNG)

**Identity Mapping**
- Identity Mapping is the process of returning the input without changing it at all which is performed by the identity function. I have presented the implementation of ResNet Architecture and Skip Connections using Fastai and PyTorch here in the snapshot.

![Image](https://github.com/ThinamXx/300Days__MachineLearningDeepLearning/blob/main/Images/Day%20255.PNG)

**Bottleneck Layers**
- Bottleneck Layers use three convolutions: Two 1X1 at the begining and the end and one 3X3. The 1X1 convolutions are much faster which facilitates to use higher number of filters in and out. The 1X1 convolutions diminish and then restore the number of channels so called Bottleneck. The overall impact is to facilitate the use of more filters in the same amount of time. I have presented the implementation of Training Deeper Networks and Bottleneck Layers using Fastai and PyTorch here in the snapshot.

![Image](https://github.com/ThinamXx/300Days__MachineLearningDeepLearning/blob/main/Images/Day%20256.PNG)
![Image](https://github.com/ThinamXx/300Days__MachineLearningDeepLearning/blob/main/Images/Day%20257.PNG)
