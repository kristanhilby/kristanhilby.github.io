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

<h4 id="contributions" style="text-align: center;">Notation & Constants</h4>
The following notation and constants are used in describing this project:


<h4 id="methods" style="text-align: center;">Theory</h4>

The theoretical efficiency for PEM driven pneumatic actuation required the theoretical evaluation of several values. Namely, the electrical energy into the system to drive electrolysis, the electrical energy out of the system from fuel cell operation, and the mechanical work out of the system due to pressurization of the generated gasses. In other words, the theoretical round trip efficiency (i.e., from electrical energy to mechanical work) is defined as the following first law efficiency:

<div class="d-flex justify-content-center">
    <div class="col-sm-5 mt-7 mt-md-0">
        {% include figure.html path="assets/img/Projects/Electrolysis/rt_efficiency.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Equation for calculating the round trip efficiency. 
</div>

###### Electrical Energy In
The maximum round trip efficiency will occur when the electrical energy into the system is minimized. As such, the minimum electrical energy required to pressurized a hydrogen reservoir can be found by evaluating the total change in Gibbs free energy of the system. The total change in Gibbs free energy of the system can be found by integrating a differential change in the Gibbs free energy. Performing the integration yields the following result:

<div class="d-flex justify-content-center">
    <div class="col-sm-5 mt-7 mt-md-0">
        {% include figure.html path="assets/img/Projects/Electrolysis/gibbsfree.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Resulting change in Gibbs free energy after integrating a differential change. 
</div>

Two observations can be made about the Gibbs free energy equation:
1. The first term can be thought of as the inherent energy penalty of performing the chemical reaction
2. The second term can be thought of as the enrgy contribution for pressurizing a gas

###### Electrical Energy Out
The maximum round trip efficiency will occur when the electrical energy out of the fuel cell is maximized. Therefore, the maximum energy that can be recovered from a fuel cell is simply the number of moles of gas, multiplied by the gibbs free energy of the fuel cell reaction. 

###### Mechanical Work Out
Finally, the maximum round trip efficiency will occur when the mechanical work out of the system is maximized. Assuming isentropic expansion of the stored gas from the compressed state _(T, p)_ to ambient pressure _p0_ yields the following maximum work:

<div class="d-flex justify-content-center">
    <div class="col-sm-6 mt-7 mt-md-0">
        {% include figure.html path="assets/img/Projects/Electrolysis/workmax.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Maximum work from an isentropic expansion of a pressurized gas.
</div>

###### Maximum Round Trip Efficiency

Populating the efficiency equation with the derived values, and simplifying, yields the following equation for maximum round trip efficiency: 

<div class="d-flex justify-content-center">
    <div class="col-sm-6 mt-7 mt-md-0">
        {% include figure.html path="assets/img/Projects/Electrolysis/rt_efficiency_max.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Effect of variable electrolyzer and fuel cell efficiencies on the overall round-trip mechanical efficiency at 1 MPa absolute when actuator efficiency is unity.
</div>

Two non-dimensional groups determine the maximum theoretical efficiency:
1. The gamma contribution: Dictated by the gas being pressurized
2. The pressure contribution

Therefore, for the PEM system, the maximum round trip efficency is purely a function of the pressure. Graphing up to 1 MPa, the typical range of interest for soft robots, yields the following result:

<div class="d-flex justify-content-center">
    <div class="col-sm-6 mt-7 mt-md-0">
        {% include figure.html path="assets/img/Projects/Electrolysis/rt_efficiency_max_graph.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Maximum round trip efficiency. 
</div>

###### Practical Round Trip Efficiency
Adding efficiency metrics to all of the above values provides the following relationship between the efficiency of the electrolyzer and fuel cell on the round trip efficiency at 1 MPa (assuming an efficiency of unity for the actuator)

<div class="d-flex justify-content-center">
    <div class="col-sm-6 mt-7 mt-md-0">
        {% include figure.html path="assets/img/Projects/Electrolysis/theory.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Effect of variable electrolyzer and fuel cell efficiencies on the overall round-trip mechanical efficiency at 1 MPa absolute when actuator efficiency is unity.
</div>

A few observations should be noted:
1. Without a fuel cell, the system will never be greater than 1% efficient,
2. To be greater than 10% efficient, the fuel cell system needs to be operating in the > 75% efficiency range, 
3. State of the art electrolyzers and fuel cells would be able to achieve 2.06% efficiency. 

<h4 id="methods" style="text-align: center;">Experimental Methods & Results</h4>

<div class="d-flex justify-content-center">
    <div class="col-sm mt-7 mt-md-0">
        {% include figure.html path="assets/img/Projects/Electrolysis/expdesign.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Overview of the components forming the experimental framework for evaluating the performance and compatibility of (a) the PEM electrolyzer and (b) the standard air compressor system. The framework consists of five systems: energy monitor, generator, pneumatic sensors, actuator, and storage. The energy monitoring subsystem measure the electrical energy flowing through the system. The pneumatic sensors subsystem measures the pressure and flow rate of the pressurized media. The actuator subsystem performs mechanical work by using the pressurized media to elongate a spring using a McKibben actuator and then measures the mechanical work using a linear variable differential transducer (LVDT) and load cell. The storage subsystem provides a means for temporarily storing pressurized media that can later be used to drive the pneumatic actuator (PAM).
</div>

Using the above experimental design, it was determined that the PEM system could produce gas at 0.06 L/min up to 0.75 MPa, but at 0.005% efficiency. The efficiency of the electrolyzer was experimentally calculated to be 53% efficient (second law), while the fuel cell was determined to be 9.6% efficient (second law). Strikingly, the actuator was calculated to be only 0.8% efficient. 

Overall, it was calculated that approximately 12.5% of the hydrogen leaked from the McKibben fiber. 

<h4 id="publication" style="text-align: center;">Relevant Citations</h4>