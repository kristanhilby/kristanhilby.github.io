---
layout: page
title: Morphing Airfoil/Wing
description: Reversible morphing airfoil
img: assets/img/Projects/MorphingAirfoil/systemrendering.png
importance: 2
category: PhD Work
categories: sample-posts toc sidebar
giscus_comments: true
related_posts: false
toc:
  sidebar: left
---

<h4 id="motivation" style="text-align: center;">Motivation</h4>
Morphing airfoils, which possess the ability to change shape during flight, offer the potential to improve the performance envelope and potentially extend the optimal aerodynamic performance of an aircraft across a wider range of flight conditions. This becomes increasingly important when applications require optimal efficiency across all flight regimes, operate across a wider range of speeds or environments, or require a large degree of maneuverability. Traditionally, morphing airfoils have been broken down into two classes: camber morphing and thickness adjusting. Camber morphing, shown below, changes the camber line of the airfoil, which can lead oto increased aerodynamic efficiency by delaying boundary layer separation. 

<div class="d-flex justify-content-center">
    <div class="col-sm mt-7 mt-md-0">
        {% include figure.html path="assets/img/Projects/MorphingAirfoil/cambermorphing.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Pictoral example of camber morphing of an airfoil, with initial airfoil configuration shown on the top, and the camber morphed version on the bottom. 
</div>

While camber morphing is more common, thickness morphing, which changes the overall thickness of an airfoil while keeping the camber constant, has been shown to change the laminar separation bubble and traling edge flow separation characteristics, providing the potential to incraese wing efficiency (i.e., L/D ratio) and decrease the viscous drag on the wing. The following is an example of a thickness morphing airfoil:

<div class="d-flex justify-content-center">
    <div class="col-sm mt-7 mt-md-0">
        {% include figure.html path="assets/img/Projects/MorphingAirfoil/thicknessmorphing.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Pictoral example of thickness morphing of an airfoil. 
</div>

While exploring stop-rotor aircraft designs, one issue that emerged (which is described in further detail on the [Stop-Rotor Aircraft Page]()) is the conflicting airfoil directionality between vertical take off and langing (VTOL) and forward flight modes, as shown here:

<div class="d-flex justify-content-center">
    <div class="col-sm mt-7 mt-md-0">
        {% include figure.html path="assets/img/Projects/MorphingAirfoil/airfoil_directionality.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Necessary airfoil directionality between Stop-Rotor aircraft modes depicted by the blue line 
</div>

The conflicting airfoil directionality necessitated the emergence of a new type of morphing airfoil -- the reversible morphing airfoil, which reverses the direction of the leading and trailing edge, as shown here:

<div class="d-flex justify-content-center">
    <div class="col-sm mt-7 mt-md-0">
        {% include figure.html path="assets/img/Projects/MorphingAirfoil/reversiblemorphing.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Pictoral example of proposed reversible airfoil class
</div>

<h4 id="contributions" style="text-align: center;">Project Contributions</h4>

1. Design of a novel reversible morphing airfoil
2. Evaluation of the airfoil strength under modeled aerodynamic forces
3. Determination of the maximum aerodyanmic force

<div class="d-flex justify-content-center">
    <div class="col-sm mt-7 mt-md-0">
        {% include figure.html path="assets/img/Projects/MorphingAirfoil/systemrendering.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Rendering of the proposed reversible airfoil mechanism. 
</div>

<h4 id="design" style="text-align: center;">Morphing Airfoil Design</h4>

The design of the morphing airfoil can be broken down into three components:

###### Flexible Strip
The flexible strip element was inspired by the roll up chair designed by Uros Vitas. The leading edge shape is formed when adjacent quadrilateral sections contact one anothe, while the trailing edge shape is formed by the flexible strip coming into contact with the base assembly. The flexible strip element is further composed of a rigid section and a flexible section, which gives the desireable flexibility where needed, but also provides needed rigidity. 

<div class="d-flex justify-content-center">
    <div class="col-sm mt-7 mt-md-0">
        {% include figure.html path="assets/img/Projects/MorphingAirfoil/flexiblestrip.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Flexible strip segment of the reversible morphing airfoil. 
</div>

###### Transmission Mechanism
The actuation component serves to transmit force from an electric motor to the flexible strip, as well as transmit aerodynamic loads from the flexible strip back to the base. The motor was chosen to be non-backdriveable, meaning motion can only be transmitted from the input to the output, to ensure that energy is not being expended to hold the system in the transformed state. 

<div class="d-flex justify-content-center">
    <div class="col-sm-9 mt-7 mt-md-0">
        {% include figure.html path="assets/img/Projects/MorphingAirfoil/transmissionmechanism.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Transmission mechanism of the reversible morphing airfoil. 
</div>

###### Base Mount
The base of the morphing airfoil serves to hold together the flexible strip and actuation components, as well as form the shape of and provide structure to the trailing edge. 

<div class="d-flex justify-content-center">
    <div class="col-sm mt-7 mt-md-0">
        {% include figure.html path="assets/img/Projects/MorphingAirfoil/baseassembly.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
   Base assembly of the reversible morphing airfoil. 
</div>

<h4 id="moi" style="text-align: center;">Experimental Characterization</h4>

<div class="d-flex justify-content-center">
    <div class="col-sm mt-7 mt-md-0">
        {% include figure.html path="assets/img/Projects/MorphingAirfoil/experimentalcharacterization.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
   Experimental setup to measure the maximum aerodynamic loads 
</div>

Experimental characterization yielded the determination that the maximum load each rib can withstand in compression is 150 N and after 1,000 cycles, minimal force softening is exhibited. 

<h4 id="citation" style="text-align: center;">Relevant Citations</h4>

{% reference Hilby2023 %}