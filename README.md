
## INSTRUCTIONS TO RUN

Download/Clone the package into the workspace and build using catkin build or catkin_make.
Source the workspace.

## 2-D Path Planning Methods

To run the below path planning algorithms, run the following from src folder the workspace:

### RRT
```bash
$ cd final_project/scripts/
$ python3 rrt.py
```

### RRT*
```bash
$ cd final_project/scripts/
$ python3 rrt_star.py
```

### RRT*-Smart
```bash
$ cd final_project/scripts/
$ python3 rrt_star_smart.py
```

### RRT-Connect
```bash
$ cd final_project/scripts/
$ python3 rrt_connect.py
```


## Gazebo+Rviz Simulation
This is using Navigation stack so is technically not correct:
However depending on the algorithm to run uncomment the lines in the move.py script 
For RRT star, RRT star smart uncomment line 78 and comment line 79 for RRT connect and RRT do visa versa.

To run the simulation:

```bash
$ roslaunch final_project world.launch
```

In another terminal run,
```bash
$  roslaunch final_project navigation.launch 
```

Make the map align with the world in rviz by moving the robot using 2D Pose Estimate.

Open a new terminal and run,
```bash
$ cd final_project/scripts/
$ python3 move.py
```
Reference: https://github.com/anikk94/enpm661_project5/tree/main/final_project 