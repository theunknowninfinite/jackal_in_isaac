# Jackal in Nvidia Isaac
## Authors

- Suriya Suresh

## 1.Packages Required 
The code uses the following libraries/modules:
* Nvidia Isaac 
* ROS Noetic 
On Ubuntu 20.04 using Nvidia Drivers 525.125.xx.

## 3. Setting up the Package

1. Clone the github repo.

```` 
$ git clone linkofrepo
````
2. Then open Nvidia Isaac and open the file jackal_outdoor under worlds.
3. Before running the simulation, run Rviz.
4. Ensure that the fixed frame reference in the left panel is given as jackel.
5. Add topics RGB and Point cloud under By Topics when you go to add a topic to visualise.
6. Run the simulation
7. Pass the following command to get the robot to move
```` 
$ rostopic pub /cmd_vel geometry_msgs/Twist '{linear:  {x: 0.0, y: 0.0, z: 0.0}, angular: {x: 0.0,y: 0.0,z: 0.0}}'
````
8. The robot starts to move slowly in the isaac window.
9. As the robot moves,rviz also gets updated with the camera feed and the point cloud from the robot.
10. Stop the simulation by pressing stop in the Nvidia Isaac Sim.

# Credits 
Nvidia Isaac Sim Documentation 

Clearpath Jackal Github Repo 

Nvidia Omniverse Forums 
