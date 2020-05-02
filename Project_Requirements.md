---
title: Project Requirements
parent: Documentation
has_children: false
nav_order: 1
---

# Project Requirements 
## Marketing Requirements (MR) 


MR-1. A complete system will consist of a Crazyflie Quadcopter (UAV) and a charging platform providing for wireless flight control of the UAV without human input.

MR-2. The system will be able to land the UAV on a designated point on the charging platform on a UAV low battery signal. 

MR-3. The charging platform must be able to fully recharge the UAV in a reasonable time frame.

MR-4. The charging platform should be able to provide a reasonable amount of recharges for the UAV.

MR-5. The UAV should have a reasonable flight time.

MR-6. The charging platform will use an upward facing camera to provide necessary feedback for landing the UAV.
MR-7. The system must have the ability to operate indoors under normal lighting conditions.

MR-8. The system must be portable.
 
MR-9. A personal computer must be able to connect wirelessly to the charging platform to query or reconfigure the control software.

MR-10. The UAV must include safety line mounting points.

## Engineering Requirements (ER)
ER-1. The UAV will successfully respond to 95% of commands issued remotely by the charging platform at a distance of 3 meters (MR-1).

MR-2. UAV will be able to land within 5 cm of target point (MR-2).

MR-3. Wireless communication between the charging platform and the UAV will have a latency under 100 ms at 3 meters (MR-2).

MR-4. The charging platform will be able to charge the UAV within 1 hour (MR-3).

MR-5. The charging platform battery will be able to provide 25 W over 4 hours (MR-4). 

MR-6. The UAV will be able to fly for at least 3 minutes, with the landing sequence taking no more than 2 minutes (MR-5).

MR-7. Charging platform is able to detect an overhead UAV within a height of 2 meters in an indoor environment lit by T8 fluorescent light bulbs (MR-6, MR-7).

MR-8. The complete system will fit within a footprint of less than 0.25 m2 (MR-8).

MR-9. The charging platform control system will support remote connection via SSH (MR-9).

MR-10. Anchor point can suspend double the weight of the UAV when attached with 5 lb rated fishing line (MR-10).



