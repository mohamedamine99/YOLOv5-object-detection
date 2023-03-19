# YOLOv5-object-detection
The GitHub repository features two different implementations of object detection using YOLOv5 and its variants, one based on functions and the other on classes. 
<p align="center">
    <img src="https://github.com/mohamedamine99/YOLOv5-object-detection/blob/main/GIFs/traffic_nano.gif" width=500></td>
</p>

This GitHub repository contains Jupyter notebooks that showcase simple object detection using YOLOv5 and its variants using the aforementioned approaches. 
The notebooks demonstrate how to apply these models to both images and video files, and provide step-by-step instructions for implementing the object detection algorithm. 
Whether you're new to deep learning or just want to learn more about YOLOv5, this repository provides a great starting point for experimenting with object detection.

<!-- TABLE OF CONTENTS -->
<details open="open">
  <summary>Table of Contents</summary>
  <ol>
    <li><a href="#repo-overview">Repo Overview</a></li>  
    <li><a href="#comparing-different-yolov5-variants">Comparing different YOLOv5 variants</a></li>
      <ul>
        <li><a href="#object-detection-on-image-files">Object detection on image files</a></li>
        <li><a href="#object-detection-on-video-files">Object detection on video files</a></li>
      </ul>

       
  </ol>
</details>

## Repo Overview:
* [YOLOv5_simple_object_detector.ipynb](https://github.com/mohamedamine99/YOLOv5-object-detection/blob/main/YOLOv5_simple_object_detector.ipynb) : Jupyter notebook for object detection on both static image files and video files with different YOLOv5 variants using a function-base approach.
* [YOLOv5_simple_Class_Based_Object_Detector.ipynb](https://github.com/mohamedamine99/YOLOv5-object-detection/blob/main/YOLOv5_simple_Class_Based_Object_Detector.ipynb) : Jupyter notebook for object detection on both static image files and video files with different YOLOv5 variants using a class-based approach.
* [Yolov5_ObjectDetector.py](https://github.com/mohamedamine99/YOLOv5-object-detection/blob/main/Yolov5_ObjectDetector.py) : a python file that contains the definition of the Yolov5_ObjectDetector class and its documentation.
* [img results](https://github.com/mohamedamine99/YOLOv5-object-detection/tree/main/img%20results) : contains results of object detection on image files.
* [video results](https://github.com/mohamedamine99/YOLOv5-object-detection/tree/main/video%20results) : contains results of object detection on video files in .avi format.
* [gifs](https://github.com/mohamedamine99/YOLOv3-simple-object-detection/tree/main/gifs) : contains results of object detection on video files in GIF format..
* [test imgs](https://github.com/mohamedamine99/YOLOv5-object-detection/tree/main/test%20imgs) : contains images of random scenes.
* [test vids](https://github.com/mohamedamine99/YOLOv5-object-detection/tree/main/test%20vids) : contains videos of random scenes.
* [coco.names](https://github.com/mohamedamine99/YOLOv5-object-detection/blob/main/coco.names) : The "coco.names" file is a plain text file that contains the names of the 80 object classes in the Microsoft Common Objects in Context (COCO) dataset.

## Comparing different YOLOv5 variants

There are several variants of YOLOv5, each with different features and capabilities:
The backbone architecture of YOLOv5 variants is based on a convolutional neural network (CNN) called CSPDarknet. This is a modified version of the Darknet architecture used in YOLOv4. CSPDarknet consists of a series of convolutional layers with shortcut connections, which helps to improve the information flow and reduce the computational cost of the network.

In this project we use 10 variants : `yolov5n`, `yolov5s`, `yolov5m`, `yolov5l` ,`yolov5x` ,`yolov5n6`, `yolov5s6`, `yolov5m6`, `yolov5l6` and `yolov5x6`.
Each YOLOv5 variant uses a different CSPDarknet backbone, which affects the size and speed of the network. Here are the CSPDarknet backbones used by each YOLOv5 variant:

* YOLOv5s: CSPDarknet53
* YOLOv5m: CSPDarknet53 + SPP (Spatial Pyramid Pooling)
* YOLOv5l: CSPDarknet53 + PAN (Path Aggregation Network)
* YOLOv5x: CSPDarknet53 + SPP + PAN

The "6" in YOLOv5l6 (or any other yolov5 variant) refers to the number of times the CSPDarknet backbone is repeated in the network. This results in a deeper and more complex network than YOLOv5l, which has only 4 repeats of the CSPDarknet backbone.

* YOLOv5n: This is the smallest and fastest variant of YOLOv5, making it ideal for real-time applications.
* YOLOv5s: This is a smaller and faster version of YOLOv5, which makes it a more suitable choice for applications that require real-time processing.
* YOLOv5m: This variant is larger and slower than YOLOv5s but provides better accuracy.
* YOLOv5l: This variant is even larger and slower than YOLOv5m but provides even better accuracy.
* YOLOv5x: This is the largest and slowest variant of YOLOv5, but it provides the highest accuracy.

<p align="center">
    <img src="https://github.com/mohamedamine99/YOLOv5-object-detection/blob/main/yolov5_6%20variants%20comparison.PNG" width=500></td>
    <img src="https://github.com/mohamedamine99/YOLOv5-object-detection/blob/main/yolov5%20variants%20comparison.PNG" width=500></td>
</p>

### Object detection on image files

<div align="center">  
<table style="margin: 0 auto; border-style: none; width:100%">
  <tr>
    <td>yolov5n</td>
    <td>yolov5s</td>
    <td>yolov5m</td>
    <td>yolov5l</td>
    <td>yolov5x</td>
  </tr>
  
  <tr> 
    <td><img src="https://github.com/mohamedamine99/YOLOv5-object-detection/blob/main/img%20results/yolov5n/highway.PNG" width=300></td>
    <td><img src="https://github.com/mohamedamine99/YOLOv5-object-detection/blob/main/img%20results/yolov5s/highway.PNG" width=300></td>
    <td><img src="https://github.com/mohamedamine99/YOLOv5-object-detection/blob/main/img%20results/yolov5m/highway.PNG" width=300></td>
    <td><img src="https://github.com/mohamedamine99/YOLOv5-object-detection/blob/main/img%20results/yolov5l/highway.PNG" width=300></td>
    <td><img src="https://github.com/mohamedamine99/YOLOv5-object-detection/blob/main/img%20results/yolov5x/highway.PNG" width=300></td>
  </tr>

  <tr> 
    <td><img src="https://github.com/mohamedamine99/YOLOv5-object-detection/blob/main/img%20results/yolov5n/people%20crossing%20the%20street.jpg" width=300></td>
    <td><img src="https://github.com/mohamedamine99/YOLOv5-object-detection/blob/main/img%20results/yolov5s/people%20crossing%20the%20street.jpg" width=300></td>
    <td><img src="https://github.com/mohamedamine99/YOLOv5-object-detection/blob/main/img%20results/yolov5m/people%20crossing%20the%20street.jpg" width=300></td>
    <td><img src="https://github.com/mohamedamine99/YOLOv5-object-detection/blob/main/img%20results/yolov5l/people%20crossing%20the%20street.jpg" width=300></td>
    <td><img src="https://github.com/mohamedamine99/YOLOv5-object-detection/blob/main/img%20results/yolov5x/people%20crossing%20the%20street.jpg" width=300></td>
  </tr>
  
  <tr>
    <td>yolov5n_6</td>
    <td>yolov5s_6</td>
    <td>yolov5m_6</td>
    <td>yolov5l_6</td>
    <td>yolov5x_6</td>
  </tr>
  
  <tr> 
    <td><img src="https://github.com/mohamedamine99/YOLOv5-object-detection/blob/main/img%20results/yolov5n6/highway.PNG" width=300></td>
    <td><img src="https://github.com/mohamedamine99/YOLOv5-object-detection/blob/main/img%20results/yolov5s6/highway.PNG" width=300></td>
    <td><img src="https://github.com/mohamedamine99/YOLOv5-object-detection/blob/main/img%20results/yolov5m6/highway.PNG" width=300></td>
    <td><img src="https://github.com/mohamedamine99/YOLOv5-object-detection/blob/main/img%20results/yolov5l6/highway.PNG" width=300></td>
    <td><img src="https://github.com/mohamedamine99/YOLOv5-object-detection/blob/main/img%20results/yolov5x6/highway.PNG" width=300></td>
  </tr>

  <tr> 
    <td><img src="https://github.com/mohamedamine99/YOLOv5-object-detection/blob/main/img%20results/yolov5n6/people%20crossing%20the%20street.jpg" width=300></td>
    <td><img src="https://github.com/mohamedamine99/YOLOv5-object-detection/blob/main/img%20results/yolov5s6/people%20crossing%20the%20street.jpg" width=300></td>
    <td><img src="https://github.com/mohamedamine99/YOLOv5-object-detection/blob/main/img%20results/yolov5m6/people%20crossing%20the%20street.jpg" width=300></td>
    <td><img src="https://github.com/mohamedamine99/YOLOv5-object-detection/blob/main/img%20results/yolov5l6/people%20crossing%20the%20street.jpg" width=300></td>
    <td><img src="https://github.com/mohamedamine99/YOLOv5-object-detection/blob/main/img%20results/yolov5x6/people%20crossing%20the%20street.jpg" width=300></td>
  </tr>
   
  
</table>
</div>

### Object detection on video files 

<div align="center">  
<table style="margin: 0 auto; border-style: none; width:100%">
  <tr>
    <td>yolov5n</td>
    <td>yolov5n6</td>

  </tr>
  
  <tr> 
    <td><img src="https://github.com/mohamedamine99/YOLOv5-object-detection/blob/main/GIFs/traffic_nano.gif" width=450></td>
    <td><img src="https://github.com/mohamedamine99/YOLOv5-object-detection/blob/main/GIFs/traffic_nano6.gif" width=450></td>
 </tr>
    
  <tr>
    <td>yolov5m</td>
    <td>yolov5x6</td>

  </tr>
  
  <tr> 
    <td><img src="https://github.com/mohamedamine99/YOLOv5-object-detection/blob/main/GIFs/traffic_medium.gif" width=450></td>
    <td><img src="https://github.com/mohamedamine99/YOLOv5-object-detection/blob/main/GIFs/traffic_x6.gif" width=450></td>
 </tr>

