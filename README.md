# raceLocalization
# Install CSM:
https://github.com/AndreaCensi/csm
place in catkin_ws/src/

# Phidgets Drivers
Install Phidgets spatial driver:\
git clone -b melodic https://github.com/ros-drivers/phidgets_drivers.git in the workspace \
catkin build \
\
Install dependencies:\
sudo apt-get install libusb-1.0-0 libusb-1.0-0-dev ros-melodic-imu-transformer ros-melodic-imu-filter-madgwick
\
Connect the IMU and launch using:\
roslaunch phidgets_imu imu.launch\
\
By default connects to the only Phidget device connected.\
You must add serial number to the launch file when multiple devices are connected.\
Make sure the usb device is accessible. Might have to use sudo.
