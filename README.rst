baxter_simulator
==============

Gazebo simulation with emulated interfaces for the Baxter Research Robot

baxter_simulator integration in NRP 
------------------------------------

This is a modified version of the baxter simulator by rethink robotics (http://sdk.rethinkrobotics.com/wiki/Baxter_Simulator) adapted to be integrated in the NRP (Neurorobotics Platform [1] ) developped in the context of the Human Brain Project [2]. 


#### Integration in a local NRP installation [3]

- clone this repository in the folder *$HBP/GazeboRosPackages/src*
- re-build the catking workspace by running *catkin_make* in *$HBP/GazeboRosPackages*

#### Add a Baxter robot to an NRP experiment

- download the baxter robot model from [here](https://drive.google.com/file/d/1VT-mZ_9cbPSzLKrRIR2Enh2iO-NfAVyv/view?usp=sharing) 
- start a new experiment in NRP:

![nrp_new_experiment](http://drive.google.com/uc?export=view&id=1bdfY7I1vk-h9XgOWGBkN7AQVqRb5Uv-B) 

- open the object library from the left pannel of NRP the front end
- upload the baxter robot model zip file. Afterwards baxter will appear in the robots object group and it will possible to clone it:

![nrp_new_experiment](http://drive.google.com/uc?export=view&id=1yO2L7_qmhhKzd8jCXT_RLe4PXnTxhp96) 

- start the simulation and load the robot controllers:

		roslaunch baxter_gazebo baxter_control.launch

[1] [https://neurorobotics.net](https://neurorobotics.net) 
[2] [https://www.humanbrainproject.eu](https://www.humanbrainproject.eu) 
[3] [https://bitbucket.org/hbpneurorobotics/neurorobotics-platform/src/master](https://bitbucket.org/hbpneurorobotics/neurorobotics-platform/src/master) 


Latest Release Information
--------------------------

http://sdk.rethinkrobotics.com/wiki/Release-Changes
