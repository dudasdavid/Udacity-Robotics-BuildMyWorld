# Robotics Software Engineer Nanodegree Program

## Project 1/5: Build My World

[//]: # (Image References)

[image1]: ./images/gazebo_screen.png "Gazebo"
[image2]: ./images/terminal_screen.png "Terminal"

### Summary of Tasks:
* Build a single floor wall structure using the Building Editor tool in Gazebo. Apply at least one feature, one color, and optionally one texture to your structure. Make sure there's enough space between the walls for a robot to navigate. 
* Model any object of your choice using the Model Editor tool in Gazebo. Your model links should be connected with joints. 
* Import your structure and two instances of your model inside an empty Gazebo World.
* Import at least one model from the Gazebo online library and implement it in your existing Gazebo world. 
* Write a C++ World Plugin to interact with your world. Your code should display “Welcome to ’s World!” message as soon as you launch the Gazebo world file. 

### Project structure:
```bash
tree -I build

.Udacity-Robotics-BuildMyWorld                  # Build My World Project
├── CMakeLists.txt                              # Link libraries
├── README.md                                   # Project documentation
├── images                                      # Images for project documentation
│   ├── gazebo_screen.png
│   └── terminal_screen.png
├── model                                       # Model files
│   ├── Building                                # Single floor building model files
│   │   ├── model.config
│   │   └── model.sdf
│   └── Robot                                   # Robot model files
│       ├── model.config
│       └── model.sdf
├── script                                      # Gazebo World plugin C++ script
│   └── welcome_message.cpp
└── world                                       # Gazebo main World containing models
    └── MyWorld.world
```

### Remarks:
* The project was built in local environment using Gazebo 9
* Local environment was Ubuntu 18.04 running in Windows WSL2
* The warning messages in the terminal window was caused by an ALSA driver issue of the WSL2

![alt text][image2]
![alt text][image1]
