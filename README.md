# Deep-Learning-Bootcamp--Dphi
From basics of deep learning to the implementation of it on various data set, covered in this Bootcamp.

## Context
Image recognition is a vital component in robotics such as driverless vehicles or domestic robots. Image recognition is also important in image search engines such as Google or Bing image search whereby you use rich image content to query for similar stuff. Like in Google photos where the system uses image recognition to categorize your images into things like cats, dogs, people and so on so that you can quickly search your albums for things like, “give me photos of my cat”, that's awesome.

Ever noticed how Facebook instantly recognises your friend’s face and asks you if you want to tag him in that photo? That’s image recognition. That’s just a basic example.

## Objective
You are working on a robotics project where you are required to train your robot so that it can differentiate between two animals. Your task here is to build a deep learning model that helps you recognize the animal in images.

## Evaluation Criteria
Submissions are evaluated using Accuracy Score.

 
# Accuracy = TP + TN / (TP + TN + FP + FN)


How do we do it? 

Once you generate and submit the target variable predictions on the test dataset, your submissions will be compared with the true values of the target variable. 

The True or Actual values of the target variable are hidden on the DPhi platform so that we can evaluate your model's performance on unseen data. Finally, an accuracy score for your model will be generated and displayed.


#Steps : 

Please follow the below instructions to load the dataset in Notebook.

Download Data From GitHub
First we need to get the data. We have given the GitHub link under the 'Data' section of the problem page which has all the required train images (to build the model) and test datat images for which one need to predict the labels (animal specie) and submit the predictions on the DPhi platform.

Download GitHub Repository
The first step is to download the repository 'Datasets' to the colab files. We can achieve this by executing the below code.

`!git clone 'https://github.com/dphi-official/Datasets/`

## To unzip train_beg.zip
`!unzip /content/Datasets/animal_data/train_beg.zip` 

## To unzip test_beg.zip
`!unzip /content/Datasets/animal_data/test_beg.zip`

```{python} {import pandas as pd
import numpy as np
train_labels = pd.read_csv("/content/Datasets/animal_data/Training_set_animals.csv")
train_labels.head()}
