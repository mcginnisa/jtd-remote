---
title: Project Requirements
parent: Documentation
has_children: true
nav_order: 1
---

# Project Requirements 
## Marketing Requirements (MR) 
MR-1. A complete system will consist of a Crazyflie Quadcopter (UAV) and a Landing Platform providing for wireless flight control of the UAV without human input.

MR-2. The system will be able to land the UAV on a designated point on the Landing Platform on UAV low battery signal. 

MR-3. The Landing Platform must be able to fully recharge the UAV in a reasonable time frame.

MR-4. The Landing Platform should be able to provide a reasonable amount of recharges for the UAV.

MR-5. The UAV should have a reasonable flight time.

MR-6. The Landing Platform will use an upward facing camera to provide necessary feedback for landing the UAV.

MR-7. The system must have the ability to operate indoors under normal lighting conditions.

MR-8. The system must be portable.

MR-9.  A personal computer must be able to connect wirelessly to the Landing Platform to query or reconfigure the control software.

MR-10. The UAV must include safety line mounting points.

## Engineering Requirements (ER)
ER-1. The UAV will successfully respond to 95% of commands issued remotely by the Landing Platform at a distance of 3 meters (MR-1).

ER-2. UAV will be able to land within 5 cm of target point (MR-2).

ER-3. Wireless communication between the Landing Platform and the UAV will have a latency under 100 ms at 3 meters (MR-2).

ER-4. The Landing Platform will be able to charge the UAV within 1 hour (MR-3).

ER-5. The Landing Platform battery will be able to provide 25 W over 4 hours (MR-4). 

ER-6. The UAV will be able to fly for at least 5 minutes, with the landing sequence taking no more than 3 minutes (MR-5).

ER-7. Landing platform is able to detect an overhead UAV within a height of 2 meters in an indoor environment lit by T8 fluorescent light bulbs (MR-6, MR-7).

ER-8. The complete system will fit within a footprint of less than 0.25 m2 (MR-8).

ER-9. The landing platform control system will support remote connection via SSH (MR-9).

ER-10. Anchor point can suspend double the weight of the UAV when attached with 5 lb rated fishing line (MR-10).


