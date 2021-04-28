---
layout: post
title: Model Predictive Control Method for Autonomous Vehicles using Time-Varying and Non-uniformly Spaced Horizon
author: Minsung Kim
date:   2018-12-06 7:00:00 -0400
permalink: /MPC
categories: projects
tags: Path-following, MPC, Collision avoidance, Intelligent vehicle
excerpt: In this study, a path-following and obstacle-avoidance algorithm was proposed for an autonomous vehicle that varied sampling time of the MPC prediction model. The path-following and collision avoidance performances were evaluated using both the CARLA simulator and a real vehi-cle.

github: https://github.com/WestsideMS
# external-website: http://dyros.snu.ac.kr/project/non-holonomic-mobile-manipulator/

image: /assets/img/project-images/1.mobile/mpc_access.png
imageAlt: MPC
image-slider: /assets/img/project-images/1.mobile/mpc_access.png

---
### Overview
This paper proposes an algorithm for path-following and collision avoidance of an autonomous vehicle based on model predictive control (MPC) using time-varying and non-uniformly spaced horizon. The MPC based on non-uniformly spaced horizon approach uses the time intervals that are small for the near future, and time intervals that are large for the distant future, to extend the length of the whole prediction horizon with a fixed number of prediction steps. This MPC has the advantage of being able to detect obstacles in advance because it can see the distant future. However, the presence of longer time interval samples may lead to poor path-following performance, especially for paths with high curvature. The proposed algorithm performs proper adjustment of the prediction interval according to a given situation. For sections with large curvature, it uses the short prediction intervals to increase the path-following performance; further, to consider obstacles over a wider range, it uses the long prediction intervals. This technique allows simultaneous improvement of the path-following performance and the range of obstacle avoidance with fixed computational complexity. The effectiveness of the proposed method is verified through an open-source simulator, CARLA and real-time experiments.

<!-- ### Experimental Equipments
The system consists of two robots. The mobile base is [**Clearpath Husky**](https://www.clearpathrobotics.com/husky-unmanned-ground-vehicle-robot/) and the manipulator is [**Franka Emika Panda**](https://www.franka.de/panda/).

It has a powerful computation unit to solve complicated whole-body dynamics and plan motions in high dimensional state space. The specification is described below.
+ CPU: Intel i7-7700K
+ RAM: 16 GB
+ Storage (SSD): 500 GB
+ OS: Ubuntu 16.04 (with preempt_rt kernel)

### Algorithms
<div class="row projects-display">
    <div class="six columns">
        <div class="images">
            <img alt="JUCE" src="{{ site.url }}/assets/img/project-images/1.mobile/nonholo.png">
        </div>
     </div>
    <div class="six columns">
        <div class="images">
            <img alt="JUCE" src="{{ site.url }}/assets/img/project-images/1.mobile/overview.png">
        </div>
    </div>
</div>
<!-- + Controller
	- Wholebody controller based on the HQP controller.
	- Task transition algorithm for the HQP frameworks (with Joint limit, singularity, and obstacle avoidance algorithm) 
	- Momentum based observer

+ Planner
	- Basic BiRRT(-connect) algorithm
	- VKC based dual-arm manipulation algorithm  -->

### Simulation and Experimental Results
<div class="row projects-display">
    <div class="seven columns images">
        <div class="video-container">
            <iframe width="560" height="315" src="https://www.youtube.com/embed/eo7fYDLGQcg" frameborder="0" allowfullscreen></iframe>
        </div>
    </div> 
</div>

