---
title: Detailed Test Plan
parent: Testing Documentation
has_children: true
nav_order: 1
---


Description of Tests

# FT.1.1.1 - 
Manual Landing of UAV: Perform controlled landings of the aerial vehicle by human operator in order to ensure adequate maneuverability for precise landings (MR.1, ER.1)

Setup: A personal computer was equipped with the Crazyradio PA module, a PlayStation 3 controller, and the Crazyflie client (a GUI control application for the Crazyflie quadcopter, distributed by the Bitcraze AB development team). We performed manual control of the Crazyflie using the PlayStation 3 controller and made multiple attempts at a precise landing on a target setpoint on smooth surface in an indoor setting.

Expected Results: Based on prior observations of indoor Crazyflie operation, the attempts were expected to demonstrate successful landings to within 105 cm of target.

Actual Results: Manual landings were consistently within 5 cm of the target.

Conclusion: The Crazyflie quadcopter was shown to be capable of an adequate degree of control precision for its intended purpose. 

# FT.1.1.2 - 
Software Landing of UAV: Perform controlled landings of the aerial vehicle by means of software-automated control commands in order to ensure adequate precision of landings upon a target set point (MR.1, ER.1)

Setup: A Raspberry Pi 3B+ computer was equipped with the Crazyradio PA module and a basic Python script capable of performing autonomous control of the Crazyflie quadcopter. The computer was also connected to the OpenMV camera module, which ran an image recognition algorithm in order to generate control commands for the quadcopter. These commands were determined by a combination of the aerial vehicle’s height and its in-frame position. We made multiple attempts at a precise landing on a target setpoint on smooth surface in an indoor setting.

Expected Results: Attempts are expected to demonstrate successful landings to within 105 cm of target

Actual Results: TBD 

Conclusion: TBD

# FT.1.1.3 - 
UAV Command Latency: Determine total command latency from the issuance of a single flight control command by the single board computer to a corresponding response by the UAV motors (MR.1, ER.1)

Setup: From a simple oscilloscope configured to display time-domain signals, one probe will be connected across the USB data pins on the Crazyradio PA module (connected to the single board computer) and another probe will be connected to one of the UAV’s motor control lines while the motors are themselves disconnects to ensure stable mtest conditions. A simple thrust command will be issued by the single board computer and transmitted to the UAV over the radio module. An observation will be made of the delay between the occurrence of a signal level change on the USB data pin and the motor control line. The latency between the control command and the UAV motor response will be profiled for various distances between the radio module and the UAV. 

Expected Results: TBD, mention the reasonable spec of 1 ms from command to USB?

Actual Results: TBD

Conclusion: TBD

# FT.2.2.1 - 
UAV Hover Endurance: Determine the total amount of time the UAV is able to hover given a battery with 250 mAH, 380 mAH, or 750 mAH capacity. (MR.2, ER.2)

Setup: Begin timing UAV once it enters the air and employs the hover setting to maintain a relative height from the ground. Continue timing until the UAV is unable to maintain height set by software. (MR-2, ER-2)

Expected Results: UAV hovers for 5 minutes at minimum with each battery. 

Actual Results: UAV able to hover for 6 minutes on average with 250 mAH battery, 8 minutes on average with 380 mAH battery, and 16 minutes<INSERT MINUTES> with 750 mAH battery. 

Conclusion: Any available battery will suffice to meet the minimum hover time of five minutes. 

# FT.2.2.2 - 
UAV Mobile Endurance: Determine the total amount of time the UAV is able to fly in a given pattern. This pattern could either be in the horizontal direction or vertical direction, thus two patterns will be used. The first is a horizontal figure eight pattern and the second is a vertical figure eight pattern. During both patterns, the UAV will be timed from take-off until it is unable to maintain flight. The pattern will be repeated for the three sizes of available battery: 250 mAH, 380 mAH, 750 mAH. (MR-2, ER-2)

Setup: TBD…

Expected Results: UAV will be able to maintain pattern for a minimum of five minutes.

Actual Results: TBD... 

Conclusion: TBD…

# FT.3.3.1 - 
UAV Charge Time Measurement: The total time required to charge the UAV given the three available batteries is acquired by depleting a battery to the point that it will no longer allow the UAV to maintain flight. This process is repeated for available battery capacities: 250 mAH, 380 mAH, 750 mAH. (MR-3, ER-3)

