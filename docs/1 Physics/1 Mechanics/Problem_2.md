# Problem 2
# Projectile Motion Analysis

## 1. Theoretical Foundation

### Derivation of Equations

We begin with Newton's Second Law:

$F = ma$

Considering only gravity acting in the negative y-direction:

$F_y = -mg$

This leads to the following accelerations:

$a_x = 0$
$a_y = -g$

Integrating with respect to time, we obtain the velocities:

$v_x = v_{0x}$
$v_y = v_{0y} - gt$

Integrating again, we get the position equations:

$x = v_{0x}t$
$y = v_{0y}t - \frac{1}{2}gt^2$

Where:

* $v_{0x} = v_0 \cos(\theta)$
* $v_{0y} = v_0 \sin(\theta)$
* $v_0$ is the initial velocity.
* $\theta$ is the launch angle.
* $g$ is the acceleration due to gravity.
* $t$ is time.

### Family of Solutions

Varying $v_0$ and $\theta$ leads to different parabolic trajectories, forming a family of solutions. Changes in $g$ also affect the trajectory.

## 2. Analysis of the Range

### Range Equation

The horizontal range (R) is given by:

$R = \frac{v_0^2 \sin(2\theta)}{g}$

### Parameter Dependence

* **Angle:** Maximum range occurs at $\theta = 45^\circ$. The range is symmetrical about this angle.
* **Initial Velocity:** Range is proportional to $v_0^2$.
* **Gravitational Acceleration:** Range is inversely proportional to $g$.

## 3. Practical Applications

* **Uneven Terrain:** Adjust the y-coordinate equation to account for terrain profile.
* **Air Resistance:** Introduce a drag force term into the differential equations.
* **Wind:** Add a wind velocity component to $v_x$.
* **Sports:** Modeling ball trajectories in various sports.
* **Engineering:** Designing artillery projectiles and rocket trajectories.
* **Astrophysics:** Modeling comet and asteroid trajectories.

## 4. Implementation



