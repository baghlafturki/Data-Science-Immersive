# Capstone Project: Detecting Atelectasis in lung X-Rays


## Executive summary
### Problem statement
Lung X-ray interpretation is not simple, and requires specialists with many years of experience. In spite of heavy trainings the specialists go thru, they could make mistakes as they are humans and could be easily affected by factors such as fatigue which could impact their decision making proces. This is dangerous because they are dealing with patients lifes and sending a positive patient home could kill them.

### The goal
The goal is to implement a model with a deployable accuracy which aid experts in their decision making process in order to reduce mistakes.

### Methodology
* Data is obtained from [Stanford ML Group](https://stanfordmlgroup.github.io/competitions/chexpert/) which consists of two types of xray images (Frontal and lateral) along with 14 pathologies 

* Data is cleaned and the Atelectasis feature is extracted 

* Experimentation with modeling is performed on the data to determine which works the best
  * Feature extraction using VGG16 and ResNet50
  * Fine tuning VGG16 and ResNet50
  * Training a model from scratch
* Metrics:
  * The focus is on the Area Under Cover (AUC) however, accuracy is also used to track performance

### Findings
1. Producing a convolutional Neural Network (CNN) model with a deployable accuracy (higher than 98% accuracy for healthcare) is a difficult task, this explains why we do not see AI and machine learning deployed in hospitals yet.
2. The best accuracy obtained from this project was 77% when we used VGG16 model to extract the features to train our classification layer
3. Fine tuning an architecture such as VGG16 requires extensive research on the layers and and a thruout understanding of the purpose of each layer which is not an easy task.
4. Creating a model from scratch requires extensive processing power. From my search online, there is no golden rule for layers selection (layer filter size ratio, number of filters ratio, etc...) which makes it a difficult task especially when training time is long but required to see how your model is behaving

### Limitations
1. Limited processing power played a major role in hindering optimization
2. Large dataset file (11GB) makes it difficult to use in both locally and cloud services such as Google Colab

## Dependencies
* The latest version of Keras with all its dependencies installed
* Tensorflow 2 with all dependencies installed
* Pandas, Numpy, sklearn

## Contents
|File name|Where to obtain|Description|
|---|---|---|
|**Capstone_compiled_notebook.ipynb**|Present in repository|Jupyter notebook which contains all the codes and analysis|
|**train.csv**|Present in repository|A file containing the path of the images in CheXpert-v1.0-small with their features for training|
|**valid.csv**|Present in repository|A file containing the path of images in CheXpert-v1.0-small with their features for validation|
|**CheXpert-v1.0-small**|[from here ](https://drive.google.com/open?id=18nxMyJG50mLH3BpWCkZROWn-50HndbTC)[ or register here](https://stanfordmlgroup.github.io/competitions/chexpert/)|A structured folder containing all the sampled X-ray images|
|**atelectasisX_binary_front.npy**|Present in repository|A clean copy of front x-ray image paths (X) for training|
|**atelectasisy_binary_front.npy**|Present in repository|A clean copy of front x-ray Atelectasis feature (y) for training|
|**atelectasisXv_binary_front.npy**|Present in repository|A clean copy of front x-ray image paths (X) for validation|
|**atelectasisyv_binary_front.npy**|Present in repository|A clean copy of front x-ray Atelectasis feature (y) for validation|
|**atelectasisX_binary_lat.npy**|Present in repository|A clean copy of lateral x-ray image paths (X) for training|
|**atelectasisy_binary_lat.npy**|Present in repository|A clean copy of lateral x-ray Atelectasis feature (y) for training|
|**atelectasisXv_binary_lat.npy**|Present in repository|A clean copy of lateral x-ray image paths (X) for validation|
|**atelectasisyv_binary_lat.npy**|Present in repository|A clean copy of lateral x-ray Atelectasis feature (y) for validation|
|**atel_front_FE_vgg_model.h5**|[here](https://drive.google.com/open?id=1dPs6kOfB8EcUv3Z3fk-Bm0aC2eUFn4SK)|Saved artifacts of vgg feature extraction on frontal x-ray experiment|
|**atel_front_FT_resnet_model.h5**|[here](https://drive.google.com/open?id=1BzNy_EJGU0WjNPfkk2leAioXEQIvWXAv)|Saved artifacts of resnet fine tuning on frontal x-ray experiment|
|**atel_front_FT_vgg_model.h5**|[here](https://drive.google.com/open?id=1b_bF1DE9J-UdoANLSOKnee47gb1XQP9C)|Saved artifacts of VGG fine tuning on frontal x-ray experiment|
|**atel_lat_FE_vgg.h5**|[here](https://drive.google.com/open?id=16J4O-nSV8xxa6Iw14eQzyzH7gv8FPCfU)|Saved artifacts of VGG feature extraction on lateral x-ray experiment|
|**atel_lat_FT_vgg.h5**|[here](https://drive.google.com/open?id=1R80Ml9PSIPJaP_0eauZlPIzo37cw201X)|Saved artifacts of VGG fine tuning on lateral x-ray experiment|



