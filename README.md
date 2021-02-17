# Robotics
## Robotics programming of selective line following and avoidance coupled with obstruction avoidance.

This is a program for the Thymio II robots https://www.thymio.org/ which run on two  identical Thymio Robot. Tshe program provided the following behaviours when the robots are running in the provided simulated Robot Arena (ASEBA Playground) https://www.thymio.org/program/aseba/:

1. The two robots are starting at initial random positions, one outside the dark blue oval track, and one inside the dark blue oval track. The track consists of a dark blue line on the Arena floor, and which is in the shape of an oval. Both robots will explore, avoiding any obstacles in the way (including the Arena Wall boundary) until the dark blue oval track is encountered.
2. When the circular track/line is encountered, the robots will both turn left and then follow the darl blue track/line (i.e. in opposite directions, one moving Clockwise (CW) and the other Counter-Clockwise (CCW)). Whenever the respective robots meet each other at any point while following the track, they will both move aside allowing them to pass each other safely without collision, then find their way back to the track/line, then carry on following the circular track/line in the same direction they were originally travelling in. They acheieved this by both moving out of the line in a semi-circular pattern and then then joining the line again. 
3. A “STOP” state/behavioural element allows one of center buttons to Stop/Start the robots.
4. A behaviour that keeps the robots within the outer boundary Dark Black line. (2)
5. the code was modified to allow the sequences in No. 2 to allow for the case when an object blocks the track
6. Implement object avoidance in the case that an object is encountered while “EXPLORE” behaviour is active and the robot is searching for a Line to follow. (2)
7. If the Line is lost while the robot is in line following state, a recovery behaviour/sequence will be triggered making transition to “WANDER” state.
