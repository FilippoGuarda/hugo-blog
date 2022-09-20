---
title: "So you are having problem with ROS"
date: 2022-09-20T15:56:25+02:00
draft: false
tags: ['ROS']
---
Do not worry, we all have been there. 

Maybe the command `roslaunch` + TAB is not listing your custom `.launch` file?  
Maybe it's `rostopic list` that still, after checking ten times that the `.msg` definitions are correct, refuses to acknowledge that there are new types of messages available.  
You can't `rosrun` your node, but the cmake configuration file of your package is there, as well as the `.xml` one.  
Catkin also builds without errors so _why the hell_ is this not working? 

It can drive a man crazy, but I might have the solution of your problems:

# The command to rule them all

> **`$ source devel/setup.bash`**  

You forgot about it, be honest.

It may not work _all_ the time, but it comes pretty close to that.  
You can also choose the nuclear option and completely delete the `build` and `devel` folders, then `$ catkin_make` again. This often solves the problem in case you transfered a package from one machine to another by saving the whole workspace. 

As always:
> remember to **`$ source devel/setup.bash`**

