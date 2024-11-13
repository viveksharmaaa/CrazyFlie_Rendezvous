# CrazyFlie-Jackal Rendezvous

## Install package dependencies

Install ROS following instructions provided here [ROS Installation Guide](http://wiki.ros.org/ROS/Installation)

Other dependencies include  cfclient , pyyaml , pyserial, rospkg , numpy ,scipy. You can install them using the following command.

pip install -r requirements.txt

## Usage
Once the packages are installed, you can run the Crazyflie-Jackal rendezvous experiment through the launch files.

## Running the Launch File

```roslaunch  trajectory_gen.launch```

The script ```trajectory_gen.launch``` creates three ROS nodes
``` 

ROS Nodes:
  --vrpn_client_node    Vicon ROS node to publish messages about positions using Motion Capture System .
  --flight_control      CrazyFlie ROS node, subscribing to messages published by vrpn_client_node.
  --jackal_control      Jackal ROS node, , subscribing to messages published by vrpn_client_node.

```


## Videos of Experiment

 [Air Ground rendezvous Part 1](https://www.youtube.com/watch?v=-Sh3pG2a6Zc)

[![Video](https://www.generationrobots.com/20343-product_cover/jackal-unmanned-ground-vehicle.jpg)](https://www.youtube.com/watch?v=-Sh3pG2a6Zc)

[Air-Ground rendezvous Part 2 (Adverserial Input)](https://www.youtube.com/watch?v=0-C5bhJe_ZM)
[![Video](https://www.bitcraze.io/images/crazyflie2-1/crazyflie_2.1_585px.jpg)](https://www.youtube.com/watch?v=0-C5bhJe_ZM)


## Visualization
Run the ```visualizer.launch``` to visualize the robot model and position in ```rviz```.

