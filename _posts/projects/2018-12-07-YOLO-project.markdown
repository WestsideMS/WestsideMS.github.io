---
layout: post
title: (Ongoing-project) SLAM + Yolo (v.3) + Informed RRT star + MPC path-following 
author: Minsung Kim
date:   2018-12-06 7:00:00 -0400
permalink: /MPC
categories: projects
tags: Path-following, MPC, Collision avoidance
excerpt: In this project, an automatic integrated parking system is implemented to address the limitations of modules.

#github: https://github.com/WestsideMS
# external-website: http://dyros.snu.ac.kr/project/non-holonomic-mobile-manipulator/

image: /assets/img/project-images/1.mobile/yolo_park.png
imageAlt: MPC
image-slider: /assets/img/project-images/1.mobile/yolo_park.png

---
### Overview
---- Automatic integrated parking system ---- 

- Localization: LeGO-LOAM SLAM 
- Recognition: Deep learning-based parking lot detection YOLO (v.3) (J. Redmon et al, YOLOv3: An Incremental Improvement, arXiv 1804.02767)
- Path planning: Informed RRT star (OMPL​)
- Path-following: Model predictive controller using a dynamic bicycle model

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
            <iframe width="560" height="315" src="https://www.youtube.com/embed/lnz1ppNMHq0" frameborder="0" allowfullscreen></iframe>
        </div>
    </div> 
</div>

