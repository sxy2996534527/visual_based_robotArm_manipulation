# visual based slam & grasping

## 1. environment issues
### ros network error
https://blog.csdn.net/nanianwochengshui/article/details/105702188

### easyhandeye error
1. catkin build, The build space at '/home/xinyu/catkin_ws/build' was previously built by 'catkin_make'. Please remove the build space or pick a dfferent build space. --solved: https://github.com/ethz-asl/maplab/issues/9

### opencv c++ (with extra modules opencv-contrib install from source)
1. https://docs.opencv.org/4.5.2/d7/d9f/tutorial_linux_install.html
2. https://github.com/opencv/opencv_contrib
3. https://blog.csdn.net/weixin_44796670/article/details/115900538

## 2. reference projects
### atenpas/gpd
#### dataset
https://rll.berkeley.edu/bigbird/
#### how to use
https://blog.csdn.net/Eeko_x/article/details/104835154

### atenpas/gpg
#### configuration error
1. boost error, ‘boost::this_thread’ has not been declared: https://openclassrooms.com/forum/sujet/probleme-de-compilation-avec-boost-87075
`#include <boost/thread.hpp>`
2. boost error linking libarary, https://www.coder.work/article/3233619

### dexnet
1. https://github.com/BerkeleyAutomation/dex-net
2. configuration version is out-of-date

### PointNetGPD
1. https://github.com/lianghongzhuo/PointNetGPD
2. dataset YCB: http://ycb-benchmarks.s3-website-us-east-1.amazonaws.com/
