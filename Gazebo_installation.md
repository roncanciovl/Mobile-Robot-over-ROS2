# Gazebo Installation

# Ignition Gazebo

Ignition Gazebo is an open source robotics simulator from the Ignition Robotics Project. It is derived from the popular robotics simulator Gazebo, featuring more advanced rendering, physics and sensor models. Supported Vehicles: Quadrotor.

### Installation

https://gazebosim.org/api/gazebo/6.1/install.html


```
sudo sh -c 'echo "deb http://packages.osrfoundation.org/gazebo/ubuntu-stable `lsb_release -cs` main" > /etc/apt/sources.list.d/gazebo-stable.list'
```
```
wget http://packages.osrfoundation.org/gazebo.key -O - | sudo apt-key add -
```
```
sudo apt-get update
```
```
sudo apt-get install libignition-gazebo6-dev
```

### Test Ignition Gazebo

Foxy Tutorial

https://docs.ros.org/en/foxy/Tutorials/Advanced/Simulators/Ignition.html

```
sudo apt install ros-foxy-ros-ign
```
```
ign gazebo -v 4 -r --render-engine ogre visualize_lidar.sdf
```

# Gazebo to ROS bridge

```
sudo apt-get install ros-foxy-ros-ign-bridge
```
```
source /opt/ros/foxy/setup.bash
```

Otro Ejemplo
```
ign gazebo -v 4 -r camera_sensor.sdf
```

## ROS packages

### Robot Steering 
```
sudo apt install ros-foxy-rqt-robot-steering
```
Comando para ejecutar
```
rqt_robot_steering
```

### Gazebo packages para ROS
```
sudo apt-get install ros-foxy-gazebo-ros-pkgs
```

### Robot Localization
```
sudo apt-get install ros-foxy-robot-localization
```

### Robot Steering GUI
```
sudo apt install ros-foxy-rqt-robot-steering
```
