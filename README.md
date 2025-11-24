# CTNet
CTNet: A Dual-Branch Contextual Feature Fusion Network for Remote Sensing Object Detection
CTNet is a novel object detection framework tailored for remote sensing imagery, built upon an enhanced YOLOv11 architecture. By integrating three key modules — CTBC, DCFOConv, and FESF — CTNet effectively addresses the challenges of small objects, dense scenes, complex backgrounds, and large scale variations commonly found in aerial and satellite images.
 Project Overview
This repository implements CTNet, which introduces:

CTBC (Concurrent Two-branch Contextual Attention)
→ Embedded in Bottleneck blocks to jointly enhance channel and spatial attention.
DCFOConv (Dual-Core Feature Optimization Convolution)
→ Replaces standard convolutions in the Neck to capture multi-scale contextual information.
FESF (Feature Enhancement and Selective Fusion)
→ Integrated into C3k modules to recover fine-grained details via high-level semantic guidance.
The model uses SIoU loss for faster convergence and higher localization accuracy. Trained and evaluated on the RSOD dataset, CTNet significantly reduces false negatives and improves detection precision.
 Getting Started
Prerequisites
Python ≥ 3.9
PyTorch ≥ 2.0
CUDA (recommended)
pip install -r requirements.txt
