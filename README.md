# Introduction

This directory contains a moded version of PyTorch YOLOv3 (https://github.com/ultralytics/yolov3). It passes the detections to a Deep Sort algorithm (https://github.com/ZQPei/deep_sort_pytorch) which keeps track of the objects.

# Description

The implementation is based on two papers:
Simple Online and Realtime Tracking with a Deep Association Metric
https://arxiv.org/abs/1703.07402
YOLOv3: An Incremental Improvement
https://arxiv.org/abs/1804.02767

# Requirements

Python 3.7 or later with all of the `pip install -U -r requirements.txt` packages including:
- `torch >= 1.3`
- `opencv-python`
- `Pillow`

All dependencies are included in the associated docker images. Docker requirements are: 
- `nvidia-docker`
- Nvidia Driver Version >= 440.44

# Tracking

In order to run the tracking on a video
`python3 detect.py --source /path/to/video`



