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
> Note: he dataset and model files are not included in this repository.
> Please download or prepare the dataset according to the structure above (e.g., by extracting the provided assignment package).
> On a **local machine**, place the dataset in the same structure and update notebook file paths to match your directories.
> Both the best mAP models can be trained from scratch using the provided notebooks.
> If you want to skip training and run inference directly, you can download the best trained model from the cloud:    
> - **Best model:** [Put your cloud link here]
> - After downloading, place the checkpoint file at: `./checkpoints_deformable_detr/best_model_by_map.pth`

## Environment Setup

- Python 3.10+
- GPU recommended (CUDA supported)

For running this project on your local machine, follow the steps below.

### Step 0: Clone the Repository

```bash
git clone https://github.com/fangfangirl/CV_HW2.git
cd CV_HW2
```
### Step1: Using Conda (Recommended do)

```bash
# Create a conda environment
conda create -n cv-hw2 python=3.10 -y

# Activate environment
conda activate cv-hw2
```
### Step2: Install PyTorch

Please install PyTorch based on your system configuration:

1. Visit: [https://pytorch.org/get-started/locally/](https://pytorch.org/get-started/locally/)
2. Select your OS, package (pip), and CUDA version
3. Run the generated command

Example (CUDA 12.6):
```bash
pip3 install torch torchvision --index-url https://download.pytorch.org/whl/cu126
```
### Step3: Install Other Dependencies
```bash
pip install -r requirements.txt
```

## Usage

### Training
