# Sock_Robot
Tutorial based project for building a mobile robot that uses a 2D camera and a manipulator to locate and pick up socks. 

## View robot in RViZ

```
roslaunch sock_description display.launch
```

## Gazebo simulation
```
roslaunch sock_gazebo sock_gazebo.launch
```

## Mapping demo

1. Launch simulation and gazebo with this command:

```
roslaunch sock_gazebo sock_gazebo.launch
```

2. Launch the gmapping demo with this command

```
roslaunch sock_2dnav gmapping_demo.launch
```

3. Store map with: 

```
rosrun map_server map_saver -f willowgarage
```

## Navigate through the willowgarage

1. Launch simulation and gazebo with this command:

```
roslaunch sock_gazebo sock_gazebo.launch
```

2. Launch amcl: 
```
roslaunch sock_2dnav sock_2damcl.launch
```

## note

There's stil quite a bit of room for improvement: 
1. Create a full map of the willowgarage
2. Optimise the slam parameters, currently the map is drifting
3. Add a mesh to the robot

