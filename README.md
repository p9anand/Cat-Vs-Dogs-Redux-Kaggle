# Cat-Vs-Dogs-Redux-Kaggle
This notebook is regarding a competition on Kaggle [https://www.kaggle.com/c/dogs-vs-cats-redux-kernels-edition]. In this tutorial
we have taken data from above mentioned competition. The data consists of images of cats and dogs and we are asked to build a
classifier which can classify these images into their respective catogeries. To get more imformation please refer to above link.

First i have a written a function to get the data. Then we have used already trained Vgg16 imagenet model. And using this model we
first created our features by predicting probabilities for each images. Vgg16 classify an image into 1000 classes. So output of
this model is taken as features. Then on top of that i have added a dense layer with input as feature i.e. 1000 classes and output
as whether it's a cat or dog. There is one thing to be noticed that we are training just last layer with our data set.

I have used Keras library because it is easy to use and can be understood by a Non-data scientist.Using this model we can achieve 
~ 96 % accuracy. Which is pretty decent. The reason for a such a decent accuracy beacause imagenet problem is very similar to our 
dataset. Infact it has already scene thousands of images of cats and dogs.

In next update, we'll learn about finetuning. How it works. And how to this using Keras.
