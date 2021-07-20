# Lunar
Lunar is a neural network aimbot that uses real-time object detection accelerated with CUDA on Nvidia GPUs.

## About

Lunar can be modified to work with a variety of FPS games; however, it is currently configured for Fortnite. Besides being general purpose, the main advantage of using Lunar is that it is virtually undetectable by anti-cheat software (no memory is meddled with).

The basis of Lunar's player detection is the [YOLOv5](https://github.com/ultralytics/yolov5) architecture written in the PyTorch framework.

https://user-images.githubusercontent.com/45726273/122703651-13542480-d220-11eb-9d0c-43f275de54a1.mp4

## Installation

1. Install a version of [Python](https://www.python.org/downloads/) 3.8 or later.

2. Navigate to the root directory. Use the package manager [pip](https://pip.pypa.io/en/stable/) to install the necessary dependencies.

```
pip install -r requirements.txt
```

## Usage
```           
python lunar.py
```
To update sensitivity settings:
```           
python lunar.py setup
```
To collect image data for annotating and training:
```           
python lunar.py collect_data
```
If you have image data with or with out annotations, please send that in a zip file to [zeyadmansourfwrd@gmail.com](mailto:zeyadmansourfwrd@gmail.com).

## Notes
- As of now, the aimbot is set to only work when targeting/scoping in (holding down the right mouse button). Therefore, it is not recommended to use at a close range.
- There is a known issue that occurs with PyTorch and GTX 1650/1660 GPUs on Windows

## Future Updates
- Use TensorRT for faster inference
- Train a model on a custom dataset
- Explore combining real-time object detection with k-means pixel clustering
- Implement better player tracking
- Make an easy-to-use GUI

## Contributing
Pull requests are welcome. If you have any suggestions, questions, or find any issues, please open an [issue](https://github.com/zeyad-mansour/Lunar/issues) and provide some detail.
If you find this project interesting or helpful, please star the repository.
