---
title: "ROI-bounded Visual Odometry"
author_profile: true
key: 1
excerpt: "Computer Vision, OpenCV"
header:
  teaser: /assets/images/visual-odom1.gif
---

This project simulates a dice colliding in a spinning cup by modeling the Lagrangian dynamics in this 6 DoF system.

## Video Demo
<iframe
    width="100%"
    height="50px"
    src="https://www.youtube.com/embed/T6qRhCT54ms"
    frameborder="0"
    allow="autoplay; encrypted-media"
    allowfullscreen
>
</iframe>

## Euler Lagrange Equations
The Euler Lagrange equations are derived by finding the body velocities of the box and the dice, defining the inertial matrices, calculating the kinetic energy and potential energy (so that we have the Lagrangian), and using the Lagrangian to derive the E-L equations. 

## Constraints
The dice can only have an impact with the box with its four corners. To define the constraints of this system, we can simplify it by only considering when the four corners of the dice touches the four edges of the box. Using the frames defined, we can define phi with the above reasoning. 

## External Forces
The external force added in the system is the force on the box in the positive y direction. This force is added to counter the gravitational pull on the box so that it doesn’t fall due to gravity.