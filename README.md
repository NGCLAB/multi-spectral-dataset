# <img src="images/ngc.png" width="20" /> Multi-Spectral Dataset with depth images

## Introduction

The multi-spectral dataset is provided for evaluating multi-spectral motion estimation methods. The dataset includes a set of sequences in diverse illumination conditions obtained on a setup consisting of a standard camera, an LWIR camera, and a Kinect2. In the dataset, each sequence contains the color, thermal, and depth images, as well as the ground-truth trajectory. The color and thermal images (640 x 480) are captured at 32Hz on hardware-synchronized devices. The depth images are provided by the Kinect2 camera at 30Hz, enabling the projection of one image onto another. The ground-truth poses are recorded from a motion capture system at 120Hz. All sensors are calibrated carefully for higher accuracy.

### Sequences

#### Bright illumination

Sequence Name | Duration(s) | Download link
------------ | ------------- | ---
desk1-halfsphere | 68.3495 | [ROS bag](http://gofile.me/3REyI/2i5Ftd4RJ)
desk1-rpy | 61.400 | [ROS bag](http://gofile.me/3REyI/5uH1tqgjy)
desk1-static | 25.2803 | [ROS bag](http://gofile.me/3REyI/kHp4vRcmO)
desk1-xyz | 48.5500 | [ROS bag](http://gofile.me/3REyI/YlQHZfX45)
desk2-circle | 34.5399 | [ROS bag](http://gofile.me/3REyI/KOdud2n2N)
desk2-halfsphere | 44.3201 | [ROS bag](http://gofile.me/3REyI/ooDVJCWgr)
desk2-rpy | 47.7005 | [ROS bag](http://gofile.me/3REyI/lLaYCERxm)
desk2-static | 33.3701 | [ROS bag](http://gofile.me/3REyI/Ph9SFPwB2)
desk2-xyz | 44.9602 | [ROS bag](http://gofile.me/3REyI/kN4lCw1Rc)
desk1-circle-person | 33.8101 | [ROS bag](http://gofile.me/3REyI/kplECtUMo)
desk1-halfsphere-person | 76.9798 | [ROS bag](http://gofile.me/3REyI/cA0yfUnLd)
desk1-rpy-person | 60.0997 | [ROS bag](http://gofile.me/3REyI/UVH9dyS6P)
desk1-rpy-person-slow | 59.5304 | [ROS bag](http://gofile.me/3REyI/zfDZx30hz)
desk1-static-person | 19.9794 | [ROS bag](http://gofile.me/3REyI/HUIivGkp0)
desk1-xyz-person| 51.1640 | [ROS bag](http://gofile.me/3REyI/jAhTahEN4)
desk1-halfsphere-dy | 64.0704 | [ROS bag](http://gofile.me/3REyI/iXXNl3QFB)
desk1-rpy-dy | 48.4592 | [ROS bag](http://gofile.me/3REyI/r86csUhd9)
desk1-static-dy | 24.9294 | [ROS bag](http://gofile.me/3REyI/F8BLNAo1Q)
desk1-xyz-dy | 48.7687 | [ROS bag](http://gofile.me/3REyI/pkjY6oRqA)

#### Varing illumination

Sequence Name | Duration(s) | Download link
------------ | ------------- | ---
desk1-rpy-ic | 62.8403 | [ROS bag](http://gofile.me/3REyI/oBOEOZFDI)
desk1-halfsphere-ic | 73.5899 | [ROS bag](http://gofile.me/3REyI/BMh1xxImI)
desk1-static-ic | 27.6798 | [ROS bag](http://gofile.me/3REyI/tboURe3jz)
desk1-static-ic-lampon | 24.7401 | [ROS bag](http://gofile.me/3REyI/LsaAFtk1q)
desk1-xyz-ic | 67.2905 | [ROS bag](http://gofile.me/3REyI/y1GluJbxQ)
desk2-circle-ic | 30.1300 | [ROS bag](http://gofile.me/3REyI/h3u2P26rw)
desk2-rpy-ic | 64.8807 | [ROS bag](http://gofile.me/3REyI/PO1N9thQT)
desk2-static-ic | 23.9501 | [ROS bag](http://gofile.me/3REyI/SCG2KZ5Jg)
desk2-xyz-ic | 52.1794 | [ROS bag](http://gofile.me/3REyI/ZMKhDO3JJ)
desk1-halfsphere-ic-person | 66.9900 | [ROS bag](http://gofile.me/3REyI/xK6X42G1u)
desk1-rpy-ic-person | 56.2300 | [ROS bag](http://gofile.me/3REyI/l3nxmDunn)
desk1-static-ic-person| 33.8796 | [ROS bag](http://gofile.me/3REyI/6tbQq7jpB)
desk1-xyz-ic-person| 54.1956 | [ROS bag](http://gofile.me/3REyI/6HZwfz5dy)

#### Dim illumination

Sequence Name | Duration(s) | Download link
------------ | ------------- | ---
desk1-halfsphere-dim| 33.8101 | [ROS bag](http://gofile.me/3REyI/ziCAII1EQ)
desk1-halfsphere-dim2| 33.8101 | [ROS bag](http://gofile.me/3REyI/Eajzct1Oi)
desk1-rpy-dim| 33.8101 | [ROS bag](http://gofile.me/3REyI/XouKWswWr)
desk1-rpy-dim2| 33.8101 | [ROS bag](http://gofile.me/3REyI/SGB4ej54e)
desk1-static-dim| 33.8101 | [ROS bag](http://gofile.me/3REyI/PFXXJHRoE)
desk1-static-dim2| 33.8101 | [ROS bag](http://gofile.me/3REyI/4DugILwLQ)
desk1-xyz-dim| 33.8101 | [ROS bag](http://gofile.me/3REyI/KuX7XLNFQ)
desk1-xyz-dim2| 33.8101 | [ROS bag](http://gofile.me/3REyI/N8srviLGn)

## Calibration Data

[Download link](http://gofile.me/3REyI/kUsHfzy4h)

## Calibration files

[Download link](http://gofile.me/3REyI/GfYCexfS3)

## Evaluation Tool

We provide MATLAB and python tools that have motion estimation function for visual odometry or SLAM works. ([Github Page](https://github.com/weichnn/Evaluation_Tools))
