Flower Classifier
==================
This project was devloped for PyTorch Scholarship Challange 2018/2019.I have used pre-trained resnet152 network.It can detect about 102 different species of flower.It has vaidation accuracy of 88.5%.

Problem Statement
==================
Udacity Data Scientist Nanodegree project for deep learning module titled as 'Image Classifier with Deep Learning' attempts to train an image classifier to recognize different species of flowers. We can imagine using something like this in a phone app that tells you the name of the flower your camera is looking at. In practice we had to train this classifier, then export it for use in our application. We had used a [dataset](http://www.robots.ox.ac.uk/~vgg/data/flowers/102/index.html) of 102 flower categories.

Approach
=========

* Used torchvision to load data.
* The dataset is split into two parts, training, validation.
* For the training, applied transformations such as random scaling, cropping, and flipping.This will help the network generalize leading to better performance.
* I have loaded pretrained Resnet152 model.
* I have modified the Resnet152 model final layer to fit the flower dataset.
* Wrote inference for classification after training and testing the model. 
* Plotted the probabilities for the top 5 classes as a bar graph, along with the input image.

Result
=======
![](https://github.com/hasnain003/Flower-Classifier/blob/master/img/e1.PNG?raw=true)
![](https://github.com/hasnain003/Flower-Classifier/blob/master/img/e2.PNG?raw=true)
![](https://github.com/hasnain003/Flower-Classifier/blob/master/img/e3.PNG?raw=true)
Area of Improvement
===================
1. Training for more epoch might result in high accuracy
2. Adjust hyperparameters such as learning rate or introduce momentum to model to increase accuracy.
3. Change the classifier architecture to get high accuracy