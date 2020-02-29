
# 2020-spring Upennalizers feature transformation

## 1. Problem Description and challenges
In previous competition, the performance of feature transformation is not good. In addition,
because our pose estimation is based on these features, 
it will really effect in the competition. Also there are penalties if robots walk out the line boundary, 
we need to improve our projection and pose corrections. 

### 1.1 Mirrored Pose Estimates (still a possible issue)
The field is symmetrical, it is very important to make sure the robot does not get too much error in the yaw direction, otherwise it can sometimes get flipped. 


### 1.2 Line and Circle Detection 

considering that using HSL is more accurate for white lines.

### 1.3 

## 2. Literature Review

There are four types of features. Check every possible intersection produced by pairs of lines which have at least 10 degrees angle difference in order to avoid
finding intersections by two continuous lines.

[Improvement of Self-Localization via 
Pose Correction Procedure in RoboCup](https://pdfs.semanticscholar.org/30d0/745ca4bacd90685288098b553c961201ca41.pdf)
We can see the chapter 4. 

## 3. Previous Work

### use cameria intrinsics 

### undistort


## 4. New implementation

### Add thresholds to two paralleled lines.




