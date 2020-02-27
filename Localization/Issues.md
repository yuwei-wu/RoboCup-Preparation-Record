##  2.27.2020

### 1. Does the camera calibrated ?

Actually in the paper, the method of RANSAC Line Fitting works well (I've read the HTWK and B-human method and our are the combination). 
It should works well, but why not?   

Actually from b-human report, they still use this method in 2019. I think it cannot be the issue.

### 2. The boundary landmark
I notice the pratical filter process and believed ths part cannot be the issue.


### 3. Better color space ? 

Actually RGB can works very well in green classification, but after I read some papers about road line detection.
If we would like to implement better line detection, maybe the netural network is needed    
https://github.com/amusi/awesome-lane-detection   
https://paperswithcode.com/task/lane-detection  

But I've seen that now B-human and other teams 2019 report still use color segmentation, 
maybe it's ok in the less complex robocup situation.  (HSL works better for line detection)

The issue is that the network works very well for line detection (LineNet) may not work well for ball detection. 
(https://arxiv.org/pdf/2002.06604v2.pdf is pretty good) 
