
# 1. method GMM for color segmentation


save the LUT as a binary file so that the Lua code can load and use it:
```
write_lut_file(lut, 'my_luar_lut.raw');
```


# data: UPennalizers/upenndev/Player/Data/


#### Buckman_USOpen2016_Apr21_8pm_Bottom.raw the lut data


Each robot calculates the position of the ball in its local robot frame. 


The current ball location is stored in shared memory. 

get ball local position
```
> ball = wcm.get_ball();
> util.ptable(ball);
```
get robot position
```
robotPose = wcm.get_pose()
> util.ptable(robotPose);
y    -0.37558883234059
x    -1.5945999399009
a    -2.6230558191345
````
The robot pose is relative to the world frame and the ball position is relative to the robot frame, 
so we can get the position of the ball in the world frame as follows:
```
ballGlobal = util.pose_global({ball.x, ball.y, 0}, {robotPose.x, robotPose.y, robotPose.a});
> print(ballGlobal)
{-2.40096, -0.806157, -2.62306}
```
usage:
Player/BodyFSM/bodyAnticipate.lua   
Player/BodyFSM/bodyChase.lua   
Player/BodyFSM/bodyGotoCenter.lua   
Player/BodyFSM/bodyOrbit.lua   
Player/BodyFSM/bodyPositionGoalie.lua   
Player/BodyFSM/position.lua   
Player/BodyFSM/targetpose.lua  
Player/Vision/Vision_webots_gps.lua   
Player/Vision/detectBall.lua   
Player/Vision/detectBall_coach.lua   
Player/Vision/detectBallv2.lua   
Player/World/World.lua   
 
The ball is symmetric so its orientation is not defined.
Here we are just using an angle of 0 for the orientation in the robot frame. 
The orientation in the world frame is not informative.












