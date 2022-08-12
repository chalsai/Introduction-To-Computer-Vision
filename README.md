# Introduction To Computer Vision


# Step 1. Business Understanding

# a) Specifying the Research Question


The supermarket chain would like to explore whether Data Science can help them adhere to alcohol laws by making sure they do not sell alcohol to people underage. You are asked to conduct that evaluation, so as you set to work, keep the following in mind:


● The shops are equipped with cameras in the checkout area which are triggered when a person is buying alcohol.

● Computer vision methods can be used to determine the age of a person from a photo.

● The task then is to build and evaluate a model for verifying people's age. To start working on the task, you'll have a set of photographs of people with their ages indicated.

# b) Defining the Metric for Success


The task then is to build and evaluate a model for verifying people's age.

#d) Project Instrusctions


● Before getting your hands dirty with the project, let's think of the Good Seed supermarket task in detail. Imagine your manager wants to check your understanding of the task. Pass this quiz to verify your understanding of the project statement.


● Perform exploratory data analysis to get an overall impression of the dataset.


● Train and evaluate the model (it needs to be done on the GPU platform).


● Combine your code, output, and findings (from the previous points) in the final notebook.


● Make conclusions of the model evaluation, add them to the notebook.

# Summary

- Given the fact that the number of image files is rather high, we will avoid reading them all at once, which would greatly consume computational resources. instead i will build a generator with the ImageDataGenerator generator.


- The data contents 7591 records and varias from one year old to 100 years old, the mean is 31, no missing values and no duplicates


- The age distribution is like a gamma distribution, which is good for our purposes of making sure we dont sell alcohol to underage persons. Although the mass is between 20-40 which are not underage.


- We have outaires like a one year old baby or a 100 year old elderly. They are not so relevant because the chances of them coming alone to buy alcohol is low.So we shall ignore them for now.


- Image Data set looks very diverse in terms of age, gender and origin which reinforces the model. The background of the image is basiclly noise and does not contribute to the model for predicting the age of the character. but because we want the model to work on new data as well, we need it to learn what relevant and whats not.



# Conclusions


I used the ResNet50 neural network in order to predict age by face image, the traning set contains 5694 images and the tesing set contains 1897 images, my final MAE score is 7.5944


# a) Did we have the right question?


Yes we did

# b) Did we have the right data?
Yes the data was right

# c) What can be done to improve the solution?

Check Code
