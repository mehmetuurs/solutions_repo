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


![image](https://github.com/user-attachments/assets/eb13d284-e24f-49dc-99cd-112cfbb51b0f)
![image](https://github.com/user-attachments/assets/65c421ab-62e2-4c28-b93c-11c3f93cc252)

