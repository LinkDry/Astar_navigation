本程序适用于ROS初学者，即第一次接触导航路径规划人群使用，所有相关代码均在nav_pkg/launch上。通过利用launch文件在Gazebo和Rviz上装载A*导航程序来达成效果。

1.安装好依赖包:move_base,rviz,map_server,amcl;（官方ROS库中均有）
             wpr_simulation（需要通过git下载）
2.将nav_pkg文件夹放入ros的工作空间（catkin_ws/src）下。
3.返回至catkin_ws使用catkin_make进行编译。
4.使用命令运行launch文件

具体步骤:
一、
#安装wpr_simulation软件包
cd catkin_ws/src/
git clone https://github.com/6-robot/wpr_simulation.git
cd wpr_simulation/scripts/
./install_for_noetic.sh 

二、
**请自行将下载好的nav_pkg解压到~/catkin_ws/src/下**

三、
#编译&&运行
cd ~/catkin_ws/
catkin_make
roslaunch nav_pkg nav.launch
