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





![image](https://github.com/user-attachments/assets/14353eb2-e4e6-46fc-9f0a-2036deb535c6)






![image](https://github.com/user-attachments/assets/e52742ca-d8fb-44a5-81f9-83cbc9b898b3)






![image](https://github.com/user-attachments/assets/ec79f9b9-381e-4075-a257-32879c755308)






![image](https://github.com/user-attachments/assets/2b8406ff-3a90-4c68-b65a-fd900ef75519)







![image](https://github.com/user-attachments/assets/39c7eeac-62bb-4993-890b-d517160aae8b)







![image](https://github.com/user-attachments/assets/55d0876f-317e-4a5b-8318-8272e4d37612)








![image](https://github.com/user-attachments/assets/8425cb4d-af97-4c38-b39d-85c7b70d18bf)







![image](https://github.com/user-attachments/assets/d84480d9-c880-4133-8353-4376efd2f316)





### 🔗 Falstad Simulation Link

You can view the circuit in the Falstad Circuit Simulator here:

[Open in Falstad](https://tinyurl.com/22q6m5yy)








![image](https://github.com/user-attachments/assets/552e3eb3-f43a-4644-9c45-8dacb346ae64)









![image](https://github.com/user-attachments/assets/65a8df13-0172-47e7-ba50-b881239edfbc)









![image](https://github.com/user-attachments/assets/6347cbf8-92ac-42fa-8118-ceb587bc7698)









![image](https://github.com/user-attachments/assets/bba76d98-aa01-4170-a20a-6481ec379638)









![image](https://github.com/user-attachments/assets/e727ee15-b389-454e-b4e4-3c45bf36cf0a)









![image](https://github.com/user-attachments/assets/b911faec-9462-4aa6-ae05-23625ea2b4ac)









![image](https://github.com/user-attachments/assets/e6c4ca10-47b4-4065-95ac-a0e8e47cc584)









![image](https://github.com/user-attachments/assets/d2de8654-83eb-4749-99c0-9d588f84b2c1)





### 🔗 Falstad Simulation Link

You can view the circuit in the Falstad Circuit Simulator here:

[Open in Falstad](https://tinyurl.com/2d6vmf9v)




