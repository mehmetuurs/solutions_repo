# Problem 1

# 🌌 Gravitational Dynamics: Analyzing Kepler’s Third Law 🌌

---

## 🎯 Objective

This notebook investigates the relationship between orbital period and radius through Kepler’s Third Law for circular orbits. It includes a derivation, computational simulation, and analysis of real-world astronomical data.

---

## 🚀 Derivation: Establishing Kepler’s Third Law

For a body in a circular orbit, the gravitational force balances the centripetal force required for circular motion:

-   **Gravitational Force**:  $F_g = \frac{G M m}{r^2}$
-   **Centripetal Force**:  $F_c = \frac{m v^2}{r}$

Equating these forces:

$$
\frac{G M m}{r^2} = \frac{m v^2}{r}
$$

Cancel $m$ (mass of the orbiting body) and simplify:

$$
v^2 = \frac{G M}{r}
$$

The orbital velocity is  $v = \frac{2\pi r}{T}$, where  $T$  is the orbital period. Substituting:

$$
\left(\frac{2\pi r}{T}\right)^2 = \frac{G M}{r}
$$

$$
\frac{4\pi^2 r^2}{T^2} = \frac{G M}{r}
$$

Rearrange by multiplying both sides by  $T^2$  and dividing by  $r$:

$$
T^2 = \frac{4\pi^2}{G M} r^3
$$

This yields  $T^2 \propto r^3$, demonstrating that the square of the orbital period is proportional to the cube of the orbital radius, a cornerstone of Kepler’s Third Law.

---

## 🌍 Astronomical Significance

Kepler’s Third Law has profound implications:

1.  **Mass Determination**: Using  $T$  and  $r$, the central body’s mass  $M$  can be calculated (e.g., Earth’s mass from the Moon’s orbit).
2.  **Distance Measurement**: Orbital periods of planets provide their distances from the Sun.
3.  **Orbital Engineering**: This relationship informs the design of satellite trajectories, such as those for navigation systems.

---

## 📊 Computational Analysis

This section implements a simulation to verify Kepler’s Third Law using real-world data and visualizations.

---

### Step 1: Orbital Data

This step presents the orbital parameters for the Moon and select Solar System planets, including their central masses, orbital radii, and periods. The Moon orbits Earth, while Earth, Mars, and Jupiter orbit the Sun, providing a range of scales to test Kepler’s Third Law. The data will serve as the foundation for verifying the  $T^2 \propto r^3$  relationship in subsequent steps.

---

### Step 2: Circular Orbit Visualization 🎬

To illustrate the dynamics of a circular orbit, an animated simulation of the Moon’s orbit around Earth is generated. The Moon’s orbital radius of 384,400 km is scaled for visualization, with Earth positioned at the origin. This animation highlights the uniform motion characteristic of a circular orbit, providing a visual representation of the period  $T$  and radius  $r$  used in Kepler’s Third Law.

---

### Step 3:  $T^2$  vs  $r^3$  Verification

A graphical representation confirms the  $T^2 \propto r^3$  relationship by plotting  $T^2$  against  $r^3$  for the Moon and planets. This visualization validates Kepler’s Third Law across different orbital scales, from the Moon’s orbit around Earth to Jupiter’s orbit around the Sun.

---

## 🌠 Extension to Elliptical Orbits

For elliptical orbits, Kepler’s Third Law applies with  $r$  representing the semi-major axis. This generalization extends its utility to diverse celestial phenomena, including comets and exoplanets.

---

## 🎨 Summary

This notebook integrates derivation, simulation, and visualization to elucidate Kepler’s Third Law.

![image](https://github.com/user-attachments/assets/a49e167b-c08f-4331-a9aa-3264d3f3d10f)



![ezgif com-video-to-gif-converter](https://github.com/user-attachments/assets/25e1a684-a3bb-40eb-bc1d-9d3313994f07)


![image](https://github.com/user-attachments/assets/9276570d-22d3-4e5d-94f5-bee49dc93125)



