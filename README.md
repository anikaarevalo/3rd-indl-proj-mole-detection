# Mole detection AI app for skinCare 


## Description
**skinCare**, a healthcare company, is in the process of launching **an AI solution that classifies skin lesions**. The company plans on presenting a prototype to their clients (i.e. professionals and experts in the field of skin medicine) whose patients stand to benefit from a tool that would be able to detect moles that need to be handled by doctors.

<img width="668" src="https://github.com/anikaarevalo/3rd-indl-proj-mole-detection/blob/150e1e90ca0d19021bd9b437a036cccd73ca3d0e/assets/app.png">

As the data scientist contracted for the job, my approach to this short mission is **transfer learning using a pre-trained deep learning model called MobileNet for image classification**. To create an end-to-end machine learning solution, I first started by downloading the HAM10000 dataset from Kaggle which were the raw materials from which a web app to classify skin lesions is based on. 


<img width="1000" alt="pipeline 2022-04-21 at 15 49 28" src="https://github.com/anikaarevalo/3rd-indl-proj-mole-detection/blob/1bc14242324b1a28bcafe6e9b70d25490d677caf/assets/TL_workflow.png">


Suffice it to say, the **key components of this machine learning API pipeline are:** 


<img width="668" alt="pipeline 2022-04-21 at 15 49 28" src="https://github.com/anikaarevalo/3rd-indl-proj-mole-detection/blob/2cb7df413f6427dfadc0db57f97e852fd205fba8/assets/ML_deploy.jpeg">


I. **Data Augmentation using Keras** to augment training data during pre-processing;

II. **Keras Callbacks** while compiling the model during training phase ; and

III. (Models run locally in the browser, meaning that the user’s data never leaves their device.)



## Installation
The following software and tools were utilised in this project:

1. Data analysis
- Python 3.9 or higher
- Pandas and Numpy
- Matplotlib 

2. Machine learning
- Scitkit Learn
- Tensorflow 2.3.0
- Keras

3. Web application deployment
- 


## Usage
This is an easily-accessible yet effective **application that accurately detects and classifies skin lesions based on a photographic image**. At this stage of the product cycle development, it is **a proof of concept that skinCare can show to their clients, such as dermatologists,** who are open to leveraging AI in their own practice. 


## Visuals
**A light visual exploratory analysis of the metadata of skin lesions**



This dataset consists of seven different types of skin diseases: actinic keratoses and intraepithelial carcinoma (**AKIEC**), basal cell carcinoma (**BCC**), benign keratosis-like lesions (**BKL**), dermatofibroma (**DF**), melanoma (**MEL**), melanocytic Nevi (**NV**), and vascular lesions (**VASC**). ***This bar plot shows that the distribution of samples is uneven, and this knowledge is taken into account in the pre-processing phase of the machine learning pipeline.*** 


## Contributor
Anika Arevalo, Junior Data Scientist⚛️ (BeCode, Ghent)


## Timeline
8 days

16/05/2022 - 25/05/2022


## Personal situation



## Pending things to do
- Methods to improve performance metrics so as to minimize the tendency of a deep learning model to overfit
- Methods to increase predictive power of the model per class
- Use other deep learning models that are more effective and efficient 
- Develop this mole detection app prototype into a full-fledged minimum viable product 
