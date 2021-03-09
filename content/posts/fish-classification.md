---
title: "Machine learning for beach litter detection 🏝"
date: 2020-04-07T14:12:24+10:00
draft: false
summary: "Training a beach litter detection model using CreateML."
---

Teach my iPhone to recognise fish species without a single line of code. This would be a great tool for new fisherman to learn about fish size restrictions and bag limits.




#### Collecting Images

I decided to train a model able to recognise five of the most common recreational fish species caught in NSW; bream, whiting, flathead, luderick and whiting. 

{{< figure src="species.png" caption="Three of the five species">}}

Using the command line tool Instaloader I scraped images from public instagram hashtags under each species (i.e #sandwhiting)  I scraped 1000+ images for each species, then went through and filtered out the best images totalling a minimum of 250.

{{< figure src="instaloader.png" caption="Using Instaloader in command line">}}


#### Training on CreateML
This is Apples no-code computer vision training tool optimised for use with iOS. You simply drag and drop a collection of class folders to begin training. My training data totalled 1,288 over 5 classes. 

{{< figure src="createml.png" caption="Training took a number of hours on my i5 Macbook Air">}}



#### Testing
I tested the model on 10 unseen images across the classes. Results were suprising, 10/10 accurate classifications.

{{< figure src="training.png" caption="Accurate even when fish is angled to the camera">}}

