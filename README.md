# ros_run_command
Run any command from ROS launch files

## Install

This is meant to be installed as a ROS package: copy to your workspace source directory, build with catkin.

## Example

```
<?xml version="1.0"?>
<launch>
  <node pkg="ros_run_command" type="ros_run_command" name="echo_some_command" output="screen"
    args="echo I AM AN ARBITRARY COMMAND"
  />
</launch>
```

naturally, this can be used to run shell scripts

```
<node pkg="ros_run_command" type="ros_run_command" name="my_shell_script" output="screen"
    args="~/MY_SHELL_SCRIPT.sh SOME_ARG SOME_OTHER_ARG"
  />
```
