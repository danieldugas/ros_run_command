# ros_run_command
Run any command from ROS launch files

## Install

This is meant to be installed as a ROS package: copy to your workspace source directory, build with catkin.

## Example

```
<?xml version="1.0"?>
<launch>
  <node pkg="ros_run_command" type="ros_run_command" name="SOME_NAME_FOR_MY_COMMAND" output="screen"
    args="echo I AM AN ARBITRARY COMMAND"
  />
</launch>
```

naturally, this can be used to run shell scripts

```
<node pkg="ros_run_command" type="ros_run_command" name="MY_SHELL_SCRIPT" output="screen"
    args="~/MY_SHELL_SCRIPT.sh SOME_ARG SOME_OTHER_ARG"
  />
```
