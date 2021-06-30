[NEMS_2017_grasping_poster.pdf](https://github.com/sxy2996534527/visual_based_robotArm_manipulation/files/6731198/NEMS_2017_grasping_poster.pdf)
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
1. https://blog.csdn.net/Eeko_x/article/details/104835154
2. ros launch demo: https://github.com/atenpas/gpd/blob/forward/launch/tutorial1.launch

### atenpas/gpg
#### configuration error
1. boost error, ‘boost::this_thread’ has not been declared: https://openclassrooms.com/forum/sujet/probleme-de-compilation-avec-boost-87075
`#include <boost/thread.hpp>`
2. boost error linking libarary, https://www.coder.work/article/3233619
#### Q & A
1. How to change the configuration so only the grasp from above are selected? -- https://githubmemory.com/repo/atenpas/gpd/issues/110

### dexnet
1. https://github.com/BerkeleyAutomation/dex-net
2. configuration version is out-of-date

### PointNetGPD
1. https://github.com/lianghongzhuo/PointNetGPD
2. dataset YCB: http://ycb-benchmarks.s3-website-us-east-1.amazonaws.com/

## 3. hardware
### photoneo
#### open source:
1. https://github.com/kevinzakka/pyphoxi
2. https://github.com/TakakiNishio/photoneo_test
3. https://github.com/Matrox-Imaging/Photoneo_PhoXi-3D-Scanner_MXSP4
4. Photoneo相机-pcl点云处理: https://blog.csdn.net/baidu_40840693/article/details/103013762 
