# Object Detection on Custom Dataset with YOLO (v5) using PyTorch and Python

Key words: Deep Learning, Computer Vision, Object Detection, Neural Network, Python.

In this project, you’ll learn how to fine-tune a pre-trained <a href='https://github.com/ultralytics/yolov5'>YOLO v5</a> model for object detection on Custom Dataset with YOLO (v5) using PyTorch and Python.

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

# Implementation code to clean data

<ol>
  <li>Clone the github repo on your machine:<br><code>git clone https://github.com/khasaad/YOLO-V5_Transfer-Learning_for_computer_vision.git</code></li>
  <li><code>pip install -r requirements.txt</code></li>
  <li>Copy the contents of <a href='https://github.com/khasaad/YOLO-V5_Transfer-Learning_for_computer_vision/tree/main/datasets'>datasets</a> in the same folder.</li>
</ol>

# New custom dataset
<p>Because there are errors in the database from <a href='https://exxact-robotics.com/'>Exxact Robotics</a> company in boundry box of sets of fruits in several images, The cleaned data is modified manually to match with <a href='https://github.com/ultralytics/yolov5'>YOLO v5</a> open source. </p>

<p>The new cleaned data called <a href='https://github.com/khasaad/YOLO-V5_Transfer-Learning_for_computer_vision/tree/main/deep_fruits_data'>deep_fruits_data</a>.</p>

<p>For the dataset to be understandable by YOLO V5, the images and labels must be contained in a specific folder tree:</p>

<pre><code>deep_fruits_data/
    images/
        train/
            &lt;all training images&gt;
        val/
            &lt;all validation imagest&gt;
 
    labels/
        train/
            &lt;all labels of training images in txt format&gt;
        val/
            &lt;all labels of validation images in txt format&gt;

</code></pre>

# Fine-tune a pre-trained <a href='https://github.com/ultralytics/yolov5'>YOLO v5</a> model for detecting and classifying fruits items from images.

<p>We will use google colab file <a href='https://github.com/khasaad/YOLO-V5_Transfer-Learning_for_computer_vision/blob/main/Transfer_Learning_fine_tune_with_YOLOv5.ipynb'>Transfer_Learning_fine_tune_with_YOLOv5.ipynb</a>:</p>
<ul>
<li>1. Make folder <a href='https://github.com/khasaad/YOLO-V5_Transfer-Learning_for_computer_vision/tree/main/deep_fruits_data'>deep_fruits_data</a> with unzip format, then put it on the workspace of google colab, once the download of unzip file is finished, unzip it. (you will find the command line to unzip folder in google colab file)</li>
<li>2. Install Python >= 3.6.0 required with all requirements.txt dependencies installed</li>
<pre>$ git clone https://github.com/ultralytics/yolov5
$ <span class="pl-c1">cd</span> yolov5
$ pip install -r requirements.txt</pre>
<li>Add deep_fruits_yaml.yaml file in the following directory yolov5/data/ to obtain this path: yolov5/data/deep_fruits_yaml.yaml<li>
<li>The all next steps to train and evaluate model exist with details on google colab.</li>  
</ul>
