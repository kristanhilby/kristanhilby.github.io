---
layout: page
title: Instrumented Door and Drawer for Robot Grasp Evaluation
description: Oregon State University
img: assets/img/Projects/instrumenteddoordrawer/overview.png
importance: 2
category: Undergraduate Work
categories: sample-posts toc sidebar
giscus_comments: true
related_posts: false
toc:
  sidebar: left
---

<h4 id="overview" style="text-align: center;">Motivation</h4>
Accessible and comprehensive datasets that encompass a range of robot hands can significantly contribute to researchers' knowledge and evaluation of optimal robot hands for specific tasks. While previous approaches involved integrating sensors into robot hands to gather real-time information on robot-object interactions during grasping, this method is not conducive and consistent data collection across various robot hands. 

<h4 id="overview" style="text-align: center;">Project Overview</h4>
We instrumented a door and drawer, ordinary objects found in everyday life, to gather kinematic data and measure force interactions during grasping. This approach can be applied to different hand designs, making it highly versatile. Through our implementation, we successfully generated comprehensive datasets using the instrumented objects. The simplicity of constructing the proposed instrumented door and drawer allows other research laboratories to easily replicate the method. Furthermore, their modular design facilitates large-scale data collection, enabling researchers to optimize robot grasping techniques for real-world scenarios.

<h4 id="contribution" style="text-align: center;">Project Contributions</h4>
<div class="d-flex justify-content-center">
    <div class="col-sm-7 mt-7 mt-md-0">
        {% include figure.html path="assets/img/Projects/instrumenteddoordrawer/door.png" title="door" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Instrumented door used for generating grasp dataset of a puppeteered, un-actuated OpenHand Model O
</div>

<div class="d-flex justify-content-center">
    <div class="col-sm-7 mt-7 mt-md-0">
        {% include figure.html path="assets/img/Projects/instrumenteddoordrawer/drawer.png" title="drawer" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Instrumented drawer used for generating grasp dataset of a puppeteered, un-actuated OpenHand Model O  
</div>
The primary contributions of this work were: 
1. An door and drawer instrumented with force sensitive resistors along 12 locations of the handle to provide both spatial and qualitative data on the grasp,
2. The instrumented handle included a silicone 3D printed skin to facilitate force distribution across the handle
3. A door instrumented with a load plate behind the handle to determine force exerted during opening
4. An hinge with a potentiometer to determine opening rate 

<h4 id="results" style="text-align: center;">Results</h4>

##### Door
Data from both successful and unsuccessful trials on the door ran with a puppeteered, un-actuated OpenHand Model O are provided in the image below. Force is quantified across the handle with green, yellow, and red equating to low, medium, and high force respectively. Qualitatively, the successful grasp makes contact fully around the handle, where the unsuccessful grasp does not apply force to the back of the handle. The grasp success is justified through the angular position data, where the failed grasp does not make it to the fully open 75 degree angle. 

<div class="d-flex justify-content-center">
    <div class="col-sm-9 mt-7 mt-md-0">
        {% include figure.html path="assets/img/Projects/instrumenteddoordrawer/door_results.png" title="door_res" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Results from puppeteered instrumented door tests.
</div>

##### Drawer
Similarly, data from both successful and unsuccessful trials on the drawer ran with a puppeteered, un-actuated OpenHand Model O are provided in the image below. Similar to the door, force is quantified across the handle with green, yellow, and red equating to low, medium, and high force respectively. Qualitatively, the successful grasp makes contact fully around and across the handle, where the unsuccessful grasp fails to apply force to the center of the handle. In the failed grasp case, the hand is able to open the drawer fully, but loses contact before it can close it. 

<div class="d-flex justify-content-center">
    <div class="col-sm mt-7 mt-md-0">
        {% include figure.html path="assets/img/Projects/instrumenteddoordrawer/drawer_results.png" title="door_res" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Results from puppeteered instrumented drawer tests.
</div>

<h4 id="citations" style="text-align: center;">Relevant Citations</h4>
{% reference CitekeyMisc %}