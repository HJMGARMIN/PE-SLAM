# PE-SLAM: An Online Visual-Inertial SLAM with Efficient IMU Initialization
# 1. Prerequisties
We have tested the library in Ubuntu 18.04 and Ubuntu 20.04, but it should be easy to compile in other Linux systems.

## C++14 Compiler
The PCL should be compiled by C++14.

## Pangolin
It is same as [ORB-SLAM3](https://github.com/UZ-SLAMLab/ORB_SLAM3).

##OpenCV
We use [OpenCV](http://opencv.org) to manipulate images and features. Dowload and install instructions can be found at: http://opencv.org. **Required at leat 3.0. Tested with OpenCV 3.2.0(Ubuntu 18.04) and 4.2.0(Ubuntu 20.04)**.

## Eigen3
Required by g2o. Download and install instructions can be found at: http://eigen.tuxfamily.org. Required at least 3.1.0. Tested with Eigen 3.3.7.

## TBB
Intel Threading Building Blocks(TBB) is used to accelerate the Tracking thread. We use parallel computation for acceleration in parts such as feature point extraction.
```
git clone https://github.com/wjakob/tbb.git
mkdir build
cd build
cmake ..
make -j
sudo make install
```
