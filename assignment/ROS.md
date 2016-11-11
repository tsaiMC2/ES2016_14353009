## ROS

<u>**定义**</u> Robot operation system，是一套框架，为软件开发者提供代码库和工具来进行机器人应用的开发，它供有硬件驱动、仿真器、消息传递功能、包管理功能等等。

##### **<u>ROS的安装</u>**

1. 需要linux环境，网上有具体教程，这里使用Ubuntu。

   首先要知道自己Ubuntu的版本号，在命令行键入：

```sh
cat /etc/issue
```

Ubuntu 14.04，15.04 请参考：http://wiki.ros.org/jade/Installation/Ubuntu
Ubuntu 15.10，16.04 请参考：http://wiki.ros.org/kinetic/Installation/Ubuntu

2. 配置Ubuntu repositories，详见https://help.ubuntu.com/community/Repositories/Ubuntu
3. 建立sources.list

```sh
sudo sh -c 'echo "deb http://packages.ros.org/ros/ubuntu $(lsb_release -sc) main" > /etc/apt/sources.list.d/ros-latest.list'
```

2. 建立钥匙

```sh
sudo apt-key adv --keyserver hkp://ha.pool.sks-keyservers.net:80 --recv-key 0xB01FA116
```

3. 安装ROS kinetic

   重新update一下确认Debian包索引是最新的：

```sh
sudo apt-get update
```

​	安装desktop-full版本的ROS kinetic：

```sh
sudo apt-get install ros-kinetic-desktop-full
```

4. 初始化rosdep


```sh
sudo rosdep init
rosdep update
```

5. 搭建环境

```sh
echo "source /opt/ros/kinetic/setup.bash" >> ~/.bashrc
source ~/.bashrc
```

6. 得到rosinstall

```sh
sudo apt-get install python-rosinstall
```







