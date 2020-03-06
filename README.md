# How-to
First of all be sure the ethernet cable is plugged in and start the Panda controller.
Be sure you can ping the Panda with:

```
ping 172.16.0.2
```

To start the RViz GUI open a terminal and

```
cd panda_ws
source devel/setup.bash
roslaunch panda_moveit_config panda_control_moveit_rviz.launch load_gripper:=false robot_ip:=172.16.0.2
```

On the planning window you can move the goal state and try to plan the motion. If it's ok you can press "execute".

Then, if you want to run the python script:

```
rosrun panda_moveit_config script1.py
```
