# YOLOv5-object-detection
This GitHub repository showcases simple object detection using different YOLOv5-based models on images and videos.

<p align="center">
    <img src="https://github.com/mohamedamine99/YOLOv5-object-detection/blob/main/GIFs/traffic_nano.gif" width=500></td>
</p>

This GitHub repository contains Jupyter notebooks that showcase simple object detection using YOLOv5 and its variants. 
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
* [YOLOv5_simple_object_detector.ipynb](https://github.com/mohamedamine99/YOLOv5-object-detection/blob/main/YOLOv5_simple_object_detector.ipynb) : Jupyter notebook for object detection on both static image files and video files with different YOLOv5 variants.
* [img results](https://github.com/mohamedamine99/YOLOv5-object-detection/tree/main/img%20results) : contains results of object detection on image files.
* [video results](https://github.com/mohamedamine99/YOLOv5-object-detection/tree/main/video%20results) : contains results of object detection on video files in .avi format.
* [gifs](https://github.com/mohamedamine99/YOLOv3-simple-object-detection/tree/main/gifs) : contains results of object detection on video files in GIF format..
* [test imgs](https://github.com/mohamedamine99/YOLOv5-object-detection/tree/main/test%20imgs) : contains images of random scenes.
* [test vids](https://github.com/mohamedamine99/YOLOv5-object-detection/tree/main/test%20vids) : contains videos of random scenes.
* [coco.names](https://github.com/mohamedamine99/YOLOv5-object-detection/blob/main/coco.names) : The "coco.names" file is a plain text file that contains the names of the 80 object classes in the Microsoft Common Objects in Context (COCO) dataset.

## Comparing different YOLOv5 variants

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
 
   </div>


    


