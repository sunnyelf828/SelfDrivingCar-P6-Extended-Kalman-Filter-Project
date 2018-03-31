# SelfDrivingCar-P6-Extended-Kalman-Filter-Project
Extended Kalman Filter Project Starter Code
Self-Driving Car Engineer Nanodegree Program

In this project you will utilize a kalman filter to estimate the state of a moving object of interest with noisy lidar and radar measurements. Passing the project requires obtaining RMSE values that are lower than the tolerance outlined in the project rubric.

This project involves the Term 2 Simulator which can be downloaded here

This repository includes two files that can be used to set up and install uWebSocketIO for either Linux or Mac systems. For windows you can use either Docker, VMware, or even Windows 10 Bash on Ubuntu to install uWebSocketIO. Please see this concept in the classroom for the required version and installation scripts.

Once the install for uWebSocketIO is complete, the main program can be built and run by doing the following from the project top directory.

mkdir build
cd build
cmake ..
make
./ExtendedKF
Tips for setting up your environment can be found here

Note that the programs that need to be written to accomplish the project are src/FusionEKF.cpp, src/FusionEKF.h, kalman_filter.cpp, kalman_filter.h, tools.cpp, and tools.h

The program main.cpp has already been filled out, but feel free to modify it.

Here is the main protcol that main.cpp uses for uWebSocketIO in communicating with the simulator.

INPUT: values provided by the simulator to the c++ program

["sensor_measurement"] => the measurement that the simulator observed (either lidar or radar)

OUTPUT: values provided by the c++ program to the simulator

["estimate_x"] <= kalman filter estimated position x ["estimate_y"] <= kalman filter estimated position y ["rmse_x"] ["rmse_y"] ["rmse_vx"] ["rmse_vy"]

Other Important Dependencies
cmake >= 3.5
All OSes: click here for installation instructions
make >= 4.1 (Linux, Mac), 3.81 (Windows)
Linux: make is installed by default on most Linux distros
Mac: install Xcode command line tools to get make
Windows: Click here for installation instructions
gcc/g++ >= 5.4
Linux: gcc / g++ is installed by default on most Linux distros
Mac: same deal as make - install Xcode command line tools
Windows: recommend using MinGW
Basic Build Instructions
Clone this repo.
Make a build directory: mkdir build && cd build
Compile: cmake .. && make
On windows, you may need to run: cmake .. -G "Unix Makefiles" && make
Run it: ./ExtendedKF
Editor Settings
We've purposefully kept editor configuration files out of this repo in order to keep it as simple and environment agnostic as possible. However, we recommend using the following settings:

indent using spaces
set tab width to 2 spaces (keeps the matrices in source code aligned)
Code Style
Please (do your best to) stick to Google's C++ style guide.

Generating Additional Data
This is optional!

If you'd like to generate your own radar and lidar data, see the utilities repo for Matlab scripts that can generate additional data.

Project Instructions and Rubric
Note: regardless of the changes you make, your project must be buildable using cmake and make!

More information is only accessible by people who are already enrolled in Term 2 of CarND. If you are enrolled, see the project resources page for instructions and the project rubric.

Hints and Tips!
You don't have to follow this directory structure, but if you do, your work will span all of the .cpp files here. Keep an eye out for TODOs.

Students have reported rapid expansion of log files when using the term 2 simulator. This appears to be associated with not being connected to uWebSockets. If this does occur, please make sure you are conneted to uWebSockets. The following workaround may also be effective at preventing large log files.

create an empty log file
remove write permissions so that the simulator can't write to log
Please note that the Eigen library does not initialize VectorXd or MatrixXd objects with zeros upon creation.

Call for IDE Profiles Pull Requests
Help your fellow students!

We decided to create Makefiles with cmake to keep this project as platform agnostic as possible. Similarly, we omitted IDE profiles in order to ensure that students don't feel pressured to use one IDE or another.

However! We'd love to help people get up and running with their IDEs of choice. If you've created a profile for an IDE that you think other students would appreciate, we'd love to have you add the requisite profile files and instructions to ide_profiles/. For example if you wanted to add a VS Code profile, you'd add:

/ide_profiles/vscode/.vscode
/ide_profiles/vscode/README.md
The README should explain what the profile does, how to take advantage of it, and how to install it.

Regardless of the IDE used, every submitted project must still be compilable with cmake and make.

How to write a README
A well written README file can enhance your project and portfolio. Develop your abilities to create professional README files by completing this free course.
