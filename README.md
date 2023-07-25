# MobileRobot-Openloopcontrol
## Aim:

To develop a python control code to move the mobilerobot along the predefined path.

## Equipments Required:
1. RoboMaster EP core
2. Python 3.7

## Procedure

Step1: Use from robomaster import robot.

<br/>

Step2: Choose the x,y,z - axis movement distance(meters).

<br/>

Step3: Give ep_chassis.move to move straight.

<br/>

Step4: Give time.sleep() for a break.

<br/>

Step5: Give ep_chassis.drive_speed to have a circular movement.

<br/>

## Program
```
from robomaster import robot
import time
from robomaster import camera

if _name=='__main_':
    ep_robot=robot.Robot()
    ep_robot.initialize(conn_type="ap")

    ep_chassis = ep_robot.chassis
    ep_led = ep_robot.led
    ep_camera = ep_robot.camera

    print("Video streaming started.....")
    ep_camera.start_video_stream(display=True, resolution = camera.STREAM_360P)

    ep_led.set_led(comp = "all",r=255,g=0,b=0,effect="on")
    ep_chassis.move(x=2.8,y=0,z=0,xy_speed=0.75).wait_for_completed()

    ep_chassis.move(x=0,y=0,z=45,xy_speed=0.75).wait_for_completed()
    ep_led.set_led(comp = "all",r=0,g=0,b=255,effect="on")

    ep_chassis.move(x=0.5,y=0,z=0,xy_speed=0.75).wait_for_completed()
    ep_led.set_led(comp = "all",r=0,g=255,b=0,effect="on")

    ep_chassis.move(x=0,y=0,z=45,xy_speed=0.75).wait_for_completed()
    ep_led.set_led(comp = "all",r=255,g=0,b=255,effect="on")


    ep_chassis.move(x=0.5,y=0,z=0,xy_speed=0.75).wait_for_completed()
    ep_led.set_led(comp = "all",r=255,g=204,b=0,effect="on")

    ep_chassis.move(x=0,y=0,z=45,xy_speed=0.75).wait_for_completed()
    ep_led.set_led(comp = "all",r=0,g=204,b=255,effect="on")

    ep_chassis.move(x=0.5,y=0,z=0,xy_speed=0.75).wait_for_completed()
    ep_led.set_led(comp = "all",r=0,g=192,b=0,effect="on")

    ep_chassis.move(x=0,y=0,z=45,xy_speed=0.75).wait_for_completed()
    ep_led.set_led(comp = "all",r=255,g=0,b=255,effect="on")

    ep_chassis.move(x=0.9,y=0,z=0,xy_speed=0.75).wait_for_completed()
    ep_led.set_led(comp = "all",r=0,g=255,b=255,effect="on")

    ep_chassis.move(x=0,y=0,z=-35,xy_speed=0.75).wait_for_completed()
    ep_led.set_led(comp = "all",r=255,g=0,b=255,effect="on")

    ep_chassis.move(x=1.9,y=0,z=0,xy_speed=0.75).wait_for_completed()
    ep_led.set_led(comp = "all",r=0,g=0,b=255,effect="on")

    ep_chassis.move(x=0,y=0,z=35,xy_speed=0.75).wait_for_completed()
    ep_led.set_led(comp = "all",r=0,g=192,b=0,effect="on")

    ep_chassis.move(x=1.44,y=0,z=0,xy_speed=0.75).wait_for_completed()
    ep_led.set_led(comp = "all",r=0,g=255,b=255,effect="on")

    ep_chassis.move(x=0,y=0,z=10,xy_speed=0.75).wait_for_completed()
    ep_led.set_led(comp = "all",r=255,g=0,b=255,effect="on")

    ep_chassis.move(x=0,y=-2.1,z=0,xy_speed=0.75).wait_for_completed()
    ep_led.set_led(comp = "all",r=0,g=192,b=0,effect="on")

    ep_chassis.move(x=0,y=0,z=-10,xy_speed=0.75).wait_for_completed()
    ep_led.set_led(comp = "all",r=0,g=0,b=255,effect="on")


    ep_chassis.move(x=-0.55,y=0,z=0,xy_speed=0.75).wait_for_completed()
    ep_led.set_led(comp = "all",r=255,g=0,b=255,effect="on")


    ep_chassis.move(x=0,y=0,z=180,xy_speed=0.75).wait_for_completed()
    ep_led.set_led(comp = "all",r=0,g=204,b=255,effect="on")














    time.sleep(4)
    
    
    ep_camera.stop_video_stream()
    print("Stopped video streaming.....")


    ep_robot.close()
```

## MobileRobot Movement Image:

![robo](./img/robomaster.png)

Insert image here
![WhatsApp Image 2023-07-18 at 11 29 44](https://github.com/AasrithSairam/mobilerobot-openloopcontrol/assets/139331438/e261f499-a2b6-4bc4-a1b6-61954c5ee550)



<br/>
<br/>
<br/>
<br/>

## MobileRobot Movement Video:

Upload your video in Youtube and paste your video-id here
https://www.youtube.com/watch?v=7Jd60ljt67c

[![IMAGE ALT TEXT HERE](https://img.youtube.com/vi/YOUTUBE_VIDEO_ID_HERE/0.jpg)](https://www.youtube.com/watch?v=YOUTUBE_VIDEO_ID_HERE)

<br/>
<br/>
<br/>
<br/>

## Result:
Thus the python program code is developed to move the mobilerobot in the predefined path.


<br/>
<br/>

```
Mobile Robotics Laboratory
Department of Artificial Intelligence and Data Science/ Machine Learning
Saveetha Engineering College
```
