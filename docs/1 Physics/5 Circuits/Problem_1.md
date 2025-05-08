# Problem 1

# 🔌 Problem 1: Equivalent Resistance Using Graph Theory

<div style="background-color: #f0f8ff; padding: 15px; border-radius: 10px;">
<h2 style="color: #2E86C1; text-align: center;">📐 Visualizing Circuit Simplification Step-by-Step</h2>
</div>

---

## 🎯 Motivation

Calculating equivalent resistance is a fundamental task in circuit analysis. While series and parallel rules work well for simple circuits, **graph theory** provides a powerful, automated way to analyze **complex resistor networks**.

A circuit is modeled as a graph:
- **Nodes** represent junctions
- **Edges** represent resistors (with weights equal to resistance)

---

## 🧠 Approach

We reduce the graph step by step using:

1. 🔗 **Series Reduction**  
   Two resistors in a chain become one with total resistance:  
   $$ R_{\text{eq}} = R_1 + R_2 $$

2. 🔁 **Parallel Reduction**  
   Two or more resistors between the same nodes:  
   $$ \frac{1}{R_{\text{eq}}} = \frac{1}{R_1} + \frac{1}{R_2} + \cdots $$

3. 🔄 Repeat until the entire network reduces to a single equivalent resistance.

---

## 🧮 Example Circuit

A simple 4-node graph with resistors:

- 2Ω between nodes (1)-(2)  
- 3Ω between nodes (2)-(3)  
- 4Ω between nodes (3)-(4)  
- 1Ω directly between nodes (1)-(4)

---

## ⚙️ Algorithm Pseudocode


while graph not reduced:
 ///
    if a node has exactly 2 neighbors:
        combine series resistors
 ///       
    if parallel resistors exist:
        combine using reciprocal rule







![image](https://github.com/user-attachments/assets/a35f353d-14b2-48df-9fb6-01356d65398d)









![image](https://github.com/user-attachments/assets/125b4b91-e407-4a75-8d79-c8169b630316)










![image](https://github.com/user-attachments/assets/f9e9ac9e-0bab-4fd2-95e3-38eb00653eba)









![image](https://github.com/user-attachments/assets/585dacf7-3a05-471f-9e5d-b9259af1ff21)

