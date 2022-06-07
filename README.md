# EYE-RecAIcle

CS5500: Foundation of Software Engineering

Team 3 - Daniel Lisko, Matthew Vargas, Michael Chang, Semaa Amin, and Yvette Green

## Project Description
Image Classification with Jetson Nano coupled with Output from Arduino
* Inspiration came from the confusion of users properly disposing of waste
* Help reduce the manual intervention of disposing of different categories of waste
* Personal vs. Commercial 
     * distributed prototypes at every waste bin can help crowdsource model improvement. The same model can help automate robotics sorting at large disposal facilities


![Website Screenshot](https://github.com/greeny90/recycle-ai/blob/main/logo.png)

## Hardware and Technologies Used
- Nvidia Jetson Nano Developer Kit: https://developer.nvidia.com/embedded/jetson-nano-developer-kit
- Kaggle: https://www.kaggle.com/
- Logitech C270 HD Webcam
- Python
- Arduino board - MKR 1010
- ThingSpeak: https://thingspeak.com/ - Channel, TalkBack & ThingTweet
- Twitter

## Original Concept 
![Website Screenshot](https://github.com/greeny90/recycle-ai/blob/main/originalconcept.png)

## Finished Product
![Website Screenshot](https://github.com/greeny90/recycle-ai/blob/main/howitworks.png)
- A USB Logitech camera is connected to the Jetson Nano and takes a picture of a piece of garbage.
- The image is compared with the machine learning model trained with Kaggle Dataset of Recyclable objects.
- The image is identified as one of the following: 
     - Cardboard: 0
     - Glass: 1
     - Metal: 2
     - Paper: 3
     - Plastic: 4
     - Trash: 5  
- ThingSpeak's ThingTweet app sends a post on Twitter. 
![Website Screenshot](https://github.com/greeny90/recycle-ai/blob/main/tweet.png)
- ThingSpeak's TalkBack feature changes the LED light on the Arduino board based on the image identified. 
     - Green Light = Recycling 
     - Red = Trash
![Website Screenshot](https://github.com/greeny90/recycle-ai/blob/main/arduino.png)

## Future Goals for the Project
- Expand on the model for more accurate predictions
   - Crowdsource to obtain images that expand our training data set (eg. captcha model)
- Connect to a database (scalability)
- Expand to include more categories 
   - E-waste and compost
- Possibly present the project at a SmartCities event
- Upgrade hardware 
   - 4GB or 8GB Jetson Nano 
   - Add better Arduino boards to include LED strip lights, LCD screens, and sound
 
## Vision for Future Product
https://user-images.githubusercontent.com/70995997/172470209-582572f7-1a16-4e21-8b8a-eb5fb72f3f3a.mp4

## Google Demo Slides
[![LINK TO SLIDES](https://github.com/coder-chick/recycle-ai/blob/main/EYE-RecAIcle%20Slides.png)](https://docs.google.com/presentation/d/1O_W9ddtD3KJIEUg6YtUYFHIBgqades3gN6sQesUPft8/edit#slide=id.g1268a7e57a3_0_249)

