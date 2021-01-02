[![License CC BY-NC-SA 4.0](https://img.shields.io/badge/license-CC4.0-blue.svg)](https://raw.githubusercontent.com/NVIDIA/FastPhotoStyle/master/LICENSE.md)
![Python 2.7](https://img.shields.io/badge/python-2.7-green.svg)
![Python 3.5](https://img.shields.io/badge/python-3.5-green.svg)

## Making this work in 2021 using Azure NC Promo VM
Modifications to the dockerfile are already availble.
### Step 1 - Create an Azure VM resource with following specs
SKU - NC Promo / NC'

Region - Northern Europe

OS - Ubuntu 16.04

Disk - HDD

### Step 2 - Enable GPU Driver in the VM host
Use https://docs.microsoft.com/en-us/azure/virtual-machines/linux/n-series-driver-setup

### Step 3 - Install Docker
Use https://docs.docker.com/engine/install/ubuntu/

### Step 4 - Install Nvidia-Docker 2
Use https://justusnithushan.medium.com/nvidia-docker2-installation-procedure-in-ubuntu16-04-a9a5d8513cba

### Step 5 - Ensure things are ok
Execute  `sudo docker run --runtime=nvidia --rm nvidia/cuda nvidia-smi`

### Step 6 - Follow [tutorial](TUTORIAL.md)

## FastPhotoStyle

### License
Copyright (C) 2018 NVIDIA Corporation.  All rights reserved.
Licensed under the CC BY-NC-SA 4.0 license (https://creativecommons.org/licenses/by-nc-sa/4.0/legalcode).

<img src="https://raw.githubusercontent.com/NVIDIA/FastPhotoStyle/master/teaser.png" width="800" title="Teaser results"> 


### What's new
 
 | Date     | News |
 |----------|--------------|
 |2018-07-25| Migrate to pytorch 0.4.0. For pytorch 0.3.0 user, check out [FastPhotoStyle for pytorch 0.3.0](https://github.com/NVIDIA/FastPhotoStyle/releases/tag/f33e07f). |
 |          | Add a [tutorial](TUTORIAL.md) showing 3 ways of using the FastPhotoStyle algorithm.|
 |2018-07-10| Our paper is accepted by the ECCV 2018 conference!!! | 


### About

Given a content photo and a style photo, the code can transfer the style of the style photo to the content photo. The details of the algorithm behind the code is documented in our arxiv paper. Please cite the paper if this code repository is used in your publications.

[A Closed-form Solution to Photorealistic Image Stylization](https://arxiv.org/abs/1802.06474) <br> 
[Yijun Li (UC Merced)](https://sites.google.com/site/yijunlimaverick/), [Ming-Yu Liu (NVIDIA)](http://mingyuliu.net/), [Xueting Li (UC Merced)](https://sunshineatnoon.github.io/), [Ming-Hsuan Yang (NVIDIA, UC Merced)](http://faculty.ucmerced.edu/mhyang/), [Jan Kautz (NVIDIA)](http://jankautz.com/) <br>
European Conference on Computer Vision (ECCV), 2018 <br>


### Tutorial

Please check out the [tutorial](TUTORIAL.md).


