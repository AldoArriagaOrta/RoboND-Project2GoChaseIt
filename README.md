# RoboND-Project2GoChaseIt

The "Go Chase It!" project's purpose is to put into pratice the lessons learned as part of the RoboND ROS Essentials lesson according to the project [rubric](https://review.udacity.com/#!/rubrics/2397/view)

Note 1: In the first project I worked locally with  ROS 2 Galactic (Ubuntu Focal) and Gazebo 9 under Ubuntu 20.04. It was too much work to make everything in the lessons compatible with ROS2 so I switched back to using the VM. 

Note 2: For some reason the changes I applied to the robot design are not shown in Gazebo, but they can be visualized in RViz.

[//]: # (Image References)

[image1]: ./images/Result.png "Result"

### Directory Structure
```
    .Project2                          # Go Chase It Project
    ├── my_robot                       # my_robot package                   
    │   ├── launch                     # launch folder for launch files   
    │   │   ├── robot_description.launch
    │   │   ├── world.launch
    │   ├── meshes                     # meshes folder for sensors
    │   │   ├── hokuyo.dae
    │   ├── urdf                       # urdf folder for xarco files
    │   │   ├── my_robot.gazebo
    │   │   ├── my_robot.xacro
    │   ├── world                      # world folder for world files
    │   │   ├── <yourworld>.world
    │   ├── CMakeLists.txt             # compiler instructions
    │   ├── package.xml                # package info
    ├── ball_chaser                    # ball_chaser package                   
    │   ├── launch                     # launch folder for launch files   
    │   │   ├── ball_chaser.launch
    │   ├── src                        # source folder for C++ scripts
    │   │   ├── drive_bot.cpp
    │   │   ├── process_images.cpp
    │   ├── srv                        # service folder for ROS services
    │   │   ├── DriveToTarget.srv
    │   ├── CMakeLists.txt             # compiler instructions
    │   ├── package.xml                # package info                  
    └──  
```

#### Results Screenshot

![alt text][image1]