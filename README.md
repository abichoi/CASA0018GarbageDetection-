# CASA0018GarbageDetection
## Aim
The aim of this project is to train an object detection model so that it can identify the type of the garbage shown in a photo. Due to the limited time, the type of garbage is limited to 6 classes, plastic, glass, paper, cardboard, metal and organic. The aim user of the model is for household applications such as self-sorting rubbish bin or an app for people like children who do not know to recycle yet. 

## Dataset source
1. Garbage Classification (12 classes)
  - Images dataset for classifying household garbage
    - Paper, cardboard, biological, metal, plastic, green-glass, brown-glass, white-glass, clothes, shoes, batteries, and trash
  - https://www.kaggle.com/datasets/mostafaabla/garbage-classification
2. Waste Classification data
  - contains 22500 images of organic and recyclable objects
  - https://www.kaggle.com/datasets/techsash/waste-classification-data

## Annotation tools
1. VGG Image Annotator
  - https://www.robots.ox.ac.uk/~vgg/software/via/via_demo.html
  - Export as CSV, json, COCO format
2. Roboflow
  - Dataset management, Annotation, image transformation
  - https://roboflow.com/

## Model used
ssd_mobilenet_v2_320x320_coco17_tpu-8

## Dataset
### Dataset 1  
  - No Augmentation  
### Dataset 2
  - Mosaic Augmentation  
### Dataset 3  
  - Mosaic Augmentation  
  - Cutout Augmentation – 5 boxes with 10% size  
  - Rotation Augmentation – Between - 45° and +45°  

## APP
https://developers.google.com/codelabs/tflite-object-detection-android#0  
The app is made by following the online tutorial above. Only the pre-set image bar at the bottom is changed from 3 food images to the 6 images from each classes of garbage, and this bar is changed to scrollable since the screen can’t fit 6 images in a row at once.
## APK files
There are two APK files for the APP. 
no_agumentation.apk uses the model trained with Dataset 1.
only_moscia.apk uses the model trained with Dataset 2.
### Installation
1. Download the APK file in the AndroidAPP folder to your Android phone
2. Install it by tapping on the file in your phone

## Presentation
More details can be found in the presentation video on Youtube https://www.youtube.com/watch?v=4jwS5hoeEt4  
An APP Demo Video is on YouTube as well https://youtu.be/2uwWVfOIYOM
