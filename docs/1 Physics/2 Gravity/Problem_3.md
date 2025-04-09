# 🌍 Trajectories of a Freely Released Payload Near Earth: Problem 3

<div style="background-color: #f0f8ff; padding: 15px; border-radius: 10px;">
<h2 style="color: #2E86C1; text-align: center;">🚀 Payload Trajectories: A Comprehensive Analysis</h2>
</div>

---

## 🎯 Task: A Comprehensive Breakdown

We aim to analyze and simulate the trajectories of a payload released near Earth, considering the following objectives:

- **Trajectory Analysis**: Explore the possible trajectories (elliptical, parabolic, hyperbolic) and their conditions.
- **Numerical Computation**: Compute the payload’s path using numerical integration.
- **Orbital Scenarios**: Relate trajectories to real-world space mission scenarios (orbital insertion, reentry, escape).
- **Computational Simulation**: Develop a Python tool to simulate and visualize the payload’s motion, with options to vary initial conditions.

---

## 📜 Trajectory Analysis: Elliptical, Parabolic, and Hyperbolic Paths

The trajectory of a payload is determined by its **total mechanical energy** ($E = KE + PE$), which depends on its initial velocity and position relative to Earth.

### 🌀 Elliptical Trajectory
- **Condition**: Total mechanical energy $E < 0$.
- **Velocity**: Initial velocity $v < v_{\text{escape}}$, where $v_{\text{escape}} = \sqrt{\frac{2GM}{r}}$.
- **Description**: The payload is gravitationally bound to Earth, following a closed elliptical orbit.
- **Application**: Used for satellites in stable orbits (e.g., Low Earth Orbit).

### 📏 Parabolic Trajectory
- **Condition**: Total mechanical energy $E = 0$.
- **Velocity**: Initial velocity $v = v_{\text{escape}}$.
- **Description**: The payload has just enough energy to escape to infinity, with velocity approaching zero at large distances.
- **Application**: Represents the boundary between bound and unbound orbits.

### 🚀 Hyperbolic Trajectory
- **Condition**: Total mechanical energy $E > 0$.
- **Velocity**: Initial velocity $v > v_{\text{escape}}$.
- **Description**: The payload escapes Earth’s gravity with excess energy, moving away with non-zero velocity at infinity.
- **Application**: Used for interplanetary missions (e.g., Voyager probes).

---

## 🧮 Numerical Analysis: Equations of Motion

### Gravitational Force
The payload’s motion is governed by Newton’s Law of Universal Gravitation:

$$
F = -\frac{G M m}{r^2} r_{\text{hat}}
$$

- $G$: Gravitational constant ($6.674 \times 10^{-11} \, \text{m}^3 \, \text{kg}^{-1} \, \text{s}^{-2}$)
- $M$: Mass of Earth ($5.972 \times 10^{24} \, \text{kg}$)
- $m$: Mass of the payload
- $r$: Distance from Earth’s center
- $r_{\text{hat}}$: Unit vector from Earth to payload

Using Newton’s Second Law ($F = m a$), the equation of motion is:

$$
\frac{d^2 r}{dt^2} = -\frac{G M r}{r^3}
$$

### Numerical Integration
We solve this equation using the **Runge-Kutta 4th Order (RK4)** method for better accuracy compared to the Euler method. The system is converted into first-order equations:

$$
\frac{d r}{dt} = v, \quad \frac{d v}{dt} = -\frac{G M r}{r^3}
$$

### Initial Conditions
- **Position**: Start at 500 km altitude ($r_0 = R_{\text{Earth}} + 500 \, \text{km}$).
- **Velocity**: Vary to achieve elliptical, parabolic, and hyperbolic trajectories.

---

## 🌐 Orbital Scenarios: Real-World Applications

### 🛰️ Orbital Insertion
- **Trajectory**: Elliptical.
- **Goal**: Achieve a stable orbit by ensuring $v < v_{\text{escape}}$.
- **Example**: Satellites like the International Space Station (ISS).

### 🔥 Reentry
- **Trajectory**: Elliptical, with perigee in the atmosphere.
- **Goal**: Control the trajectory to manage heat and forces during atmospheric reentry.
- **Example**: Space Shuttle reentry.

### 🌌 Escape
- **Trajectory**: Parabolic or hyperbolic.
- **Goal**: Exceed escape velocity to leave Earth’s gravitational influence.
- **Example**: Interplanetary probes like New Horizons.

---

## 💻 Computational Simulation: Visualizing Payload Motion

We’ll simulate the payload’s motion for three trajectories (elliptical, parabolic, hyperbolic) and visualize them with:
- **Static Plots**: Trajectories, velocity vs. time, and energy analysis.
- **Animations**: Animated GIFs showing the payload’s motion around Earth.



![image](https://github.com/user-attachments/assets/8d323f14-93ae-475e-8e08-fec157eb9d1f)



![image](https://github.com/user-attachments/assets/d5ef14c9-fbbf-4e8f-b884-133824d934cd)



![image](https://github.com/user-attachments/assets/7df9c4f9-9bd9-4ebc-a5e5-fce480d5947f)



