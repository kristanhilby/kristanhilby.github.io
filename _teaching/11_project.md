---
layout: page
title: MICA Initiative
description: Measurement Instrumentation Control and Analysis
img: assets/img/MICA/revfc_render.png
importance: 3
category: Prior Teaching Experience
---

[Description](#descript_mica)

[Personal Contributions](#percont_2131)
* [PEM Reversible Fuel Cell](#mica_PEM)
* [Actuator Characterization](#mica_actuator)
* [Doppler Effect](#mica_doppler)
* [Cooking Methods](#mica_cooking)

<h4 id="descript_mica" style="text-align: center;"> Description</h4>

> "MICA is an educational initiative that aims to bring low-cost, wireless sensors, generators and desktop robots into the hands of students. MICA focuses on hands-on, data-driven STEM education. Sophisticated enough for research, simple enough for kindergarten. 
> 
> The MICA Education Initiative aims to empower students of all ages by providing hands-on, data-driven STEM learning experiences. We harness the power of technology to improve student learning based on three core ideas. First, students are most engaged with their learning when they have a deep motivation for why a task is relevant. Second, "learning by doing" produces a much deeper and robust understanding than "learning by listening". Finally, measurement and quantification of physical phenomenon are essential for understanding how the world works.
>
>MICA is an ecosystem of hardware, software, and curriculum. The technology is low-cost and easy to use but powerful and accurate for laboratory research. By leveraging miniaturized sensing technologies, economies of scale, advanced communication protocols, and world-class content, MICA makes quantification approachable and accessible to all." 
>
>[Bilab Website](https://bioinstrumentation.mit.edu/mica.html)

The MICA initiative encompasses a standardized framework of instrumentation crafted to facilitate experiential learning across a multitude of principles. Within the academic context, MICA has been successfully employed in the instructional setting of the esteemed [2.131 Advanced Instrumentation and Measure]({% link _teaching/6_project.md %}) course at MIT, thereby affording students the invaluable prospect of acquiring knowledge through active participation and concurrently contributing to the advancement of the program itself.

<h4 id="percont_2131" style="text-align: center;"> Personal Contributions</h4>

I have personally worked to develop the following MICA setups:

<h4 id="mica_PEM" style="text-align: center;">1. Reversible Proton Exchange Membrane (PEM) Fuel Cell</h4>

<div class="d-flex justify-content-center">
    <div class="col-sm-4 mt-3 mt-md-0">
        {% include figure.html path="assets/img/MICA/revfc_render.png" title="revfc_apparatus" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Photorealistic rendering of the developed MICA Reversible PEM Fuel Cell apparatus.
</div>

##### Working Principle

This apparatus includes a PEM that utilizes the following electrolysis reaction to use electricity to turn liquid water into hydrogen and oxygen gas:

<div class="d-flex justify-content-center">
    <div class="col-sm-4 mt-3 mt-md-0">
        {% include figure.html path="assets/img/MICA/electrolysis.png" title="electrolysis_reaction" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Water splitting reaction.
</div>

Once the voltage source is removed, the membrane will spontaneously perform the reverse of the previous reaction, turning hydrogen and oxygen gas into liquid water, while generating electricity. 

##### Apparatus Instrumentation

The developed apparatus demonstrates the capablity of a PEM to perform both the forward electrolysis reaction, as well as the reverse fuel cell reaction using a [Quattro Electrolyzer](https://www.google.com/search?client=safari&rls=en&q=fuel+cell+store+quattro+electrolyzer&ie=UTF-8&oe=UTF-8). Throughout operation, electrical energy flow is observed and recorded using the [Tinkerforge Voltage/Current Bricklet 2.0](https://www.google.com/search?client=safari&rls=en&q=tinkerforge+voltage+current+2.0&ie=UTF-8&oe=UTF-8). An electrical load is applied with a variable potentiometer. 

Furthermore, the apparatus incorporates a [Tinkerforge DC Brick](https://www.tinkerforge.com/en/doc/Hardware/Bricks/DC_Brick.html), which enables the application of a variable direct current (DC) signal to the electrolyzer. To impliment a binary stochastic signal with the Tinkerforge DC Brick, the [Digilent Analog Discover 2](https://www.googleadservices.com/pagead/aclk?sa=L&ai=DChcSEwjH5aXF75X_AhVb9OMHHWYoDtsYABARGgJ5bQ&ae=2&ohost=www.google.com&cid=CAESbOD2vrzUaQhsF1LI97cH3NzLZ00TRgDf413_UGx2yuKOYqv2oOC2RxBV62hCKHWS2-wjjPG582V6Kj-GMPOhGqBKx9OMbVw2NPa8ahJk9YkCdoO6Yq0MoCWDDh8Kv6UDTCLTpymtQ9tmXgrYpw&sig=AOD64_3yuIZFT9PVdJKlqDgUBjBc8W9N-w&q&adurl&ved=2ahUKEwjn9JbF75X_AhWJKlkFHbfVCxEQ0Qx6BAgHEAM&nis=2&dct=1) is included. Following the completion of the experimental tests, efficiency and polarization plots are generated to provide visual representations of the PEM's performance. Additionally, the binary stochastic signal is used to conduct system identification analysis on the polarization effects of the membrane. 

<h4 id="mica_actuator" style="text-align: center;">2. Actuator Characterization</h4>

##### Working Principle
Actuator characterization plays a crucial role in assessing the suitability of actuators for specific applications and serves as a fundamental step towards their widespread implementation. Traditionally, actuator tests have been classified into two categories: isotonic tests, which involve the actuator moving under tension, and isometric tests, where the actuator is held at a constant length. Isotonic tests focus on evaluating metrics such as elongation or contraction percentage, work density, power density, and bandwidth. Conversely, the main parameter of interest in isometric tests is the maximum force output achievable at a given displacement. These quantifiable parameters collectively provide designers with valuable insights into the compatibility of an actuator with their specific system, enabling them to make informed decisions regarding its appropriateness and functionality.

<div class="d-flex justify-content-center">
    <div class="col-sm-4 mt-3 mt-md-0">
        {% include figure.html path="assets/img/MICA/IMG_3989.jpg" title="actuator_characterization" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Actuator Characterization Apparatus.
</div>

##### Apparatus Instrumentation

The actuator characterization apparatus enables the execution of both isometric and isotonic testing methodologies. In isotonic tests, the apparatus employs a linear variable differential transformer (LVDT) to accurately measure the displacement of the actuator. Additionally, a load cell captures the force exerted by the actuator during the experiment. To monitor the energy consumption of the actuator throughout the testing process, an energy monitor is incorporated into the apparatus.

For isometric testing, the actuator is connected at one end of a linear actuator to regulate the length during the isometric tests. The other end of the linear actuator is linked to a load cell, which accurately measures the force output after the actuator has been activated. This comprehensive setup ensures precise measurements and data acquisition, enabling a thorough evaluation of the actuator's performance under both isometric and isotonic conditions.

<h4 id="mica_doppler" style="text-align: center;">3. Doppler Effects</h4>

##### Working Principle
Doppler shift, a fundamental concept in physics and wave phenomena, describes the alteration in the frequency or wavelength of a wave as observed by an observer in motion relative to the source of that wave. The Doppler effect manifests in everyday experiences, such as the change in pitch of a passing siren or the shifting colors of celestial objects. By understanding the principles of Doppler shift, scientists and researchers can extract valuable information about the velocity, direction, and properties of moving objects or phenomena. Doppler shift is characterized through the following equation: 

<div class="d-flex justify-content-center">
    <div class="col-sm-4 mt-3 mt-md-0">
        {% include figure.html path="assets/img/MICA/doppler.jpg" title="doppler_effect" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Doppler Effect Relationship.
</div>


##### Apparatus Instrumentation

<h4 id="mica_cooking" style="text-align: center;">4. Cooking Method Efficiency</h4>

##### Working Principle

Cooking efficiency plays a pivotal role in determining the overall cost of cooking, encompassing factors such as the time required to cook, energy expenditure, and even the health risks associated with the cook. Four main methods of cooking were identified: namely conduction, radiation, induction, and Joule heating. Conduction involves the transfer of heat through direct contact between the cooking vessel and the food. Radiation refers to the emission and absorption of electromagnetic waves, such as infrared radiation, by the food and cooking surfaces. Induction cooking utilizes magnetic fields to generate heat directly within the cookware, thus minimizing energy loss. Joule heating, on the other hand, involves the conversion of electrical energy into heat as it passes through the resistance of the cooking medium.

By conducting a comprehensive assessment of the efficiencies of these cooking methods, valuable insights can be gained regarding the optimal utilization of each technique. This knowledge empowers individuals to make informed decisions regarding time management, energy consumption, and the well-being of cooks. It allows for the selection of cooking methods that not only yield desirable culinary outcomes but also minimize resource usage, reduce cooking durations, and mitigate potential health hazards associated with certain cooking techniques.

<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
        {% include figure.html path="assets/img/MICA/2.131_testing_setup.jpg" title="cooking_apparatus" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-4 mt-3 mt-md-0">
        {% include figure.html path="assets/img/MICA/CAD_model.jpg" title="cooking_cad" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Overview of the developed cooking methods apparatus with (left) the real set up and (right) the CAD model
</div>

##### Apparatus Instrumentation
The apparatus for evaluating the different cooking techniques is comprised of four sample tubes, each equipped with a different method for cooking. In this apparatus, conduction heating is performed by directly contacting the test material with the heating element, which allows for direct heat flow from the heating element to the test material. Radiation heating is performed by  heating a coil at a distance from the test material, which then radiates out heatfor the test material to absorb. Induction heating is performed by running an electrical current through a coil around the material, generating heat in the material itself. Since foods generally do not contain a ferromagnetic material, an iron wire, which acts as the heated element, is inserted through the center of the sample. Joule heating is performed by running an electrical current directly through the material such that the material’s inherent resistance causes heat generation.

A linear stage and thermal camera are mounted behind the test samples to monitor the cooking rate and energy distribution over time. Efficiency is calculated by monitoring the electrical energy going into operating the heating mechanism and comparing to the theoretical value of energy needed to cook the sample. The cooking process was monitored using impedance analysis. 