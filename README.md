# Acitivity_Recognition_in_Beef_Cattle
This repository contains training and testing code for activity recognition in beef cattle using computer vision

## CLIP training
For training CLIP on our custom dataset, check the notebook clip_train_on_6_classes. It assumes the dataset structure is a standard image classification dataset. Separate folders for train, val, and test. Within each folder, there should be separate folders for each class containing images of that class

## YOLO training
We used YOLOv11 classification model (small version). Check the Yolov11_cls notebook for training this model. We assume the same dataset structure as above.

## Segmentation and Activity classification on videos
Check the notebook Segment_and_predict_activity for applying segmentation followed by activity recognition (using our trained YOLO model) on each detected cow. You can check a sample [processed frame](segment_classify_sample_frame.jpg)

## Results
[YOLO results on our test set](yolo_confusion_matrix.png)

