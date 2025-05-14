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




![image](https://github.com/user-attachments/assets/cb7af229-a28c-4950-ba0e-3153fb5e47d9)






![image](https://github.com/user-attachments/assets/3edaf3ba-c62f-43a3-8d30-560dc46cfbd0)







![image](https://github.com/user-attachments/assets/28e0ec63-bfda-4064-80af-d52aaeb99307)








![image](https://github.com/user-attachments/assets/acb9a471-62dc-46d3-9c59-4d4010486ead)







![image](https://github.com/user-attachments/assets/df9a7a38-3a58-4887-92e8-f3b6c7ad7ecc)





****







![image](https://github.com/user-attachments/assets/3fa34e79-b587-434e-b507-ab33dde73188)









![image](https://github.com/user-attachments/assets/f1a2e90f-4082-48a8-9aaa-f3df2d37f4d7)








![image](https://github.com/user-attachments/assets/0df3838c-711b-46b2-965f-6f879fed6de5)









![image](https://github.com/user-attachments/assets/c202c135-9aa2-4977-9e4a-c9019945541a)







![image](https://github.com/user-attachments/assets/2e63eae1-0b18-4880-8f9f-db627e1fe8b6)










![image](https://github.com/user-attachments/assets/8135dc4a-1cc6-4d8f-bd26-d24a2aaeae4d)



****






![image](https://github.com/user-attachments/assets/85cfc774-4291-412f-9283-f81991304fa2)







![image](https://github.com/user-attachments/assets/cb006959-8a50-4582-a3a6-4ac6ce74968a)








![image](https://github.com/user-attachments/assets/e61b0ff4-ae9f-4afd-9edc-0f19f8adbc76)








![image](https://github.com/user-attachments/assets/ce7fb978-f24c-45c0-938b-c7332d596816)









![image](https://github.com/user-attachments/assets/4a403fbd-54e2-4a98-9981-ac3761893de1)
