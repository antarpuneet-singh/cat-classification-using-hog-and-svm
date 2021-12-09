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
______________________________________________________________________________________________________________________________________________________________________
# Datasets

For the images of cats, I have used the dataset available at : https://www.kaggle.com/crawford/cat-dataset
<br>
I have taken 1618 random images from this dataset. Some of these are displayed below: 
<br> 
![00000100_002](https://user-images.githubusercontent.com/48234795/145378022-657d9673-b3bc-41b8-bbd8-2a1535b398eb.jpg)
![00000100_007](https://user-images.githubusercontent.com/48234795/145378058-b0a5faa9-969d-4dff-a917-5d00301af694.jpg)

![00000101_012](https://user-images.githubusercontent.com/48234795/145378210-b02f24db-40ef-4dac-bae6-178a31f3ced7.jpg)
