# slam_lidar_by_myself
lidar slam developed by myself.

ubuntu 20.04  
set(CMAKE_CXX_STANDARD 17)  # C++ 17  
option(BUILD_WITH_UBUNTU1804 OFF)  
eigen>=3.3.4; best 3.3.7  #pkg-config --modversion eigen3; search the version of eigen  
sophus  
pcl>=1.9  
opencv=4.2.0  # pkg-config --modversion opencv4; search the version of opencv  

# run as follows:  
cd build  
cmake ..  
make  
./test_ndt  
