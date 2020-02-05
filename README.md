# Yolov3 + Deep Sort with PyTorch

![](Town.gif)

## Introduction

This directory contains a moded version of PyTorch YOLOv3 (https://github.com/ultralytics/yolov3). It passes the detections to a Deep Sort algorithm (https://github.com/ZQPei/deep_sort_pytorch) which tracks the detected objects.

## Description

The implementation is based on two papers:

- Simple Online and Realtime Tracking with a Deep Association Metric
https://arxiv.org/abs/1703.07402
- YOLOv3: An Incremental Improvement
https://arxiv.org/abs/1804.02767

## Requirements

Python 3.7 or later with all of the `pip install -U -r requirements.txt` packages including:
- `torch >= 1.3`
- `opencv-python`
- `Pillow`

All dependencies are included in the associated docker images. Docker requirements are: 
- `nvidia-docker`
- Nvidia Driver Version >= 440.44

## Tracking

`track.py` runs tracking on any video source:

```bash
python3 track.py --source ...
```

- Video:  `--source file.mp4`
- Webcam:  `--source 0`
- RTSP stream:  `--source rtsp://170.93.143.139/rtplive/470011e600ef003a004ee33696235daa`
- HTTP stream:  `--source http://wmccpinetop.axiscam.net/mjpg/video.mjpg`

## Other information

For more detailed information about the algorithms used in this project access their official github implementations.

