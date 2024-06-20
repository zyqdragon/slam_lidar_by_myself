# slam_lidar_by_myself
lidar slam developed by myself.

ubuntu 20.04  
cmake>=3.24.3  
https://blog.csdn.net/fyc300/article/details/135282561?spm=1001.2014.3001.5506  
dowanload cmake-3.24.3.tar.gz from: https://cmake.org/files/v3.24/  
cd cmake-3.24.2  
./bootstrap  
make  
sudo make install  

eigen:  
https://blog.csdn.net/qq_62964142/article/details/133346724?spm=1001.2014.3001.5506  
download eigen 3.4.0 from: https://gitlab.com/libeigen/eigen/-/releases  
mkdir build  
cd build  
cmake ..  
sudo make install  

Sophus  
https://blog.csdn.net/qq_62964142/article/details/133346724?spm=1001.2014.3001.5506  
安装fmt  
创建fmt文件夹，在终端打开，输入如下命令：  
git clone  https://github.com/fmtlib/fmt.git  
cd fmt  
mkdir build  
cd build  
cmake ..  
make  
sudo make install  
安装Sophus  
创建Sophus文件夹，在终端打开，输入如下命令： 
git clone https://github.com/strasdat/Sophus.git  
cd Sophus/  
mkdir build  
cd build  
cmake ..  
make  
sudo make install  
# https://blog.csdn.net/qq_62964142/article/details/133346724 

pcl:  
1. 先更新,然后直接安装  
sudo apt update  
sudo apt install libpcl-dev  
卸载：  
sudo apt remove libpcl-dev  
#仅限用上面方式安装的PCL卸载  
显示pcl版本  
apt-cache show libpcl-dev  


#######################################################################  
set(CMAKE_CXX_STANDARD 17)  # C++ 17  
option(BUILD_WITH_UBUNTU1804 OFF)  
eigen>=3.3.4; best 3.3.7  #pkg-config --modversion eigen3; search the version of eigen  
sophus  
pcl>=1.9  
opencv=4.2.0  # pkg-config --modversion opencv4; search the version of opencv  

run test_ndt as follows:  
cd build  
cmake ..  
make  
./test_ndt  
