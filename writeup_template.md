## **Extended Kalman Filter**

Once again, without all of the lectures and quizes in this module, I would not have stood a chance. I used a couple of different files to complete this project. The source code for this project can be found in the src folder of this repository. This project was a complete copy and paste job from the quizzes with just a tad bit of tunning.

The goals / steps of this project are the following:

* The goal of this project is to implement an unscented Kalman filter using the CTRV motion model in C++. I was provided simulated lidar and radar measurements detecting a bicycle (graphic is a car though?) that travels around a vehicle. I used a Kalman filter, lidar measurements, and radar measurements to track the bicycle's(possibly a car's) position and velocity.

[//]: # (Image References)

[image1]: ./Runs/Dataset1.PNG "Dataset 1"
[image2]: ./Runs/Dataset2.PNG "Dataset 2"


## [Rubric](https://review.udacity.com/#!/rubrics/748/view) Points
Here I will consider the rubric points individually and describe how I addressed each point in my implementation.  

---

# Compiling

1. Code must compile with cmake and make.

The code compiles with cmake and make. This is my second go around with this and it went quite smooth. I am not very familiar with the how to use a debugger with this, because that would have saved days on this project. I will find out how in the future.

# Accuracy

1. Your algorithm will be run against Dataset 1 in the simulator which is the same as "data/obj_pose-laser-radar-synthetic-input.txt" in the repository. We'll collect the positions that your algorithm outputs and compare them to ground truth data. Your px, py, vx, and vy RMSE should be less than or equal to the values [.09, .10, 0.40, 0.30]. Alot of data collection and guess and check went into finding my tunned standard deviations.

I passed while using Dataset #1, and just missed when using Dataset #2. Below are my results:

 Dataset 1
![alt text][image1]

 Dataset 2
![alt text][image2]

# Follows Correct Algorithm

1. Follows general processing as taught in the lessons.

My program follows the general processing as taught in the lessons. 

This can be found in the ukf.cpp file in the src folder.

# Smell Test
1. Most of the code was provided for me, so if it doesn't pass the smell test...I don't know.

### Discussion
The Unscented Kalman Filter is yet another amazing and powerful tool. I learned that setting Process noise standard deviations can be quite the chore.




