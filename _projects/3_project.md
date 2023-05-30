---
layout: page
title: Untethered Pneumatic Actuation
description: Evaluation of electrolysis of water as a method for untethered pneumatic actuation
img: assets/img/Projects/Electrolysis/theory.png
importance: 3
category: Graduate Work
---

<h4 id="overview" style="text-align: center;">Motivation</h4>

Pneumatically actuated soft robots offer advantages such as safe human-robot interactions, adaptability to dynamic environments, lightweight construction, high power output, smooth motion, and environmentally friendly actuation. However, the traditional reliance on heavy, noisy, tethered, and inefficient air compressors has been a drawback. To address this, researchers have explored various untethered methods for pneumatic actuation. 

<h4 id="contributions" style="text-align: center;">Project Contributions</h4>
1. Analysis of the theoretical performance of a PEM electrolyzer to pressurize gas, perform work, and recover energy from the generated hydrogen gas
2. Experimental determination and comparison of the actuation performance (i.e., flow rate, maximum pressurization, and efficiency) with state-of-the-art methods for achieving untethered pneumatic actuation
3. Analysis of the compatibility of hydrogen gas with an existing off the shelf pneumatic actuator, namely the McKibben actuator due to its popularity

<h4 id="overview" style="text-align: center;">Project Overview</h4>

<div class="d-flex justify-content-center">
    <div class="col-sm-7 mt-7 mt-md-0">
        {% include figure.html path="assets/img/Projects/Electrolysis/overview.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Overview of the working principle for reversible water electrolysis using a proton exchange membrane to generate pneumatic actuation. The electrolysis operation (a) applies a voltage across the membrane that splits the water into hydrogen and oxygen gas, which can be used to inflate a pneumatic actuator. Fuel cell operation (b) applies a resistive load across the membrane, which then converts the hydrogen and oxygen gas back into water and thereby deflates the pneumatic actuator.
</div>

This work focuses on evaluating a proton exchange membrane (PEM) electrolyzer as an untethered pneumatic actuation method. By utilizing hydrogen as an intermediate, electrolysis offers the potential for improved efficiency through energy recovery. Experimental tests were conducted to assess the performance and compatibility of different pneumatic generation methods. The PEM electrolyzer outperformed other untethered actuation methods, achieving a maximum pressure of **0.75 MPa** gauge and a flow rate of **0.06 L/min** (STP). While the experimental efficiencies were modest at **0.005%**, theoretical calculations suggest that efficiencies of **up to 2%** are achievable with modern hardware.

<h4 id="moi" style="text-align: center;">Metrics of Interest</h4>
The chosen metrics, maximum pressure, flow rate, efficiency, and permeability, are by no means exhaustive. Rather, they are meant to provide insight into the range of applications where PEM driven pneumatic actuation may be used in place of other methods. 

1. Maximum Pressure: Maximum achievable pressure determines the maximum output force and/or displacement a pneumatic source can achieve in a given actuator. For the purposes of exploring compatibility with existing pneumatic actuators, the maximum possible pressure was the maximum operating pressure of the chosen actuator.
2. Flow Rate: Flow rate provides insight into the maximum bandwidth for an accompanying pneumatic actuator and/or the rate at which a pressurized reservoir can be filled. It is a crucial metric for understanding how quickly an arbitrary actuator can operate.
3. Efficiency: Efficiency is a measure of how well energy is converted from one form to another
   * Theoretical vs. Practical Efficiency

        **Theoretical Efficiency** 
        : The thermodynamic maximum efficiency of a system

        **Practical Efficiency** 
        : The efficiency calculated directly from experimental data 

   * First vs. Second Law Efficiency

        **First Law Efficiency** 
        : The ratio between usable energy flowing out of the system and into the system

        **Second Law Efficiency** 
        : The normalization of first law efficiency 

4. Permeability: qualitative metric for measuring the compatibility of a pressurized media with an actuator. If the pneumatic actuator is permeable to the pressurized media, further losses will be introduced into the system that ultimately reduce the round-trip efficiency. Permeability is indirectly measured through comparing the possible actuator cycles from a given pressure and volume of gas.

<h4 id="methods" style="text-align: center;">Theory</h4>

<div class="d-flex justify-content-center">
    <div class="col-sm-6 mt-7 mt-md-0">
        {% include figure.html path="assets/img/Projects/Electrolysis/theory.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Effect of variable electrolyzer and fuel cell efficiencies on the overall round-trip mechanical efficiency at 1 MPa absolute when actuator efficiency is unity.
</div>



<h4 id="methods" style="text-align: center;">Experimental Methods</h4>

<div class="d-flex justify-content-center">
    <div class="col-sm mt-7 mt-md-0">
        {% include figure.html path="assets/img/Projects/Electrolysis/expdesign.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Overview of the components forming the experimental framework for evaluating the performance and compatibility of (a) the PEM electrolyzer and (b) the standard air compressor system. The framework consists of five systems: energy monitor, generator, pneumatic sensors, actuator, and storage. The energy monitoring subsystem measure the electrical energy flowing through the system. The pneumatic sensors subsystem measures the pressure and flow rate of the pressurized media. The actuator subsystem performs mechanical work by using the pressurized media to elongate a spring using a McKibben actuator and then measures the mechanical work using a linear variable differential transducer (LVDT) and load cell. The storage subsystem provides a means for temporarily storing pressurized media that can later be used to drive the pneumatic actuator (PAM).
</div>

<h4 id="results" style="text-align: center;">Results</h4>

<h4 id="publication" style="text-align: center;">Associated Publication</h4>