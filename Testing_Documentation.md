---
title: Detailed Test Plan
parent: Documentation
has_children: true
nav_order: 1
---

## FT.1.1.1 - UAV Command Reliability: Confirm reliability of wireless communication between Landing Platform and UAV. (MR-1, ER-1)

Setup: The UAV will be connected to the Landing Platform’s Single Board Computer via CrazyRadio PA module. The Single Board Computer will run a Python script that queries the battery voltage on the UAV. This script will be run at increasing distances between the Single Board Computer and the UAV.

Expected Outcome: The UAV will successfully respond to commands sent by the Single Board Computer at least 95% of the time, up to a distance of 3 m.

Actual Results: TBD
Conclusion: TBD

## FT.2.2.1 - Manual Landing of UAV: Perform controlled landings of the aerial vehicle by human operator in order to ensure adequate maneuverability for precise landings. (MR-2, ER-2)

Setup: A personal computer was equipped with the Crazyradio PA module, a PlayStation 3 controller, and the Crazyflie client (a GUI control application for the Crazyflie quadcopter, distributed by the Bitcraze AB development team). We performed manual control of the Crazyflie using the PlayStation 3 controller and made multiple attempts at a precise landing on a target setpoint on smooth surface in an indoor setting.

Expected Outcome: Based on prior observations of indoor Crazyflie operation, the attempts were expected to demonstrate successful landings to within 5 cm of target.

Actual Results: Manual landings were consistently within 5 cm of the target.

Conclusion: The Crazyflie quadcopter was shown to be capable of an adequate degree of control precision for its intended purpose. 

## FT.2.2.2 - Software Landing of UAV: Perform controlled landings of the aerial vehicle by means of software-automated flight control commands in order to ensure adequate precision of landings upon a target set point. (MR-2, ER-2)

Setup: A Raspberry Pi 3B+ computer will be equipped with the Crazyradio PA module and a basic Python script capable of performing autonomous control of the Crazyflie quadcopter. The computer will be connected to the OpenMV camera module, which runs an image recognition algorithm in order to generate control commands for the quadcopter. These commands will be determined by a combination of the aerial vehicle’s height and its in-frame position. We will make multiple attempts at a precise landing on a target setpoint on smooth surface in an indoor setting.

Expected Outcome: Attempts are expected to demonstrate successful landings to within 5 cm of target, thus demonstrating that software landing can achieve ideal placement upon a wireless charging pad

Actual Results: TBD

Conclusion: TBD

## FT.2.3.1 - UAV Command Latency: Determine total command latency from the issuance of a single flight control command by the Single Board Computer to a corresponding response by the UAV motors. (MR-2, ER-3)

Setup: From a simple oscilloscope configured to display time-domain signals, one probe will be connected across the USB data pins on the Crazyradio PA module (connected to the single board computer) and another probe will be connected to one of the UAV’s motor control lines while the motors are themselves disconnects to ensure stable mtest conditions. A simple thrust command will be issued by the single board computer and transmitted to the UAV over the radio module. A measurement will be made of the delay between the occurrence of a signal level change on the USB data pin and the motor control line. The latency between the control command and the UAV motor response will be profiled for various distances between the radio module and the UAV.

Expected Outcome: Latency under 100 ms for adequate control timing.[8]

Actual Results: TBD

Conclusion: TBD

## FT.3.4.1 - UAV Charge Time: Determine the total time required to charge the UAV battery using the Qi wireless charging pad. (MR-3, ER-4).

Setup: The UAV will perform flight operations until its battery is depleted to the point of being unable to maintain flight. The UAV will then be placed on the Qi charger pad and timed until it reports a full battery status. Multiple iterations of this test will be performed for the various compatible battery capacities (250 mAH, 380 mAH, and 750 mAH).

Expected Outcome: The UAV battery will be fully charged within 1 hour.

Actual Results: TBD 

Conclusion: TBD

## FT.4.5.1 - Camera Power Consumption: Test the power consumed by the camera when our chosen image-recognition algorithm is running. (MR-4, ER-5)

Setup: The camera module ran a specific image-recognition algorithm. The power consumption over a 25 minute period was determined via USB power monitor. The test was performed once while a detectable object was the frame and once without any detectable object in frame.

Expected Outcome: The Camera module will consume no more than 5 W, regardless of whether or not a detectable object is in frame.

Actual Results: The camera module consumed, on average, less than 1 W for both scenarios.

Conclusion: The camera module meets the specified power requirements. 

## FT.4.5.2 - Qi Charger Power Consumption: Test power consumption of Qi charger while actively recharging UAV battery. (MR-4, ER-5)

Setup: Using a multimeter, we will measure the peak product of the voltage and current flowing to the transmitting Qi charger while the UAV battery is charging.

Expected Outcome: Qi charger should consume no more than 10 W.

Actual Results: TBD 

Conclusion: TBD

## FT.4.5.3 - Single Board Computer Power Consumption: Test power consumption of single board computer in Landing Platform. (MR-4, ER-5)

