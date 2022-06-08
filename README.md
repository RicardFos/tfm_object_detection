# Underwater Species Detection in Images and Videos

This repository includes the docummentation and presentation slides for my Master's Thesis project titled "Underwater Species Detection in Images and Videos" and the jupyter notebooks that include the training and evaluation of Object Detection Models on the Luderick-Seagrass Dataset.

The included files are the following:
* <b>TFM Ricard Fos.pdf</b>: The documentation of the master's thesis
* <b>SlidesTFM.pdf</b>: The slides of the thesis presentation in pdf format
* <b>notebooks</b>: This folder includes the following Jupyter Notebooks:
  * `Data Preprocessing Luderick Seagrass.ipynb`: analizes and preprocesses de data from the luderick-seagrass dataset and saves new preprocessed dataframes as .csv
  * `Luderick Detection Faster R-CNN - Training.ipynb`: Trains a Faster R-CNN model on the Luderick-seagrass dataset
  * `Luderick Detection Faster R-CNN - Inference.ipynb`: Uses and evaluates the trained Faster R-CNN model
  * `Luderick Segmentation Mask R-CNN - Training.ipynb`: Trains a Mask R-CNN model on the Luderick-seagrass dataset
  * `Luderick Segmentation Mask R-CNN - Inference.ipynb`: Uses and evaluates the trained Mask R-CNN model
  * `Luderick Detection YOLOv5 - Training.ipynb`: Trains a YOLOv5 model on the Luderick-seagrass dataset
  * `Luderick Detection YOLOv5 - Inference.ipynb`: Uses and evaluates the trained YOLOv5 model
  * `Luderick Tracking.ipynb`: Implements a simple object tracking algorithm on the trained YOLOv5 results

>The used libraries are included in `requirements.txt` inside the notebooks folder

>The Luderick-Seagrass Dataset can be found in the following repository:
https://github.com/globalwetlands/luderick-seagrass



## Thesis Abstract:

The topic of this study belongs to the area of Deep Learning, which means using neural networks to create predictive models. Concretely, this thesis is about object detection models using Deep Learning to be able to detect and classify underwater species on images and on video in real-time.

The study of Deep Learning methods is more relevant each year, as it is being used on more kinds of problems as the research expands. Object detection is a very useful tool and is becoming the backbone for autonomous robots. Detecting underwater species is an important task given the difficulty of humans to stay in that habitat. Underwater cameras can be used to find given species and can be used to count them and study their behavior.

A study of the origins and evolution of object detection models has been conducted and two detection models and one instance segmentation model have been retrained for the detection of underwater species on a public dataset.  The resulting models have been evaluated in terms of detection speed and precision using the standard metric for object detection called Mean Average Precision. Resulting videos have been generated with drawn detections and segmentation masks. 

Additionally, a simple tracking algorithm has been developed that is able to assign unique ids to each fish on camera and track them until they get out of sight. 

By the end of the thesis the best detection model for underwater videos has been found to be YOLOv5, which achieves good accuracy and framerate.
