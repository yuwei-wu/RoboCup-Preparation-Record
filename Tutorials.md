
## [Computer Vision: Algorithms and Applications](http://szeliski.org/Book/)

## Part One: Image formation

### 1. [Photometric image formation](https://cseweb.ucsd.edu/classes/sp15/cse152-a/lec6.pdf)

### 2. Color
[HSV](https://en.wikipedia.org/wiki/HSL_and_HSV) (Hue, Saturation, and Value)
[RGB](https://en.wikipedia.org/wiki/RGB_color_model) (Red, Green, and Blue)  
[YUV](https://en.wikipedia.org/wiki/YUV) (luma(Y′), two chrominance components U (blue projection) and V (red projection) respectively.)

RBG is good from the hardware standpoint of view, since it is how the pixels are captured and displayed (Bayer filter is one good example) but does not capture the way humans perceive the colors.

[WPI HSV](https://docs.wpilib.org/en/latest/docs/software/vision-processing/introduction/identifying-and-processing-the-targets.html#what-is-hsl-hsv)

### 3. object distance
[WPI Dis](https://docs.wpilib.org/en/latest/docs/software/vision-processing/introduction/identifying-and-processing-the-targets.html#distance)


### 4. your digit camera (Lifecam)
calibration / setting /  Read and Process Video


## Part Two: Deal with the images

### 1.Image preprocessing

### 2.Feature detection and matching

### 3.Segmentation

### 4.Object Tracking 

### 5.[Edge Detection](https://alliance.seas.upenn.edu/~cis581/Lectures/Fall2019/cis581-2019-Convolution3-py.pdf)

## Part Three: First Robots

### 1. Color panel 

 segments the highest-resolution color images   
 build and train the classifier (Baysian Method/Unimodal Gaussian/ Gaussian mixture model)     
 forms connected regions     
 recognizes objects from the statistics of the colored regions   

[color segmentation](https://www.cs.cmu.edu/~dst/Tekkotsu/Tutorial/colorsegment.shtml)

### 2. Target recognition and Lighting (shooting)

#### [RoboRealm tutorials](http://www.roborealm.com/tutorials.php)

#### SmartDashboard Camera Extension (programmed in Java, works with any robot language)

#### [GRIP](https://docs.wpilib.org/en/latest/docs/software/vision-processing/grip/introduction-to-grip.html)

[Generating Code from GRIP](https://docs.wpilib.org/en/latest/docs/software/vision-processing/grip/generating-code-from-grip.html) 

## [Camera Server](https://first.wpi.edu/FRC/roborio/beta/docs/java/edu/wpi/first/wpilibj/CameraServer.html)

