# Jetson-Nx-Setup


Jetson Nx OS kurulumu için uygulama : https://developer.nvidia.com/nvidia-sdk-manager
Kullanılan versiyon : jetpack4.5.1

Ros Melodic Kurulumu:

$ git clone https://github.com/jetsonhacks/installROSXavier.git
$ cd installROSXavier
$ ./installROS.sh -p ros-melodic-desktop
$ rosdep init
$ rosdep update
$ ./setupCatkinWorkspace.sh
$ echo "source ~/catkin_ws/devel/setup.bash" >> ~/.bashrc

Mavros Kurulumu: 

$ sudo apt-get install ros-melodic-mavros ros-melodic-mavros-extras
$ cd && wget https://raw.githubusercontent.com/mavlink/mavros/master/mavros/scripts/install_geographiclib_datasets.sh
$ sudo bash ./install_geographiclib_datasets.sh   


Realsense - ros kurulumu:

$ sudo apt-get install ros-$ROS_DISTRO-realsense2-camera
$ sudo apt-get install ros-$ROS_DISTRO-realsense2-description

