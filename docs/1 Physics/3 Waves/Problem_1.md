# 🌊 Wave Interference: Patterns on a Water Surface 🌊

---

## 🎯 Objective
This notebook analyzes the interference patterns formed on a water surface due to circular waves emitted from point sources positioned at the vertices of a regular polygon. By simulating the superposition of these waves, we aim to understand wave interactions, identify regions of constructive and destructive interference, and visualize the resulting patterns.

---

## 📜 Background: Wave Interference
When waves from multiple sources overlap, they create interference patterns due to the principle of superposition. The total displacement at any point is the sum of the displacements from each wave:

\[
\eta_{\text{total}}(x, y, t) = \sum_{i=1}^N \eta_i(x, y, t)
\]

For a circular wave emitted from a point source at $(x_s, y_s)$, the displacement is given by:

\[
\eta(x, y, t) = A \cos(k r - \omega t + \phi)
\]

where:
- $\eta(x, y, t)$: Displacement at point $(x, y)$ and time $t$.
- $A$: Amplitude.
- $k = \frac{2\pi}{\lambda}$: Wave number, with $\lambda$ as the wavelength.
- $r = \sqrt{(x - x_s)^2 + (y - y_s)^2}$: Distance from the source.
- $\omega = 2\pi f$: Angular frequency, with $f$ as the frequency.
- $\phi$: Initial phase.

**Interference Types**:
- **Constructive Interference**: Occurs when waves are in phase (phase difference $\Delta\phi \approx 0$), leading to amplification (larger displacement).
- **Destructive Interference**: Occurs when waves are out of phase (phase difference $\Delta\phi \approx \pi$), leading to cancellation (smaller or zero displacement).

---

## 📊 Simulation Setup
We will simulate interference patterns using the following steps:
1. **Choose a Regular Polygon**: Select a square with four vertices as the positions of the wave sources.
2. **Position the Sources**: Place the sources at the vertices of the square.
3. **Wave Equations**: Define the wave equation for each source.
4. **Superposition**: Compute the total displacement by summing the contributions from all sources.
5. **Visualization**: Plot the interference patterns to identify constructive and destructive regions.

---

### Step 1: Define the Polygon and Source Positions
We choose a square with side length 2 units, centered at the origin. The vertices (and thus the positions of the wave sources) are:
- $(1, 1)$
- $(1, -1)$
- $(-1, -1)$
- $(-1, 1)$

---

### Step 2: Wave Parameters
We assume the following parameters for all sources (coherent waves):
- Amplitude $A = 1$ unit.
- Wavelength $\lambda = 0.5$ units.
- Frequency $f = 1$ Hz.
- Initial phase $\phi = 0$.

Thus:
- Wave number $k = \frac{2\pi}{\lambda} = \frac{2\pi}{0.5} = 4\pi$.
- Angular frequency $\omega = 2\pi f = 2\pi \times 1 = 2\pi$.

---

### Step 3: Simulate the Interference Pattern
We will:
- Create a 2D grid to represent the water surface.
- Calculate the displacement from each source at each grid point.
- Sum the displacements to get the total wave pattern.
- Visualize the pattern at a fixed time $t$ (e.g., $t = 0$).

---

### Step 4: Visualize the Results
We’ll use a heatmap to show the displacement $\eta_{\text{total}}(x, y, t)$ across the water surface, highlighting regions of constructive and destructive interference. We’ll also create an animated plot to show how the pattern evolves over time.

---

## 🔍 Analysis of Interference Patterns
After simulating the interference, we will analyze:
- **Constructive Interference**: Regions where the displacement is maximized (bright areas in the heatmap).
- **Destructive Interference**: Regions where the displacement is minimized or zero (dark areas in the heatmap).

---

## 🌟 Applications
Understanding wave interference on a water surface has applications in:
- **Physics Education**: Visualizing wave superposition in a tangible way.
- **Acoustics**: Designing sound systems to avoid dead spots (destructive interference).
- **Optics**: Analyzing light interference in phenomena like thin-film interference.
- **Oceanography**: Studying wave interactions in coastal engineering.

---
