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


![image](https://github.com/user-attachments/assets/58c66c8d-0ee5-4d22-8492-bc3a0563b16d)



### 5. Analyze Interference Patterns
- **Constructive Interference**: Occurs where waves from all sources are in phase (e.g., crests align), resulting in larger amplitudes (bright red/blue regions in the plot).
- **Destructive Interference**: Occurs where waves are out of phase (e.g., crest meets trough), resulting in near-zero displacement (white regions).

For the equilateral triangle:
- Symmetry in the pattern reflects the triangle's geometry.
- High-amplitude regions form near the center and along symmetric axes.
- Cancellation occurs in regions where waves from different sources arrive with opposite phases.

### 6. Visualization
The plot above shows the water surface displacement at $t = 0$. Red and blue indicate positive and negative displacements (crests and troughs), while white indicates destructive interference.

## Results
The interference pattern for three sources at the vertices of an equilateral triangle exhibits:
- A central region of constructive interference due to overlapping crests.
- Radiating bands of alternating constructive and destructive interference, forming a triangular symmetry.
- The pattern evolves over time with $\omega t$, but the snapshot at $t = 0$ captures the initial state.

This simulation illustrates how wave superposition depends on source positioning and phase coherence, offering insights into wave physics in a tangible, visual format.
