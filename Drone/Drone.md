---
tags: drone , itron , programming
---
# Begining
After participated in the TDK competition last week , I started to be interested in making the drone by myself and the programming about the computer vision. I decide to start learning from now and hope  I will be able to join the drone competition of TDk few years later. No matter whether I will persist , I will learn something along this way  at least.

# 2022/10/19 
I found a youtuber recorded himself making drones to track himself , incredible
[his channel](https://www.youtube.com/c/MattClarke)

down below are some keywords
ORB-SLAM2
structure form motion
waveshare imx219-83
left and right camera
depth map and inference
set point GPS
controlled flight
navidia jetson nano (central controll)
opencv
steroBGM
yoloR
damping mount

# 2022/10/23 
search for how to build a drone

## components
1. fly controller 
![[Pasted image 20221023122759.png]]
![[Pasted image 20221023123200.png]]

why not perform stabilization on the flight computer?
> The speed of the flight computer is not guaranteed constant and also it prone to freezing or crashing.
- fly computer

2. frame
3. VTX (要接電線才能通電 不然會燒掉)   [VTX教學](https://www.youtube.com/watch?v=uFbuDqg424c)
4. LiPo battery
5. brushless motor
6. 飛行控制器
7. antennas
8. camera
9. ESC : electronic speed controllers 



## some unknown stuff
1. imu : inertial measurement unit
2. gyro : 陀螺儀
3. EKF : 
- extended Kalman filter  擴展卡曼濾波器 computer vision
- SLAM的其中一種算法
- [詳細EKF](https://www.cnblogs.com/gaoxiang12/p/5560360.html)
4. [不錯的教學網站](https://prg.cs.umd.edu/enae788m)
5. stereo from odometry (2d 轉 3d)
6. ORB feature matching (opencv 有函式庫)
7. optical flow (光流 用來在移動中辨識物體之類的)
 

[四軸無人機project example](https://www.youtube.com/watch?v=2r0fX_8A8ms)
![[Pasted image 20221023124740.png]]
![[Pasted image 20221023125708.png]]
![[Pasted image 20221023125811.png]]
![[Pasted image 20221023132356.png]]
![[Pasted image 20221023132437.png]]  
![[Pasted image 20221023132609.png]]
![[Pasted image 20221023132740.png]]

## To kick start

