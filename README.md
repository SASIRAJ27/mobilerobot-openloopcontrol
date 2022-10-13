# MobileRobot-Openloopcontrol
## Aim:

To develop a python control code to move the mobilerobot along the predefined path.

## Equipments Required:
1. RoboMaster EP core
2. Python 3.7

## Procedure

Step1:

Initiate the MobileRobot

Step2:

Connect your PC with the MobileRobot.

Step3:

Open Python program.

Step4:

Program the movements of the robot using python code.

Step5:

Execute the python program.

## Program
```python
from robomaster import robot
import time
from robomaster import camera

if __name__ == '__main__':
    ep_robot = robot.Robot()
    ep_robot.initialize(conn_type="ap")

    ep_chassis = ep_robot.chassis

    ep_chassis.drive_speed(x=0.2,y=0,z=-8.5)
    time.sleep(9.8)
    ep_chassis.move(x=0.9, y=0, z=0, xy_speed=0.75).wait_for_completed()
    ep_chassis.drive_speed(x=0.2,y=0,z=15)
    time.sleep(9.5)
    ep_chassis.move(x=2.3, y=0, z=0, xy_speed=0.75).wait_for_completed()
    ep_chassis.drive_speed(x=0.4,y=0,z=21)
    time.sleep(13)
    ep_chassis.move(x=0, y=0, z=0.5, xy_speed=2).wait_for_completed()
    ep_chassis.move(x=2.3, y=0, z=0, xy_speed=1).wait_for_completed()
    ep_chassis.drive_speed(x=0.4,y=0,z=25)
    time.sleep(2.3)
    ep_chassis.move(x=1, y=0, z=0, xy_speed=1).wait_for_completed()
    ep_chassis.drive_speed(x=0.4,y=0,z=30)
    time.sleep(2.6)
    ep_chassis.drive_speed(x=-0.5,y=0,z=-18)
    time.sleep(2.3)
    ep_chassis.move(x=0.3, y=0, z=30, xy_speed=1).wait_for_completed()
    ep_chassis.move(x=1.3, y=0, z=0, xy_speed=2).wait_for_completed()
    ep_robot.close()
```

## MobileRobot Movement Image:

![robo](./img/robomaster.png)

image
![OUTPUT](roboby.png)
![OUTPUT](rodody.png)
## MobileRobot Movement Video:

Upload your video in Youtube and paste your video-id here

[![IMAGE ALT TEXT HERE](https://img.youtube.com/vi/YOUTUBE_VIDEO_ID_HERE/0.jpg)](https://www.youtube.com/watch?v=3HZ450alq8k)

https://www.youtube.com/watch?v=3HZ450alq8k

## Result:
Thus the python program code is developed to move the mobilerobot in the predefined path.


<br/>
<br/>

```
Mobile Robotics Laboratory
Department of Artificial Intelligence and Data Science/ Machine Learning
Saveetha Engineering College
```