Setup: A UAV, with Qi charging capability, will perform flight operations until battery is relatively depleted. The UAV will then be placed on the Qi charger platform and monitored until it reports a full battery. 

Expected Results: The UAV battery will be fully charged within 6 hours. 

Actual Results: TBD... 

Conclusion: TBD…

# FT.4.4.1 - 
Single Board Computer Power Consumption: Power consumed by single board computer when in a basic standby mode and in a computation heavy scenario. (MR.4, ER.4)

Setup: A USB power consumption monitor will be placed incline with the single board computer and a suitable power supply. The single board computer will be allowed to idle for 25 minutes. Then the single board computer will run a stress test program which utilizes > 75% CPU capacity for 25 minutes. The power consumption in both cases will be averaged over the recorded period.

Expected Results: Single board computer will not consume more than 15W maximum.

Actual Results: TBD... 

Conclusion: TBD…

# FT.4.4.2 - 
Camera Power Consumption: Power consumed by camera when chosen algorithm is active. (MR.4, ER.4)

Setup: The camera module will be set to a specific algorithm. The power consumption over a twenty five minute period is determined via USB power monitor when an object is in the frame and when an object is not in the frame. 

Expected Results: The Camera module will consume, at most, 5 Watts when an object is or is not within the frame of view. 

Actual Results: The camera module consumed, on average, less than 1 Watt for both scenarios. 

Conclusion: The camera module meets the specified power requirements. 

# FT.4.4.3 - 
Qi Charger Power Consumption: Power consumed by Qi charger when the UAV is being charged by it.  (MR.1, ER.1)

Setup: Measure the peak product of the voltage and current flowing to the transmitting Qi charger when the UAV is charging using a multimeter. 

Expected Results:Qi charger should consume 10W maximum

Actual Results: TBD... 

Conclusion: TBD…

# FT.5.5.1 - 
Network Access Test: Determine if single board computer can be accessed via SSH (MR.5, ER.5)

Setup: Repeatedly connect to the single board computer twenty times to determine if the diagnostic and service connection can be reliably accessed. 

Expected Results: The single board computer should connect successfully 51% of the time.

Actual Results: TBD... 

Conclusion: TBD…

# FT.6.6.1 - 
Algorithm(s) Height vs. Distance: The chosen algorithm will be used to detect the height of the UAV. (MR.6, ER.6)

Setup: The camera module will enter the desired detection mode. Once there the UAV will be moved at regular intervals to determine if the UAV is detectable at the maximum range of 10 feet from the camera.
Expected Results: The camera module will detect the UAV up to 10 feet consistently.

Actual Results: The camera module detected the UAV up to 9.5 feet, 6 feet, and 5 feet with RGB, Frame Difference, and April Tag detection algorithms respectively.  

Conclusion: The RGB detection algorithm will be used to determine the position of the drone as it functions nearest to the desired heights. 

# FT.6.6.2 - 
Object at Velocity Detection Rate: Perform a (MR.6, ER.6)

Setup: The camera module will be set to desired detection algorithm. Once setup, the UAV will be moved at varying speeds through the view. The overall accuracy is determined by how often the camera reports a positive contact while the UAV is within view. 

Expected Results: TBD…

Actual Results: TBD... 

Conclusion: TBD…

# FT.7.7.1 - 
Anchor point weight test: Determine if twice the UAV weight will break the anchor line. The anchor line secures the UAV to a point in it’s surroundings, so that it does not travel a certain radius away from a chosen point. (MR.7, ER.7)

Setup: The line will be tied to a secure location, and weights equal to twice the UAV weight will be attached to the other end and allowed to hang. The UAV and weights will be weighed by the same scale with milligram precision.

Expected Results: The anchor point will not fail.

Actual Results: TBD... 

Conclusion: TBD…

# FT.7.7.2 -  Anchor point thrust test: Determine if the UAV applying maximum thrust will break the anchor line. The anchor line secures the UAV to a point in its surroundings, so that it does not travel a certain radius away from a chosen point. (MR.7, ER.7)

Setup: The anchor line will be attached to the UAV, and the other end will be securely tied to an anchor point. The UAV battery will be fully charge, and all four motors will be set to maximum thrust. 

Expected Results: The anchor point will not fail.

Actual Results: TBD... 

Conclusion: TBD…
