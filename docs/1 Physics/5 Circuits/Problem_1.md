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



Initial circuit graph:
Edge 1-2: 2.0Ω


Edge 1-4: 1.0Ω


Edge 2-3: 3.0Ω


Edge 3-4: 4.0Ω


Series reduction at node 2: 2.0Ω + 3.0Ω = 5.0Ω


Series reduction at node 3: 4.0Ω + 5.0Ω = 9.0Ω


Equivalent resistance between nodes 1 and 4: 9.0Ω






![image](https://github.com/user-attachments/assets/6e44ec63-df4a-4821-a74c-2e873794a11c)









--- Series Configuration Example ---
Before simplification:
o1–o2: 5 Ω
o2–o3: 3 Ω



![image](https://github.com/user-attachments/assets/847d778c-5fe5-4d8f-b514-2221605e8f40)









Series reduction: o1–o2–o3 → o1–o3 = 5 + 3 = 8 Ω
After simplification:
o1–o3: 8 Ω



![image](https://github.com/user-attachments/assets/ff539206-bd5f-4db6-a1e2-dec927daae16)










--- Parallel Configuration Example ---
Before simplification:
o1–o3 (key=0): 4 Ω
o1–o3 (key=1): 6 Ω




![image](https://github.com/user-attachments/assets/8a57bf28-a3eb-4084-8752-2c520b054520)










Parallel reduction: o1 ⇄ o3 → 1/4 + 1/6 = 1/2.40 Ω
After simplification:
o1–o3 (key=0): 2.4 Ω





![image](https://github.com/user-attachments/assets/6459fe1a-73a7-4a1d-970c-2baca31cbd15)







--- Mixed Configuration Example ---
Initial mixed circuit:
1–2: 2 Ω
2–3: 3 Ω
2–4: 6 Ω
3–4: 6 Ω
4–5: 1 Ω





![image](https://github.com/user-attachments/assets/a3bff879-be64-40fc-abe2-838cc3d6107d)








Step 1: Parallel between 2–4 and 3–4 → Req = 3Ω



![image](https://github.com/user-attachments/assets/d3a95d69-5a9e-444f-aa73-30a4da52598c)







Step 2: Series → 2–3 (3Ω) + 2–4 (3Ω) = 6Ω



![image](https://github.com/user-attachments/assets/2bb0d635-4419-4bd0-8b12-9676c37a8cf9)







Step 3: Series → 1–2 + 2–4 + 4–5 = 2 + 6 + 1 = 9Ω


Final equivalent resistance between 1 and 5 = 9 Ω

































































