# Touch_tmr

Need to setup a catkin workspace and build before use.

Install the udev rules for the Razer Hydra by running the configure script in the razer_hydra directory:

roscd razer_hydra
./configure_udev_rules



Source the setup file in devel folder before running, and when you try to display/echo the controller data in a new terminal.

For publishing the raw controller data, launch:
roslaunch razor_hydra hydra.launch

For publishing processed data, launch after publishing the raw controller data:
roslaunch touch_tmr hydra_sub_pub.launch
