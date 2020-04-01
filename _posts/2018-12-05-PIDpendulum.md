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
- writing the first draft of the report and editing

The other coded several of the functions not provided by the course, fixed several issues with our wire connections, took videos and pictures, and wrote most the report.

<p>&nbsp;</p> 

## Construction <a name="2"></a>

### Set up and Wiring Diagram <a name="2a"></a>

The pendulum’s angle is measured by the rotary encoder as the pendulum rotates about the shaft. The motor is connected to a motor controller (ESC) and through it the motor is powered with 12V and 6.4A. The Arduino receives a signal from the encoder, determines a new motor speed based on a PID control logic, and sends a signal to the ESC to control the motor.

![img](/images/projects/pendulum/physicle_layout_wiringD.PNG "Set up"){:height="400"} 

<p>&nbsp;</p> 

## Results <a name="3"></a>

### Step Response <a name="3a"></a>

PID constants were Kp = 0.05, Ki = 0.00125 (ms^-1), Kd = 1250 (ms)

![img](/images/projects/pendulum/step_response.PNG "Step Response graphed from Arduino software"){:height="300"} 

As seen in the above response, the system achieves a rise time less than 2.6 sec which meets the requirement of a 3.95s rise time. The system overshoot is negligible and therefore meets the requirements for maximum overshoot and rise time.

### Displacement Correction <a name="3b"></a>

PID constants were kept the same: Kp = 0.05, Ki = 0.00125 (ms^-1), Kd = 1250 (ms)

![img](/images/projects/pendulum/disturbance_response.PNG "Returns to Set of 30 Degrees"){:height="300"} 

<figure class="video_container">
  <video controls="true" allowfullscreen="true" height="300">
    <source src="/images/projects/pendulum/static_and_return.mp4" type="video/mp4">
  </video>
</figure> 

<figure class="video_container">
  <video controls="true" allowfullscreen="true" height="300">
    <source src="/images/projects/pendulum/static_and_return2.mp4" type="video/mp4">
  </video>
</figure> 

The system responds very fast to disturbances and clearly meets the required rise time. The system overshoots by approximately 4-5 degrees for large disturbances which exceeds the system requirements of 5% or 1.5 degrees. There were hardware limitations to achieving 5% overshoot and the system at one point would meet this requirement.

### Sine Wave <a name="3c"></a>

10 second period oscillating from 15 to 45 degrees. PID constants were Kp = 1.5, Ki = 0.01 (ms^-1), Kd = 200(ms)

![img](/images/projects/pendulum/sin_response.PNG "Step Response graphed from Arduino software"){:width="400"} 

<figure class="video_container">
  <video controls="true" allowfullscreen="true" height="300">
    <source src="/images/projects/pendulum/sin_graphed.mp4" type="video/mp4">
  </video>
</figure> 

The system responds very well to the iput sine wave. As the target is not constant steady state, overshoot, and rise time cannot be analyzed. This response was achieved mainly due to a large integral term.

<p>&nbsp;</p> 

## NOTES:
under construction!


