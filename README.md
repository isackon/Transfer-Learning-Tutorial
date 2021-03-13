﻿# Transfer-Learning-Tutorial

In this tutorial I trained a convolutional neural network for image classification using transfer learning based on the ***AlexNet***, ***VGG***, and ***Inception*** models.

According to [cs231](https://cs231n.github.io/transfer-learning/):
> In practice, very few people train an entire Convolutional Network from scratch (with random initialization), because it is relatively rare to have a dataset of sufficient size. Instead, it is common to pretrain a ConvNet on a very large dataset (e.g. ImageNet, which contains 1.2 million images with 1000 categories), and then use the ConvNet either as an initialization or a fixed feature extractor for the task of interest.

According to [TRANSFER LEARNING FOR COMPUTER VISION TUTORIAL
](https://pytorch.org/tutorials/beginner/transfer_learning_tutorial.html), These two major transfer learning scenarios look as follows:

>* ***Finetuning the convnet:*** Instead of random initializaion, we initialize the network with a pretrained network, like the one that is trained on imagenet 1000 dataset. Rest of the training looks as usual.
> * ***ConvNet as fixed feature extractor:*** Here, we will freeze the weights for all of the network except that of the final fully connected layer. This last fully connected layer is replaced with a new one with random weights and only this layer is trained.
