---
layout: post
title: "Controlled Motorized Pendulum"
sub_title: "a"
categories:
  - Projects
tags:
- Projects
last_modified_at: 2018-12-05
---

# Controlling the Angle of a Motorized Pendulum

1. [Introduction](#1)
2. [Construction](#2)
    1. [Set up and Wiring Diagram](#2a)
    2. [Code](#2b)
3. [Results](#3)
    1. [Step Response](#3a)
    2. [Displacement Correction](#3b)
    3. [Sine Wave](#3c)

<p>&nbsp;</p> 

## Introduction <a name="1"></a>

I worked on a team of four, with Adrian Cheung, Kyle McCarroll, and Nebojsa Jovanovic to build and program a motorized pendulum. 
The goal was to control the angle of the pendulum with using the rotor, motor controller, rotary encoder and Arduino. 
It had to return to the set angle when displaced near immediately.

My responsibilies were:
- to cut and set up the pendulum
- connect and solder the wires
- most of the tuning with Kyle, but Adrian and Nebojsa also spent many hours with us
Other fixed several issues with our wire connections,  took videos and pictures, and wrote most the report.

<p>&nbsp;</p> 

## Construction <a name="2"></a>

### Set up and Wiring Diagram <a name="2a"></a>

The pendulum’s angle is measured by the rotary encoder as the pendulum rotates about the shaft. The motor is connected to a motor controller (ESC) and through it the motor is powered with 12V and 6.4A. The Arduino receives a signal from the encoder, determines a new motor speed based on a PID control logic, and sends a signal to the ESC to control the motor.

![img](/images/projects/pendulum/physicle_layout_wiringD.PNG "Set up"){:height="400"} 

### Majority of Code <a name="2b"></a>

{::options parse_block_html="true" /}

<details>
  <summary markdown="span">Click to see code!</summary>
  
  ''' 
  add later
  '''
  
</details>

{::options parse_block_html="false" /}

<p>&nbsp;</p> 

## Results <a name="3"></a>

### Step Response <a name="3a"></a>

![img](/images/projects/pendulum/step_response.PNG "Step Response graphed from Arduino software"){:height="400"} 

### Displacement Correction <a name="3b"></a>

![img](/images/projects/pendulum/disturbance_response.PNG "Returns to Set of 30 Degrees"){:height="400"} 

|<figure class="video_container"><video controls="true" allowfullscreen="true" height="300"><source src="/images/projects/pendulum/static_and_return.mp4" type="video/mp4"></video></figure> |
<figure class="video_container"><video controls="true" allowfullscreen="true" height="300"><source src="/images/projects/pendulum/static_and_return2.mp4" type="video/mp4"></video></figure> |

### Sine Wave <a name="3c"></a>

| ![img](/images/projects/pendulum/sin_response.PNG "Step Response graphed from Arduino software"){:height="300"} 
| <figure class="video_container"><video controls="true" allowfullscreen="true" height="300"><source src="/images/projects/pendulum/sin_graphed.mp4" type="video/mp4"></video></figure> |

<p>&nbsp;</p> 

## NOTES:
under construction!


