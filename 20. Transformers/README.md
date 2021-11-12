# **Fastai : Transformers Model**

**Note:**
- 📑[**Transformers**](https://github.com/ThinamXx/Fastai/blob/main/20.%20Transformers/Transformers.ipynb)

**GPT2 Model**
- There are several versions of GPT2 Model : [**Transformers Documentation**](https://huggingface.co/transformers/pretrained_models.html). I will inspect the Tokenizer and Model. The Tokenizers in HuggingFace usually do the tokenization and numericalization in one step. The Model can generate predictions. I have presented the implementation of Pretrained GPT2 Model and Tokenizer and Transformed DataLoaders using Fastai and PyTorch here in the snapshot.

![Image](https://github.com/ThinamXx/300Days__MachineLearningDeepLearning/blob/main/Images/Day%20299a.PNG)

**Transformers Tokenizer**  
- Fastai Transform is defined as:
  - an encodes method that is applied when transform is called.
  - a decodes method that is applied when decode method of transform is called.
  - a setups method that sets inner state of Transform.

![Image](https://github.com/ThinamXx/300Days__MachineLearningDeepLearning/blob/main/Images/Day%20299b.PNG)

**Fine Tuning Model**
- Since it is a Language Model, I will pass perplexity as a metric. Perplexity is the exponential of the cross entropy loss function. I have presented the implementation of Initializing DataLoaders, Fine Tuning GPT2Model and LR Finder using Fastai and PyTorch here in the snapshot. 

![Image](https://github.com/ThinamXx/300Days__MachineLearningDeepLearning/blob/main/Images/Day%20300a.PNG)
![Image](https://github.com/ThinamXx/300Days__MachineLearningDeepLearning/blob/main/Images/Day%20300b.PNG)
