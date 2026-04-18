# NYCU Computer Vision 2026 HW2

* **Student ID:** 314511037
* **Name:** 張周芳

## Introduction
This project implements an object detection pipeline for HW2 using a DETR-based architecture with a ResNet-50 backbone.  
The final model is based on Deformable DETR and is designed to improve detection performance on small RGB images.

The project includes:
- A notebook for training the detection model
- A notebook for inference on the test dataset
- Validation evaluation using COCO-format metrics
- Visualization utilities for prediction analysis

## Dataset
Place the dataset folder under the following structure:

```bash
CV_HW2/
├─ nycu-hw2-data/
│   ├─ train/
│   ├─ valid/
│   ├─ test/
│   ├─ train.json
│   └─ valid.json
├─ checkpoints_deformable_detr/
│   └─ best_model_by_map.pth
├─ cv-hw2-training.ipynb
├─ cv-hw2-inference.ipynb
├─ README.md
└─ requirements.txt
```
> Note: The dataset and trained checkpoint files are not included in this repository.
> Please prepare the dataset according to the assignment structure before running the notebooks.
> If you would like to run inference directly, place the trained model checkpoint at:
`./checkpoints_deformable_detr_baby/best_model_by_map.pth`
