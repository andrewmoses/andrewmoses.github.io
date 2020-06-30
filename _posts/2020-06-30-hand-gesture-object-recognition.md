---
layout: post
title: "Hand Gesture Game with Object recognition techniques"
date: 2020-06-30
---

BIG Thanks to <a href="http://zerotogans.com" target="_blank">PyTorch: Zero to GANs</a> - the motivation for this blog post.

Imagine a game which can interact with the user without touch input or heft consoles. Kinect made it possible. But here we are gonna see the same objective getting full filled using a webcam.

Okay, I'm kind of hyping it overly :P

Glimpse of the output:

<iframe width="560" height="315" src="https://www.youtube.com/embed/izI0_gtwsis" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

# What I did

Before I build a model, I need a dataset using which my model can learn to recognize my hand gestures.

On searching the web, I found this publicly available dataset which solves my objective. It has the hand signs of almost all of the english alphabets.

Dataset link: <a href="http://empslocal.ex.ac.uk/people/staff/np331/index.php?section=FingerSpellingDataset" target="_blank">Click Here</a>

<img src="http://empslocal.ex.ac.uk/people/staff/np331/examples.png"/>

I utilized 3 classes to build my model, why not all? simply to speed up my training time.

* Using Pytorch I took a pretrained ResNet34 model and removed its last layer and added a softmax to find the probability of an image to the respective 3 classes.

I have two notebooks and one structured py script

Notebook 1: <a href="https://github.com/andrewmoses/handgesture/blob/master/sign_lang.ipynb">Click Here</a>

Will have the step by step code snippets from processing the dataset to training the model

Notebook 2: <a href="https://github.com/andrewmoses/handgesture/blob/master/trained_integration.ipynb">Click Here</a>

Utilizing the trained weights of the model and integration of the solution with opencv and game concept script.

Structured PY script: <a href="https://github.com/andrewmoses/handgesture/blob/master/webcam_drama.py">Click Here</a>

Trained model's weights: <a href="https://github.com/andrewmoses/handgesture/blob/master/resnet_signlang_andrew_v3.pth">Click Here</a>


The END!



<br><br>
