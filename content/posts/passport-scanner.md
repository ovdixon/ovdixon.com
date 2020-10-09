---
title: "Mobile Passport Scanner"
date: 2020-04-07T14:12:24+10:00
draft: false
---

#### Problem
In the hospitality industry, hotels are often required to provide passport data of guests to immigration services. Passport data can be manually entered and forwarded on, however this is inefficient when dealing with a large number of guests.

#### Ideation
A mobile application that uses the phones camera to scan the Machine Readable Zone (MRZ) from passports. From this MRZ, the passport can be verified and necessary guest data recorded to be forwarded onto immigration. 


{{< figure src="ideation.png" caption="Simple wireframe sketch (left) served as a template for designing the storyboard (right)">}}


#### Implementation
The app was developed for iOS using Xcode. An image of the passport is captured using the system document scanner, VisionKit. The scanned image is then processed using the VNRecognizeTextRequest class, an image analysis request that finds and recognises the the machine readable zone (MRZ) at the bottom of the passport. The MRZ lines are then parsed using third-party [QKMRZParser](https://github.com/Mattijah/QKMRZParser) framework to extract the name, passport number, nationality, date of birth, sex, and passport expiration date.


{{< figure src="demo.gif" caption="Demo of scanning a passport into the app (running on iPad Pro 11)" width="90%">}}

#### Challenges
This was my first iOS project so I had some difficulty with Xcode but overall enjoyed the experience of coding in Swift. Because the app  processes sensitive passport information, I had to consider data privacy and protection. All data processed is stored locally on device, however the app would benefit from adding password protection. The app should adhere to GDRP laws as there is a legal basis for providing passport data to immigration services.