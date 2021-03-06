# Mole detection AI app for skinCare 


## Description
**skinCare**, a healthcare company, is in the process of launching **an AI solution that classifies skin lesions**. The company plans on presenting a prototype to their clients (i.e. professionals and experts in the field of skin medicine) whose patients stand to benefit from a tool that would be able to detect moles that need to be handled by doctors.

<img width="800" src="https://github.com/anikaarevalo/3rd-indl-proj-mole-detection/blob/150e1e90ca0d19021bd9b437a036cccd73ca3d0e/assets/app.png">

As the data scientist contracted for the job, my approach to this short mission is **transfer learning using a pre-trained deep learning model called MobileNet for image classification**. To create an end-to-end machine learning solution, I first started by downloading the HAM10000 dataset from Kaggle which were the raw materials from which a web app to classify skin lesions is based on. 


<img width="1000" alt="pipeline 2022-04-21 at 15 49 28" src="https://github.com/anikaarevalo/3rd-indl-proj-mole-detection/blob/1bc14242324b1a28bcafe6e9b70d25490d677caf/assets/TL_workflow.png">


Suffice it to say, the **key components of this machine learning API pipeline are:** 


<img width="668" alt="pipeline 2022-04-21 at 15 49 28" src="https://github.com/anikaarevalo/3rd-indl-proj-mole-detection/blob/2cb7df413f6427dfadc0db57f97e852fd205fba8/assets/ML_deploy.jpeg">


I. **Data Augmentation using Keras** to augment training data during pre-processing;

II. **Keras Callbacks** while compiling the model during training phase in order to capture the 'best' version of the model in training ; and

III. The predictive deep learning model runs locally in the browser (there are advantages to local deployment where the user’s data never leaves their device) or deployed via a platform such as Heroku.



## Installation
The following software and tools were utilised in this project:

1. Data analysis
- Google Drive
- Python 3.9 or higher
- Pandas and Numpy
- Matplotlib 

2. Machine learning
- Google Colab
- Scitkit Learn
- Tensorflow 2.3.0
- Keras

3. API deployment (locally and/or mobile)
- Streamlit


## Usage
This is an easily-accessible yet effective **application that accurately detects and classifies skin lesions based on a photographic image**. At this stage of the product cycle development, it is **a proof of concept that skinCare can show to their clients, such as dermatologists,** who are open to leveraging AI in their own practice. 


## Visuals
                         A light visual exploratory analysis of the metadata of skin lesions

<img width="1000" src="https://github.com/anikaarevalo/3rd-indl-proj-mole-detection/blob/fc6260b3adebd658dcff3b706e68eea4bb96e4e7/assets/benchmark_skin_lesion_dataset.png">

This dataset consists of seven different types of skin diseases: actinic keratoses and intraepithelial carcinoma (**AKIEC**), basal cell carcinoma (**BCC**), benign keratosis-like lesions (**BKL**), dermatofibroma (**DF**), melanoma (**MEL**), melanocytic Nevi (**NV**), and vascular lesions (**VASC**). ***This bar plot shows that the distribution of samples is uneven, and this knowledge is taken into account in the pre-processing phase of the machine learning pipeline.*** 


                                 Pre-trained MobileNetv2 model and transfer learning


<img width="500" src="https://github.com/anikaarevalo/3rd-indl-proj-mole-detection/blob/b4526088088ea5b4deab0b71c229e47f61864b5b/assets/Evaluation_report_MobileNetv2_skin_lesion_classifier.png">

The **re-trained MobileNetv2 model** has modest performance and that **a significant number of test examples for label nv were classified correctly**. The model mostly predicts nv (324) and mel (105) correctly, but struggles with akiec and df. The model confuses mel with nv (328), bkl (102), bcc (44) and akiec (32). The model still has much more room for improvement


                                  Model prediction on a sample skin lesion image
                                  
<img width="500" src="https://github.com/anikaarevalo/3rd-indl-proj-mole-detection/blob/e3bbd38958c12afa40a67daf6fe915a6447d4090/assets/vasc_sample.png">



## Contributor
Anika Arevalo, Junior Data Scientist⚛️ (BeCode, Ghent)


## Timeline
8 days

16/05/2022 - 25/05/2022


## Personal situation
The client's request appeared to be straightforward initially i.e. there is demand in the market for a mobile app that can detect skin cancer. But having taken a good look at the available benchmark data sourced from Kaggle, ***classifying skin cancer on the basis of 7 pre-determined skin lesion categories is no simple matter.*** That and the limitations of my resources such as hardware (e.g. my computer does not possess a GPU which is ideal for providing optimal accuracy for deep learning algorithms) were taken into account especially during the re-training phase of my chosen pre-trained CNN. 


## Pending things to do
- Cleaning the code (due to storage issues of the contributor's pc, notebooks were migrated from jupyter to Google colab on the fly. That being said,
she also stopped leveraging Git ops and its versioning capabilities in the middle of this project :( .)
- Methods to improve performance metrics so as to minimize the tendency of a deep learning model to overfit
- **Methods to improve predictive power of the model per class** (the model needs to be properly trained).
- Use other deep learning models that are more effective and efficient 
- Deploy API not only locally but also as a bonafide mobile app
- Develop this mole detection app prototype into a full-fledged minimum viable product 
