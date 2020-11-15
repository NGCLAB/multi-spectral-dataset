# Dataset sequences

## Naming

We provide several types of sequences for evaluating the multi-spectral nvigation systems. The naming is explained below. The key words have been bolded.

- Scene: 
    - **desk**: Sequences in the room with Motion Capture system, where ground truth poses are available for the entire trajectory.
    - **magistrale**: Sequences featuring a walk around in a university building. Ground truth poses are available for the start and end segments.
    - **outdoor**: Outdoor sequences. Ground truth poses are available for the start and end segments.
    - **lift**: Specially changeling sequences which contain the camera leads to different floors via elevator. Ground truth poses are available for the start and end segments.
- Illumination:
    - bright: Most **desk** sequences recorded in bright environments,
    - varing: **ic** data with lights turned on and off randomly. 
    - dim: **dim** data where the scene is dark.
    - complex: **magistrale** and **outdoor** sequences are recorded under complex illumination.
- Motion: 
    - **halfsphere** : the camera moves along the trajectory of a halfsphere with a diameter of 1m.
    - **xyz** : the camera moves approximately along the x, y, and z axes.
    - **rpy** : the camera only rotates with roll, pitch, and yaw motion.
    - **circle** : the camera moves approximately around a circle.
    - **static** : the camera is nearly motionless.
- Other:
    - **dy** : a person is walking around in front of the setup to add disturbances.
    - **person** : a person sitting in front of a desk to provide striking contrasts in textures in the thermal images.
    - **day** : the data is collected before sunset
    - **night** : the data is collected after sunset

## Topic

 The bag files contain the following message topics:

- **/camera/image_raw (sensor_msgs/Image)**: raw color images from the standard
camera
- **/optris/thermal_image (sensor_msgs/Image)**: raw thermal images from the LWIR
camera
- **/camera/flag_state (msdi_ros/Flag)**: flag states of the LWIR camera
- **/kinect2/qhd/image_color_rect (sensor_msgs/Image)**: Rectified color images from Kinect2
- **/kinect2/qhd/image_depth_rect (sensor_msgs/Image)**: Rectified depth images from Kinect2
- **/kinect2/sd/image_ir_rect (sensor_msgs/Image)**: Rectified near infrared (NIR) images from Kinect2
- **/imu/data (sensor_msgs/Imu)**: IMU data
- **/vrpn_client_node/RigidBody/pose (geometry_msgs/PoseStamped)**: raw poses from the motion capture system

### New ROS msg

