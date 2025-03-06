# Problem 1

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



import numpy as np
import matplotlib.pyplot as plt

def calculate_range(v0, theta_deg, g):
    theta_rad = np.radians(theta_deg)
    return (v0**2 * np.sin(2 * theta_rad)) / g

def simulate_projectile(v0, theta_deg, g, time_steps=100):
    theta_rad = np.radians(theta_deg)
    t = np.linspace(0, (2 * v0 * np.sin(theta_rad)) / g, time_steps)
    x = v0 * np.cos(theta_rad) * t
    y = v0 * np.sin(theta_rad) * t - 0.5 * g * t**2
    return x, y

g = 9.81
v0_values = [10, 20, 30]
theta_degrees = np.linspace(0, 90, 91)

plt.figure(figsize=(10, 6))
for v0 in v0_values:
    ranges = [calculate_range(v0, theta, g) for theta in theta_degrees]
    plt.plot(theta_degrees, ranges, label=f'v0 = {v0} m/s')

plt.title('Projectile Range vs. Launch Angle')
plt.xlabel('Launch Angle (degrees)')
plt.ylabel('Range (meters)')
plt.legend()
plt.grid(True)
plt.show()

plt.figure(figsize=(10, 6))
for v0 in v0_values:
    x, y = simulate_projectile(v0, 45, g)
    plt.plot(x, y, label=f'v0 = {v0} m/s')
plt.title("Projectile Trajectory at 45 Degrees")
plt.xlabel("Distance (m)")
plt.ylabel("Height (m)")
plt.grid(True)
plt.legend()
plt.show()

v0 = 25;
angles = [25, 45, 65]
plt.figure(figsize = (10,6))
for angle in angles:
    x,y = simulate_projectile(v0, angle,g)
    plt.plot(x,y, label = f'angle = {angle}')
plt.title("Projectile Trajectory at varying angles")
plt.xlabel("Distance (m)")
plt.ylabel("Height (m)")
plt.grid(True)
plt.legend()
plt.show()