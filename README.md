###  Melanoma Detection Project  

## Objective:  
  Develop a CNN-based model to accurately detect melanoma from medical images, aiding dermatologists in early detection and reducing manual diagnosis effort.  

## Problem Statement*:  
  Melanoma, a type of skin cancer, accounts for 75% of skin cancer deaths. Early detection can significantly improve patient outcomes. This solution aims to automate and enhance diagnostic accuracy.  

## Dataset Overview:  
  - Source: International Skin Imaging Collaboration (ISIC).  
  - Total Images: 2,357 medical images.  
  - Image Categories: Classified based on ISIC standards.  
  - Class Distribution: Balanced subsets, except for melanomas and moles, which are slightly overrepresented.  

## Disease Categories in Dataset:  
  1. Actinic Keratosis  
  2. Basal Cell Carcinoma  
  3. Dermatofibroma  
  4. Melanoma  
  5. Nevus  
  6. Pigmented Benign Keratosis  
  7. Seborrheic Keratosis  
  8. Squamous Cell Carcinoma  
  9. Vascular Lesion  

## Significance:  
  A successful model will support dermatologists by automating image evaluation, improving diagnostic accuracy, and reducing manual effort in identifying skin cancer types.

## Conclusions

1. After loading the data set , we have used a simple architecture with no dropout layer and ran for 20 Epochs.

Train accuracy - 0.85

Validation accuracy - 0.49

We see that there is a severe overfit on the training data

2. In the second model , we have included few droup out layers and here are the stats:

Train accuracy - 0.54

Validation accuracy - 0.53

We see that the overall fit of the model in validation has increased but significantly decreased on test and now the model is Underfitting both Train and Validation

3. In the third and final model , we have included few drop out layers and used augmentor to add in 500 additional datapoints per class with slight rotation

Train accuracy - 0.88

Validation accuracy - 0.83

We see that the overall fit of the model in validation and training has increased and has improved the accuracy as well. Though it is not the best performing model. This is a good place to start. With more data points and epochs , the value can improve significantly.



Technologies Used
tensorflow - 2.18.0
numpy - version 2.0.1
pandas - version 2.2.2
seaborn - version 0.13.2



## Contact
Created by [@Lokavishruth] - feel free to contact me!

