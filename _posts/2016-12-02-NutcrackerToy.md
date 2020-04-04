---
layout: post
title: "Designing Automaton Nutcracker"
sub_title: "a"
categories:
  - Projects
tags:
- Product Design
- Kinematics and Dynamics
- Robotics
last_modified_at: 2016-12-02 
---

1. [Introduction](#1)
2. [Analysis of Original Design](#2)
    1. [Loop Analysis](#2a)
3. [Creation and Design of the New Design](#3)
    1. [Acceleration and Force Calculations](#3a)
    
    
## Introduction <a name="1"></a>
This was for the UofT course course MIE301: Kinematics and Dynamic of Machines. I worked in a team of 5 with Dahlia Milevsky, Julia Filiplic, Romaissa Allalou and Yiran Lu. 

The project Goal was to, essentially, redesign a mechanism to have more complex kinematics. It should take a product and ideally improve it. As a result, we had near complete freedom on what to do and remake - and thus, part of the project involved creating a client, their request and how we would address it professionally (i.e. reports). 

Our team decided to combine the nutcracker and an automaton toy, and make the movement to be more humanlike.

<p>&nbsp;</p> 

## Analysis of Original Design <a name="2"></a>

![img](/images/projects/nutcracker/og_design.PNG "The Automaton Toy Ee Combined with the Classic Nutcracker"){:width="600"}

| Kinematic Diagram | With Loops for Analysis|
|:-----------------:|:-----------------------|
| ![img](/images/projects/nutcracker/og_design_kd.PNG "Simplified KD"){:width="600"} | ![img](/images/projects/nutcracker/og_design_kd_eqtn.PNG "KD with Loops"){:width="600"} |

Loop analysis allows the output position, velocity and acceleration to be calculated and traced. As seen in Figure 4, the maximum values of R11 and  R12 is the position where the flogger hits the dead horse. The velocity of point G, and several acceleration formulas are needed to calculate the original force output of the mechanism for point G. 

### Loop Analysis <a name="2a"></a>

{::options parse_block_html="true" /} 

<details>
  
  <summary markdown="span">Click to see Loop Analysis Details!</summary>
  
  | rAC2 = 2.8cm <br>rBD = 17.6cm <br>rFG = 18.6cm <br>rO3_B = 4.8cm <br>rAB = 12.4cm <br>rDE = 13.2cm | rEG = 21.8cm <br>rO5_FB = 8.89cm <br>rBC3= 12.7cm <br>rEF = 3.0cm <br>rO2_A = 4.8cm <br> rO2_O5 = 9.4cm ĵ +0.5cm î |
  |:-----------------:|:---------------------:|
  | ![img](/images/projects/nutcracker/og_loopAnalysis1.PNG "Simplified KD"){:width="375"} | ![img](/images/projects/nutcracker/og_loopAnalysis2.PNG "Simplified KD"){:width="320"} |
  | ![img](/images/projects/nutcracker/og_loopAnalysis3.PNG "Simplified KD"){:width="350"} | ![img](/images/projects/nutcracker/og_loopAnalysis4.PNG "Simplified KD"){:width="310"} |
  
</details>

{::options parse_block_html="false" /}

<p>&nbsp;</p> 

## Creation and Design of the New Design <a name="3"></a>

| Simplified Kinematic Diagram <br> of the New Design | Kinematic Model from Simulation |
|:---:|:---:|
| ![img](/images/projects/nutcracker/final_design_kd.PNG "Simplified KD"){:width="400"} | ![img](/images/projects/nutcracker/final_design_kd_eqtn.PNG "Simplified KD"){:width="400"} |


### Acceleration and Force Calculations <a name="3a"></a>

|Graph showing composite accelerations and magnitude | |
|:---:|:---:|
|![img](/images/projects/nutcracker/accel_graph.PNG "Composite Accelerations"){:width="500"} | Blue shows the greatest acceleration <br>along the x-axis, orange the y-axis. <br>Grey shows the magnitude of the acceleration.|
| **Graph showing only the magnitude** | |
|![img](/images/projects/nutcracker/accel_graph_mag_only.PNG "Acceleration Magnitude"){:width="500"} | The greatest is 0.938m/s^2 at -3rad, <br>or at about 3.14secs into <br> movement with an input of 10rpm.|
| **Kinematic model at point of greatest acceleration** |  |
|![img](/images/projects/nutcracker/greatest_accl_neg2-9rad.PNG "Simulation Paused at Greatest Acceleration"){:width="500"}|  This is at -3rad or 3.14 secs. <br>The Yellow line shows the magnitide and <br>points the eopposite direction of the acceleration.| 

Thus, with the acceleration known, all we need is mass to gain the force required. With research we found walnuts would reliable crack at 400Pa. We assumed the surface of the hammer is 1cm^2.

P = F/m^2 => F = P x m^2 = 400 x 0.01 x 0.01 = 0.04N

F = ma    =>    m = F/a     =>    m = 0.04/0.938 = 0.0426kg = 42.6g

| Showing how human toy would be placed and attached to linkages |
|:--:|
|![img](/images/projects/nutcracker/final_design_placement.PNG "With Human"){:width="450"} |

<p>&nbsp;</p> 

[Link to modeling program](https://designengrlab.github.io/PMKS/pmks.html?mech=ground,2,R,0.000,0.000,0.000,ttft%7C2,3,R,-30.000,0.000,0.000,ffff%7C3,4,R,100.000,150.000,0.000,ffff%7C4,ground,R,100.000,0.000,0.000,ffff%7C2,5,R,-30.000,30.000,0.000,ffff%7C5,4,RP,100.000,200.000,90.000,ffff%7C5,6,R,0.000,68.000,0.000,ffff%7C6,7,R,-30.000,68.000,0.000,ffff%7C8,4,R,100.000,250.000,25.000,ffff%7C6,ground,RP,-55.000,48.000,45.000,tfff%7C7,8,R,-30.000,200.000,0.000,ffff%7C8,R,350.000,150.000,0.000,ffff%7C )

Note: you need silverlight. Currently also seems to not work for me, even with silverlight. Will need to see if anything can be done for that...

[comment]: # ( https://docs.google.com/document/d/11p94HGvVMrtGJnBlE4-7jnZ_2klZ_HOIyMy73pJye-A/edit )
[comment]: # ( https://docs.google.com/document/d/1fPsFOBVk9J_k5i0bj0PYX3kzWta-xdNT7pqmTRZ0BbE/edit )

<p>&nbsp;</p> 

## Notes
A fair amount of the writing was summarized and all the diagrams were pulled from our reports, credit to my teammates.

This page to be incomplete, but sufficient. More details and edits to be added in time.
