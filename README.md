# Code Structure of LIO-Livox (A Robust LiDAR-Inertial Odometry for Livox LiDAR)
This readme file is a code explaination of code structure of LIO-Livox **Developer**: [Livox](www.livoxtech.com). 

This algorithm implements a robust SLAM algorithm on Livox LiDARs with built-in IMU.

The overall algothm composes  4 files and 7 folders. 4 files are a CMakeLists.txt, a license, a readme.md and a package.xml, and 7 folds are cmake, config, doc, include, launch, rviz_cfg, and src. 

## 4 Files

CMakeLists claims minimum required cmake version, standard of cmake compiler, required packages, required dictionaries, required ROS packages, executable files' name, linking realationships and libraries. 

Lisense is like the BSD 3-Clause Lisence with preserved rights.

readme.md introduces the algo and provides tutorials to repeat it.

Package.xml file defines the  packages' features, mainly name here.

## 7 folders
### cmake
Two files exits here, FindEigen3.cmake and FindSuiteSparse, mainly for compilation.
FindEigen3.cmake provides eigen version, the eigen include directory and its version.

### src
There are two parts in src. The first is segment segmentation. segment.cpp completes the function of removing dynamic objects from the radar point cloud. pointsCorrect completes the function of making the distribution of feature points larger and more uniform.







