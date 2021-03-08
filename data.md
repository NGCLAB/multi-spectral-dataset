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

### The environment under bright illumination

Sequence Name | Duration(s) | Size(GB)  |Avg. Trans. Vel. [m/s]| Avg. Rot. Vel. [deg/s]| link(Baidu Pan）| link(Google Drive)|Difficulty
------------ | ----------- | ------|------- | ------|----|--- | ------
desk1-halfsphere | 68.34 | 5.18 | 0.1266 |13.2977| 提取码: ztbz [链接](https://pan.baidu.com/s/1RdSZAqfG2uEXCcZoOGvzyA) | [Download](https://drive.google.com/file/d/1aH2vDYbGu6PE29JIgwCtiP9hgCaiBr2R/view?usp=sharing) | Easy
desk1-rpy | 61.40 | 7.32 |0.0524|15.6739| 提取码: myuc [链接](https://pan.baidu.com/s/1J13QTOwiKfvgmsQyAvBcTw) |[Download](https://drive.google.com/file/d/1A9IhQ39s-XmLRXWBVDRICvWKT0kgoNLF/view?usp=sharing) | Easy
desk1-static | 25.28 | 3.03 |0.0014|1.2815| 提取码: rm96 [链接](https://pan.baidu.com/s/1csVeoQXXPHALIgJ0Yw8x_g) |[Download](https://drive.google.com/file/d/1Vq368GUY7uEuX9YtvWhTFfBNg7GjXvFk/view?usp=sharing)| Easy
desk1-xyz | 48.55 | 5.93 |0.1662|12.5325| 提取码: mpuk [链接](https://pan.baidu.com/s/18FbnK_qWJVDudngCgWqhaw) |[Download](https://drive.google.com/file/d/1ipQ3Kii7bPG4PKWl2mNoth8__ahMtLWF/view?usp=sharing)| Easy
desk2-circle | 34.53 | 3.81 |0.1261|9.7276| 提取码: 2dq5 [链接](https://pan.baidu.com/s/1RWvY7-4HP5rdzP7irQoAyQ) |[Download](https://drive.google.com/file/d/196DvgrwPIduHjdQjU6xzEvVmFWtiIH2o/view?usp=sharing)| Easy
desk2-halfsphere | 44.32 | 5.18 | 0.0965|8.6699| 提取码: 5c9m [链接](https://pan.baidu.com/s/1D5hs8Z8tVs9IEXLXwPIrqA) |[Download](https://drive.google.com/file/d/1GdHNtEllZvAKWlny3pm-lgrPfVpbC114/view?usp=sharing)| Easy
desk2-rpy | 47.70 | 5.52 | 0.0450|13.3737|提取码: 936f [链接](https://pan.baidu.com/s/1ywyE9gRqBydQf1xslJfFng) |[Download](https://drive.google.com/file/d/1TPiR3Wr1UDpZqjSSDc1vfIp31L3mfGFo/view?usp=sharing)| Easy
desk2-static | 33.37 | 3.99|0.0113|2.6567| 提取码: uyu2 [链接](https://pan.baidu.com/s/1e3mQdkdLQ6maMt2wIMsLAQ) |[Download](https://drive.google.com/file/d/14WDS_vbnuHAz_eLsptJD6vNijNWvq4yu/view?usp=sharing)| Easy
desk2-xyz | 44.96 | 3.99|0.1492|8.2026| 提取码: 9jt8 [链接](https://pan.baidu.com/s/1l4WQ3Pp1IXQLyntHzS85ug) | [Download](https://drive.google.com/file/d/16HsuZOQFtvMKSVJ_6gBxFYAc9UpIrc_W/view?usp=sharing)|  Easy
desk1-circle-person | 33.81 | 4.07 |0.2060 |13.3581|提取码: bhgk [链接](https://pan.baidu.com/s/1kwfJoD_rowuJJwrXA-3NcQ) |[Download](https://drive.google.com/file/d/1hCEpbQAWVuV53hkBTVcOpwMs4Z7jJ1cv/view?usp=sharing)| Easy
desk1-halfsphere-person | 76.97  | 9.37| 0.1097|10.7502|提取码: i827 [链接](https://pan.baidu.com/s/1O8nVUQcXMTX6BdJFYoiPqQ) |[Download](https://drive.google.com/file/d/1Qhq71gRrjL35m44VV4TuProC74jXsNZA/view?usp=sharing)| Easy
desk1-rpy-person | 60.09 | 7.10 |0.0484 |15.7353|提取码: d2di [链接](https://pan.baidu.com/s/1_0SNWvMWEoFOmIhs59Tasg) |[Download](https://drive.google.com/file/d/1U8KUmtbBDg0OzLLiHKgYdw5--JBnof1M/view?usp=sharing)| Easy
desk1-rpy-person-slow | 59.53 | 6.93 | 0.0448|18.3272|提取码: queg [链接](https://pan.baidu.com/s/1lPgHpVdropFhxzd0hiMucQ) |[Download](https://drive.google.com/file/d/1LdJh3sR-Fqt3Jm2fqGJz59Gl99Mt0RAl/view?usp=sharing)| Easy
desk1-static-person | 19.97 | 2.14 |0.0020 |1.4005|提取码: j94s [链接](https://pan.baidu.com/s/18q0ukNwTTDojDzkk5N-TaQ) |[Download](https://drive.google.com/file/d/1NijBupzl1FfF_qRj9o4vymvsPbuJ132N/view?usp=sharing)| Easy
desk1-xyz-person| 51.16 | 6.23 |0.1422 |11.9822|提取码: 69ue [链接](https://pan.baidu.com/s/10mHosWzfCEqnSTd2tTmNRg) |[Download](https://drive.google.com/file/d/19Ws9ndbD1qsYdjb1BMBiJU8pquPmOixM/view?usp=sharing)| Easy
desk1-halfsphere-dy | 64.07 |7.28 |0.1425 |13.0772|提取码: kfjj [链接](https://pan.baidu.com/s/1hQrc5oPevW3aALahjFQ4YQ) |[Download](https://drive.google.com/file/d/1cfPCM5aJjrQ7vV8XYbdNWU337ZPEAonL/view?usp=sharing)| Easy
desk1-rpy-dy | 48.45 | 5.48 | 0.0546|14.5771|提取码: gced [链接](https://pan.baidu.com/s/1ooc0NKylGw-n94OhIXGZPQ) |[Download](https://drive.google.com/file/d/1jm9yt2gu9QurpZLJLDjRPqRBFzbWBFSE/view?usp=sharing)| Easy
desk1-static-dy | 24.92 | 2.81 )| 0.0013|0.4209|提取码: s4ye [链接](https://pan.baidu.com/s/136gRHzqtChQOCZNyvlcrbQ) |[Download](https://drive.google.com/file/d/13m36bZX5yvQQGsRIJQhy5QxsMiK9Yge5/view?usp=sharing)| Easy
desk1-xyz-dy | 48.76 | 5.38 | 0.1542| 7.5778 |提取码: 3axs [链接](https://pan.baidu.com/s/1SaskfehN43sPdsiYGfOYhg) |[Download](https://drive.google.com/file/d/1_78AvVnbt8cBR9ru2EnpchJ5_nminDX5/view?usp=sharing)| Easy

### The environment under varing illumination

Sequence Name | Duration(s)| Size(GB)|Avg. Trans. Vel. [m/s]| Avg. Rot. Vel. [deg/s] | link(Baidu Pan) | link(Google Drive) | Difficulty
-----|----|--- | --------|----- | -----|------|----- 
desk1-rpy-ic | 62.84 | 7.20 | 0.0485 |15.5414|提取码: vat8 [链接](https://pan.baidu.com/s/1kd-pplif5so9ToHlF-9oEg) | [Download](https://drive.google.com/file/d/1vRHSmeG_1Ig3jbX2-po2Qgz5lj1QcI7I/view?usp=sharing) |Hard
desk1-halfsphere-ic | 73.58 | 8.48 |0.1125|12.2998| 提取码: 8vti [链接](https://pan.baidu.com/s/1LoJLm3905GdjMqQwKHxdFQ) |[Download](https://drive.google.com/file/d/1ib14-3QLFW9J62ItX-AYptdNa_uymJXX/view?usp=sharing)| Hard
desk1-static-ic | 27.67 | 3.05 | 0.0015|0.4493| 提取码: tf7k [链接](https://pan.baidu.com/s/1jR5z3_J2BTzqPsvQb8X2og) |[Download](https://drive.google.com/file/d/1R3aVmjRTZaI4n4IxNC4gBoI8NQKdqnmz/view?usp=sharing)| Hard
desk1-static-ic-lampon | 24.74 | 2.77| 0.0009|0.4519|提取码: 9k6t [链接](https://pan.baidu.com/s/1xak1SPhGB5gCqunLGFSAaA) |[Download](https://drive.google.com/file/d/1rd5ogP-VB6eSbutMTBw1dj298dEQufv1/view?usp=sharing)| Hard
desk1-xyz-ic | 67.29 | 7.81 |0.1243|9.6570| 提取码: gac5 [链接](https://pan.baidu.com/s/1Ts8B-GPLcbhYQag9VqSrKA) |[Download](https://drive.google.com/file/d/13vTap7lxmBhFatgJDXHg6FIwriZLl1xA/view?usp=sharing)| Hard
desk2-circle-ic | 30.13 | 3.36| 0.1246|7.5655| 提取码: ccgx [链接](https://pan.baidu.com/s/1h6RVlDp3ueezHyBEHyiUsQ) |[Download](https://drive.google.com/file/d/1RP2jWpYkDyQIAvrYIxCCZSx7ektFW2UE/view?usp=sharing)| Hard
desk2-rpy-ic | 64.88 | 7.30 |0.0475|10.9869| 提取码: htej [链接](https://pan.baidu.com/s/15eUnxlpf1_tNU_sSM5MOLA) |[Download](https://drive.google.com/file/d/1J4jNKGDhgLDmhILF6ii98rNSQc6jH1z0/view?usp=sharing)| Hard
desk2-static-ic | 23.95 | 2.74 |0.0348|5.4931| 提取码: iw59 [链接](https://pan.baidu.com/s/1OmYeRWJq7iUkgHjDLgvDEg) |[Download](https://drive.google.com/file/d/1CLML9S4vxAEROJhdvlx55QlDa-9z0uFn/view?usp=sharing)| Hard
desk2-xyz-ic | 52.17 | 5.77 | 0.1150|11.8753|提取码: pc4k [链接](https://pan.baidu.com/s/1ozXPCkpOT3blZQe2B2ht4g) |[Download](https://drive.google.com/file/d/1RCJ8KBlw-u24ONFVei-I4ogrBT9VlkOe/view?usp=sharing)| Hard
desk2-halfsphere-ic | 73.58 | 8.48 | 0.1005|8.0885| 提取码: tw2d [链接](https://pan.baidu.com/s/1dfHAStGtoP5Tse0llatlPw) |[Download](https://drive.google.com/file/d/1maKx12QkCYA8jdTZmNfHKIH7_5e2c7hN/view?usp=sharing)| Hard
desk1-halfsphere-ic-person | 66.99 | 7.45 |0.1158|13.6747| 提取码: fcbb [链接](https://pan.baidu.com/s/1KMxfbkU-JGIYOwLZUlyTLQ) |[Download](https://drive.google.com/file/d/1qDNFKYoXgIPRJowA0kT2OVlPW2Ry7Oy5/view?usp=sharing)| Hard
desk1-rpy-ic-person | 56.23 | 6.32 |0.0464|16.4843| 提取码: h48m [链接](https://pan.baidu.com/s/1jm6tTwGb_GmPBy_wEIP7OA) |[Download](https://drive.google.com/file/d/11k9wcR0c_2xZFOZK2H3u2BlzX16sS-_S/view?usp=sharing)| Hard
desk1-static-ic-person| 33.87 | 3.74 |0.0082|2.6343| 提取码: 9vhm [链接](https://pan.baidu.com/s/1biCeEAFBaNpP0ypHxCltfA) |[Download](https://drive.google.com/file/d/1qheWW55YnPxqOw0418Uw3p9Mb6WK9L6_/view?usp=sharing)| Hard
desk1-xyz-ic-person| 54.19 | 6.19 |0.1550|11.9565| 提取码: xp9u [链接](https://pan.baidu.com/s/1gJ4Z5WlSBIvlmmuY2vCDEA) |[Download](https://drive.google.com/file/d/159EqCR_VzFewjQlBEHLOJ52Q-f9nulCW/view?usp=sharing)| Hard

### The environment under dim illumination

Sequence Name | Duration(s) | Size(GB)|Avg. Trans. Vel. [m/s]| Avg. Rot. Vel. [deg/s] | link(Baidu Pan)| link(Google Drive)| Difficulty
-----|----|--- | -------|----|---|----|-------
desk1-halfsphere-dim| 69.23 | 7.12 | 0.1348|12.6894|提取码: tcmr [链接](https://pan.baidu.com/s/1DQ3RptLC59NvD3giDZ-sxw) |[Download](https://drive.google.com/file/d/1uv-8UkJGATEkL8Ustph2MxxI0Rqoj-sz/view?usp=sharing)| Medium
desk1-halfsphere-dim2| 67.89 | 6.98 | 0.1346|11.7965|提取码: h36m [链接](https://pan.baidu.com/s/1wrQAeZqRpYavUO6tz2EsrA)|[Download](https://drive.google.com/file/d/1wLY3845qg5xcnrdTpFPFifjzWGtR0d-2/view?usp=sharing)| Medium
desk1-rpy-dim| 48.01 | 4.92 |0.0490|14.6452| 提取码: cqs3 [链接](https://pan.baidu.com/s/1L7zi7nxjhPsLGeYEgsmw-w)|[Download](https://drive.google.com/file/d/1k0wZ1gHWO_O2BhpzzP8dp_mWgro5yuEH/view?usp=sharing)| Medium
desk1-rpy-dim2| 52.57 | 5.39 |0.0501|13.9791| 提取码: 4sch [链接](https://pan.baidu.com/s/1XMbKmjMHH7ZaH90OOzeL0A)|[Download](https://drive.google.com/file/d/1rH7Hw3fIHhHL3kDJhCjIrEspDtoWEl5Z/view?usp=sharing)| Medium
desk1-static-dim| 21.53 | 2.18 |0.0009|0.2913| 提取码: vsgf [链接](https://pan.baidu.com/s/1b92QhEeKpOVx9mdN6dwfRQ)|[Download](https://drive.google.com/file/d/17xafOR7lbK44TUr7ECvxO4YjnQ_PLMNo/view?usp=sharing)| Medium
desk1-static-dim2| 19.42 | 1.97 |0.0028|1.4049| 提取码: yp49 [链接](https://pan.baidu.com/s/1uzMaNTRXVu-Q5dupXswXUg)|[Download](https://drive.google.com/file/d/1sgFwOZPhbir59c4rSSMUDGfW9S2jziTK/view?usp=sharing)| Medium
desk1-xyz-dim| 53.69 | 5.51 |0.1463|7.5768| 提取码: uqir [链接](https://pan.baidu.com/s/15PB0MPjzNGRSIl1qMo4itA)| [Download](https://drive.google.com/file/d/1cx5_u_dqpk1fCibsNM-vTBRO27OqE7aM/view?usp=sharing)|Medium
desk1-xyz-dim2| 53.81 | 5.52|0.1564|7.5196| 提取码: djkd [链接](https://pan.baidu.com/s/1-EuP3azpj6k_1XxjI980CA)|[Download](https://drive.google.com/file/d/1eeG_c99jSVnkr9DVG-5CjuASH4eJupn1/view?usp=sharing)| Medium

### The complex environment

Sequence Name  | Size(GB) | link（Baidu Pan）| link(Google Drive)| Difficulty
------------ | --------|-----|------|-------
magistrale-23-day1 | 28.70 |  提取码: wi6j [链接](https://pan.baidu.com/s/1_Kfho-gC4cjtUT9kFJ-SFg) | [Download](https://drive.google.com/file/d/1jJlgB2VaXcnFrQml9HsARoq_GkQN7nWQ/view?usp=sharing) | Crazy
magistrale-23-day2 | 27.89 |  提取码: dbx3 [链接](https://pan.baidu.com/s/1KtL1arsCSwAcguUopvRQeg)|[Download](https://drive.google.com/file/d/1KQ9Zja4cv2nFc_pBDJHYg98IspO-XWt_/view?usp=sharing) | Crazy
magistrale-23-night1 | 24.71 | 提取码: hgf5 [链接](https://pan.baidu.com/s/1iEKKmHAbIfJqyQq9OSdHiA)|[Download](https://drive.google.com/file/d/1KotrbDvvpm4GjQ0FnixQIRI9sUHXaQPN/view?usp=sharing)| Crazy
magistrale-23-night2 | 27.91 | 提取码: r16u [链接](https://pan.baidu.com/s/1glYupnZT-gZfyhqBo1HcHg)|[Download](https://drive.google.com/file/d/15C-G-FEg1o80h6cnQvcmXqKnTwmC9cna/view?usp=sharing)| Crazy
magistrale-24-night1 | 33.45 | 提取码: 4v3f [链接](https://pan.baidu.com/s/1t_hAaeN7ynaN_SLkG_SnUA)|[Download](https://drive.google.com/file/d/1ez2kYOnV1qYvGsVGhzXS33JW6nMz7cAs/view?usp=sharing)| Crazy
magistrale-24-night2 | 35.09 | 提取码: uq7k [链接](https://pan.baidu.com/s/1yAJ1iP5GXIZVHjI-9xEWRQ)| [Download](https://drive.google.com/file/d/1Dz_NMXXLPTIZ_LyFXGnoTfHh-4gKgX0V/view?usp=sharing) | Crazy
magistrale-24-night3 | 35.54 | 提取码: p9wk [链接](https://pan.baidu.com/s/1jM114cUS9x80zXUKwvqLmQ)| [Download](https://drive.google.com/file/d/19ARAzWoGS4L9I7gfIXdxAR_3u19ZBHZl/view?usp=sharing) | Crazy
magistrale-lift-23-night | 15.64 | 提取码: 5muf [链接](https://pan.baidu.com/s/1Ppc2k1U8Vl7PEDHUr67LEw)| [Download](https://drive.google.com/file/d/15mmPZusdIt_v0lmma7FC8fvXNqNW1L1n/view?usp=sharing) |Crazy
magistrale-lift-24-night | 23.35 | 提取码: ksqz [链接](https://pan.baidu.com/s/1HRhO7cjcEev0iftiqaG8QA)| [Download](https://drive.google.com/file/d/1Hlgmjzs5ZGbXgdX5vzLRJuLoES0uqd0A/view?usp=sharing) | Crazy
magistrale-lift-234-night | 29.42 | 提取码: uxut [链接](https://pan.baidu.com/s/1IJGrIv6n8j6IpqopN8LIbw)| [Download](https://drive.google.com/file/d/1B_hUS_n5mOKdcsHHI1fTDQvn5b6Mt5fv/view?usp=sharing) | Crazy
outdoor-night1 | 60.05 |  提取码: jyej [链接](https://pan.baidu.com/s/1Bu3-H87_Bd97Dcazb4todw)| [Download](https://drive.google.com/file/d/1OgqQoBivzs_YPMirGehbb0-bZGVF0jmK/view?usp=sharing) | Crazy
outdoor-night2 | 61.25 |  提取码: s12u [链接](https://pan.baidu.com/s/1PXDGJlVvwfKlpUIO5sDWEQ)| [Download](https://drive.google.com/file/d/1hKGghVjd0irlkPbfI1K3mfsP9hrwP5nG/view?usp=sharing) | Crazy
