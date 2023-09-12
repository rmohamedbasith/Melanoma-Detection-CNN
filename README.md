# Melanoma-Detection
To build a CNN based model which can accurately detect melanoma. Melanoma is a type of cancer that can be deadly if not detected early. It accounts for 75% of skin cancer deaths. A solution that can evaluate images and alert dermatologists about the presence of melanoma has the potential to reduce a lot of manual effort needed in diagnosis.


## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)

## General Information
- The dataset consists of 2357 images of malignant and benign oncological diseases, which were formed from the International Skin Imaging Collaboration (ISIC). All images were sorted according to the classification taken with ISIC, and all subsets were divided into the same number of images, with the exception of melanomas and moles, whose images are slightly dominant.
- The data set contains the following diseases:

- Actinic keratosis
- Basal cell carcinoma
- Dermatofibroma
-  Melanoma
- Nevus
- Pigmented benign keratosis
- Seborrheic keratosis
- Squamous cell carcinoma
- Vascular lesion
  
**Solution Pipeline**
  - Data Reading/Data Understanding → Defining the path for train and test images 
  - Dataset Creation→ Create train & validation dataset from the train directory with a batch size of 32. Also, make sure you resize your images to 180*180.
  - Dataset visualisation → Create a code to visualize one instance of all the nine classes present in the dataset 
  - Model Building & training : 
    - Create a CNN model, which can accurately detect 9 classes present in the dataset. While building the model, rescale images to normalize pixel values between (0,1).
    - Choose an appropriate optimiser and loss function for model training
    - Train the model for epochs
  - Chose an appropriate data augmentation strategy to resolve underfitting/overfitting 
  - Model Building & training on the augmented data :
  - Class distribution: Examine the current class distribution in the training dataset 
  - Handling class imbalances: Rectify class imbalances present in the training dataset with Augmentor library.



## Conclusions
- Training Performance: The training loss is relatively low at 0.2303, indicating that the model is fitting the training data quite well. This suggests that the model is learning the patterns within the training data with a high degree of accuracy, achieving a training accuracy of 91.19%.

- Validation Performance: While the validation loss is higher than the training loss, which is expected, it remains relatively low at 0.4360. This indicates that the model is performing well on data it hasn't seen during training. The validation accuracy of 87.01% reflects the model's ability to generalize to new, unseen data.

- Generalization: The relatively small gap between the training accuracy (91.19%) and validation accuracy (87.01%) suggests that the model is not overfitting the training data. It demonstrates a good balance between learning from the training data and generalizing to new data.

- Model Capability: These results imply that the model has been well-trained and is proficient in capturing the underlying patterns in the data. It has the potential for practical applications with a high level of accuracy in both training and validation.

Overall, the model appears to be well-trained and exhibits strong performance on both the training and validation datasets, indicating its potential for effective real-world use.


## Technologies Used
- tensorflow==2.12.0
- numpy==1.23.5
- pandas==1.5.3
- PIL==9.4.0
- keras.api._v2.keras==2.12.0
- Augmentor==0.2.12

## Contact
Created by [@rmohamedbasith] - feel free to contact me!
