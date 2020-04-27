# NBA-Face-Recogntion

An iOS application that recognize NBA players' face by photos and real-time camera.

Build with VGG-16, which is one of state-of-the-art face recognition deep learning algorithm.

To reduce the interference of the training process, all the player images that were crawled from google were captured only face section. The deep learning model identifies players based on face features of the player and the results achieve around 95 percent accuracy.


## Features
Users can either upload pictures from the photo library to identify NBA player or turn on the camera to carry out real-time face recognition.

### Phote Library Upload
The system will identify the face in the entire picture, crop the face and then send the face section to the deep learning model to recognize the result. If users upload an image without a human face or the player is not in our dataset, the system will show "couldn’t find any face" and "unknown".

<img src="Face/image/photo.GIF" width=240 height=400>

### Camera Real-Time
As the camera moves, the system continuously recognizes the face on the screen, also displays the predict player name and probability. The structure and function were inspired by [Rosebrock](https://www.pyimagesearch.com/2018/04/23/running-keras-).

<img src="Face/image/camera.GIF" width=240 height=400>
