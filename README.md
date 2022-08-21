# CMPE249_Project

# Installation Steps
The steps below will allow you to generate an environment that should allow you to execute the Jupyter Notebooks that will generate disparity map, disparity map errors and visualization for the various models.

## 1) Go To directory to store repo
    $ cd <directory to store repos>

## 2) Clone Project Git Repo
    $ git clone git@github.com:curtisjm17/CMPE249_Project.git
    $ cd CMPE249_Project

## 3) Create and activate Conda environment
    $ conda create --name argoStereo python=3.8 -y
    $ conda activate argoStereo

## 4) Install dependencies
    $ pip install opencv-contrib-python
    $ pip install plotly
    $ pip install open3d
    $ pip install torch
    $ pip install torchvision
    
## 5) Clone PSMNet Repo and get pre-trained model
    $ git clone git@github.com:curtisjm17/argoverse-api.git

## 6) Install Argoverse
    $ pip install -e ./argoverse-api/

## 7) Clone PSMNet Repo and get pre-trained model
    $ git clone git@github.com:JiaRenChang/PSMNet.git
    $ wget https://drive.google.com/u/0/uc?id=1pHWjmhKMG4ffCrpcsp_MTXMJXhgl3kF9 -O ./PSMNet/pretrained_model_KITTI2015.tar 

## 8) Create Argoverse data directory structure
    $ mkdir <directory to store repos>/argoverse_stereo_v1.1

## 9) Download Argo Stereo Dataset from following location
    $ wget https://s3.amazonaws.com/argoai-argoverse/rectified_stereo_images_v1.1.tar.gz -O ./argoverse_stereo_v1.1/rectified_stereo_images_v1.1.tar.gz
    $ wget https://s3.amazonaws.com/argoai-argoverse/disparity_maps_v1.1.tar.gz -O ./argoverse_stereo_v1.1/disparity_maps_v1.1.tar.gz 

## 10) Untar data
    $ gunzip disparity_maps_v1.1.tar.gz
    $ tar -xf disparity_maps_v1.1.tar
    $ gunzip rectified_stereo_images_v1.1.tar.gz
    $ tar -xf rectified_stereo_images_v1.1.tar

# Results
Results generated from these models can be found here:\
https://drive.google.com/drive/folders/1qzRZFK35v3Jdq8aCoflg6QV_ajw-339O?usp=sharing
