# ⚡ Electromagnetism Problem 1: Simulating the Effects of the Lorentz Force

<div style="background-color: #f0f8ff; padding: 15px; border-radius: 10px;">
<h2 style="color: #2E86C1; text-align: center;">🌐 Exploring Charged Particle Motion in Electric and Magnetic Fields</h2>
</div>

---

## 🎯 Motivation

The Lorentz force, given by $F = q(E + v \times B)$, governs the motion of charged particles in electric ($E$) and magnetic ($B$) fields. It plays a critical role in fields like plasma physics, particle accelerators, and astrophysics. By simulating the motion of a charged particle, we can visualize complex trajectories and understand practical applications such as cyclotrons, mass spectrometers, and magnetic confinement in fusion devices.

---

## 📜 Task Breakdown

1. **Exploration of Applications**:
   - Identify systems where the Lorentz force is key (e.g., particle accelerators, mass spectrometers, plasma confinement).
   - Discuss the roles of electric ($E$) and magnetic ($B$) fields in controlling particle motion.
2. **Simulating Particle Motion**:
   - Simulate the trajectory of a charged particle under:
     - A uniform magnetic field.
     - Combined uniform electric and magnetic fields.
     - Crossed electric and magnetic fields.
   - Capture circular, helical, or drift motion based on initial conditions.
3. **Parameter Exploration**:
   - Vary field strengths ($E$, $B$), initial velocity ($v$), and particle properties ($q$, $m$).
   - Analyze their effects on the trajectory.
4. **Visualization**:
   - Create 2D and 3D plots of the particle’s path for different scenarios.
   - Highlight phenomena like the Larmor radius and drift velocity.

---

## 🌟 Exploration of Applications

### Systems Involving the Lorentz Force
- **Particle Accelerators (e.g., Cyclotrons)**: The magnetic field causes charged particles to move in circular paths, while electric fields accelerate them. The Lorentz force ensures particles gain energy with each cycle.
- **Mass Spectrometers**: The Lorentz force separates ions by mass-to-charge ratio, as particles follow curved paths in a magnetic field.
- **Plasma Confinement (e.g., Tokamaks)**: Magnetic fields confine charged particles in helical paths to sustain high-temperature plasmas for fusion.
- **Astrophysics**: The Lorentz force governs the motion of charged particles in cosmic magnetic fields, such as in the aurora or solar wind interactions.

### Roles of Electric and Magnetic Fields
- **Electric Field ($E$)**: Exerts a force $F_E = qE$, accelerating the particle in the direction of the field (for positive $q$).
- **Magnetic Field ($B$)**: Exerts a force $F_B = q(v \times B)$, perpendicular to both the velocity and the field, causing circular or helical motion.
- **Combined Fields**: In crossed fields ($E \perp B$), particles exhibit drift motion, such as the $E \times B$ drift, which is crucial in plasma physics.

---

## 🧮 Simulating Particle Motion

### Lorentz Force Equation
The Lorentz force on a charged particle is:

$$
F = q(E + v \times B)
$$

Using Newton’s Second Law ($F = m a$), the acceleration is:

$$
a = \frac{dv}{dt} = \frac{q}{m} (E + v \times B)
$$

We also have:

$$
\frac{dr}{dt} = v
$$

### Numerical Integration
We use the **Runge-Kutta 4th Order (RK4)** method  to solve these differential equations numerically, ensuring accurate trajectories.

### Scenarios to Simulate
1. **Uniform Magnetic Field**: $B$ along the z-axis, $E = 0$. Expect circular or helical motion.
2. **Combined Electric and Magnetic Fields**: $B$ along z, $E$ along x. Expect helical motion with acceleration.
3. **Crossed Fields**: $E$ along x, $B$ along z. Expect $E \times B$ drift motion.

---

## 💻 Computational Simulation: Visualizing Particle Trajectories

We’ll simulate the particle’s motion for the three scenarios, visualize the trajectories in 2D and 3D, and explore parameter variations.




![lorentz_uniform_B](https://github.com/user-attachments/assets/16638062-2d63-48f6-95cf-604084a7faf3)












![lorentz_E_plus_B](https://github.com/user-attachments/assets/d7083279-5cc3-4542-8406-748a3a097e1c)














![lorentz_crossed_E_B](https://github.com/user-attachments/assets/7904a574-30af-4137-b844-ee7a02244dec)

















## 🔍 Physical Phenomena

**Larmor Radius (Uniform B)**: $1.48 \times 10^{-3}$ m

**E x B Drift Velocity (Crossed Fields)**: $1.00 \times 10^{5}$ m/s

---

## 📝 Discussion and Practical Applications

**Uniform Magnetic Field**: The particle follows a helical path due to the magnetic field, with a Larmor radius proportional to the perpendicular velocity and inversely proportional to the field strength. This is the principle behind cyclotrons, where particles are accelerated in circular paths.

**Combined E and B Fields**: The electric field accelerates the particle along the x-axis, while the magnetic field causes helical motion, resulting in a stretched helix. This is relevant in particle accelerators where both fields are used to control motion.

**Crossed Fields**: The particle exhibits E x B drift, moving in the y-direction due to the perpendicular E and B fields. This drift is crucial in plasma confinement devices like tokamaks, where it helps stabilize the plasma.

**Parameter Exploration**: Increasing the magnetic field strength reduces the Larmor radius, tightening the helical path, as seen in the B-field variation plot.

### Suggestions for Extension
- Introduce non-uniform magnetic fields (e.g., a magnetic bottle) to simulate magnetic trapping.
- Add time-varying fields to explore phenomena like magnetic reconnection.
- Include relativistic effects for high-speed particles, modifying the Lorentz force equation.


