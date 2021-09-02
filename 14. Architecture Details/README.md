# **Fastai : Architecture Details**

- The [**Architecture Details**](https://github.com/ThinamXx/Fastai/blob/main/14.%20Architecture%20Details/Architectures.ipynb) notebook contains all the dependencies required to create a complete state of art computer vision models. It presents some aspects of natural language processing as well. 

**Note:**
- 📑[**Architecture Details**](https://nbviewer.jupyter.org/github/ThinamXx/Fastai/blob/main/14.%20Architecture%20Details/Architectures.ipynb)

**Body and Head of Network**
- The head of a neural net is the part that is specialized for a particular task. For a Convolutional Neural Network, it's generally the part after the adaptive average pooling layer. The body of the neural net contains everything except the head of a network and also includes the stem of the network. I will use pretrained model to create the encoder. The last layer of the encoder has 512 features so the head of the network will receive 512X4 features. Here 4 is used because there are 2 images and 2 for concatenation and pooling.

**Splitter Function**
- A splitter is a function that tells the fastai library how to split the model into parameter groups which are used to train only the head of the model during transfer learning. The params is just a function that returns all parameters of a given module. I have presented the implementation of Siamese Network Model, Loss Function and Splitter Function using Fastai and PyTorch here in the snapshot.

![Image](https://github.com/ThinamXx/300Days__MachineLearningDeepLearning/blob/main/Images/Day%20258.PNG)
