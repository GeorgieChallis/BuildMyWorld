# Build My World (Robotics Software Nanodegree)
Submission for Project 1 of the Udacity Robotics Nanodegree - introduction to Gazebo simulator by creating a world with a simple building and 4 wheeled dumb 'robot' model. Plugin use demonstrated with a command line 'Hello World' introduction when the world is instantiated.

## Build and Run
### To build with CMake
In the repository root directory:
```
$ mkdir build
$ cd build
$ cmake ../
$ make
$ export GAZEBO_PLUGIN_PATH=${GAZEBO_PLUGIN_PATH}:~/workspace/RoboND_BuildMyWorld/build
```

### Run in ROS
Change back to main repo directory and run gazebo: 
```
$ cd ../
$ gazebo world/number25world-v2
```

<img src="https://github.com/GeorgieChallis/RoboND_BuildMyWorld/blob/master/img/Gazebo.png" width="640">

### Directory Structure
```
    .RoboND_BuildMyWorld            # myrobot lab main folder              
    ├── model                          
    │   ├── 4wheel		            # Model files for a 4 wheel 'robot' 
    │   │   ├── model.config	       
    │   │   ├── model.sdf
    │   ├── Number25		        # Model files for 2 basic rooms
    │   │   ├── model.config
    │   │   ├── model.sdf
    ├── script                      # Gazebo World plugin C++ script      
    │   ├── hello.cpp
    ├── world                       # Gazebo main World scene
    │   ├── number25world-v2
    ├── CMakeLists.txt              # Link libraries 
                             
```

