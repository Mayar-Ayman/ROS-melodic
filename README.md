
#task2 : installing of ROS on jetson nano steps

All of the commands were taken from this link :
https://github.com/AnbuKumar-maker/ROS-Installation-on-Jetson-Nano/tree/m

Now the steps and commands go as follows :

Install the package
sudo sh -c 'echo "deb http://packages.ros.org/ros/ubuntu $(lsb_release -sc) main" > /etc/apt/sources.list.d/ros-latest.list

Put the package key
sudo apt-key adv --keyserver 'hkp://keyserver.ubuntu.com:80' --recv-key C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654

Update the package
sudo apt update

Install Melodic ROS
sudo apt install ros-melodic-desktop

ROS initiation
sudo rosdep init

Update your ROS
rosdep update

Get the source of the ROS Melodic
echo "source /opt/ros/melodic/setup.bash" >> ~/.bashr

Confirm the source
source ~/.bashrc

Make sure of the type by using this command rosversion -d
