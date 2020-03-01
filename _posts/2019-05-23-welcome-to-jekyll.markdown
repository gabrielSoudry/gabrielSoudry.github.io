---
layout: post
title:  "Position and Speed Control of a DC Motor using ROS"
date:   2019-05-23 21:03:36 +0530
---

I decided for this first tutorial to make a tutorial about PID with ROS. It's probaly the most important part of a autonomous robot... And the most complicaded.

So first let's begin by the beginning... What's PID ? 

A proportional integral derivative controller (PID controller) is a common method of controlling robots. PID theory will help you design a better control equation for your robot.

Put same voltage on a two motors will not help your robot to go straight. (Like many people believe)
You will need an feedback of your motors to help the microcontroller to send the right voltage on your motors to go straight ! 

So let's begin with some definition : 

Proportional Integrative Differential (PID) controller is used for a variety of applications. A proportional controller stands in a case where the input is proportional to the output. Here if the input has less noise, the output will be all most exact with no errors but minimal errors in some cases. In contrast, if the noise content is much in the input, then even the errors will be very high and the process is very slow. So this process wanted an updation to it and hence came the Proportional Differential controllers. In PID controllers, the Integrative part does the operations by integrating the current values and minimizing the errors as much as possible. Next part is the Differential part where the output can soon be predicted with the help of differentiating  the current values thus making the operations as fast as possible and also as accurate as possible. This PID controllers as costlier compared to the other controllers but they are worth their cost. They are now being used in control systems in most of the industries. (Source [PID][PID])

![texture theme preview](http://drive.google.com/uc?export=view&id=1RUp7PhoLMYdfMKSe9lBZftWdADfVmKKi)

