---
layout: post
title: "Lac Megantic Accident Analysis"
sub_title: "a"
categories:
  - Projects
tags:
- Projects
last_modified_at: 2019-04-11
---

1. [Introduction](#1)
2. [Background Information](#2)
    1. [Lac Megantic Train Disaster](#2a)
    2. [CAST and STAMP](#2b)
3. [CAST Analysis](#3)
    1. [Safety Goal, System](#3a)
    2. [Hazards and Constraints](#3b)
    2. [Safety Control Strcuture](#3c)

<p>&nbsp;</p> 

## Introduction <a name="1"></a>

I collaborated with Ryan Chappus, Yunzhe Liu and Cissy Yao for UofT course APS440: Making Sense of Accidents. The final project was to analysze a well-documented disaster using a systems-engineering approach; Specifically, to apply CAST.

Our group analysed the Lac-Mégantic Train Derailment Disaster.

My responsibilities were to:
- define the hazards and constraints.
- define what an accident secifically meant
- create the Safety Control Strcuture with Cissy.

With my group, we all:
- defined the safety goal, system, and assumptions.
- researched the accident.
- write the report, create the presentation and present it to our class.


## Background Information <a name="2"></a>

On July 5th, 2013, 10:50 pm:
- a Montreal, Maine & Atlantic Railway (MMA) train is parked on descending grade (i.e. downward slope) in Nantes, Québec.

The Situation with the Train:
- 5 locomotives & 72 Class 111 Tanks cars
- 7.7M L of petroleum crude oil
- Traveling from New Town, North Dakota to Saint John, New Brunswick

What the Locomotive Engineer (LE) did:
- Common company practice: hand brakes on all locomotives + 2 additional cars
- Left lead locomotive running powered locomotive air brakes
-- false impression of security
- Railway rules: force of hand brakes alone hold train
- Contacted Rail Traffic Controller (RTC) in Farnham Québec: ‘train secure’
- contacted RTC in Bangor, Maine, which supervised trains east of Lac Mégantic

Thre were several mechanical issues with locomotive:
- Black & white smoke from lead locomotive
- Persisted from a series of non-standard repairs
- Expected to settle → LE & RTC decided to leave train until following morning, where replacement LE would continue journey. 

Response from the Nantes Fire Department:
- 911 emergency; fire on the lead locomotive
- shut off fuel supply to lead locomotive & turned electrical breakers off (followed railway guidelines) 
- Surete de Québec (SQ) contacted Farnham RTC & sent track foreman to consult firefighters
- All individuals declared the train safe & left
- No power → air compressors shut down → air brakes began to leak, reducing retarding force

1 am: train rolled toward Lac Mégantic → top speed of 65 mph; Derailed at Centre town

Results:
- 63 cars derailed;
- 6 million litres of crude oil spilt;
- Fire and explosion;
- 47 people killed;
- 2000 more forced from homes;
- Downtown core destroyed;
- Surrounding land & water contaminated;

A coordinated emergency response helped to prevent further damage & loss.


### Lac Mégantic Train Derailment Disaster <a name="2a"></a>

### CAST and STAMP <a name="2b"></a>


<p>&nbsp;</p> 

## Analysis <a name="3"></a>

### Safety Goal, System <a name="3a"></a>

| ![img](/images/projects/lacMegantic/mma_railmap.PNG "MMA Railway System"){:width="500"} |**Safety Goal:** <br>To effectively and safely <br>transport goods, both <br>dangerous and not, <br>across North America <br>via railway system.<br> <br>**System:**<br>The Montreal, Maine and <br>Atlantic Railway and the <br>surrounding community and <br>regulatory environment.<br> <br>**Assumptions:**<br>Ignores Orford Express, <br>a minor tourist line <br>that ran between Magog<br> and Sherbrooke. <br> The system is the <br>MMA railways that <br>only transports goods, <br>not passengers. |

### Hazards and Constraints <a name="3b"></a>

In CAST, Accidents are events that result in a loss, and may include factors beyond the control of the system.

Hazards are a set of conditions in the system that ultimately lead to an accident (i.e. a loss). And they should be mitigated or eliminated by the safety control system.

For this system, an accident is:
 - Any death or injury to a person, whether employee or member of the public, due to the trains or due to a good that is currently being transported by a train.
 
 4 Hazards were identified. In order to prevent them, the safety control structure must have these requirements (i.e. constraints):


|           Hazards         |   Hazard Specific Constraints   |
|:-------------------------|:-------------------------------|
|                         **1: A Runaway Train**                        | **For both Hazard 1 and 2** |
| - The train is unsupervised or unmanned<br> while it is running to a location.<br> - The train is running and manned<br> but cannot be controlled by the staff.| - Locomotive & Tank Car runaways<br> and derailments must be prevented. <br> - Trains with dangerous goods<br> cannot exceed 50 mph at any point. |
|                         **2: A Speeding Train**                       | **For both Hazard 1 and 2** |
| - The train is traveling faster than<br> the speed limits of the track.<br> - The train is traveling so fast<br> that it risks derailing | - Unsupervised trains must be<br> properly secured so that it cannot start moving.<br> - Must have redundant systems to ensure<br> it cannot move or will be stopped if securements fail. |
|    **3: A damaged/improperly-implemented<br> safety system/component**    |       **For Hazard 3**      |
| - The equipment <br>(ex. brakes, derailers, etc) is broken<br> or is about to break at next use.<br> - Automatic safety systems are<br> disabled or shut down. | - Must routinely maintain and improve<br> railway infrastructure, equipment and vehicles.<br> - Valuable equipment must not be damaged. <br> - Railways must be kept in good condition. <br> - Equipment dealing with goods must be<br> in good condition.|
| **4: A train with dangerous goods<br> exposed to the public/environment** |       **For Hazard 4**      |
| - Dangerous goods are out of<br> their containment (i.e. not safely contained). <br> - Dangerous goods are not<br> contained with the proper<br> equipment and in proximity to<br> people or environment it can damage. | - Goods must be properly managed. <br> - There must be proper identification<br> of goods and classification of goods. <br> - Sufficient frequency checking<br> classification.<br> - Goods must be transported<br> by the proper safety equipment<br> as per classification . |


**General Safety Constraints:**

**Emergency Procedures Must be in place**
- Redundant safety systems in place
- Both physical defences and procedural/social defences

**Uphold public safety and trust**
- Following the above constraints
- Prevent harm to people (employees and citizens), property and environment.


### Safety Control Strcuture <a name="3c"></a>


![img](/images/projects/lacMegantic/SafetyControlStructure.png "The entire diagram"){:width="800"}

{::options parse_block_html="true" /} 

<details>
  <summary markdown="span">Click to see close ups and details of the diagram</summary>
  
  |                                Close Up                                |                      Details                     |
  |:----------------------------------------------------------------------:|:------------------------------------------------:|
  |![img](/images/projects/lacMegantic/federal_lvl.PNG ""){:width="600"}   |  |
  |![img](/images/projects/lacMegantic/us_federal.PNG ""){:width="600"}    |  |
  |![img](/images/projects/lacMegantic/petro_lvl.PNG ""){:width="600"}     |  |
  |![img](/images/projects/lacMegantic/mma_lvl.PNG ""){:width="600"}       |  |
  |![img](/images/projects/lacMegantic/inside_mma_lvl.PNG ""){:width="600"}|  |
  |![img](/images/projects/lacMegantic/municipal_lvl.PNG ""){:width="600"} |  |

</details>

{::options parse_block_html="false" /}



[comment]: # ( https://docs.google.com/presentation/d/1OcjaekwV8_MK_EE-1yhC48vIdhXToG-TKoZI4XIym1c/edit#slide=id.g57bad39807_0_26 )

[comment]: # (  the folder is https://drive.google.com/drive/u/0/folders/1GGamzCrhwR5RrRxuc87aAQntM-23AL34 )
