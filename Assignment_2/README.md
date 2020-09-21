# Assignment 2- Recognize an Animal in an Image

### About the Data

The training dataset consists of 1200 medium quality animal images belonging to 2 categories: mucca (cow) and pecora (sheep). All the images have been collected from "google images" and have been checked by humans. There is some erroneous data to simulate real conditions (eg. images taken by users of your app).

### Dataset Link: (https://github.com/dphi-official/Datasets/tree/master/animal_data)

There are 4 files:

**train_beg.zip** - contains the images of cows and sheeps that are to be used for training and validation of the model. Each image has a unique name like - image_1, image_2, etc.
 
**Training_set_animals.csv** - contains the image’s filename and their corresponding target value (i.e. the actual animal name). You can load this file using the below command:

`Training_set_animals = pd.read_csv`("https://raw.githubusercontent.com/dphi-official/Datasets/master/animal_data/Training_set_animals.csv")
 
**test_beg.zip** - contains the images of cows and sheeps whose predictions you are to submit on the DPhi platform. Instructions to load this data is given in assignment 2 guidelines on the Deep Learning Bootcamp dashboard.
 
**Testing_set_animals.csv** - this is the order of the predictions for each image that is to be submitted on the platform. Make sure the predictions you download are with their image’s filename in the same order as given in this file. You can load this file using the given command (please notice that the test set does not have any header):

`Testing_set_animals = pd.read_csv`("https://raw.githubusercontent.com/dphi-official/Datasets/master/animal_data/Testing_set_animals.csv", header=None)
