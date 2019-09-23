baxter_simulator
==============

Gazebo simulation with emulated interfaces for the Baxter Research Robot

baxter_simulator integration in NRP 
------------------------------------

This is a modified version of the baxter simulator by rethink robotics (http://sdk.rethinkrobotics.com/wiki/Baxter_Simulator) adapted to be integrated in the NRP (Neurorobotics Platform [1] ) developped in the context of the Human Brain Project [2]. 


#### Integration of baxter_simulator in a local NRP installation [3]

- clone this repository in the folder *$HBP/GazeboRosPackages/src* of your local installation
- build the catkin workspace by running *catkin_make* in *$HBP/GazeboRosPackages*

#### Create an experiment with a Baxter robot

- download the baxter robot model from [here](https://raw.githubusercontent.com/EloyRC/baxter_simulator/master/baxter_simulator/baxter_gazebo/media/baxter_robot.zip) 
- start a new experiment in NRP:

![nrp_new_experiment](https://raw.githubusercontent.com/EloyRC/baxter_simulator/master/baxter_simulator/baxter_gazebo/media/nrp_new_experiment.png) 

- open the object library from the left pannel of NRP the front end
- upload the baxter robot model zip file. Afterwards baxter will appear in the robots object group and it will possible to clone it:

![nrp_new_experiment](https://raw.githubusercontent.com/EloyRC/baxter_simulator/master/baxter_simulator/baxter_gazebo/media/nrp_clone_baxter.png) 

- load the robot controllers (before starting the simulation in NRP!):

		roslaunch baxter_gazebo baxter_control.launch
		
- add a brain and Transfer Functions to the experiment

[1] [https://neurorobotics.net](https://neurorobotics.net) 
[2] [https://www.humanbrainproject.eu](https://www.humanbrainproject.eu) 
[3] [https://bitbucket.org/hbpneurorobotics/neurorobotics-platform/src/master](https://bitbucket.org/hbpneurorobotics/neurorobotics-platform/src/master) 


Latest Release Information
--------------------------

http://sdk.rethinkrobotics.com/wiki/Release-Changes
