# XV-11 and Botvac LIDAR Scanner driver for ROS

This is a clone of the standrd one.   New features are planned
* Documwentation and a how-to
* Actions to allow the scanner to be powered up and down
* Control over the speed

## Download and build
`
cd catkin_ws/src
git clone https://github.com/chrisalbertson/xv_11_laser_driver.git
cd ..
catkin_make
source devel/setup.bash
`

## Run
Note that you miust specify the firmware version.
Almost every LIDAR you will find today ues verion 2 firmware.
Only the very old ones use verion 1.

`
rosrun xv_11_laser_driver neato_laser_publisher _port:=/dev/ttyACM0 _firmware_version:=2
`

Use rviz to look at the data.



