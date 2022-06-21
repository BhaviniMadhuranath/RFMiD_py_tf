# RFMiD_py_tf

A model built to detect 46 types of retinal disorders using a Retinal Fundus Multi-disease Image Dataset (RFMiD) 

## Description of data

### Source of dataset

https://www.kaggle.com/datasets/andrewmvd/retinal-disease-classification

1. The dataset contains 3200 fundus images captured by 3 different fundus cameras.
2. A total of 46 conditions have been annotated through the adjudicated consensus of two senior retinal experts
3. The 3200 images are divided into 
   - training set 
     - 1920 images
     - csv file containing annotations
   - test set 
     - 640 images
     - csv file containing annotations
   - evaluation set 
     - 640 images
     - csv file containing annotations
4. Each image is of size `2144 x 1424` pixels