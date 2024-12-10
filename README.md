# Acitivity_Recognition_in_Beef_Cattle
This repository contains training and testing code for activity recognition in beef cattle using computer vision

## CLIP training
For training CLIP on our custom dataset, check the [clip training notebook](clip_train_6_classes.ipynb). It assumes the dataset structure is a standard image classification dataset. Separate folders for train, val, and test. Within each folder, there should be separate folders for each class containing images of that class

## YOLO training
We used YOLOv11 classification model (small version). Check the [YOLO](Yolo11_Cls.ipynb) notebook for training this model. We assume the same dataset structure as above.

## Segmentation and Activity classification on videos
Check the [video processing notebook](Segment_and_predict_activity.ipynb) for applying segmentation followed by activity recognition (using our trained YOLO model) on each detected cow. You can check a sample [processed frame](segment_classify_sample_frame.jpg)

## Results
[YOLO results on our test set](yolo_confusion_matrix.png)

