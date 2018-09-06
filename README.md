[![Build Status](https://travis-ci.org/UofA-SPEAR/station2.svg?branch=master)](https://travis-ci.org/UofA-SPEAR/station2)
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
Cython: `$ python3 -m pip install cython --user`<br>
Pygame: `$ python3 -m pip install pygame --user`<br>
Kivy: `$ python3 -m pip install kivy --user`<br>
libqt (required by Nimbro): `$ apt-get install libqt4-dev`<br>
qmake (required by Nimbro): `$ apt-get install qt4-qmake`<br>

Then clone the repository, and run the `unpack.sh` command located within.

This will setup your catkin workspace for development.

