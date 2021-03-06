[[Build Status](https://travis-ci.org/UofA-SPEAR/station2.svg?branch=master)](https://travis-ci.org/UofA-SPEAR/station2)
# Station 2
This is the ground control package. It contains all the tools nessesary for
controlling the rover. 


## Setup Instructions
To install first make sure you have the dependecies. The
First is ROS, which we use for almost everything on the rover. The second is for
encoding video. The third is Kivy, which is what the UI is written in.

ROS: follow the instructions
[here](http://wiki.ros.org/kinetic/Installation/Ubuntu)<br>
x264: `$ apt-get install libx264-dev`<br>
Cython: `$ python -m pip install cython --user`<br>
Pygame: `$ python -m pip install pygame --user`<br>
Kivy: `$ python -m pip install kivy --user`<br>
Kivy Garden: `$ python -m pip install kivy-garden --user`<br>
Kivy Knob: `$ garden install knob`<br>
ROS Joy: `$ sudo apt-get install ros-kinetic-joy`<br>
libqt (required by Nimbro): `$ apt-get install libqt4-dev`<br>
qmake (required by Nimbro): `$ apt-get install qt4-qmake`<br>

Note: ROS Kinetic requires the python 2 versions of all modules.

Then clone the repository, and run the `unpack.sh` command located within.

This will setup your catkin workspace for development.

## Running "remote" launch files ##

Current status is: not working but close.

For now, just ssh into the remote and run the main launch file.
Then on the local machine, run:

```
export ROS_MASTER_URI=http://tegra-ubuntu:11311/
```

And then any nodes you run on your local machine will automatically
connect to the remote machine.

### How To (not working yet) ###

See [this post](https://answers.ros.org/question/41446/a-is-not-in-your-ssh-known_hosts-file/)

## Code Formatting ##

### Python ###

```
autopep8 --in-place filename.py
```
