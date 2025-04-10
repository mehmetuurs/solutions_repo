# Problem 2

## 1. Theoretical Foundation

### Differential Equation

The differential equation governing the motion of a forced damped pendulum is:

$\frac{d^2\theta}{dt^2} + b\frac{d\theta}{dt} + \frac{g}{L}\sin(\theta) = A\cos(\omega t)$

Where:

* $\theta$ is the angular displacement.
* $b$ is the damping coefficient.
* $g$ is the acceleration due to gravity.
* $L$ is the length of the pendulum.
* $A$ is the driving amplitude.
* $\omega$ is the driving frequency.

### Small-Angle Approximation

For small angles, $\sin(\theta) \approx \theta$. The equation simplifies to:

$\frac{d^2\theta}{dt^2} + b\frac{d\theta}{dt} + \frac{g}{L}\theta = A\cos(\omega t)$

### Approximate Solutions

The general solution is the sum of the homogeneous (transient) and particular (steady-state) solutions.

### Resonance Conditions

Resonance occurs when $\omega \approx \sqrt{g/L}$, leading to maximum amplitude oscillations.

## 2. Analysis of Dynamics

* **Damping Coefficient (b):** Influences the rate of decay of oscillations.
* **Driving Amplitude (A):** Affects the amplitude of oscillations and can lead to nonlinear behavior.
* **Driving Frequency (ω):** Determines the system's response; resonance occurs when $\omega$ is close to the natural frequency.
* **Transition to Chaos:** Can be observed through phase portraits, Poincaré sections, and bifurcation diagrams.

## 3. Practical Applications

* Energy harvesting devices
* Suspension bridges
* Oscillating circuits
* Metronomes
* Various mechanical systems

## 4. Implementation

![image](https://github.com/user-attachments/assets/ef628fde-6174-4f79-9f12-a73d52c24575)



![image](https://github.com/user-attachments/assets/cbab938a-247c-40ec-8d49-ceddf8929682)




![image](https://github.com/user-attachments/assets/1d84821c-469e-4dcf-a2e9-289442a06c71)




![image](https://github.com/user-attachments/assets/1a51850f-41dc-49ee-b532-b2b79d5045e8)




![image](https://github.com/user-attachments/assets/a9bafb27-58ad-4355-9481-df23fce32283)





Pendulum Motion: The angle and angular velocity plots show the transient decay due to damping and the steady-state oscillation driven by the external force. The nonlinear and linear solutions are similar because the initial angle (0.1 rad) is small, but the nonlinear solution shows slight deviations at larger amplitudes.


Phase Portrait: The phase portrait with multiple initial conditions shows the system converging to a limit cycle, indicating stable periodic motion at resonance (ω = ω₀). The trajectories spiral inward due to damping.


Poincaré Section: The Poincaré section shows a cluster of points, suggesting periodic motion. The color gradient indicates the evolution over time, confirming the system has settled into a steady state.


Resonance Curve: The resonance curve peaks near the natural frequency ω₀ ≈ 3.13 rad/s, confirming the resonance condition. The amplitude increases significantly at resonance, as expected.


Transition to Chaos: With the current parameters (A = 1.0), the system exhibits periodic motion. To observe chaos, we would need a higher driving amplitude (e.g., A > 1.5) or a different frequency.








