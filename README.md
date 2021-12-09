# Introduction
Feature descriptors have been long used in the field of Computer Vision. Nowadays, modern deep learning models have taken over. But traditional ways of extracting features from images still play an important role.
<br>
In this project, I have built a cat classification model using Histogram of gradients descriptor and a Support Vector Machine.
<br>
This project is inspired from the "Histogram of Oriented Gradients for Human Detection" paper published by Dalal and Triggs in 2005. 
<br>
The HOG descriptor is based on the structure of the object. It extracts the gradient and orientation from different segments of an image and then creates a histogram representing this information.
<br>
After we have extracted the features of an image using HOG, we use a classifier like SVM to perform the classification task.
<br>
![download](https://user-images.githubusercontent.com/48234795/145380646-653056fd-e029-4f19-a8df-e146784fad19.png)
<br>
______________________________________________________________________________________________________________________________________________________________________
# Datasets

For the images of cats, I have used the dataset available at : https://www.kaggle.com/crawford/cat-dataset
<br>
I have taken 1618 random images from this dataset. Some of these are displayed below: 
<br> 
![00000100_002](https://user-images.githubusercontent.com/48234795/145378022-657d9673-b3bc-41b8-bbd8-2a1535b398eb.jpg)
![00000100_007](https://user-images.githubusercontent.com/48234795/145378058-b0a5faa9-969d-4dff-a917-5d00301af694.jpg)

![00000101_012](https://user-images.githubusercontent.com/48234795/145378210-b02f24db-40ef-4dac-bae6-178a31f3ced7.jpg)

For negative examples in our dataset, I have taken 1330 random images from flickr dataset avaialble at : https://www.kaggle.com/hsankesara/flickr-image-dataset
<br>
Some of the images are displayed below :

<br>

![4729870194](https://user-images.githubusercontent.com/48234795/145378593-435a7568-132a-4d5c-bcc9-27acc6a0c215.jpg)

![4729750820](https://user-images.githubusercontent.com/48234795/145378627-2d10d6ab-4f59-4f7c-9562-c76f4dae3dbc.jpg)

![4735873109](https://user-images.githubusercontent.com/48234795/145378730-e8d010c6-a156-45e8-a89f-a601d7e0d2c5.jpg)


# Code and results
The notebook provided contains the code for getting the names of all images in a directory and then extracting their features. Then a dataset is built by shuffling both positive and negative examples. SVM with a radial basis function produces 81 % accuracy and 87% recall.

