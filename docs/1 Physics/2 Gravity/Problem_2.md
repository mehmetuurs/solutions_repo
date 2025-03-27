# Escape Velocities and Cosmic Velocities: 

## Problem 2: Cosmic Velocities 


### **Task: A Comprehensive Overview**

1. **Define and Explain:** Define the first, second, and third cosmic velocities, and provide a detailed explanation of their physical meaning and implications.
2. **Mathematical Derivations:** Present and analyze the mathematical derivations of these velocities, highlighting the parameters that influence them.
3. **Calculations and Visualizations:** Calculate and visualize these velocities for Earth, Mars, and Jupiter, comparing their magnitudes.
4. **Space Exploration Significance:** Discuss the crucial role of these velocities in space exploration, from satellite launches to interstellar missions.

### **Definitions: 

# First Cosmic Velocity (Orbital Velocity, v1)

This is the minimum velocity required for an object to enter a stable circular orbit around a celestial body, just above its surface (neglecting atmospheric drag).

It represents the balance between the gravitational force pulling the object towards the body and the centrifugal force pushing it outward.

Physically, it's the speed at which the object's trajectory continuously curves to match the curvature of the celestial body.


## Second Cosmic Velocity (Escape Velocity, v2)

This is the minimum velocity needed for an object to completely escape the gravitational pull of a celestial body, moving infinitely far away with zero kinetic energy.

It's the velocity at which the object's kinetic energy equals the magnitude of its gravitational potential energy.

Physically, it means the object has enough energy to overcome the gravitational potential well of the body.


## Third Cosmic Velocity (v3)

This is the minimum velocity required for an object to escape the gravitational influence of a star system, such as our Solar System, starting from a planet's surface.

It involves escaping the planet's gravity, then the star's gravity, and the galaxy's gravity.

Since the velocity is relative to the Sun, and the Earth is already orbiting the Sun, we need to add the velocity of the Earth in orbit around the Sun to the velocity required to escape the solar system.

Physically, it's the speed required to break free from the combined gravitational effects of the entire star system.

### **Mathematical Derivations: The Equations Behind the Velocities**

#### **First Cosmic Velocity ($v_1$)**

- For a stable circular orbit, the gravitational force provides the centripetal force:

$$
\frac{GMm}{r^2} = \frac{mv_1^2}{r}
$$

where:
- $G$ is the gravitational constant ($6.674 \times 10^{-11} \, \text{m}^3 \, \text{kg}^{-1} \, \text{s}^{-2}$).
- $M$ is the mass of the celestial body.
- $m$ is the mass of the orbiting object.
- $r$ is the orbital radius (approximately the body's radius).
- $v_1$ is the first cosmic velocity.

- Solving for $v_1$:

$$
v_1 = \sqrt{\frac{GM}{r}}
$$

#### **Second Cosmic Velocity ($v_2$)**

- Using the principle of conservation of energy, the initial kinetic energy must equal the gravitational potential energy:

$$
\frac{1}{2}mv_2^2 - \frac{GMm}{r} = 0
$$

- Solving for $v_2$:

$$
v_2 = \sqrt{\frac{2GM}{r}}
$$

- Notice that $v_2 = \sqrt{2} v_1$.

#### **Third Cosmic Velocity ($v_3$)**


- It's generally calculated in stages:
  1. Escaping Earth's gravity (using $v_2$ for Earth).
  2. Escaping the Sun's gravity from Earth's orbital distance.
  3. Adding the Earth's orbital velocity around the Sun.

- Let's break down the calculation:
  - Earth's escape velocity ($v_{\text{esc}, \text{Earth}}$) is approximately 11.2 km/s.
  - Earth's orbital speed around the Sun ($v_{\text{orb}, \text{Earth}}$) is approximately 29.8 km/s.
  - The escape velocity from the Sun at Earth's distance ($v_{\text{esc}, \text{Sun}}$) is approximately 42.1 km/s.

- The third cosmic velocity can be approximated as:

$$
v_3 \approx \sqrt{(v_{\text{esc}, \text{Sun}} - v_{\text{orb}, \text{Earth}})^2 + v_{\text{esc}, \text{Earth}}^2}
$$

$$
v_3 \approx \sqrt{(42.1 - 29.8)^2 + 11.2^2} \approx 16.6 \, \text{km/s}
$$

- A simplified approximation from Earth's surface is approximately 16.6 km/s.

### **Parameters Affecting Velocities: What Influences the Numbers?**

## Mass of the Celestial Body (M):

A more massive body exerts a stronger gravitational pull, requiring higher velocities to orbit or escape.

This is evident in the equations, where $M$ is directly proportional to $v_1$ and $v_2$.

## Radius (r):

A smaller radius (for the same mass) means a stronger gravitational field at the surface, again requiring higher velocities.

This is inversely proportional to the square root of $r$ in the equations.

# Importance in Space Exploration: Practical Applications

## Launching Satellites:

The first cosmic velocity is essential for placing satellites in stable orbits around Earth or other planets.

It determines the initial velocity needed to achieve orbit.

## Interplanetary Missions:

The second cosmic velocity is crucial for sending probes and spacecraft to other planets.

It ensures that the spacecraft can escape the planet's gravitational pull and travel to its destination.

## Interstellar Travel:

The third cosmic velocity (or higher) is necessary for future missions that aim to leave our Solar System and explore interstellar space.

This is a large hurdle, and extremely hard to achieve with current technology.


### Where:

- $G$ is the gravitational constant ($6.674 \times 10^{-11} \, \text{m}^3 \, \text{kg}^{-1} \, \text{s}^{-2}$).
- $M$ is the mass of the celestial body.
- $m$ is the mass of the orbiting object.
- $r$ is the orbital radius (approximately the body's radius).
- $v_1$ is the first cosmic velocity.

![image](https://github.com/user-attachments/assets/4858b1f2-83eb-4549-85b6-568f58dc9277)

Earth:
  First cosmic velocity: 7909.68 m/s
  Second cosmic velocity: 11185.98 m/s
  
Mars:
  First cosmic velocity: 3546.94 m/s
  Second cosmic velocity: 5016.13 m/s
  
Jupiter:
  First cosmic velocity: 42567.51 m/s
  Second cosmic velocity: 60199.54 m/s
