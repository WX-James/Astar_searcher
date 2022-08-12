# A*搜索Demo

## 1. 编译

catkin_make

## 2. 运行程序

source devel/setup.bash

roslaunch grid_path_searcher demo.launch

## 3. 主要工程文件

（1）/grid_path_searcher/src/demo_node.cpp

node文件，接收topic（点云、目标点），规划路径，显示

（2）/grid_path_searcher/src/Astar_searcher.cpp

实现A星搜索算法

（3）/grid_path_searcher/src/random_complex_generator.cpp

随机生成三维栅格地图

（4）/waypoint_generator/src/waypoint_generator.cpp

接收RVIZ上发送的2D Nav Goal，生成emo_node.cpp所需的目标点并显示