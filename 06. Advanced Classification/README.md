# **Fastai : Advanced Classification**

The [**Imagenette Classification**](https://github.com/ThinamXx/Fastai/blob/main/6.%20Advanced%20Classification/ImagenetteClassification.ipynb) notebook contains all the dependencies required to train a state of art machine learning model in computer vision whether from scratch or using transfer learning. It contains explanations and implementation of **Normalization**, **Progressive Resizing**, **Test Time Augmentation**, **Mixup Augmentation** and **Label Smoothing**. 

**Note:**
- 📑[**Imagenette Classification**](https://github.com/ThinamXx/Fastai/blob/main/6.%20Advanced%20Classification/ImagenetteClassification.ipynb)

**Progressive Resizing**
- Progressive Resizing is the process of gradually using larger and larger images as training progresses. When the model is training, it helps if the input data is normalized i.e has a mean of 0 and standard deviation of 1. I have presented the implementation of Initializing DataBlock and DataLoaders, Normalization and Progressive Resizing using Fastai and PyTorch here in the snapshot.

![Image](https://github.com/ThinamXx/300Days__MachineLearningDeepLearning/blob/main/Images/Day%20217a.PNG)
![Image](https://github.com/ThinamXx/300Days__MachineLearningDeepLearning/blob/main/Images/Day%20217b.PNG)

**Test Time Augmentation**
- During inference or validation, creating multiple versions of each image using data augmentation and then taking the average or maximum of the predictions for each augmented version of the image is called Test Time Augmentation.

**Mixup Augmentation**
- Mixup Augmentation works as follows:
    - Select another image from the dataset at random.
    - Pick a weight at random.
    - Take a weighted average using the weight from above of the selected image with your image and it will be independent variable.
    - Take a weighted average using the same weight of this image label with your image label and it will be dependent variable.

**Label Smoothing**
- Label Smoothing is a process which replaces all the labels i.e 1s with a number a bit less than 1 and 0s with a number a bit more than 0 for training. It will make training more robust even if there is mislabeled data which results to be a model that generalizes better at inference. I have presented the implementation of Progressive Resizing, Test Time Augmentation, Mixup Augmentation and Label Smoothing using Fastai and PyTorch here in the snapshot.

![Image](https://github.com/ThinamXx/300Days__MachineLearningDeepLearning/blob/main/Images/Day%20218.PNG)
