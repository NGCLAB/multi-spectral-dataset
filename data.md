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
- Other:
    - *dy*: a person is walking around in front of the setup to add disturbances.
    - *person*: a person sitting in front of a desk to provide striking contrasts in textures in the thermal images.
    - *day*: the data is collected before sunset
    - *night*: the data is collected before sunset

### The environment under bright illumination

Sequence Name | Duration(s) | Size(GB)  | link(Synology) | link（Baidu Pan）| Difficulty
------------ | ------------- | ------------- | ------------- | ------------- | ------
desk1-halfsphere | 68.34 | 5.18 | [ROS bag](http://gofile.me/3REyI/2i5Ftd4RJ) | 提取码: ztbz [链接](https://pan.baidu.com/s/1RdSZAqfG2uEXCcZoOGvzyA) | Easy
desk1-rpy | 61.40 | 7.32 | [ROS bag](http://gofile.me/3REyI/5uH1tqgjy) | 提取码: myuc [链接](https://pan.baidu.com/s/1J13QTOwiKfvgmsQyAvBcTw) | Easy
desk1-static | 25.28 | 3.03 | [ROS bag](http://gofile.me/3REyI/kHp4vRcmO)| 提取码: rm96 [链接](https://pan.baidu.com/s/1csVeoQXXPHALIgJ0Yw8x_g) | Easy
desk1-xyz | 48.55 | 5.93 | [ROS bag](http://gofile.me/3REyI/YlQHZfX45)| 提取码: mpuk [链接](https://pan.baidu.com/s/18FbnK_qWJVDudngCgWqhaw) | Easy
desk2-circle | 34.53 | 3.81 | [ROS bag](http://gofile.me/3REyI/KOdud2n2N)| 提取码: 2dq5 [链接](https://pan.baidu.com/s/1RWvY7-4HP5rdzP7irQoAyQ) | Easy
desk2-halfsphere | 44.32 | 5.18 | [ROS bag](http://gofile.me/3REyI/ooDVJCWgr)| 提取码: 5c9m [链接](https://pan.baidu.com/s/1D5hs8Z8tVs9IEXLXwPIrqA) | Easy
desk2-rpy | 47.70 | 5.52 | [ROS bag](http://gofile.me/3REyI/lLaYCERxm)| 提取码: 936f [链接](https://pan.baidu.com/s/1ywyE9gRqBydQf1xslJfFng) | Easy
desk2-static | 33.37 | 3.99| [ROS bag](http://gofile.me/3REyI/Ph9SFPwB2)| 提取码: uyu2 [链接](https://pan.baidu.com/s/1e3mQdkdLQ6maMt2wIMsLAQ) | Easy
desk2-xyz | 44.96 | 3.99|[ROS bag](http://gofile.me/3REyI/kN4lCw1Rc)| 提取码: 9jt8 [链接](https://pan.baidu.com/s/1l4WQ3Pp1IXQLyntHzS85ug) | Easy
desk1-circle-person | 33.81 | 4.07 | [ROS bag](http://gofile.me/3REyI/kplECtUMo)| 提取码: bhgk [链接](https://pan.baidu.com/s/1kwfJoD_rowuJJwrXA-3NcQ) | Easy
desk1-halfsphere-person | 76.97  | 9.37| [ROS bag](http://gofile.me/3REyI/cA0yfUnLd)| 提取码: i827 [链接](https://pan.baidu.com/s/1O8nVUQcXMTX6BdJFYoiPqQ) | Easy
desk1-rpy-person | 60.09 | 7.10 | [ROS bag](http://gofile.me/3REyI/UVH9dyS6P)| 提取码: d2di [链接](https://pan.baidu.com/s/1_0SNWvMWEoFOmIhs59Tasg) | Easy
desk1-rpy-person-slow | 59.53 | 6.93 |[ROS bag](http://gofile.me/3REyI/zfDZx30hz)| 提取码: queg [链接](https://pan.baidu.com/s/1lPgHpVdropFhxzd0hiMucQ) | Easy
desk1-static-person | 19.97 | 2.14 | [ROS bag](http://gofile.me/3REyI/HUIivGkp0)| 提取码: j94s [链接](https://pan.baidu.com/s/18q0ukNwTTDojDzkk5N-TaQ) | Easy
desk1-xyz-person| 51.16 | 6.23 | [ROS bag](http://gofile.me/3REyI/jAhTahEN4)| 提取码: 69ue [链接](https://pan.baidu.com/s/10mHosWzfCEqnSTd2tTmNRg) | Easy
desk1-halfsphere-dy | 64.07 |7.28 | [ROS bag](http://gofile.me/3REyI/iXXNl3QFB)| 提取码: kfjj [链接](https://pan.baidu.com/s/1hQrc5oPevW3aALahjFQ4YQ) | Easy
desk1-rpy-dy | 48.45 | 5.48 | [ROS bag](http://gofile.me/3REyI/r86csUhd9)| 提取码: gced [链接](https://pan.baidu.com/s/1ooc0NKylGw-n94OhIXGZPQ) | Easy
desk1-static-dy | 24.92 | 2.81 | [ROS bag](http://gofile.me/3REyI/F8BLNAo1Q)| 提取码: s4ye [链接](https://pan.baidu.com/s/136gRHzqtChQOCZNyvlcrbQ) | Easy
desk1-xyz-dy | 48.76 | 5.38 | [ROS bag](http://gofile.me/3REyI/pkjY6oRqA)| 提取码: 3axs [链接](https://pan.baidu.com/s/1SaskfehN43sPdsiYGfOYhg) | Easy

### The environment under varing illumination

Sequence Name | Duration(s)| Size(GB) | link(Synology) | link（Baidu Pan）| Difficulty
------------ | --------|----- | -----|----------- | ------
desk1-rpy-ic | 62.84 | 7.20 | [ROS bag](http://gofile.me/3REyI/oBOEOZFDI)| 提取码: vat8 [链接](https://pan.baidu.com/s/1kd-pplif5so9ToHlF-9oEg) | Hard
desk1-halfsphere-ic | 73.58 | 8.48 | [ROS bag](http://gofile.me/3REyI/BMh1xxImI)| 提取码: 8vti [链接](https://pan.baidu.com/s/1LoJLm3905GdjMqQwKHxdFQ) | Hard
desk1-static-ic | 27.67 | 3.05 | [ROS bag](http://gofile.me/3REyI/tboURe3jz)| 提取码: tf7k [链接](https://pan.baidu.com/s/1jR5z3_J2BTzqPsvQb8X2og) | Hard
desk1-static-ic-lampon | 24.74 | 2.77 | [ROS bag](http://gofile.me/3REyI/LsaAFtk1q)| 提取码: 9k6t [链接](https://pan.baidu.com/s/1xak1SPhGB5gCqunLGFSAaA) | Hard
desk1-xyz-ic | 67.29 | 7.81 | [ROS bag](http://gofile.me/3REyI/y1GluJbxQ)| 提取码: gac5 [链接](https://pan.baidu.com/s/1Ts8B-GPLcbhYQag9VqSrKA) | Hard
desk2-circle-ic | 30.13 | 3.36 | [ROS bag](http://gofile.me/3REyI/h3u2P26rw)| 提取码: ccgx [链接](https://pan.baidu.com/s/1h6RVlDp3ueezHyBEHyiUsQ) | Hard
desk2-rpy-ic | 64.88 | 7.30 | [ROS bag](http://gofile.me/3REyI/PO1N9thQT)| 提取码: htej [链接](https://pan.baidu.com/s/15eUnxlpf1_tNU_sSM5MOLA) | Hard
desk2-static-ic | 23.95 | 2.74 | [ROS bag](http://gofile.me/3REyI/SCG2KZ5Jg)| 提取码: iw59 [链接](https://pan.baidu.com/s/1OmYeRWJq7iUkgHjDLgvDEg) | Hard
desk2-xyz-ic | 52.17 | 5.77 | [ROS bag](http://gofile.me/3REyI/ZMKhDO3JJ)| 提取码: pc4k [链接](https://pan.baidu.com/s/1ozXPCkpOT3blZQe2B2ht4g) | Hard
desk1-halfsphere-ic-person | 66.99 | 7.45 | [ROS bag](http://gofile.me/3REyI/xK6X42G1u)| 提取码: fcbb [链接](https://pan.baidu.com/s/1KMxfbkU-JGIYOwLZUlyTLQ) | Hard
desk1-rpy-ic-person | 56.23 | 6.32 | [ROS bag](http://gofile.me/3REyI/l3nxmDunn)| 提取码: h48m [链接](https://pan.baidu.com/s/1jm6tTwGb_GmPBy_wEIP7OA) | Hard
desk1-static-ic-person| 33.87 | 3.74 | [ROS bag](http://gofile.me/3REyI/6tbQq7jpB)| 提取码: 9vhm [链接](https://pan.baidu.com/s/1biCeEAFBaNpP0ypHxCltfA) | Hard
desk1-xyz-ic-person| 54.19 | 6.19 | [ROS bag](http://gofile.me/3REyI/6HZwfz5dy)| 提取码: xp9u [链接](https://pan.baidu.com/s/1gJ4Z5WlSBIvlmmuY2vCDEA) | Hard

### The environment under dim illumination

Sequence Name | Duration(s) | Size(GB)| link(Synology) | link（Baidu Pan）| Difficulty
------------ | -------|------ | ----|-------|-------
desk1-halfsphere-dim| 69.23 | 7.12 | [ROS bag](http://gofile.me/3REyI/ziCAII1EQ)| 提取码: tcmr [链接](https://pan.baidu.com/s/1DQ3RptLC59NvD3giDZ-sxw) | Medium
desk1-halfsphere-dim2| 67.89 | 6.98 | [ROS bag](http://gofile.me/3REyI/Eajzct1Oi)| 提取码: h36m [链接](https://pan.baidu.com/s/1wrQAeZqRpYavUO6tz2EsrA)| Medium
desk1-rpy-dim| 48.01 | 4.92 |[ROS bag](http://gofile.me/3REyI/XouKWswWr)| 提取码: cqs3 [链接](https://pan.baidu.com/s/1L7zi7nxjhPsLGeYEgsmw-w)| Medium
desk1-rpy-dim2| 52.57 | 5.39 | [ROS bag](http://gofile.me/3REyI/SGB4ej54e)| 提取码: 4sch [链接](https://pan.baidu.com/s/1XMbKmjMHH7ZaH90OOzeL0A)| Medium
desk1-static-dim| 21.53 | 2.18 | [ROS bag](http://gofile.me/3REyI/PFXXJHRoE)| 提取码: vsgf [链接](https://pan.baidu.com/s/1b92QhEeKpOVx9mdN6dwfRQ)| Medium
desk1-static-dim2| 19.42 | 1.97 | [ROS bag](http://gofile.me/3REyI/4DugILwLQ)| 提取码: yp49 [链接](https://pan.baidu.com/s/1uzMaNTRXVu-Q5dupXswXUg)| Medium
desk1-xyz-dim| 53.69 | 5.51 | [ROS bag](http://gofile.me/3REyI/KuX7XLNFQ)| 提取码: uqir [链接](https://pan.baidu.com/s/15PB0MPjzNGRSIl1qMo4itA)| Medium
desk1-xyz-dim2| 53.81 | 5.52 | [ROS bag](http://gofile.me/3REyI/N8srviLGn)| 提取码: djkd [链接](https://pan.baidu.com/s/1-EuP3azpj6k_1XxjI980CA)| Medium

### The complex environment

Sequence Name  | Size(GB)| link(Synology) | link（Baidu Pan）| Difficulty
------------ | -------|------ | ----|-------|-------
magistrale-23-day1 | 28.70 | [ROS bag](http://gofile.me/3REyI/F6j14ZBRW)| 提取码: wi6j [链接](https://pan.baidu.com/s/1_Kfho-gC4cjtUT9kFJ-SFg) | Crazy
magistrale-23-day2 | 27.89 | [ROS bag](http://gofile.me/3REyI/aCGULn8GO)| 提取码: dbx3 [链接](https://pan.baidu.com/s/1KtL1arsCSwAcguUopvRQeg)| Crazy
magistrale-23-night1 | 24.71 |[ROS bag](http://gofile.me/3REyI/IQfOq10R6)| 提取码: hgf5 [链接](https://pan.baidu.com/s/1iEKKmHAbIfJqyQq9OSdHiA)| Crazy
magistrale-23-night2 | 27.91 | [ROS bag](http://gofile.me/3REyI/n5C1mv0FA)| 提取码: r16u [链接](https://pan.baidu.com/s/1glYupnZT-gZfyhqBo1HcHg)| Crazy
magistrale-24-night1 | 33.45 | [ROS bag](http://gofile.me/3REyI/Zb4Tz3zcH)| 提取码: 4v3f [链接](https://pan.baidu.com/s/1t_hAaeN7ynaN_SLkG_SnUA)| Crazy
magistrale-24-night2 | 35.09 | [ROS bag](http://gofile.me/3REyI/WNtF5g3Mx)| 提取码: uq7k [链接](https://pan.baidu.com/s/1yAJ1iP5GXIZVHjI-9xEWRQ)| Crazy
magistrale-24-night3 | 35.54 | [ROS bag](http://gofile.me/3REyI/1tm1Zc3XC)| 提取码: p9wk [链接](https://pan.baidu.com/s/1jM114cUS9x80zXUKwvqLmQ)| Crazy
magistrale-lift-23-night | 15.64 | [ROS bag](http://gofile.me/3REyI/kdswzdGMn)| 提取码: 5muf [链接](https://pan.baidu.com/s/1Ppc2k1U8Vl7PEDHUr67LEw)| Crazy
magistrale-lift-24-night | 23.35 | [ROS bag](http://gofile.me/3REyI/AvNHt2cXz)| 提取码: ksqz [链接](https://pan.baidu.com/s/1HRhO7cjcEev0iftiqaG8QA)| Crazy
magistrale-lift-234-night | 29.42 | [ROS bag](http://gofile.me/3REyI/X7KQhAb70)| 提取码: uxut [链接](https://pan.baidu.com/s/1IJGrIv6n8j6IpqopN8LIbw)| Crazy
outdoor-night1 | 60.05 | [ROS bag](http://gofile.me/3REyI/6YBPy9fnN)| 提取码: jyej [链接](https://pan.baidu.com/s/1Bu3-H87_Bd97Dcazb4todw)| Crazy
outdoor-night2 | 61.25 | [ROS bag](http://gofile.me/3REyI/LDHS4vGRf)| 提取码: s12u [链接](https://pan.baidu.com/s/1PXDGJlVvwfKlpUIO5sDWEQ)| Crazy
