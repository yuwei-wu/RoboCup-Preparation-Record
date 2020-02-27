
usage:    

#### Player/Vision/detectBallv5.lua    
```
    local headAngle = Body.get_head_position(); --{yaw, pitch}
```

#### Player/Vision/Vision_thread.lua    
```
  vcm['set_image'..cidx..'_count'](self.img_count);
  headAngles = Body.get_head_position();
  HeadTransform.update(cidx-1, headAngles);

```

## 2. Pose estimation Error
bad performance (can we print the pose without vision?)



## 3. Vision Detection Error
it's easy to see in our monitor

## 4. Feature transformation/ projection Error

can see in the monitor but need more testing
