---
layout: page
title: Drone Testing Rig
description: Roll-Pitch-Yaw Gimbal
img: assets/img/Projects/Testingapparatus/TestingApparatus.png
importance: 2
category: Graduate Work
categories: sample-posts toc sidebar
giscus_comments: true
related_posts: false
toc:
  sidebar: lefts
---

<h4 id="motivation" style="text-align: center;">Motivation</h4>
This gimbal was developed to serve as a platform for evaluating the stability and to perform testing in a safe manner on experimental drones. Particularly, stability in roll, pitch, and yaw were of primary concern. In addition to evaluating the stability of the drone, the apparatus was also configured for performing and validating system identification on the drone. 

<image src="assets/img/Projects/Testingapparatus/youtube-video-gif.gif" alt="crash" width="450" /> 

<h4 id="contributions" style="text-align: center;">Project Contributions & Overview</h4>

<div class="row justify-content-sm-center">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/Projects/Testingapparatus/TestingApparatus.png" title="Testing Apparatus" class="img-fluid rounded z-depth-1" %}
    </div>
    <img src="https://media.giphy.com/media/v1.Y2lkPTc5MGI3NjExMWZlMzQ1NGRlNTJjOWYwODY3ZjlmODI3ZjQ3YzNjOThiNGM1NmQzNyZlcD12MV9pbnRlcm5hbF9naWZzX2dpZklkJmN0PWc/SEwIQnjGOhuSpIEuQz/giphy.gif" width="270" height="480" />
</div>
<div class="caption">
    CAD rendering of the designed drone testing rig for evaluating stability in roll, pitch, and yaw (left), 
</div>

The primary contribution of this work was an open-source design of the gimbal system shown above. The files can be found here: [Link to Github](). 

<h5 id="bearingdesign" style="text-align: center;">Bearing Joint Design</h5>

One of the primary challenges in designing the testing rig was to reduce the friction in the gimbal and to ensure that the forces from the drone on the testing rig are adequately transferred between joints. To achieve low friction and adequate transfer, the following joint design was used:

<div class="d-flex justify-content-center">
    <div class="col-sm mt-7 mt-md-0">
        {% include figure.html path="assets/img/Projects/Testingapparatus/bearing.png" title="bearing_design" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
   Cross section of the bearing joints used in the design
</div>

As shown in the image, two 3D printed casings were used to inclose a [rotary thrust bearing](#TODO FIX LINK) that utilizes a bolt to transfer load between the two links in a low friction way. 

<h5 id="upgrades" style="text-align: center;">Proposed Upgrades</h5>
1. Reduce inertia of the linkages by using a lighter weight material or different construction
2. Explore different configurations for improving the space usage