**msdi_ros/Flag** is a msg defined in Bag_extractor package([Github Page](https://github.com/weichnn/bag_extractor)). It only has two parts:
```
Header header
uint32 flag_state
```

## Bag extractor

A example ([Github Page](https://github.com/weichnn/bag_extractor)) of how to extract multi-spectal data from bags and how to genarate dense depth images on the standard camera's viewpoint.

## Download link

We are trying our best to upload the data to Google drive.

### The environment under bright illumination

Sequence Name | Duration(s) | Size(GB)  | link(Baidu Pan）| link(Google Drive)|Difficulty
------------ | ----------- | ------------- | ------|------- | ------
desk1-halfsphere | 68.34 | 5.18  | 提取码: ztbz [链接](https://pan.baidu.com/s/1RdSZAqfG2uEXCcZoOGvzyA) | [Download](https://drive.google.com/file/d/1aH2vDYbGu6PE29JIgwCtiP9hgCaiBr2R/view?usp=sharing) | Easy
desk1-rpy | 61.40 | 7.32 | 提取码: myuc [链接](https://pan.baidu.com/s/1J13QTOwiKfvgmsQyAvBcTw) |[Download](https://drive.google.com/file/d/1A9IhQ39s-XmLRXWBVDRICvWKT0kgoNLF/view?usp=sharing) | Easy
desk1-static | 25.28 | 3.03 | 提取码: rm96 [链接](https://pan.baidu.com/s/1csVeoQXXPHALIgJ0Yw8x_g) |[Download](https://drive.google.com/file/d/1Vq368GUY7uEuX9YtvWhTFfBNg7GjXvFk/view?usp=sharing)| Easy
desk1-xyz | 48.55 | 5.93 | 提取码: mpuk [链接](https://pan.baidu.com/s/18FbnK_qWJVDudngCgWqhaw) |[Download](https://drive.google.com/file/d/1ipQ3Kii7bPG4PKWl2mNoth8__ahMtLWF/view?usp=sharing)| Easy
desk2-circle | 34.53 | 3.81 | 提取码: 2dq5 [链接](https://pan.baidu.com/s/1RWvY7-4HP5rdzP7irQoAyQ) |[Download](https://drive.google.com/file/d/196DvgrwPIduHjdQjU6xzEvVmFWtiIH2o/view?usp=sharing)| Easy
desk2-halfsphere | 44.32 | 5.18 | 提取码: 5c9m [链接](https://pan.baidu.com/s/1D5hs8Z8tVs9IEXLXwPIrqA) |[Download](https://drive.google.com/file/d/1GdHNtEllZvAKWlny3pm-lgrPfVpbC114/view?usp=sharing)| Easy
desk2-rpy | 47.70 | 5.52 | 提取码: 936f [链接](https://pan.baidu.com/s/1ywyE9gRqBydQf1xslJfFng) |[Download](https://drive.google.com/file/d/1TPiR3Wr1UDpZqjSSDc1vfIp31L3mfGFo/view?usp=sharing)| Easy
desk2-static | 33.37 | 3.99| 提取码: uyu2 [链接](https://pan.baidu.com/s/1e3mQdkdLQ6maMt2wIMsLAQ) |[Download](https://drive.google.com/file/d/14WDS_vbnuHAz_eLsptJD6vNijNWvq4yu/view?usp=sharing)| Easy
desk2-xyz | 44.96 | 3.99| 提取码: 9jt8 [链接](https://pan.baidu.com/s/1l4WQ3Pp1IXQLyntHzS85ug) | [Download](https://drive.google.com/file/d/16HsuZOQFtvMKSVJ_6gBxFYAc9UpIrc_W/view?usp=sharing)|  Easy
desk1-circle-person | 33.81 | 4.07 | 提取码: bhgk [链接](https://pan.baidu.com/s/1kwfJoD_rowuJJwrXA-3NcQ) |[Download](https://drive.google.com/file/d/1hCEpbQAWVuV53hkBTVcOpwMs4Z7jJ1cv/view?usp=sharing)| Easy
desk1-halfsphere-person | 76.97  | 9.37| 提取码: i827 [链接](https://pan.baidu.com/s/1O8nVUQcXMTX6BdJFYoiPqQ) |[Download](https://drive.google.com/file/d/1Qhq71gRrjL35m44VV4TuProC74jXsNZA/view?usp=sharing)| Easy
desk1-rpy-person | 60.09 | 7.10 | 提取码: d2di [链接](https://pan.baidu.com/s/1_0SNWvMWEoFOmIhs59Tasg) |[Download](https://drive.google.com/file/d/1U8KUmtbBDg0OzLLiHKgYdw5--JBnof1M/view?usp=sharing)| Easy
desk1-rpy-person-slow | 59.53 | 6.93 | 提取码: queg [链接](https://pan.baidu.com/s/1lPgHpVdropFhxzd0hiMucQ) |[Download](https://drive.google.com/file/d/1LdJh3sR-Fqt3Jm2fqGJz59Gl99Mt0RAl/view?usp=sharing)| Easy
desk1-static-person | 19.97 | 2.14 | 提取码: j94s [链接](https://pan.baidu.com/s/18q0ukNwTTDojDzkk5N-TaQ) |[Download](https://drive.google.com/file/d/1NijBupzl1FfF_qRj9o4vymvsPbuJ132N/view?usp=sharing)| Easy
desk1-xyz-person| 51.16 | 6.23 | 提取码: 69ue [链接](https://pan.baidu.com/s/10mHosWzfCEqnSTd2tTmNRg) |[Download](https://drive.google.com/file/d/19Ws9ndbD1qsYdjb1BMBiJU8pquPmOixM/view?usp=sharing)| Easy
desk1-halfsphere-dy | 64.07 |7.28 | 提取码: kfjj [链接](https://pan.baidu.com/s/1hQrc5oPevW3aALahjFQ4YQ) |[Download](https://drive.google.com/file/d/1cfPCM5aJjrQ7vV8XYbdNWU337ZPEAonL/view?usp=sharing)| Easy
desk1-rpy-dy | 48.45 | 5.48 | 提取码: gced [链接](https://pan.baidu.com/s/1ooc0NKylGw-n94OhIXGZPQ) |[Download](https://drive.google.com/file/d/1jm9yt2gu9QurpZLJLDjRPqRBFzbWBFSE/view?usp=sharing)| Easy
desk1-static-dy | 24.92 | 2.81 )| 提取码: s4ye [链接](https://pan.baidu.com/s/136gRHzqtChQOCZNyvlcrbQ) |[Download](https://drive.google.com/file/d/13m36bZX5yvQQGsRIJQhy5QxsMiK9Yge5/view?usp=sharing)| Easy
desk1-xyz-dy | 48.76 | 5.38 | 提取码: 3axs [链接](https://pan.baidu.com/s/1SaskfehN43sPdsiYGfOYhg) |[Download](https://drive.google.com/file/d/1_78AvVnbt8cBR9ru2EnpchJ5_nminDX5/view?usp=sharing)| Easy

### The environment under varing illumination

Sequence Name | Duration(s)| Size(GB) | link(Synology) | link(Baidu Pan) | link(Google Drive) | Difficulty
------------ | --------|----- | -----|------|----- | ------- |------
desk1-rpy-ic | 62.84 | 7.20 | [ROS bag](http://gofile.me/3REyI/oBOEOZFDI)| 提取码: vat8 [链接](https://pan.baidu.com/s/1kd-pplif5so9ToHlF-9oEg) | |Hard
desk1-halfsphere-ic | 73.58 | 8.48 | [ROS bag](http://gofile.me/3REyI/BMh1xxImI)| 提取码: 8vti [链接](https://pan.baidu.com/s/1LoJLm3905GdjMqQwKHxdFQ) |[Download](https://drive.google.com/file/d/1ib14-3QLFW9J62ItX-AYptdNa_uymJXX/view?usp=sharing)| Hard
desk1-static-ic | 27.67 | 3.05 | [ROS bag](http://gofile.me/3REyI/tboURe3jz)| 提取码: tf7k [链接](https://pan.baidu.com/s/1jR5z3_J2BTzqPsvQb8X2og) || Hard
desk1-static-ic-lampon | 24.74 | 2.77 | [ROS bag](http://gofile.me/3REyI/LsaAFtk1q)| 提取码: 9k6t [链接](https://pan.baidu.com/s/1xak1SPhGB5gCqunLGFSAaA) || Hard
desk1-xyz-ic | 67.29 | 7.81 | [ROS bag](http://gofile.me/3REyI/y1GluJbxQ)| 提取码: gac5 [链接](https://pan.baidu.com/s/1Ts8B-GPLcbhYQag9VqSrKA) || Hard
desk2-circle-ic | 30.13 | 3.36 | [ROS bag](http://gofile.me/3REyI/h3u2P26rw)| 提取码: ccgx [链接](https://pan.baidu.com/s/1h6RVlDp3ueezHyBEHyiUsQ) || Hard
desk2-rpy-ic | 64.88 | 7.30 | [ROS bag](http://gofile.me/3REyI/PO1N9thQT)| 提取码: htej [链接](https://pan.baidu.com/s/15eUnxlpf1_tNU_sSM5MOLA) || Hard
desk2-static-ic | 23.95 | 2.74 | [ROS bag](http://gofile.me/3REyI/SCG2KZ5Jg)| 提取码: iw59 [链接](https://pan.baidu.com/s/1OmYeRWJq7iUkgHjDLgvDEg) || Hard
desk2-xyz-ic | 52.17 | 5.77 | [ROS bag](http://gofile.me/3REyI/ZMKhDO3JJ)| 提取码: pc4k [链接](https://pan.baidu.com/s/1ozXPCkpOT3blZQe2B2ht4g) || Hard
desk2-halfsphere-ic | 73.58 | 8.48 | [ROS bag](http://gofile.me/3REyI/16N6mtW7Y)|  提取码: tw2d [链接](https://pan.baidu.com/s/1dfHAStGtoP5Tse0llatlPw) |[Download](https://drive.google.com/file/d/1maKx12QkCYA8jdTZmNfHKIH7_5e2c7hN/view?usp=sharing)| Hard
desk1-halfsphere-ic-person | 66.99 | 7.45 | [ROS bag](http://gofile.me/3REyI/xK6X42G1u)| 提取码: fcbb [链接](https://pan.baidu.com/s/1KMxfbkU-JGIYOwLZUlyTLQ) || Hard
desk1-rpy-ic-person | 56.23 | 6.32 | [ROS bag](http://gofile.me/3REyI/l3nxmDunn)| 提取码: h48m [链接](https://pan.baidu.com/s/1jm6tTwGb_GmPBy_wEIP7OA) || Hard
desk1-static-ic-person| 33.87 | 3.74 | [ROS bag](http://gofile.me/3REyI/6tbQq7jpB)| 提取码: 9vhm [链接](https://pan.baidu.com/s/1biCeEAFBaNpP0ypHxCltfA) || Hard
desk1-xyz-ic-person| 54.19 | 6.19 | [ROS bag](http://gofile.me/3REyI/6HZwfz5dy)| 提取码: xp9u [链接](https://pan.baidu.com/s/1gJ4Z5WlSBIvlmmuY2vCDEA) || Hard

### The environment under dim illumination

Sequence Name | Duration(s) | Size(GB) | link(Baidu Pan)| link(Google Drive)| Difficulty
------------ | -------|----|---|----|-------
desk1-halfsphere-dim| 69.23 | 7.12 | 提取码: tcmr [链接](https://pan.baidu.com/s/1DQ3RptLC59NvD3giDZ-sxw) |[Download](https://drive.google.com/file/d/1uv-8UkJGATEkL8Ustph2MxxI0Rqoj-sz/view?usp=sharing)| Medium
desk1-halfsphere-dim2| 67.89 | 6.98 | 提取码: h36m [链接](https://pan.baidu.com/s/1wrQAeZqRpYavUO6tz2EsrA)|[Download](https://drive.google.com/file/d/1wLY3845qg5xcnrdTpFPFifjzWGtR0d-2/view?usp=sharing)| Medium
desk1-rpy-dim| 48.01 | 4.92 | 提取码: cqs3 [链接](https://pan.baidu.com/s/1L7zi7nxjhPsLGeYEgsmw-w)|[Download](https://drive.google.com/file/d/1k0wZ1gHWO_O2BhpzzP8dp_mWgro5yuEH/view?usp=sharing)| Medium
desk1-rpy-dim2| 52.57 | 5.39 | 提取码: 4sch [链接](https://pan.baidu.com/s/1XMbKmjMHH7ZaH90OOzeL0A)|[Download](https://drive.google.com/file/d/1rH7Hw3fIHhHL3kDJhCjIrEspDtoWEl5Z/view?usp=sharing)| Medium
desk1-static-dim| 21.53 | 2.18 | 提取码: vsgf [链接](https://pan.baidu.com/s/1b92QhEeKpOVx9mdN6dwfRQ)|[Download](https://drive.google.com/file/d/17xafOR7lbK44TUr7ECvxO4YjnQ_PLMNo/view?usp=sharing)| Medium
desk1-static-dim2| 19.42 | 1.97 | 提取码: yp49 [链接](https://pan.baidu.com/s/1uzMaNTRXVu-Q5dupXswXUg)|[Download](https://drive.google.com/file/d/1sgFwOZPhbir59c4rSSMUDGfW9S2jziTK/view?usp=sharing)| Medium
desk1-xyz-dim| 53.69 | 5.51 | 提取码: uqir [链接](https://pan.baidu.com/s/15PB0MPjzNGRSIl1qMo4itA)| [Download](https://drive.google.com/file/d/1cx5_u_dqpk1fCibsNM-vTBRO27OqE7aM/view?usp=sharing)|Medium
desk1-xyz-dim2| 53.81 | 5.52 )| 提取码: djkd [链接](https://pan.baidu.com/s/1-EuP3azpj6k_1XxjI980CA)|[Download](https://drive.google.com/file/d/1eeG_c99jSVnkr9DVG-5CjuASH4eJupn1/view?usp=sharing)| Medium

### The complex environment

Sequence Name  | Size(GB)| link(Synology) | link（Baidu Pan）| link(Google Drive)| Difficulty
------------ | -------|------|-----|------|-------
magistrale-23-day1 | 28.70 | [ROS bag](http://gofile.me/3REyI/F6j14ZBRW)| 提取码: wi6j [链接](https://pan.baidu.com/s/1_Kfho-gC4cjtUT9kFJ-SFg) | [Download](https://drive.google.com/file/d/1jJlgB2VaXcnFrQml9HsARoq_GkQN7nWQ/view?usp=sharing) | Crazy
magistrale-23-day2 | 27.89 | [ROS bag](http://gofile.me/3REyI/aCGULn8GO)| 提取码: dbx3 [链接](https://pan.baidu.com/s/1KtL1arsCSwAcguUopvRQeg)|[Download](https://drive.google.com/file/d/1KQ9Zja4cv2nFc_pBDJHYg98IspO-XWt_/view?usp=sharing) | Crazy
magistrale-23-night1 | 24.71 |[ROS bag](http://gofile.me/3REyI/IQfOq10R6)| 提取码: hgf5 [链接](https://pan.baidu.com/s/1iEKKmHAbIfJqyQq9OSdHiA)|[Download](https://drive.google.com/file/d/1KotrbDvvpm4GjQ0FnixQIRI9sUHXaQPN/view?usp=sharing)| Crazy
magistrale-23-night2 | 27.91 | [ROS bag](http://gofile.me/3REyI/n5C1mv0FA)| 提取码: r16u [链接](https://pan.baidu.com/s/1glYupnZT-gZfyhqBo1HcHg)|[Download](https://drive.google.com/file/d/15C-G-FEg1o80h6cnQvcmXqKnTwmC9cna/view?usp=sharing)| Crazy
magistrale-24-night1 | 33.45 | [ROS bag](http://gofile.me/3REyI/Zb4Tz3zcH)| 提取码: 4v3f [链接](https://pan.baidu.com/s/1t_hAaeN7ynaN_SLkG_SnUA)|[Download](https://drive.google.com/file/d/1ez2kYOnV1qYvGsVGhzXS33JW6nMz7cAs/view?usp=sharing)| Crazy
magistrale-24-night2 | 35.09 | [ROS bag](http://gofile.me/3REyI/WNtF5g3Mx)| 提取码: uq7k [链接](https://pan.baidu.com/s/1yAJ1iP5GXIZVHjI-9xEWRQ)| | Crazy
magistrale-24-night3 | 35.54 | [ROS bag](http://gofile.me/3REyI/1tm1Zc3XC)| 提取码: p9wk [链接](https://pan.baidu.com/s/1jM114cUS9x80zXUKwvqLmQ)| | Crazy
magistrale-lift-23-night | 15.64 | [ROS bag](http://gofile.me/3REyI/kdswzdGMn)| 提取码: 5muf [链接](https://pan.baidu.com/s/1Ppc2k1U8Vl7PEDHUr67LEw)| |Crazy
magistrale-lift-24-night | 23.35 | [ROS bag](http://gofile.me/3REyI/AvNHt2cXz)| 提取码: ksqz [链接](https://pan.baidu.com/s/1HRhO7cjcEev0iftiqaG8QA)| [Download](https://drive.google.com/file/d/1Hlgmjzs5ZGbXgdX5vzLRJuLoES0uqd0A/view?usp=sharing) | Crazy
magistrale-lift-234-night | 29.42 | [ROS bag](http://gofile.me/3REyI/X7KQhAb70)| 提取码: uxut [链接](https://pan.baidu.com/s/1IJGrIv6n8j6IpqopN8LIbw)| [Download](https://drive.google.com/file/d/1B_hUS_n5mOKdcsHHI1fTDQvn5b6Mt5fv/view?usp=sharing) | Crazy
outdoor-night1 | 60.05 | [ROS bag](http://gofile.me/3REyI/6YBPy9fnN)| 提取码: jyej [链接](https://pan.baidu.com/s/1Bu3-H87_Bd97Dcazb4todw)|| Crazy
outdoor-night2 | 61.25 | [ROS bag](http://gofile.me/3REyI/LDHS4vGRf)| 提取码: s12u [链接](https://pan.baidu.com/s/1PXDGJlVvwfKlpUIO5sDWEQ)|| Crazy
