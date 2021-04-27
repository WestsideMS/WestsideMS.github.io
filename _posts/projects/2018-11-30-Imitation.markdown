---
layout: post
title: Autonomous Parking Method Using Model Predictive Control:a feasibility and stability study 
author: Minsung Kim
date:   2021-04-23 7:00:00 -0400
permalink: /Switching-project
categories: projects
tags: MPC
excerpt: Considering the recursive feasibility and stability of the MPC problem while parking maneuver  

image: /assets/img/project-images/1.mobile/auto_switching.png
imageAlt: HQP logo
image-slider: /assets/img/project-images/1.mobile/auto_switching.png

---
### Overview
This is an ongoing project in order to address the recursive feasibility and stability of the MPC problem while parking maneuver.

### Algorithms and Results
<div class="row projects-display">
	<div class="six columns">
        <div class="video-container">
            <iframe width="560" height="315" src="https://www.youtube.com/watch?v=KJVo_7RSWbk" frameborder="0" allowfullscreen></iframe>
        </div>
	</div>
</div>
<div class="row projects-display">
	<div class="six columns">
		<h5> FABRIK based algorithm</h5>
		<li> We used Forward And Backward Reaching Inverse Kinematics (FABRIK) in order to calculate joint position.  </li>
		<li> To track my motion, I used VR device.</li>
		<li> See more <a href="{{site.url}}/UR2018"> UR2018</a> </li>
	</div>
	<div class="six columns">
        <div class="video-container">
            <iframe width="560" height="315" src="https://www.youtube.com/embed/PfxoOjAHuBw" frameborder="0" allowfullscreen></iframe>
        </div>
	</div>
</div>
<div class="row projects-display">
	<div class="six columns">
		<div class="images">
			<img alt="Awesome Check In" height="100" src="{{ site.url }}/assets/img/project-images/7.imitation/rnn.png">
		</div>
	</div>
	<div class="six columns">
		<h5> Recurrent Neural Network based algorithm</h5>
		<li> We used Recurrent Neural Network in order to train the human motion.  </li>
		<li> We validated it in robotic simulator, V-REP. </li>
		<li> See more <a href="{{site.url}}/URAI2016"> URAI2016</a> </li> 
	</div>
</div>

