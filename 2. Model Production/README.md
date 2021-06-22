# **Fastai : Model to Production**

The [**BearDetector**](https://github.com/ThinamXx/Fastai/edit/main/2.%20Model%20Production/README.md) notebook contains all the dependencies for a complete **Image Classification** project. 

**Note:**
- 📑[**Image Classification: Bear Detector**](https://nbviewer.jupyter.org/github/ThinamXx/Fastai/blob/main/2.%20Model%20Production/BearDetector.ipynb)

**Initializing Dataset:**
- I will use [DuckDuckGo](https://duckduckgo.com/) to download images. It is a privacy first search service with many useful features. I have presented the implementation of Gathering Data for Object Detection using Duck Duck Go and Fastai here in the snapshot. 

![Image](https://github.com/ThinamXx/300Days__MachineLearningDeepLearning/blob/main/Images/Day%20194.PNG)
![Image](https://github.com/ThinamXx/300Days__MachineLearningDeepLearning/blob/main/Images/Day%20195.PNG)

**Data to DataLoaders:**
- DataLoaders is defined as a Fastai class that stores multiple DataLoader objects you pass to it. Resize crops the images to fit a square shape of the size requested using the full width or height. This can result in losing some important details. Therefore I will ask Fastai to pad the images or stretch or squish the images. When the images are squished or stretched, they end up as unrealistic shapes and leading to a model that learns that things look different from how they actually are and results in lower accuracy. Therefore I will randomly select part of the image and then crop to just that part. On each epoch I will randomly select a different part of each image which means that the model can learn to focus on and recognize different features in images. It also reflects how images work in the real world: different photos of the same thing may be framed in slightly different ways.

**Data Augmentation:**
- Data Augmentation refers to creating random variations of the input data such that they appear different but do not change the meaning of the data. RandomResizedCrop is a specific example of Data Augmentation.

**Training the Model:**
- I have presented the implementation of Data Loaders, Data Augmentation and Training the Model using Fastai here in the snapshot.

![Image](https://github.com/ThinamXx/300Days__MachineLearningDeepLearning/blob/main/Images/Day%20196.PNG)

**Model Inference:**
- When the model is used for getting predictions instead of training, it is called Inference. To create a Inference Learner, I will use exported file.  I have presented the implementation of Classification Interpretation, Cleaning Dataset, Inference Model and Parameters using Fastai here in the snapshot. 

![Image](https://github.com/ThinamXx/300Days__MachineLearningDeepLearning/blob/main/Images/Day%20197.PNG)
