# **Fastai : Language Model from Scratch**

The [**LanguageModel**](https://github.com/ThinamXx/Fastai/blob/main/11.%20Language%20Model/LanguageModel.ipynb) notebook contains all the dependencies that is inside **AWD-LSTM** architecture for **Text Classification**. It presents the implementation of **Language Model** using simple **Linear Model**, **Recurrent Neural Network**, **Long Short Term Memory**, **Dropout Regularization** and **Activation Regularization**.  

**Note:**
- 📑[**Language Model**](https://nbviewer.jupyter.org/github/ThinamXx/Fastai/blob/main/11.%20Language%20Model/LanguageModel.ipynb)

**Loading the Data**
- I will use **Human Numbers** dataset here. It contains the first 10000 numbers written out in English. I will tokenize the dataset by splitting on spaces. Then I will create a list of unique tokens called vocab for Numericalization. Then I will convert the tokens into numbers by looking up in the index of each in the vocab. I have presented the implementation of Preparing Sequence of Tensors for Language Model using Fastai and PyTorch here in the snapshot.

![Image](https://github.com/ThinamXx/300Days__MachineLearningDeepLearning/blob/main/Images/Day%20241.PNG)

**Language Model**
- I will create neural network architecture that takes three words as input and returns the predictions of the probability of each possible next word in the vocab. I will use three standard linear layers. The first linear layer will use only the first words embedding as activations. The second layer will use the second words embedding plus the first layers output activations and the third layer will use the third words embedding plus the second layers output activations. The key effect is that every word is interpreted in the information context of any words preceding it. Each of these three layers will use the same weight matrix. I have presented the implementation of Creating Data Loaders, Language Model from Scratch and Training using Fastai and PyTorch here in the snapshot.

![Image](https://github.com/ThinamXx/300Days__MachineLearningDeepLearning/blob/main/Images/Day%20242.PNG)

**Recurrent Neural Networks**
- I will simplify the neural networks model or module defined above by replacing the duplicated code that calls the layers with a for loop. The module can work equally to token sequences of different lengths. Recurrent Neural Network is a network which is a refactoring of a multilayer neural network using for loop. I will define a stateful Recurrent Neural Network as it remembers its activations between different calls to forward which represents its use for different samples in the batch. I have presented the implementation of Recurrent Neural Networks and Language Model using Fastai and PyTorch here in the snapshot.

![Image](https://github.com/ThinamXx/300Days__MachineLearningDeepLearning/blob/main/Images/Day%20243.PNG)

**Backpropagation Through Time**
- Backpropagation through Time is a process of treating a neural network with effectively one layer per time step as one big model and calculating gradients on it in the usual way. The BPTT technique is used to avoid running out of memory and time which detaches the history of computation steps in the hidden state every few time steps. 

![Image](https://github.com/ThinamXx/300Days__MachineLearningDeepLearning/blob/main/Images/Day%20244.PNG)
![Image](https://github.com/ThinamXx/300Days__MachineLearningDeepLearning/blob/main/Images/Day%20245b.PNG)

**Long Short Term Memory**
![Image](https://github.com/ThinamXx/300Days__MachineLearningDeepLearning/blob/main/Images/LSTM.png)
- The green circles are elementwise operations and the four orange boxes represent four neural network layers which are also called gates with the activations. The first gate from left is called the forget gate. The second gate is called the input gate and the third gate is sometimes called the cell gate. The last gate is the output gate. Tanh is just a Sigmoid function rescaled to the range of -1 and 1. 

**Dropout Regularization**
- Dropout is a regularization technique which randomly changes some activations to zero at a training time.

**Activation Regularization**
- Activation Regularization is a process of adding the small penalty to the final activations produced by the LSTM to make it as small as possible. It is a regularization method very similar to weight decay.

![Image](https://github.com/ThinamXx/300Days__MachineLearningDeepLearning/blob/main/Images/Day%20248.PNG)
