# IF-LIO
## IF-LIO: Intensity-Enhanced Front-End Matching for Robust LiDAR–Inertial Odometry under Geometric Degeneracy

### Introduction
IF-LIO is a degeneration-aware intensity-assisted LiDAR-SLAM framework that improves localization robustness in geometrically degenerate environments by selectively leveraging intensity information as complementary constraints.

![Overview](figs/overview.png)

### 1 Build
```bash
cd <your workspace>
mkdir src
cd src
git clone https://github.com/usersky-cmyk/IF-LIO.git
cd ..
catkin_make
```

### 2 Run
#### 2.1 Newer College Dataset
Download Newer College Dataset from https://ori-drs.github.io/newer-college-dataset/
```bash
source devel/setup.bash
roslaunch if_lio Newer_college.launch
```
#### 2.2 ENWIDE Dataset
Download ENWIDE Dataset from https://projects.asl.ethz.ch/datasets/enwide/
```bash
source devel/setup.bash
roslaunch if_lio ENWIDE.launch
```

### 3 Mapping Result
#### 3.1 Newer College Dataset 
##### quad-hard
![quard_hard](figs/quad_hard.png)

#### 3.2 ENWIDE Dataset 
##### runway_d
![runway_d](figs/runway_d.png)

#### 3.3 self-collected Dataset
##### playground


### 4 Acknowledgements
Thanks for the below great open-source project for providing references to this work.
- [FAST-LIO](https://github.com/hku-mars/FAST_LIO)
- [btsa](https://github.com/thisparticle/btsa)
- [RMS](https://github.com/ctu-mrs/RMS)
- [PV-LIO](https://github.com/HViktorTsoi/PV-LIO)

