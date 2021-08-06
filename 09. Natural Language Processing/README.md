# **Fastai : Natural Language Processing**

The [**NLP**](https://github.com/ThinamXx/Fastai/blob/main/9.%20Natural%20Language%20Processing/NLP.ipynb) notebook contains all the dependencies required build **Language Model** that can generate texts and a **Classifier Model** that determines whether a review is positive or negative. It presents the state of art **Classifier Model** which is build using a pretrained language model and fine tuned it to the corpus of task. Then the **Encoder** model is used for classification. 

**Note:**
- 📑[**Natural Language Processing**](https://nbviewer.jupyter.org/github/ThinamXx/Fastai/blob/main/9.%20Natural%20Language%20Processing/NLP.ipynb)

**Loading the Data**
- I will get the IMDB Dataset here. I have presented the implementation of Loading the Data and Word Tokenization using Fastai and PyTorch here in the snapshot. **Token** is a element of a list created by the Tokenization process which could be a word, a part of a word or subword or a single character. 

![Image](https://github.com/ThinamXx/300Days__MachineLearningDeepLearning/blob/main/Images/Day%20232.PNG)

**Word Tokenization**
- Word Tokenization splits a sentence on spaces as well as applying language specific rules to try to separate parts of meaning even when there are no spaces. Generally punctuation marks are also split into separate tokens. Token is a element of a list created by the Tokenization process which could be a word, a part of a word or subword or a single character.

**Subword Tokenization**
- Word Tokenization relies on an assumption that spaces provide a useful separation of components of meaning in a sentence which is not always appropriate. Languages such as Chinese and Japanese don't use spaces and in such cases Subword Tokenization generally plays the best role. Subword Tokenization splits words into smaller parts based on the most commonly occurring sub strings. I have presented the implementation of Subword Tokenization and Numericalization using Fastai and PyTorch here in the snapshot.

![Image](https://github.com/ThinamXx/300Days__MachineLearningDeepLearning/blob/main/Images/Day%20233.PNG)

**Numericalization**
- Numericalization is the process of mapping tokens to integers. It involves making a list of all possible levels of that categorical variable or the vocab and replacing each level with its index in the vocab. I have presented the implementation of Creating Data Loaders and Data Block for Language Model using Fastai and PyTorch here in the snapshot.

![Image](https://github.com/ThinamXx/300Days__MachineLearningDeepLearning/blob/main/Images/Day%20234.PNG)

**Training the Classifier Model**
- I will use Embeddings to convert the integer word indices into activations that can be used for the neural networks. These embeddings are feed into Recurrent Neural Network using and architecture called AWD-LSTM. Encoder is defined as the model which doesn't contain task specific final layers. The term Encoder means much the same thing as body when applied to vision CNN but Encoder tends to be more used for NLP and generative models. I will train the Classifier with discriminative learning rates and gradaul unfreezing. In computer vision unfreezing the model at once is common approach but for NLP Classifier unfreezing a few layers at a time will make a real difference. I have presented the implementation of Training Text Classifier Model using Discriminative Learning Rates and Gradual Unfreezing using Fastai and PyTorch here in the snapshot.

![Image](https://github.com/ThinamXx/300Days__MachineLearningDeepLearning/blob/main/Images/Day%20235a.PNG)
![Image](https://github.com/ThinamXx/300Days__MachineLearningDeepLearning/blob/main/Images/Day%20235b.PNG)
