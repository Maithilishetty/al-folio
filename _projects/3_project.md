---
layout: page
title: Traffic light recognition 
description: Project with Adastec corporation
img: assets/img/demo_yolo.png
importance: 3
---

This project was in collaboration with [Adastec Corporation](https://www.adastec.com/) as part of my Techlab @ MCity course. ADASTEC specializes in the delivery of level 4 automated driving software that is ready for real-world transit application. As part of our winter 2022 project, we implemented traffic light recognition using Deep Learning. 

Traffic light recognition is an important safety feature for autonomous vehicles. In this project, we developed a deep learning model for traffic light recognition using the Faster RCNN and YOLOv4 algorithms.The Faster RCNN algorithm is a popular choice for object detection tasks because it is both accurate and efficient. 
For more details on this methods, see [here](https://arxiv.org/abs/1506.01497). For the purpose of training this model, we make use of the Tensorflow object detection API.
YOLOv4, on the other hand, is a newer algorithm that has demonstrated state-of-the-art performance on a variety of object detection benchmarks. 
To train and evaluate our models, we used the [BOSCH Small Traffic Light Dataset](https://hci.iwr.uni-heidelberg.de/content/bosch-small-traffic-lights-dataset). 

The results were also tested by the data collected at MCity and also with that provided by Adastec. The below set of figures show the detection performance of YOLOv4. 

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path=
"assets/img/chart_yolov4_6000.png" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/chart_yolov4-bosch_11100.png" %}
    </div>
</div>
<div class="caption">
   Left: Performance of YOLOv4 with the pre-trained model. Right: Performance of YOLOv4 with additional training of upto 48 hours. 
</div>

The below videos demonstrate the performance of the model for the MCity and Adastec data. It can be seen that the model is capable of predicting the location and the state of the traffic light with increased accuracy. The extended goal of this project is to fuse V2X and deep learning to make robust detections and classifications of the traffic signals especially during adverse weather conditions. Additionally, as part of the project we collected SPaT messages from the Mcity testing facility. 

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        <iframe src="https://drive.google.com/file/d/1sEHBhkTVZHOAnWgS7GgNStrNX__WLE4U/preview" width="350" height="323" allow="autoplay"></iframe>
    </div>
    <div class="col-sm mt-3 mt-md-0">
        <iframe src="https://drive.google.com/file/d/1QGdxSzRrVoG3RrqHWJp5-BbPZdsuB_fy/preview" width="350" height="323" allow="autoplay"></iframe>
    </div>
</div>
<div class="caption">
   Left: Testing the model on Mcity Data. Right: Testing the model on Adastec Data (particulary data collected in bad weather). 
</div>