# High degree-of-freedom cell
This repository contains packages for simulating robotic cells from 3 degree of freedom to 18 degree of freedom.

It is possible to use OMPL pipeline or DIRRT pipeline.

## Usage
You can launch MoveIt! demo by running:

roslaunch high_dof_[DOF]_moveit_config demo.launch pipeline:=[PIPELINE]

where:
- DOF can be equal to 3, 6, 9, 12, 15, 18.
- PIPELINE can be equal to:
  - ompl: standard OMPL MoveIt! planner
  - dirrt: motion planner from human_aware_motion_planner [human_aware_motion_planners](https://bitbucket.org/iras-ind/human_aware_motion_planners/src/master/)
  - multiple: you can chose between ompl and dirrt live (Noetic required).


## Loading collision objects

you can load predefined test scene

1) four big boxes around the robot.
roslaunch high_dof_test_scenes scene_spawner.launch
