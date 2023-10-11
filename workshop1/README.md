# Project Name

A brief description of what this project does and who it's for

# Workshop 1 - Intro To ROS

## Table of Contents

- [Usage](#usage)
- [Example](#example)

## Usage

Clone the repo into a catkin workspace and build it.

Run the following in a terminal:

```bash
mkdir -p ~/catkin_ws/src
cd ~/catkin_ws/src
git clone https://github.com/jrkre/ros-workshops.git
cd ..
catkin_make
```
This should have built the project -you can now run the listener and talker nodes!

## Example

In a terminal run:

```bash
roscore
```

This is the master node that will allow the other nodes to communicate.

In a new terminal run:

```bash
source devel/setup.bash
rosrun workshop1 listener.py
```

This will run the listener node which will listen for messages from the talker node.

In a new terminal run:

```bash
source devel/setup.bash
rosrun workshop1 talker.py
```

You should now see the talker node sending messages to the listener node.

