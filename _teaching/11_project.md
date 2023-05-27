---
layout: page
title: MICA Initiative
description: Measurement Instrumentation Control and Analysis
img: assets/img/1.jpg
importance: 3
category: Prior Teaching Experience
---

### Description
> "MICA is an educational initiative that aims to bring low-cost, wireless sensors, generators and desktop robots into the hands of students. MICA focuses on hands-on, data-driven STEM education. Sophisticated enough for research, simple enough for kindergarten. 
> 
> The MICA Education Initiative aims to empower students of all ages by providing hands-on, data-driven STEM learning experiences. We harness the power of technology to improve student learning based on three core ideas. First, students are most engaged with their learning when they have a deep motivation for why a task is relevant. Second, "learning by doing" produces a much deeper and robust understanding than "learning by listening". Finally, measurement and quantification of physical phenomenon are essential for understanding how the world works.
>
>MICA is an ecosystem of hardware, software, and curriculum. The technology is low-cost and easy to use but powerful and accurate for laboratory research. By leveraging miniaturized sensing technologies, economies of scale, advanced communication protocols, and world-class content, MICA makes quantification approachable and accessible to all." 
>
>[Bilab Website](https://bioinstrumentation.mit.edu/mica.html)

The MICA initiative consists of a standardized framework of instrumentation designed to enable the experiential learning of various principles. MICA has been utilized in MIT's [2.131 Advanced Instrumentation and Measure]({% link _teaching/6_project.md %}) class, bringing students the opportunity to both learn from and develop the program. 

### Personal Contributions
I have personally worked to develop the following MICA setups:

<h4 style="text-align: center;">1. Reversible Proton Exchange Membrane (PEM) Fuel Cell</h4>

<div class="d-flex justify-content-center">
    <div class="col-sm-4 mt-3 mt-md-0">
        {% include figure.html path="assets/img/MICA/revfc_render.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Photorealistic rendering of the developed MICA Reversible PEM Fuel Cell apparatus.
</div>

##### Working Principle

This apparatus includes a PEM that utilizes the following electrolysis reaction to use electricity to turn liquid water into hydrogen and oxygen gas:

<div class="d-flex justify-content-center">
    <div class="col-sm-4 mt-3 mt-md-0">
        {% include figure.html path="assets/img/MICA/electrolysis.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Water splitting reaction.
</div>

Once the voltage source is removed, the membrane will spontaneously perform the reverse of the previous reaction, turning hydrogen and oxygen gas into liquid water, while generating electricity. 

##### Apparatus Instrumentation

The developed apparatus is capable of performing both the forward electrolysis reaction, as well as the reverse fuel cell reaction using a [Quattro Electrolyzer](https://www.google.com/search?client=safari&rls=en&q=fuel+cell+store+quattro+electrolyzer&ie=UTF-8&oe=UTF-8). During operation, the electrical energy flow is observed and recorded using the [Tinkerforge Voltage/Current Bricklet 2.0](https://www.google.com/search?client=safari&rls=en&q=tinkerforge+voltage+current+2.0&ie=UTF-8&oe=UTF-8). A load is applied with a variable potentiometer. 

The apparatus is also equipped with a [Tinkerforge DC Brick](https://www.tinkerforge.com/en/doc/Hardware/Bricks/DC_Brick.html) for sending a variable DC signal to the electrolyzer. A [Digilent Analog Discover 2](https://www.googleadservices.com/pagead/aclk?sa=L&ai=DChcSEwjH5aXF75X_AhVb9OMHHWYoDtsYABARGgJ5bQ&ae=2&ohost=www.google.com&cid=CAESbOD2vrzUaQhsF1LI97cH3NzLZ00TRgDf413_UGx2yuKOYqv2oOC2RxBV62hCKHWS2-wjjPG582V6Kj-GMPOhGqBKx9OMbVw2NPa8ahJk9YkCdoO6Yq0MoCWDDh8Kv6UDTCLTpymtQ9tmXgrYpw&sig=AOD64_3yuIZFT9PVdJKlqDgUBjBc8W9N-w&q&adurl&ved=2ahUKEwjn9JbF75X_AhWJKlkFHbfVCxEQ0Qx6BAgHEAM&nis=2&dct=1) is incorporated to generate a binary stochastic signal. Once tests are complete, efficiency and polarization plots are generated for the experiment. The binary stochastic signal is used to perform system identification on the polarization effects of the membrane. 

<h4 style="text-align: center;">2. Actuator Characterization</h4>


##### Working Principle

<h4 style="text-align: center;">3. Doppler Effects</h4>

##### Working Principle