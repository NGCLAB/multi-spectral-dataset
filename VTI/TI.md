
# Thermal Inertial SLAM Experiment data

# Sensor Setup

## Platform

The experiment data is collected by hand-held equipment.

<div align="center">
<img src="images/equip.png" width="300" />
</div>

## Senor Parameters

All the sensors and track devices and their most important parameters are listed as below:

- **Lidar**  Velodyne VLP-16
- **RGB Camera** ImageSource DFK 22BUC03. Global shutter. 640x480. 32Hz
- **LWIR Camera** Optris PI 640. 640×480. 32Hz
- **IMU** Xsens MTi-G-710 GNSS/INS

The rostopics of our rosbag sequences are listed as follows:

- **RGB Camera**: `/camera/image_raw`
- **LWIR Camera**: `/optris/thermal_image`
- **IMU**: `/imu/data`
- **OptiTrack**: `/vrpn_client_node/threebody/pose`
- **Lidar**: `/velodyne_points`

# Sequences

## Lab (Indoor)

Lab sequences are captured in a office room.

<div align="center">
<img src="images/LabIndoor.png" width="600" />
</div>


| Location |   Sequence   | Illumination | Length(m) | Duration(s) |     GT    | Size(GB) | BaiduPan Link |
|:--------:|:------------:|:------------:|:---------:|:-----------:|:---------:|:--------:|:----:|
|    Lab   |     xyz1     |     dark     |   12.989  |     49.1    | OptiTrack |    2.2   |[Link](https://pan.baidu.com/s/1q3ilZBtaIemymFGFfgP2ow?pwd=9ggr)|
|    Lab   |     xyz2     |    varying   |   11.917  |     39.1    | OptiTrack |    1.7   |[Link](https://pan.baidu.com/s/1O7iYwOEDFx8A6uuH1eSYmw?pwd=vd2u)|
|    Lab   |     xyz3     |    varying   |   12.438  |     38.7    | OptiTrack |    1.4   |[Link](https://pan.baidu.com/s/1qlfM3WpFNs8D1NZxvh0MZQ?pwd=9q6x)|
|    Lab   |     xyz4*    |    bright    |   13.024  |      59     | OptiTrack |    2.6   |[Link](https://pan.baidu.com/s/1zpyko7cujjJRicNJcVgGuQ?pwd=rdml)|
|    Lab   |     xyz5*    |    varying   |   11.109  |     45.2    | OptiTrack |    2.1   |[Link](https://pan.baidu.com/s/1Pp5CiXVFyUsgGEsv0m1Dfg?pwd=c51q)|
|    Lab   |     xyz6*    |     dark     |   13.656  |     51.9    | OptiTrack |    2.3   |[Link](https://pan.baidu.com/s/1awCqxN2dvW-lWKHZxojtSw?pwd=d1hx)|
|    Lab   |  halfsphere1 |     dark     |   13.749  |      63     | OptiTrack |    2.8   |[Link](https://pan.baidu.com/s/1ZbIjp2EVt2IcpYrZ5voUhA?pwd=a3jm)|
|    Lab   |  halfsphere2 |    bright    |   14.013  |      62     | OptiTrack |    2.8   |[Link](https://pan.baidu.com/s/1lxeDvMHjt0bLQX_-9zl59A?pwd=4c8k)|
|    Lab   |  halfsphere3 |    bright    |   9.488   |     36.3    | OptiTrack |    1.4   |[Link](https://pan.baidu.com/s/1BQUp7uregFz1aRyIfSicWQ?pwd=rm1g)|
|    Lab   | halfsphere4* |    bright    |   10.011  |     47.8    | OptiTrack |    2.1   |[Link](https://pan.baidu.com/s/1w7NdqxbvOmP7nldkTy06LQ?pwd=7twk)|
|    Lab   | halfsphere5* |    varying   |   10.217  |     48.9    | OptiTrack |    2.1   |[Link](https://pan.baidu.com/s/1dNJOZOD3YoV9790jUp-gGw?pwd=4wbk)|
|    Lab   | halfsphere6* |     dark     |   14.597  |      63     | OptiTrack |    2.8   |[Link](https://pan.baidu.com/s/1MEZaDgmodqT6IssqmhFWsQ?pwd=efcn)|
|    Lab   |    circle1   |    bright    |   13.832  |      75     | OptiTrack |    3.3   |[Link](https://pan.baidu.com/s/1dAAeJW7_v-_ieCtDd_UVxA?pwd=93vf)|
|    Lab   |    circle2   |    bright    |   14.897  |     51.9    | OptiTrack |    2.1   |[Link](https://pan.baidu.com/s/1RLOWpCWqjsQsw6UkBKTi5w?pwd=1es6)|
|    Lab   |   circle4*   |    bright    |   14.036  |     49.1    | OptiTrack |    2.2   |[Link](https://pan.baidu.com/s/1ajKE604SoMrw63_NFZDQBA?pwd=pd36)|
|    Lab   |   circle5*   |    varying   |   23.841  |      62     | OptiTrack |    2.5   |[Link](https://pan.baidu.com/s/1tR-1iPEyiwGgV12qIRgXYw?pwd=wlsw)|
|    Lab   |   circle6*   |     dark     |   14.141  |     45.4    | OptiTrack |    2.0   |[Link](https://pan.baidu.com/s/1wxnbg07-u_ZUctFvjSlSRg?pwd=efja)|
|    Lab   |   circleN1   |    bright    |   35.856  |     118     | OptiTrack |    5.2   |[Link](https://pan.baidu.com/s/1gPBZbz2MkkEWIIsezjvJxw?pwd=o17d)|
|    Lab   |   circleN2   |     dark     |   46.173  |      86     | OptiTrack |    2.7   |[Link](https://pan.baidu.com/s/1CXJfnb2RDho3hOJPnQqsVw?pwd=89qi)|
|    Lab   |   circleN3   |    varying   |   23.841  |      62     | OptiTrack |    2.5   |[Link](https://pan.baidu.com/s/1TIFIx4g7jkdVX8V7wAE26Q?pwd=33m6)|

**Notice**: Sequences with `*` are illumination data in the paper.

## Parking-lot (Indoor)

parking lot sequences are captured in a underground parking lot.
The illumination condition is mainly dark and dim.

<div align="center">
<img src="images/ParkingIndoor.png" width="600" />
</div>

|   Location  | Sequence | Length(m) | Duration(s) |  GT  | Size(GB) | BaiduPan Link |
|:-----------:|:--------:|:---------:|:-----------:|:----:|:--------:|:----:|
| Parking_lot | parklot1 |  127.135  |     132     | LOAM |    6.8   |[Link](https://pan.baidu.com/s/1elVbzkUiTVmEFCii1gHUag?pwd=emay)|
| Parking_lot | parklot2 |  126.318  |     132     | LOAM |    6.6   |[Link](https://pan.baidu.com/s/1EGPa9Jw7B3ZnFvWZv3fFGw?pwd=7ppf)|
| Parking_lot | parklot3 |   94.286  |     108     | LOAM |    5.2   |[Link](https://pan.baidu.com/s/1iJZO7KosBFcnSTjzFKmQaA?pwd=c1gf)|
| Parking_lot | parklot4 |  181.708  |     170     | LOAM |    8.7   |[Link](https://pan.baidu.com/s/1zAics3rK0NKvvZdVczqNvw?pwd=dty1)|
| Parking_lot | parklot5 |  352.303  |     305     | LOAM |   15.5   |[Link](https://pan.baidu.com/s/1RXk6Ga0J09spn6qR9ANQQA?pwd=c9vn)|

## Residential Area (Outdoor)

Outdoor sequences are captured in residential area at NIGHT. The illumination condition is quite bad for visible camera.

<div align="center">
<img src="images/ResidentialOutdoor.png" width="600" />
</div>

|     Location     |   Sequence   | Length(m) | Duration(s) |  GT  | Size(GB) | BaiduPan Link |
|:----------------:|:------------:|:---------:|:-----------:|:----:|:--------:|:----:|
| Residential Area | residential1 |  363.338  |     292     | LOAM |   14.9   |[Link](https://pan.baidu.com/s/1WewAuDfkb69lgljc2tiqRQ?pwd=ojnk)|
| Residential Area | residential2 |  184.873  |     175     | LOAM |    8.9   |[Link](https://pan.baidu.com/s/16zSgyw1_I4oXDYF7z9_4CA?pwd=4vx7)|
| Residential Area | residential3 |  190.852  |     168     | LOAM |    8.6   |[Link](https://pan.baidu.com/s/1-0Rr9t0a2Fqg4u-MD8ju2A?pwd=mvvj)|

# Calibration

The calibration files are stored in `calibration` folder.
