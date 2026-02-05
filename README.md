3-DOF Planar Robotic Arm – Forward Kinematics

This repository demonstrates the forward kinematics calculation of a
3-degree-of-freedom (3-DOF) planar robotic arm.

The objective is to calculate the end-effector position (x, y)
using the link lengths and joint angles.

--------------------------------------------------

Arm Parameters

Link lengths:
L1 = 15 cm
L2 = 10 cm
L3 = 4 cm

Joint angles (degrees):
Theta1 = 45
Theta2 = 30
Theta3 = -15

Note:
A negative angle represents clockwise rotation.

--------------------------------------------------

Forward Kinematics Equations

The end-effector position is calculated as:

x = L1*cos(Theta1)
  + L2*cos(Theta1 + Theta2)
  + L3*cos(Theta1 + Theta2 + Theta3)

y = L1*sin(Theta1)
  + L2*sin(Theta1 + Theta2)
  + L3*sin(Theta1 + Theta2 + Theta3)

--------------------------------------------------

Step-by-Step Calculations

After first link (L1):

x1 = 15*cos(45) = 10.61
y1 = 15*sin(45) = 10.61

Position:
(x1, y1) = (10.61, 10.61)

--------------------------------------------------

After second link (L2):

x2 = 15*cos(45) + 10*cos(75) = 13.20
y2 = 15*sin(45) + 10*sin(75) = 20.26

Position:
(x2, y2) = (13.20, 20.26)

--------------------------------------------------

End-Effector Position (L3):

x = 15*cos(45) + 10*cos(75) + 4*cos(60) = 15.20
y = 15*sin(45) + 10*sin(75) + 4*sin(60) = 23.73

--------------------------------------------------

Final Result

End-Effector Position:
(x, y) = (15.20, 23.73) cm

--------------------------------------------------

Notes

- This is a planar (2D) robotic arm
- Angles are cumulative
- Calculations use degrees, not radians

--------------------------------------------------

Author

Created for educational purposes to demonstrate
forward kinematics of a robotic arm.
