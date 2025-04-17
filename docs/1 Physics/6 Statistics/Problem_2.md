# Problem 2


# 🧮 Problem 2: Estimating π Using Monte Carlo Methods

<div style="background-color: #f0f8ff; padding: 15px; border-radius: 10px;">
<h2 style="color: #2E86C1; text-align: center;">🎲 Monte Carlo Methods: Estimating π Through Randomness</h2>
</div>

---

## 🎯 Motivation

Monte Carlo simulations allow us to estimate complex values using randomness. A famous example is estimating **π**, using either:
- **Geometric probability** (Circle-in-a-Square Method)
- **Buffon’s Needle** (a probabilistic geometry problem)

These simulations not only visualize randomness in action but reveal convergence and computational tradeoffs in statistical estimation.

---

## 🔵 Part 1: Circle-Based Monte Carlo Method

### 📐 Theoretical Foundation

A unit circle (radius = 1) inscribed in a square of side length 2 has:

- Circle area:  
  $$ A_{\text{circle}} = πr^2 = π $$

- Square area:  
  $$ A_{\text{square}} = (2r)^2 = 4 $$

By randomly generating points in the square and checking if they fall inside the circle:

- The ratio of points inside the circle approaches  
  $$ π/4 $$

- Therefore:  
  $$ π \approx 4 \cdot \frac{\text{Points in circle}}{\text{Total points}} $$

---

## 🧪 Part 2: Buffon’s Needle Simulation

### 📐 Theoretical Foundation

Buffon's Needle experiment estimates π by dropping a needle of length $l$ on a plane with parallel lines spaced $d$ units apart ($l \leq d$).

The probability that the needle crosses a line is:  
$$
P = \frac{2l}{dπ}
$$

Rearranging gives:  
$$
π \approx \frac{2l \cdot N}{d \cdot C}
$$

Where:
- $N$ = total needle drops  
- $C$ = number of times the needle crosses a line

---

## 📈 Deliverables

- Circle Method: Plots of random points with circle overlay
- Buffon’s Needle: Plots of needle positions and crossings
- Convergence plots showing how π estimates improve with more samples
- A comparison of both methods in terms of **accuracy** and **efficiency**

---

## 🌟 Real-World Significance

Monte Carlo methods are used in:
- Physics simulations
- Risk assessment in finance
- AI (random search, Monte Carlo Tree Search)
- Quality control and integration

---

## 🧠 Final Insight

> Monte Carlo methods beautifully illustrate how randomness, probability, and geometry combine to approximate one of the most fundamental constants in mathematics.




![image](https://github.com/user-attachments/assets/85f6840f-248b-4d98-a6bd-21c6f94eb156)




![image](https://github.com/user-attachments/assets/a5c36565-b9cd-4bd8-a4dd-9c0949b9127a)





![image](https://github.com/user-attachments/assets/d873d465-3ec6-4d46-a01a-d5f60331bace)






![image](https://github.com/user-attachments/assets/2d0341a7-892f-43a9-b45f-0673a5d5f0f8)




![image](https://github.com/user-attachments/assets/b77eb437-3cd6-4c8c-8dea-713e9e150c3b)




![image](https://github.com/user-attachments/assets/c9b3ff14-9108-40c7-bc73-36e20a770800)




--------------------------





![image](https://github.com/user-attachments/assets/1b4cc552-a208-424d-beeb-984a1dba2c19)




![image](https://github.com/user-attachments/assets/b7acb5af-b895-49bb-a92e-28787308649a)





![image](https://github.com/user-attachments/assets/82ea31d3-8d73-4043-9e77-3a7508e62a7a)




![image](https://github.com/user-attachments/assets/4d66462c-3559-4633-a771-7a033a16bba8)






![image](https://github.com/user-attachments/assets/d9cd74c6-1a68-442d-bf0e-090c7fded679)






![image](https://github.com/user-attachments/assets/e4317995-ce3e-452a-933b-a6e5bdfbc93a)

