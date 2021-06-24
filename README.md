# Object Detection on Custom Dataset with YOLO (v5) using PyTorch and Python

Key words: Deep Learning, Computer Vision, Object Detection, Neural Network, Python.

In this project, you’ll learn how to fine-tune a pre-trained <a href='https://github.com/ultralytics/yolov5'>YOLO v5</a> model for detecting and classifying fruits items from images.

Here’s what we’ll go over:

<ul>
<li>Install required libraries</li>
<li>Build a custom dataset in YOLO/darknet format</li>
<li>Fine-tune the largest YOLO v5 model</li>
<li>Evaluate the model</li>
<li>Look at some predictions</li>
</ul>

# Custom dataset

<p>The custom dataset is from <a href='https://exxact-robotics.com/'>Exxact Robotics</a> company which contains a set of fruits.</p>

<p>First, we need to clean the dataset called <a href='https://github.com/khasaad/YOLO-V5_Transfer-Learning_for_computer_vision/tree/main/datasets'>datasets</a> to match with <a href='https://github.com/ultralytics/yolov5'>YOLO v5</a> open source github.</p> 
<p>To do this, you need to use <a href='https://github.com/khasaad/YOLO-V5_Transfer-Learning_for_computer_vision/blob/main/cleaned_data.ipynb'>cleaned_data.ipynb</a></p>

<p>Because there are errors in the database from <a href='https://exxact-robotics.com/'>Exxact Robotics</a> company in boundry box of sets of fruits in several images, The cleaned data is modified manually to match with <a href='https://github.com/ultralytics/yolov5'>YOLO v5</a> open source. </p>

<p>The new cleaned data called <a href='https://github.com/khasaad/YOLO-V5_Transfer-Learning_for_computer_vision/tree/main/deep_fruits_data'>deep_fruits_data</a>.</p>

