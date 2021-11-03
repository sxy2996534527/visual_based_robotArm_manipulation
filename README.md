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

### 6dof graspnet
1. https://github.com/NVlabs/6dof-graspnet

### robotic-grasping
1. https://github.com/skumra/robotic-grasping

### contact_graspnet
1. https://github.com/NVlabs/contact_graspnet

## 3. hardware
### photoneo
#### open source:
1. https://github.com/kevinzakka/pyphoxi
2. https://github.com/TakakiNishio/photoneo_test
3. https://github.com/Matrox-Imaging/Photoneo_PhoXi-3D-Scanner_MXSP4
4. Photoneo相机-pcl点云处理: https://blog.csdn.net/baidu_40840693/article/details/103013762
5. hand-eye calibration: https://wiki.photoneo.com/index.php/Robot-Camera_Calibration_Tool, https://blog.csdn.net/yaked/article/details/77161160?utm_medium=distribute.pc_relevant.none-task-blog-2%7Edefault%7EBlogCommendFromMachineLearnPai2%7Edefault-17.control&depth_1-utm_source=distribute.pc_relevant.none-task-blog-2%7Edefault%7EBlogCommendFromMachineLearnPai2%7Edefault-17.control, https://blog.csdn.net/weixin_42156097/article/details/109753021, https://blog.csdn.net/weixin_42156097/article/details/110957847?ops_request_misc=%257B%2522request%255Fid%2522%253A%2522162545252516780269853907%2522%252C%2522scm%2522%253A%252220140713.130102334.pc%255Fblog.%2522%257D&request_id=162545252516780269853907&biz_id=0&utm_medium=distribute.pc_search_result.none-task-blog-2~blog~first_rank_v2~rank_v29-3-110957847.pc_v2_rank_blog_default&utm_term=pcl&spm=1018.2226.3001.4450

## 4. 点云标注
1. https://blog.csdn.net/Dujing2019/article/details/104068721

## unseen object segmentation in robotic environment
1. https://github.com/chrisdxie/uois#models
2. https://github.com/BerkeleyAutomation/sd-maskrcnn
3. Class Agnostic的物体检测/分割, https://blog.csdn.net/eight_Jessen/article/details/105547549

## 5. Suction-Based Grasping
### (1). https://github.com/andyzeng/arc-robot-vision: lua和torch环境配置的问题太多，暂时放弃
#### a. install torch with cuda10.0: https://github.com/nagadomi/waifu2x/issues/253#issuecomment-445448928
#### b. Unsupported HDF5 version: 1.10.0, https://github.com/deepmind/torch-hdf5/issues/76

### (2). suction grasp estimate： https://github.com/triwahyuu/suction_grasp_estimate, 未给出预训练模型
### (3). cv pipeline: https://github.com/jayef0/cv_pipeline
### (4). OpenCV_for_suction_grasps: https://github.com/shisha101/OpenCV_for_suction_grasps, 代码bug太多，未给出使用示例

## 6. planar grasp
### (1). grasp detector: https://github.com/lerrel/Grasp-Detector
#### a. 环境： python2 tensorflow1.0 测试效果良好

## 7. Grasping Dataset
1. [Cornell Grasping Dataset](http://pr.cs.cornell.edu/grasping/rect_data/data.php), [PaperWithCode](https://paperswithcode.com/sota/robotic-grasping-on-cornell-grasp-dataset-1)
2. [Jacquard Dataset](https://jacquard.liris.cnrs.fr/), [PaperWithCode](https://paperswithcode.com/sota/robotic-grasping-on-jacquard-dataset)
3. [grasp_multiobject](https://github.com/ivalab/grasp_multiObject), [PaperWithCode](https://paperswithcode.com/dataset/grasp-multiobject)
