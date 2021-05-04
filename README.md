# multirobot_auction_tasks
The robots coordinate to cover specific locations in a common reference frame. One robot is an auctioneer and other robots bid on a single location independently. The auctioneer assigns a task to robots following "sequential auction" mechanism until each task is allocated to a robot. Check out media/3_robots_sequential_auction_demo.mp4 for a demo on 3 robots in an empty world in gazebo simulator.

## Requirements
<ul><li>ROS -- tested on Melodic, but other versions may work
  </li><li>catkin_make -- used for building the application</li><li>turtlebot3_description -- https://github.com/AnmolChachra/turtlebot3_description (clone this in your src dir)</li></ul>

## Build
Once cloned in a ROS workspace, e.g. `/root/catkin/`, run the following commands to build it:
```
catkin_make
source devel/setup.bash
```

### Run for gazebo
```
roslaunch multirobot_auction_tasks multirobot_auction_tasks_gazebo.launch
```
