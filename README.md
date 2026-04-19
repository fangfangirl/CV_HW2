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
│   └─ best_model_by_map.pth # test mAP model
├─ cv-hw2-training.ipynb
├─ cv-hw2-inference.ipynb
├─ README.md
└─ requirements.txt
```
> Note: The dataset and trained checkpoint files are not included in this repository.
> Please prepare the dataset according to the assignment structure before running the notebooks.
> If you want to skip training and run inference directly, you can download the best trained model from the cloud:
> - **Best model:** [Put your cloud link here]
> - After downloading, place the checkpoint file at: `./checkpoints_deformable_detr/best_model_by_map.pth`
> If you want to **skip training** and run inference directly, you can download the pretrained models from the cloud:  
> - [Teacher model](https://drive.google.com/file/d/1nqS_6sRFx52BCtmqBfd8aG7UL62c1ryw/view?usp=sharing)  
> - [Student model](https://drive.google.com/file/d/11-vZi80MOn4BH1DpQdgalRQlvz7mb7SD/view?usp=sharing)
