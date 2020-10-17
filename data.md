## Calibration Data

[Download link（Synology）](http://gofile.me/3REyI/kUsHfzy4h)

[Download link（Baidu Pan）](https://pan.baidu.com/s/1DSh0r_CxN8FoRVxf-V5uUg)(pyue)

## Calibration files

[Download link（Synology）](http://gofile.me/3REyI/GfYCexfS3)

[Download link（Baidu Pan）](https://pan.baidu.com/s/1t1ViINDmI8Mv3KVICzXNRQ)(r8vq)

## Dataset sequences

We provide several types of sequences for evaluating the multi-spectral nvigation systems. The naming is explained below. 

- Scene: 
    - *desk*: Sequences in the room with Motion Capture system, where ground truth poses are available for the entire trajectory.
    - *magistrale* : Sequences featuring a walk around in a university building. Ground truth poses are available for the start and end segments.
    - *outdoor* : Outdoor sequences. Ground truth poses are available for the start and end segments.
    - *lift* : Specially changeling sequences which contain the camera leads to different floors via elevator.. Ground truth poses are available for the start and end segments.
- Illumination:
    - bright: Most *desk* sequences recorded in bright environments,
    - varing: *ic*: data with lights turned on and off randomly. 
    - dim: *dim*: data where the scene is dark.
    - complex: *magistrale* and *outdoor* sequences are recorded under complex illumination.
- Motion: 
    - *halfsphere*: the camera moves along the trajectory of a halfsphere with a diameter of 1m.
    - *xyz*: the camera moves approximately along the x, y, and z axes.
    - *rpy*: the camera only rotates with roll, pitch, and yaw motion.
    - *circle*: the camera moves approximately around a circle.
    - *static*: the camera is nearly motionless.

#### Bright illumination

Sequence Name | Duration(s) | link(Synology) | link（Baidu Pan）| Difficulty
------------ | ------------- | ------------- | ------------- | ------
desk1-halfsphere | 68.3495 | [ROS bag](http://gofile.me/3REyI/2i5Ftd4RJ) | 提取码: ztbz [链接](https://pan.baidu.com/s/1RdSZAqfG2uEXCcZoOGvzyA) | Easy
desk1-rpy | 61.400 | [ROS bag](http://gofile.me/3REyI/5uH1tqgjy) | 提取码: myuc [链接](https://pan.baidu.com/s/1J13QTOwiKfvgmsQyAvBcTw) | Easy
desk1-static | 25.2803 | [ROS bag](http://gofile.me/3REyI/kHp4vRcmO)| 提取码: rm96 [链接](https://pan.baidu.com/s/1csVeoQXXPHALIgJ0Yw8x_g) | Easy
desk1-xyz | 48.5500 | [ROS bag](http://gofile.me/3REyI/YlQHZfX45)| 提取码: mpuk [链接](https://pan.baidu.com/s/18FbnK_qWJVDudngCgWqhaw) | Easy
desk2-circle | 34.5399 | [ROS bag](http://gofile.me/3REyI/KOdud2n2N)| 提取码: 2dq5 [链接](https://pan.baidu.com/s/1RWvY7-4HP5rdzP7irQoAyQ) | Easy
desk2-halfsphere | 44.3201 | [ROS bag](http://gofile.me/3REyI/ooDVJCWgr)| 提取码: 5c9m [链接](https://pan.baidu.com/s/1D5hs8Z8tVs9IEXLXwPIrqA) | Easy
desk2-rpy | 47.7005 | [ROS bag](http://gofile.me/3REyI/lLaYCERxm)| 提取码: 936f [链接](https://pan.baidu.com/s/1ywyE9gRqBydQf1xslJfFng) | Easy
desk2-static | 33.3701 | [ROS bag](http://gofile.me/3REyI/Ph9SFPwB2)| 提取码: uyu2 [链接](https://pan.baidu.com/s/1e3mQdkdLQ6maMt2wIMsLAQ) | Easy
desk2-xyz | 44.9602 | [ROS bag](http://gofile.me/3REyI/kN4lCw1Rc)| 提取码: 9jt8 [链接](https://pan.baidu.com/s/1l4WQ3Pp1IXQLyntHzS85ug) | Easy
desk1-circle-person | 33.8101 | [ROS bag](http://gofile.me/3REyI/kplECtUMo)| 提取码: bhgk [链接](https://pan.baidu.com/s/1kwfJoD_rowuJJwrXA-3NcQ) | Easy
desk1-halfsphere-person | 76.9798 | [ROS bag](http://gofile.me/3REyI/cA0yfUnLd)| 提取码: i827 [链接](https://pan.baidu.com/s/1O8nVUQcXMTX6BdJFYoiPqQ) | Easy
desk1-rpy-person | 60.0997 | [ROS bag](http://gofile.me/3REyI/UVH9dyS6P)| 提取码: d2di [链接](https://pan.baidu.com/s/1_0SNWvMWEoFOmIhs59Tasg) | Easy
desk1-rpy-person-slow | 59.5304 | [ROS bag](http://gofile.me/3REyI/zfDZx30hz)| 提取码: queg [链接](https://pan.baidu.com/s/1lPgHpVdropFhxzd0hiMucQ) | Easy
desk1-static-person | 19.9794 | [ROS bag](http://gofile.me/3REyI/HUIivGkp0)| 提取码: j94s [链接](https://pan.baidu.com/s/18q0ukNwTTDojDzkk5N-TaQ) | Easy
desk1-xyz-person| 51.1640 | [ROS bag](http://gofile.me/3REyI/jAhTahEN4)| 提取码: 69ue [链接](https://pan.baidu.com/s/10mHosWzfCEqnSTd2tTmNRg) | Easy
desk1-halfsphere-dy | 64.0704 | [ROS bag](http://gofile.me/3REyI/iXXNl3QFB)| 提取码: kfjj [链接](https://pan.baidu.com/s/1hQrc5oPevW3aALahjFQ4YQ) | Easy
desk1-rpy-dy | 48.4592 | [ROS bag](http://gofile.me/3REyI/r86csUhd9)| 提取码: gced [链接](https://pan.baidu.com/s/1ooc0NKylGw-n94OhIXGZPQ) | Easy
desk1-static-dy | 24.9294 | [ROS bag](http://gofile.me/3REyI/F8BLNAo1Q)| 提取码: s4ye [链接](https://pan.baidu.com/s/136gRHzqtChQOCZNyvlcrbQ) | Easy
desk1-xyz-dy | 48.7687 | [ROS bag](http://gofile.me/3REyI/pkjY6oRqA)| 提取码: 3axs [链接](https://pan.baidu.com/s/1SaskfehN43sPdsiYGfOYhg) | Easy

#### Varing illumination

Sequence Name | Duration(s) | link(Synology) | link（Baidu Pan）| Difficulty
------------ | ------------- | -----|----------- | ------
desk1-rpy-ic | 62.8403 | [ROS bag](http://gofile.me/3REyI/oBOEOZFDI)| 提取码: vat8 [链接](https://pan.baidu.com/s/1kd-pplif5so9ToHlF-9oEg) | Hard
desk1-halfsphere-ic | 73.5899 | [ROS bag](http://gofile.me/3REyI/BMh1xxImI)| 提取码: 8vti [链接](https://pan.baidu.com/s/1LoJLm3905GdjMqQwKHxdFQ) | Hard
desk1-static-ic | 27.6798 | [ROS bag](http://gofile.me/3REyI/tboURe3jz)| 提取码: tf7k [链接](https://pan.baidu.com/s/1jR5z3_J2BTzqPsvQb8X2og) | Hard
desk1-static-ic-lampon | 24.7401 | [ROS bag](http://gofile.me/3REyI/LsaAFtk1q)| 提取码: 9k6t [链接](https://pan.baidu.com/s/1xak1SPhGB5gCqunLGFSAaA) | Hard
desk1-xyz-ic | 67.2905 | [ROS bag](http://gofile.me/3REyI/y1GluJbxQ)| 提取码: gac5 [链接](https://pan.baidu.com/s/1Ts8B-GPLcbhYQag9VqSrKA) | Hard
desk2-circle-ic | 30.1300 | [ROS bag](http://gofile.me/3REyI/h3u2P26rw)| 提取码: ccgx [链接](https://pan.baidu.com/s/1h6RVlDp3ueezHyBEHyiUsQ) | Hard
desk2-rpy-ic | 64.8807 | [ROS bag](http://gofile.me/3REyI/PO1N9thQT)| 提取码: htej [链接](https://pan.baidu.com/s/15eUnxlpf1_tNU_sSM5MOLA) | Hard
desk2-static-ic | 23.9501 | [ROS bag](http://gofile.me/3REyI/SCG2KZ5Jg)| 提取码: iw59 [链接](https://pan.baidu.com/s/1OmYeRWJq7iUkgHjDLgvDEg) | Hard
desk2-xyz-ic | 52.1794 | [ROS bag](http://gofile.me/3REyI/ZMKhDO3JJ)| 提取码: pc4k [链接](https://pan.baidu.com/s/1ozXPCkpOT3blZQe2B2ht4g) | Hard
desk1-halfsphere-ic-person | 66.9900 | [ROS bag](http://gofile.me/3REyI/xK6X42G1u)| 提取码: fcbb [链接](https://pan.baidu.com/s/1KMxfbkU-JGIYOwLZUlyTLQ) | Hard
desk1-rpy-ic-person | 56.2300 | [ROS bag](http://gofile.me/3REyI/l3nxmDunn)| 提取码: h48m [链接](https://pan.baidu.com/s/1jm6tTwGb_GmPBy_wEIP7OA) | Hard
desk1-static-ic-person| 33.8796 | [ROS bag](http://gofile.me/3REyI/6tbQq7jpB)| 提取码: 9vhm [链接](https://pan.baidu.com/s/1biCeEAFBaNpP0ypHxCltfA) | Hard
desk1-xyz-ic-person| 54.1956 | [ROS bag](http://gofile.me/3REyI/6HZwfz5dy)| 提取码: xp9u [链接](https://pan.baidu.com/s/1gJ4Z5WlSBIvlmmuY2vCDEA) | Hard

#### Dim illumination

Sequence Name | Duration(s) | link(Synology) | link（Baidu Pan）| Difficulty
------------ | ------------- | ----|-------|-------
desk1-halfsphere-dim| 69.2399 | [ROS bag](http://gofile.me/3REyI/ziCAII1EQ)| 提取码: tcmr [链接](https://pan.baidu.com/s/1DQ3RptLC59NvD3giDZ-sxw) | Medium
desk1-halfsphere-dim2| 67.8903 | [ROS bag](http://gofile.me/3REyI/Eajzct1Oi)| 提取码: h36m [链接](https://pan.baidu.com/s/1wrQAeZqRpYavUO6tz2EsrA)| Medium
desk1-rpy-dim| 48.0199 | [ROS bag](http://gofile.me/3REyI/XouKWswWr)| 提取码: cqs3 [链接](https://pan.baidu.com/s/1L7zi7nxjhPsLGeYEgsmw-w)| Medium
desk1-rpy-dim2| 52.5703 | [ROS bag](http://gofile.me/3REyI/SGB4ej54e)| 提取码: 4sch [链接](https://pan.baidu.com/s/1XMbKmjMHH7ZaH90OOzeL0A)| Medium
desk1-static-dim| 21.5306 | [ROS bag](http://gofile.me/3REyI/PFXXJHRoE)| 提取码: vsgf [链接](https://pan.baidu.com/s/1b92QhEeKpOVx9mdN6dwfRQ)| Medium
desk1-static-dim2| 19.4200 | [ROS bag](http://gofile.me/3REyI/4DugILwLQ)| 提取码: yp49 [链接](https://pan.baidu.com/s/1uzMaNTRXVu-Q5dupXswXUg)| Medium
desk1-xyz-dim| 53.6903 | [ROS bag](http://gofile.me/3REyI/KuX7XLNFQ)| 提取码: uqir [链接](https://pan.baidu.com/s/15PB0MPjzNGRSIl1qMo4itA)| Medium
desk1-xyz-dim2| 53.8106 | [ROS bag](http://gofile.me/3REyI/N8srviLGn)| 提取码: djkd [链接](https://pan.baidu.com/s/1-EuP3azpj6k_1XxjI980CA)| Medium

