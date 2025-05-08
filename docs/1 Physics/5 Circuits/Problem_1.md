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



![image](https://github.com/user-attachments/assets/c4778c16-8887-4365-a705-46bd8e8ca5c1)








![image](https://github.com/user-attachments/assets/a6c74389-b9df-45a8-9d56-9c698cf5dde5)













![image](https://github.com/user-attachments/assets/6b6e93fc-5cab-4288-b3c9-d5701e41853f)













![image](https://github.com/user-attachments/assets/94ed1029-fe05-48ee-8e2f-85c33a90201e)











![image](https://github.com/user-attachments/assets/7139a272-e9ac-4a7b-8371-5ab90371b758)












### 🔗 Falstad Simulation Link

You can view the circuit in the Falstad Circuit Simulator here:


[Open in Falstad](https://tinyurl.com/2yjth3ga)











![image](https://github.com/user-attachments/assets/247e0309-ac74-4c7b-876e-8baf09f8bfb5)















![image](https://github.com/user-attachments/assets/bc6051bf-f573-408f-be8b-6abf7d0d5e5b)












![image](https://github.com/user-attachments/assets/193f48d1-9efe-4ea9-a2f0-1877ea6b10ee)











![image](https://github.com/user-attachments/assets/de95ea72-2778-47d2-9966-11f58e692bbe)












![image](https://github.com/user-attachments/assets/b75811fd-6af3-4d6c-9f5d-841520f85954)
















![image](https://github.com/user-attachments/assets/745bc438-6a2d-4a07-8daf-6a770ee6dfa3)







### 🔗 Falstad Simulation Link

You can view the circuit in the Falstad Circuit Simulator here:

[Open in Falstad](https://tinyurl.com/2b3v9p88)




