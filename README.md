# SLAM-simulation
The fourth task of smart methods training

# First Step :
Install the tools needed to run the simulation using the following codes

$ sudo apt-get install ros-melodic-diff-drive-controller\
$ sudo apt-get install ros-melodic-amcl\
$ sudo apt-get install ros-melodic-gmapping\
$ sudo apt-get install ros-melodic-navigation

# Second Step:
Create a hipspace using the following codes

$ mkdir -p 2DAutoSlambot/src\
$ cd 2DAutoSlambot\
$ catkin_make\
$ cd src\
$ catkin_create pkg gslambot\
$ cd gslambot

![WhatsApp Image 2021-08-09 at 6 01 46 PM](https://user-images.githubusercontent.com/86194970/128728954-700d864d-32da-4aeb-aa1d-faa9c1a87302.jpeg)

# Third Step:
We make copies of the package using the code

git clone https://github.com/YuCodes/2DAutoSlambot/edit/master/README.md

# Fourth step:
To run the package, use the following codes

$ roslaunch gslambot gmaprobot.launch model:=path to the /urdf/gmapbot.xacro file\
$ roslaunch gslambot move_base.launch

![4](https://user-images.githubusercontent.com/86194970/128729142-1b6cfed8-a338-45a4-9470-4b07406a0e5b.png)
![4-1](https://user-images.githubusercontent.com/86194970/128729160-bba1845c-6676-49b7-a9e5-fc078a6d50cf.png)

# Fifth step:
And in the end we need to save the map using the code

$ rosrun map_server map_saver -f ~/map
