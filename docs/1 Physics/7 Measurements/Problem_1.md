# 🧪 Problem 1: Measuring Earth's Gravitational Acceleration with a Pendulum

---

## 🔍 Motivation

The acceleration $g$ due to gravity is a fundamental constant that affects many physical systems. One reliable way to measure $g$ is using a **simple pendulum**, where the **period of oscillation** depends on $g$ and the pendulum's length.

---

## 🎯 Task

Measure $g$ using a pendulum and perform a full **uncertainty analysis**. This includes:

- Measuring the pendulum length and timing multiple oscillations.
- Calculating $g$ from the period using the formula  
  $$ g = \frac{4 \pi^2 L}{T^2} $$
- Propagating the measurement uncertainties  
  $$
  \Delta g = g \cdot \sqrt{ \left( \frac{\Delta L}{L} \right)^2 + \left( 2 \cdot \frac{\Delta T}{T} \right)^2 }
  $$

---

## 🧪 Procedure

### 1. Materials

- String (1.0 m length)
- Small weight (key, coin bag, etc.)
- Stopwatch (or phone timer)
- Ruler or tape measure

### 2. Setup

- Attach the weight and fix the string to a support.
- Measure the **length $L$** from the suspension point to the center of the mass.
- Resolution of ruler = 1 mm →  
  $$ \Delta L = \frac{1\, \text{mm}}{2} = 0.0005\, \text{m} $$

---

## 📊 Data Collection

- Displace pendulum <$15^\circ$ and release.
- Time 10 full oscillations.
- Repeat 10 times.

### 🔢 Table of Measurements

| Trial | $T_{10}$ (s) |
|-------|--------------|
| 1     | 20.12        |
| 2     | 20.09        |
| 3     | 20.15        |
| 4     | 20.13        |
| 5     | 20.10        |
| 6     | 20.11        |
| 7     | 20.14        |
| 8     | 20.08        |
| 9     | 20.16        |
| 10    | 20.12        |

---

## 📈 Results and Calculations

- $L = 1.000$ m  
- $\Delta L = 0.0005$ m  
- $\overline{T}_{10} = 20.120$ s  
- $\sigma_T = 0.0261$ s  
- $\Delta T_{10} = \dfrac{\sigma_T}{\sqrt{10}} = 0.0083$ s  
- $T = \dfrac{\overline{T}_{10}}{10} = 2.0120$ s  
- $\Delta T = \dfrac{\Delta T_{10}}{10} = 0.00083$ s  

---

## 🧮 Gravity and Uncertainty

- Gravitational acceleration:  
  $$ g = \frac{4 \pi^2 L}{T^2} = 9.760 \, \text{m/s}^2 $$

- Propagated uncertainty:  
  $$
  \Delta g = g \cdot \sqrt{ \left( \frac{\Delta L}{L} \right)^2 + \left( 2 \cdot \frac{\Delta T}{T} \right)^2 }
  = 0.008 \, \text{m/s}^2
  $$

---

## ✅ Final Result

$$
g = 9.760 \pm 0.008 \, \text{m/s}^2
$$

---

## 📌 Analysis

1. **Comparison**  
   - Standard value: $9.81 \, \text{m/s}^2$  
   - Measured value is close, minor deviation expected due to rounding, timing precision.

2. **Sources of Uncertainty**  
   - **$\Delta L$**: Determined by resolution of ruler (1 mm → ±0.5 mm).
   - **$\Delta T$**: Affected by human reaction time and stopwatch resolution.
   - Short oscillation times reduce uncertainty.

3. **Limitations**  
   - Air resistance, pivot friction, imperfect small-angle assumption.
   - Stopwatch timing might vary slightly between trials.

---

## 📦 Deliverables Recap

- Tabulated $T_{10}$ measurements
- Calculated:  
  $\overline{T}_{10}$, $\sigma_T$, $\Delta T$, $T$, $g$, $\Delta g$
- Full uncertainty analysis and comparison to $g = 9.81$


```

L = 1.000 m ± 0.0005 m
T10 measurements: [20.12 20.09 20.15 20.13 20.1  20.11 20.14 20.08 20.16 20.12]

T10_mean = 20.120 s
T10_std = 0.0258 s
ΔT10 = 0.0082 s

T = 2.01200 s ± 0.00082 s
g = 9.752 m/s² ± 0.009 m/s²





![pendulum_gravity](https://github.com/user-attachments/assets/0a16e65c-1b2f-4a08-aa28-94ec1bf77ea8)

