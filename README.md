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

## Preprocessing of data

### Statistical analysis of data

#### Libraries used

- pandas
- matplotlib

#### Tasks performed

1. csv files created into dataframes
2. New dataframes created based on only `ID` and `Disease_Risk`
3. Converted binary values of `Disease_Risk` to string values
4. Plotted bar plots of frequency of each retinal disease in each set
5. Plotted bar plots of frequency of healthy and unhealthy retinas in each set

#### Results

1. the most common disease is Diabetic Retinopathy (D)R followed by Macular Hole (MH)
2. the ratio of healthy to unhealthy retinal images is about 3.77

### Classification of data

#### Libraries used

- os
- shutil

#### Tasks performed

1. subdirectories `healthy` and `unhealthy` created for each set
2. image sets iterated and segregated into respected subdirectories based on `Disease_Risk`