Setup: A USB power consumption monitor will be placed inline with the single board computer and a suitable power supply. The single board computer will be allowed to idle for 25 minutes while a idle-state power consumption measurements are taken. The single board computer’s power consumption will then be measured while running a stress test program which will utilize > 75% CPU capacity for 25 minutes. For both test iterations, the power consumption measurements will be averaged over the recorded test period.

Expected Outcome: Single board computer will consume no more than 15 W during either test iteration.

Actual Results: TBD

Conclusion: TBD

## ST.4.5.1 - System Battery Life: Confirm that the Landing Platform’s battery supports system operation over the specified time period. (MR-4, ER-5)

Setup: The Landing Platform will be powered by a fully-charged 11.1 V battery pack, as specified by the system design. All components of the landing platform - camera, single board computer, and Qi charger - will be switched on to maximize the system’s power consumption. The system’s total operation time until failure of at least one component will be measured.

Expected Outcome: The system will maintain operation for at least 4 hours.

Actual Results: TBD

Conclusion: TBD

## FT.5.6.1 - UAV Hover Endurance: Determine the total amount of time the UAV is able to hover for various battery capacities (250 mAH, 380 mAH, and 750 mAH). (MR-5, ER-6)

Setup: Begin timing UAV once it lifts off and commences a software-defined hover routine at a fixed height from the ground. Continue timing until the UAV is unable to maintain the hover height.

Expected Outcome: UAV hovers for at least 5 minutes with each battery. 

Actual Results: On average, the UAV was able to hover for 6 minutes with a 250 mAH battery and 8 minutes with a 380 mAH battery. The 750 mAH battery will be tested upon receipt from vendor.

Conclusion: Any of the previously-identified compatible batteries will adequately meet the minimum hover time of five minutes. 

## FT.5.6.2 - UAV Mobility Endurance: Determine the total amount of time the UAV is able to fly a given autonomous flight pattern. This pattern could either be in the horizontal or vertical planes. (MR-5, ER-6)

Setup: Two autonomous flight routines will be performed by a UAV equipped with a fully-charged onboard battery. The first routine will be a horizontal figure-eight pattern and the second will be a vertical figure-eight pattern. The UAV will be timed from initial take-off until flight failure due to inadequate battery power. The tests will be performed for the various compatible battery capacities (250 mAH, 380 mAH, and 750 mAH).

Expected Outcome: UAV will be able to maintain either autonomous flight routine for at least five minutes.

Actual Results: TBD 

Conclusion: TBD

## FT.5.6.3 -  Landing Routine Duration Test: Determine the total amount of time required to autonomously land the UAV. (MR-5, ER-6)

Setup:  An in-flight UAV will be positioned at the edge of the Landing Platform’s detectable range (at the maximum specified height) and the completion of the autonomous landing sequence will be timed. Only successful landings will be considered valid data points. The tests will be performed for the various compatible battery capacities (250 mAH, 380 mAH, and 750 mAH).

Expected Outcome: The time trials should indicate that successful landings can be made within three minutes for all specified batteries.

Actual Results: TBD 

Conclusion: TBD

## FT.6.7.1 - Algorithm Detection - Range: Determine the range of reliable UAV detection by various image-detection algorithms. (MR-6, MR-7, ER-7)

Setup: The camera module was configured for a desired image-recognition mode. The UAV was manually brought into frame and raised to various height intervals to determine the limits of reliably detecting the UAV with a given image-recognition algorithm (RBG detection, Frame Difference, and April Tag detection). This range determination was made for each of the various image-recognition modes

Expected Outcome: The camera module should consistently detect the UAV up to 2 m.

Actual Results: The camera module reliably detected the UAV up to 2.9 m, 1.8 m, and 1.5 m for the RGB, Frame Difference, and April Tag detection algorithms, respectively.  

Conclusion: The RGB detection algorithm will be used to determine the position of the UAV as it performs favorably to the other methods and provides the adequate range. 

## ST.8.8.1 -  Dimension Measurement: Confirm that the complete system is constrained to a size which supports portability. (MR-8, ER-8)

Setup: The Landing Platform’s physical dimensions will be measured with a ruler and its footprint will be determined.
Expected Outcome: The Landing Platform will have a footprint under 0.25 m2.

Actual Results: TBD 

Conclusion: TBD

## FT.9.9.1 - Network Access Test: Confirm that Landing Platform’s single board computer can be accessed via SSH (MR-9, ER-9)

Setup: A remote user PC was used to make numerous SSH connection attempts to the single board computer in order to determine reliable access.

Expected Outcome: The single board computer should be able to make a successful connection to 95% of the time.

Actual Results: Consistently-successful SSH connections were made between multiple user PCs and the Landing Platform’s single board computer.

Conclusion: The system adequately supports remote machine access via SSH.

## FT.10.10.1 - Anchor Point Weight Test: Confirm that the UAV anchor points will support twice the weight of the UAV on an anchor line. (MR-10, ER-10)

Setup: A 5 lb fishing line will be affixed to the UAV’s anchor point, with its loose end secured to a weight equivalent to twice the weight of the UAV. The UAV will be securely mounted to a fixed structure while the anchor point’s durability is tested with the freely-hanging weight.

Expected Outcome: The anchor point will not fail, and support the specified weight without compromising its structural integrity.

Actual Results: TBD 

Conclusion: TBD
