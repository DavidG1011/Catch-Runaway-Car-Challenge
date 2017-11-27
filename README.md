[//]: # (Image References)

[image1]: ./imgs/caught.PNG "Runaway Caught"

# Run Away Robot with Unscented Kalman Filter Bonus Challenge Starter Code

Self-Driving Car Engineer Nanodegree Program

---

Overview

This repository contains all the code needed to complete the Bonus Challenge: Catch the Run Away Car with Unscented Kalman Filter.

Project Introduction

In this project, an UKF is used to catch an escaped car driving in a circular path. 
The run away car will be being sensed by a stationary sensor, that is able to measure both noisy lidar and radar data. The capture vehicle will need to use these measurements to close in on the run away car. To capture the run away car the capture vehicle needs to come within .1 unit distance of its position. However the capture car and the run away car have the same max velocity, so if the capture vehicle wants to catch the car, it will need to predict where the car will be ahead of time.

Running the Code

This project involves the Term 2 Simulator which can be downloaded [here](https://github.com/udacity/self-driving-car-sim/releases)

This repository includes two files that can be used to set up and intall uWebSocketIO for either Linux or Mac systems. For windows you can use either Docker, VMware, or even Windows 10 Bash on Ubuntu to install uWebSocketIO.

Once the install for uWebSocketIO is complete, the main program can be built and ran by doing the following from the project top directory.

mkdir build 

cd build 

cmake .. make 

./UnscentedKF


## Dependencies

* cmake >= v3.5
* make >= v4.1
* gcc/g++ >= v5.4
* uWebSocketIO

## Basic Build Instructions

1. Clone this repo.
2. Make a build directory: `mkdir build && cd build`
3. Compile: `cmake .. && make`
4. Run it: `./UnscentedKF 


---


# UKF(Unscented Kalman Filter)

This bonus challenge successfully uses an unscented kalman filter to predict the position of a constantly moving runaway car and catches it with a car moving at the same max velocity. 

More detail can be found about the UKF algorithm on my main project repo located [Here](https://github.com/DavidG1011/Udacity-Unscented-Kalman-Filter). 

# Solution And Stats

### Solution

My solution involves moving in the opposite direction the runaway car is to face it head on. 

### Stats

The car is consistently caught with my UKF algorithm at about 4.5 seconds with my best distance typically < 0.05

![alt text][image1]
