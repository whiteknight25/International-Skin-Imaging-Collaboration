# Project Name
We need to build  a multiclass classification model using a custom convolutional neural network in TensorFlow. 

Problem statement: To build a CNN based model which can accurately detect melanoma. Melanoma is a type of cancer that can be deadly if not detected early. It accounts for 75% of skin cancer deaths. A solution that can evaluate images and alert dermatologists about the presence of melanoma has the potential to reduce a lot of manual effort needed in diagnosis.



## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)

<!-- You can include any other section that is pertinent to your problem -->

## General Information
The dataset consists of 2357 images of malignant and benign oncological diseases, which were formed from the International Skin Imaging Collaboration (ISIC). All images were sorted according to the classification taken with ISIC, and all subsets were divided into the same number of images, with the exception of melanomas and moles, whose images are slightly dominant.
The data set contains the following diseases:

Actinic keratosis
Basal cell carcinoma
Dermatofibroma
Melanoma
Nevus
Pigmented benign keratosis
Seborrheic keratosis
Squamous cell carcinoma
Vascular lesion

We have built a CNN network from scratch and improved it with few trials. The model architecture consists of the below.
1.  Conv 2d with 32 filters
2.  Max pooling layer
3.  Conv 2d with 32 filters
4.  Max pooling layer
5.  Conv 2d with 64 filters
6.  Max pooling layer
7.  Conv 2d with 64 filters
8.  Max pooling layer
9.  A batch normalization layer
10. A drop out layer with 25% drop out rate
11. Last conv 2d layer with 128 filters
12. Max pooling layer
13. Second batch normalization layer
14. Second dropout layer with 40% drop out rate
15. Flattening layer
16. 1st dense layer with 256 neurons
17. Last dropout layer with 40% dropout rate
18. Softmax output layer



## Conclusions
The final derived model shows overfitting trend as the gap between the training accuracy and validation accuracy is quite large. Still we managed to achieve a validation accuracy close to 80%. 
we belive the model can be further tunes with hyper parameter adjustments and more trials.


## Technologies Used

This assignment is completed in google colab pro and the train/tet files were feed from google drive by mounting the drive in colab. A new folder as Train_Augmented is created in parallel to the given train directory where we store the augmented files under class specific sub directories.

Google drive link for the project 
(https://drive.google.com/drive/u/1/folders/1ZP0rVG18IzBYm9PBLtcJ4mVDbVAagWTw)

- Pandas
- Numpy
- Matplotlib
- Keras
- Tensor flow
- SKLearn 


## Contact
Created by [@whiteknight25] - feel free to contact me!
