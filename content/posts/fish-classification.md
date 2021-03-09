---
title: "Teaching my iPhone to recognise fish species without a single line of code 🐠"
date: 2020-12-07T14:12:24+10:00
draft: false
summary: "A foray into image classification using CreateML"
---

Fishing has always been a hobby of mine. To ensure the sustainiblity of recreational fish stocks it is important that fisherman understand are able to recognise different fish species and know size restrictions / bag limits. I thought this application could help new anglers for identifying the fish they catch.


#### Collecting Images

I decided to train a model able to recognise five of the most common recreational fish species caught in NSW; bream, whiting, flathead, luderick and whiting. 

{{< figure src="species.png" caption="Three of the five species">}}

Using the command line tool Instaloader I scraped images from public instagram hashtags under each species (i.e #sandwhiting)  I scraped 1000+ images for each species, then went through and filtered out the best images totalling a minimum of 250.

{{< figure src="instaloader.png" caption="Using Instaloader in command line">}}


#### Training on CreateML
This is Apples no-code computer vision training tool optimised for use with iOS. You simply drag and drop a collection of class folders to begin training. My training data totalled 1,288 over 5 classes. 

{{< figure src="training.png" caption="Training took a number of hours on my i5 Macbook Air">}}



#### Testing
I tested the model on 10 unseen images across the classes. Results were suprising, 10/10 accurate classifications.

{{< figure src="testing.png" caption="Accurate even when fish is angled to the camera">}}


#### Deployment
I deployed the model to my iPhone 12 Pro using a public project called [MLModelCamera](https://github.com/shu223/MLModelCamera). It allows for Drag-and-Drop testing of Core ML models.

{{< figure src="deployment.png" caption="I haven't had a chance to test it live on a fishing trip, will update the post hence.">}}
