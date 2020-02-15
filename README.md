# dli_thumbs

NVIDIA IoT [Deep Learning Institute](https://www.nvidia.com/en-us/deep-learning-ai/education/) thumbs image classifier at the edge (IoT) project for Jetson Nano. 

This project is meant to be run at the edge on an NVIDIA Jetson Nano (or similar ARM IoT architecture computer).  

## Requirements
* Jetpack SDK or [DLI Jetson Nano image](https://developer.download.nvidia.com/training/nano/ainano_v1-1-1_20GB_200203B.zip) (preferably the latter for headless mode compatibility)
* [Jetcam](https://github.com/NVIDIA-AI-IOT/jetcam)
* Jupyter Notebooks (AKA IPython)
* Pytorch


## Repository structure ##

### [data](data) 
Contains 600 images taken and used for training. The images were encrypted for privacy purposes.

### [models](models) 
Contains different model iterations and are named after the total training images and epochs. The best performing model is the *thumbs300dp_30ep.pth* model which was trained with 300 images per class and for a total of 30 epochs.

### [notebooks](notebooks)
Contains the Jupyter notebook used to interactively train and evaluate a thumbs position (up or down) model using deep learning and PyTorch.

### [src](src)
Standard src scripts and utilities plus a folder structure generator script.

## License
[MIT License](https://github.com/socd06/dli_thumbs/blob/master/LICENSE)
