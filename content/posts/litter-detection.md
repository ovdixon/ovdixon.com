---
title: "Machine learning for beach litter detection 🏝"
date: 2020-04-07T14:12:24+10:00
draft: false
summary: "Training a beach litter detection model using CreateML."
---

#### Inspiration

{{< figure src="beach-bottle.jpg" caption="A single-use plastic water bottle on a beach">}}

Huge amounts of litter wash up on along Australian coastlines every day. The most widely used method for monitoring this is visual counting, requiring large teams of peoples. However if we consider the sheer size and accessibility of coastal areas this is overwhelmingly inefficient. 


#### Ideation

I sought to explore how computer vision technology could can be leveraged to monitor coastal litter. For example, a drone could map a beach to identify the amount and type of litter present. This data could then be fed back to community cleanup groups. Alternatively, someone could take a photo of the plastic they collected on their morning beach stroll. This image could be automatically processed through computer vision for data contributing to a citizen science project.


#### Implementation
I scraped 40 images rom Instagram the hashtag #take3forthesea; a community initiative where people collect three pieces of rubbish every time they visit a beach, waterway, or anywhere. I trained my model to recognise two pieces of rubbish.




