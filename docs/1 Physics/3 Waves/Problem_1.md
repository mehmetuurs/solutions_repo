# Interference Patterns on a Water Surface

## Motivation
Interference occurs when waves from different sources overlap, creating new patterns. On a water surface, this can be observed when ripples from multiple points meet, forming distinctive interference patterns. These patterns demonstrate how waves combine, either reinforcing (constructive interference) or canceling each other (destructive interference). Studying these patterns provides a visual and intuitive way to understand wave behavior and explore concepts like phase relationships and multi-source interactions, with applications in physics and engineering.

## Problem Statement
We aim to analyze the interference patterns formed by the superposition of circular waves emitted from point sources located at the vertices of a regular polygon. For this example, we choose an **equilateral triangle** as the regular polygon.

A single circular wave from a point source at position $(x_s, y_s)$ is described by the equation:

$$ \eta(x, y, t) = A \cos(k r - \omega t + \phi) $$

where:
- $\eta(x, y, t)$ is the water surface displacement at point $(x, y)$ and time $t$,
- $A$ is the amplitude,
- $k = \frac{2\pi}{\lambda}$ is the wave number, with $\lambda$ as the wavelength,
- $r = \sqrt{(x - x_s)^2 + (y - y_s)^2}$ is the distance from the source,
- $\omega = 2\pi f$ is the angular frequency, with $f$ as the frequency,
- $\phi$ is the initial phase.

For multiple sources, the total displacement is the sum of individual waves (superposition):

$$ \eta_{\text{total}}(x, y, t) = \sum_{i=1}^{N} \eta_i(x, y, t) $$

where $N$ is the number of sources (vertices of the polygon).

## Steps and Solution

### 1. Select a Regular Polygon
We choose an **equilateral triangle** with vertices at:
- $(x_1, y_1) = (0, 1)$,
- $(x_2, y_2) = \left(\frac{\sqrt{3}}{2}, -\frac{1}{2}\right)$,
- $(x_3, y_3) = \left(-\frac{\sqrt{3}}{2}, -\frac{1}{2}\right)$.

These coordinates place the triangle's centroid at the origin $(0, 0)$ with a side length of $\sqrt{3}$.

### 2. Position the Sources
The wave sources are placed at the triangle's vertices as listed above.

### 3. Wave Equations
For each source $i$ at $(x_i, y_i)$, the wave equation is:

$$ \eta_i(x, y, t) = A \cos(k r_i - \omega t + \phi) $$

where $r_i = \sqrt{(x - x_i)^2 + (y - y_i)^2}$. We assume:
- $A = 1$ (same amplitude for all sources),
- $\lambda = 1$ (wavelength), so $k = \frac{2\pi}{1} = 2\pi$,
- $f = 1$ (frequency), so $\omega = 2\pi \cdot 1 = 2\pi$,
- $\phi = 0$ (coherent sources with no phase difference).

### 4. Superposition of Waves
The total displacement is:

$$ \eta_{\text{total}}(x, y, t) = \sum_{i=1}^{3} A \cos(k r_i - \omega t) $$

### 5. Python Simulation
Below is a Python script to simulate and visualize the interference pattern at $t = 0$:

```python
import numpy as np
import matplotlib.pyplot as plt

# Parameters
A = 1.0      # Amplitude
k = 2 * np.pi  # Wave number (lambda = 1)
omega = 2 * np.pi  # Angular frequency (f = 1)
t = 0.0      # Time snapshot
phi = 0.0    # Phase

# Source positions (equilateral triangle vertices)
sources = [(0, 1), (np.sqrt(3)/2, -0.5), (-np.sqrt(3)/2, -0.5)]

# Grid for simulation
x = np.linspace(-2, 2, 200)
y = np.linspace(-2, 2, 200)
X, Y = np.meshgrid(x, y)

# Calculate total displacement
eta_total = np.zeros_like(X)
for (xs, ys) in sources:
    r = np.sqrt((X - xs)**2 + (Y - ys)**2)
    eta_total += A * np.cos(k * r - omega * t + phi)

# Plotting
plt.figure(figsize=(8, 8))
plt.contourf(X, Y, eta_total, levels=20, cmap='RdBu')
plt.colorbar(label='Displacement $\eta_{\text{total}}$')
plt.scatter([s[0] for s in sources], [s[1] for s in sources], 
            c='black', label='Sources')
plt.title('Interference Pattern for Equilateral Triangle Sources')
plt.xlabel('$x$')
plt.ylabel('$y$')
plt.legend()
plt.grid(True)
plt.show()