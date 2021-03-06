---
layout: post
title: (Ongoing-project) Path-following and collision avoidance with Variable Interval Prediction MPC (VIP-MPC)
author: Minsung Kim
date:   2018-12-05 7:00:00 -0400
permalink: /VIPMPC-project
categories: projects
tags: HQP
excerpt: Path-following and collision avoidance with Variable Interval Prediction MPC (VIP-MPC)

github: https://github.com/WestsideMS
# external-website: http://dyros.snu.ac.kr/hqptasks/

image: /assets/img/project-images/2.task/mpc_carsim.png
imageAlt: 
image-slider: /assets/img/project-images/2.task/mpc_carsim.png

---
<!-- ### Overview
The robots with high Degrees of Freedom (DoF) such as humanoids and mobile manipulators are expected to perform multiple tasks simultaneously. Hierarchical Quadratic Programming (HQP) can effectively compute a solution for strictly prioritized tasks. However, the continuity of control input is not guaranteed when the priorities of the tasks are modified during operation. This paper proposes a continuous task transition method for HQP based controller to insert, remove, and swap arbitrary tasks without discontinuity. Smooth task transition is assured because our approach uses activation parameters of the new and existing tasks without modifying control structure. The proposed approach is applied to various task transition scenarios including joint limit, singularity, and obstacle avoidance to guarantee the stable execution of the robot. The proposed control scheme was implemented on a 7-DoF robotic arm, and its performance was demonstrated by the continuity of control input during various task transition scenarios.  -->

### Experimental Results
<div class="row projects-display">
    <div class="seven columns images">
        <div class="video-container">
            <iframe width="560" height="315" src="https://www.youtube.com/embed/zjRWDb2kr3o" frameborder="0" allowfullscreen></iframe>
        </div>
    </div>
</div>



<!-- ### Experimental Equipments
<div class="row projects-display">
	<div class="six columns">
		<div class="images">
			<img alt="Awesome Check In" height="100" src="{{ site.url }}/assets/img/project-images/2.task/structure.png">
		</div>
	</div>

	<div class="six columns">
		<h5> Overview of the robot we used </h5>
		<li> Kinamatic sturture of the robot is the left figure </li>
		<li> Torque controlled 7-DoFs actuators with 2000 Hz</li>
		<li> Ubuntu 14.04/16.04 with real-time Kernel </li>
		<li> Quite strong friction, so we implemented simple friction compensator.</li>
	</div>
</div>

### Algorithms
+ Task transition algorithm with HQP (Summitted the paper in RAL)
	- We proposed the task transition algorithm based on HQP frameworks.
	- The proposed algorithm can treat not only equality tasks but also inequality tasks. 
    - We tested various task transition senarios including joint limit, singularity, and obstacle avoidance.
	- See also [**RAL2019**]({{ site.url}}/HQP-transition) and [**Mobile Project**]({{ site.url}}/HQP-project)

+ Task transition algorithm in the operational space
	- We also implemented our previous task transition algorithms of [**[1]**](http://dyros.snu.ac.kr/paper/TRO-task-transition-published-version.pdf) and  [**[2]**](http://dyros.snu.ac.kr/wp-content/plugins/uploadingdownloading-non-latin-filename/download.php?id=1979).
	- However, we cannot operate robot with these algorithm, because of very heavy computation.  

### Why we used HQP?
+ Easy to implement
	- Although pseudo inverse based method is a little faster than HQP based controller, the HQP based controller is more easy to treat both equality and inequality tasks.
	- This is quite good point, because many inequality constraints are related on the stablity of the robot. (For example, friction cone of the foot in the humanoid.)
+ Solve Inverse Kinematics (IK) and Inverse Dynamics (ID) problems.
	- HQP can solve IK and ID easily.
	- Although the operational space controller also can solve ID, this method needs "Lambda matrix" which has very big complexity.
+ Calculation speed of the HQP is not slow to operate robot.
	- Many researches on the improvement of the computation time of the HQP solver.
	- Thus, this method is acceptable to the robotic community. -->


