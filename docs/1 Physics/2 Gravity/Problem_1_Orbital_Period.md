# Gravity and Orbital Motion

## Problem 1: Orbital Period and Orbital Radius

### **Motivation: Why is this Important?**

One of the most fascinating aspects of planetary motion is that the relationship between a planet's orbital period and its distance from the central body follows a simple yet profound mathematical pattern. This pattern is known as **Kepler’s Third Law** and is essential in astronomy, space exploration, and understanding gravity.  

By studying this law, we can:  
1. **Predict planetary positions** in the Solar System.  
2. **Determine the masses of celestial bodies** (such as the mass of the Sun or planets).  
3. **Calculate satellite orbits** for GPS, communication, and space missions.  
4. **Understand exoplanet systems**, where distant planets are detected using orbital data.  

This law applies to **any object in orbit**, whether it's the Moon around the Earth, satellites around a planet, or planets around a star. Now, let’s derive this relationship.

---

## **Step 1: Deriving Kepler’s Third Law for Circular Orbits**

Newton’s version of **Kepler’s Third Law** states:

$$ T^2 = \frac{4\pi^2 r^3}{GM} $$

where:  
- $T$ = orbital period (seconds)  
- $r$ = orbital radius (meters)  
- $G$ = universal gravitational constant ($6.674 \times 10^{-11} \text{m}^3 \text{kg}^{-1} \text{s}^{-2}$)  
- $M$ = mass of the central body (kilograms, e.g., Earth or the Sun)

### **Understanding the Physics Behind It**
The force keeping an object in orbit is **gravity**, which acts as a centripetal force:

$$ F_g = \frac{GMm}{r^2} $$

where $m$ is the mass of the orbiting body (e.g., a satellite or planet).  
At the same time, the object moves in a circular path, meaning the centripetal force is:

$$ F_c = \frac{m v^2}{r} $$

Since gravity is the only force keeping the object in orbit, these two forces must be equal:

$$ \frac{GMm}{r^2} = \frac{m v^2}{r} $$

Canceling out $m$ and solving for velocity $v$:

$$ v^2 = \frac{GM}{r} $$

Since orbital velocity is also given by $ v = \frac{2\pi r}{T} $, we substitute:

$$ \left( \frac{2\pi r}{T} \right)^2 = \frac{GM}{r} $$

Expanding and solving for $T^2$:

$$ T^2 = \frac{4\pi^2 r^3}{GM} $$

This proves that the **square of the orbital period is directly proportional to the cube of the orbital radius**.

---

## **Step 2: Why Does This Matter?**

### **Real-World Applications**
- **The Moon’s Orbit:** By measuring the Moon’s orbital period, we can determine the mass of the Earth.  
- **Planetary Motion:** Scientists use this law to predict how planets move around the Sun.  
- **Space Missions:** Space agencies calculate satellite orbits using this principle.  
- **Exoplanet Discovery:** Astronomers use orbital periods to estimate the masses and distances of planets outside our Solar System.

### **Verification with Data**
- If we measure orbital radius ($r$) and period ($T$) for different satellites and planets, plotting $T^2$ vs. $r^3$ should give a straight line.
- This confirms the law experimentally.

---

## **Step 3: Computational Model & Simulations**

To make this law more intuitive, let’s visualize it using Python.  
We will:
1. **Plot the relationship between $T^2$ and $r^3$** to confirm the law.
2. **Simulate a circular orbit** to visualize planetary motion.

---

## **Python Code for Simulations**
import numpy as np
import matplotlib.pyplot as plt
from scipy.constants import G

# Define constants
M = 5.972e24  # Mass of Earth (kg)
R = np.linspace(6.7e6, 4e8, 100)  # Orbital radius from low Earth orbit to Moon (m)

# Compute Orbital Period using Kepler's Third Law
T = np.sqrt((4 * np.pi**2 * R**3) / (G * M))

# Plot T^2 vs. R^3 to verify Kepler's Third Law
plt.figure(figsize=(8, 6))
plt.plot(R**3, T**2, label="$T^2$ vs. $r^3$", color='b')
plt.xlabel("$r^3$ (m³)")
plt.ylabel("$T^2$ (s²)")
plt.title("Verification of Kepler's Third Law")
plt.legend()
plt.grid()
plt.show()

# Circular Orbit Simulation
fig, ax = plt.subplots(figsize=(6,6))
ax.set_xlim(-R[-1], R[-1])
ax.set_ylim(-R[-1], R[-1])
ax.set_xlabel("X (m)")
ax.set_ylabel("Y (m)")
ax.set_title("Circular Orbit Simulation")

# Generate Circular Orbit
theta = np.linspace(0, 2*np.pi, 300)
x = R[-1] * np.cos(theta)
y = R[-1] * np.sin(theta)
ax.plot(x, y, label="Orbit", color='r')
ax.scatter(0, 0, color='black', label="Central Body")
ax.legend()
ax.grid()
plt.show()

![alt text](image.png)
![alt text](image.png)