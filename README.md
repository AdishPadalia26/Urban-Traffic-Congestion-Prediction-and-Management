# Urban-Traffic-Congestion-Prediction-and-Management 

[Research paper](https://ieeexplore.ieee.org/document/10724090)

This project proposes an AI-powered framework for predicting and managing traffic congestion in urban environments. By integrating Gated Recurrent Unit models, Vehicle-to-Infrastructure communication, and SUMO-based simulation, the framework aims to optimize traffic signals and reduce congestion in real time.

## Technology Stack Used

| Category                     | Technology/Tool                                                             |
| ---------------------------- | --------------------------------------------------------------------------- |
| **Programming Language**     | Python                                                                      |
| **Deep Learning Framework**  | TensorFlow / PyTorch                                                        |
| **Model Architecture**       | Gated Recurrent Unit (GRU)                                                  |
| **Traffic Simulation**       | SUMO (Simulation of Urban Mobility)                                         |
| **Communication Protocols**  | Vehicle-to-Infrastructure (V2I), Dedicated Short Range Communication (DSRC) |
| **Data Processing**          | NumPy, Pandas                                                               |
| **Visualization**            | Matplotlib, Seaborn                                                         |
| **Machine Learning**         | Scikit-learn                                                                |
| **Simulation Input Mapping** | OpenStreetMap, GIS Data                                                     |

## Model Implementation

### 1. GRU Model Architecture
This diagram illustrates the internal workings of the Gated Recurrent Unit (GRU) used for traffic prediction. It shows how the update gate and reset gate manage the flow of sequential information, enabling the model to capture temporal dependencies in urban traffic data.

![image](https://github.com/user-attachments/assets/155a4559-fad9-487e-ba7f-3590392bc0bb)

### 2. V2I Communication Flow
A representation of Vehicle-to-Infrastructure (V2I) communication, where vehicles exchange real-time data with roadside units (RSUs). This enables adaptive signal control based on current traffic conditions.

![image](https://github.com/user-attachments/assets/eaec2993-d367-411b-a7b8-c14d37113fa3)

### 3. DSRC Communication
This figure shows how Dedicated Short Range Communication (DSRC) facilitates both V2V (vehicle-to-vehicle) and V2I interactions. DSRC helps in collision avoidance, traffic signal optimization, and real-time data sharing.

![image](https://github.com/user-attachments/assets/825121a7-cdbc-4d1b-b223-469b8239273a)

### 4. SUMO Traffic Simulation Flow
A flowchart describing the steps in SUMO simulation—from importing GIS data, defining traffic demand, integrating the GRU prediction model, to real-time signal adjustments via V2I. It validates the effectiveness of the proposed approach.

![image](https://github.com/user-attachments/assets/d46c7408-cc4c-4eef-876e-3819fb318e65)

### 5. GRU Prediction vs. Actual Traffic Data (Junction-wise)
These graphs compare predicted traffic volumes from the GRU model with actual recorded values for different junctions. The close alignment between the two lines indicates high predictive accuracy, validating the model's effectiveness.

![image](https://github.com/user-attachments/assets/018a2e91-6174-407f-b570-1921c1a1ced5)
![image](https://github.com/user-attachments/assets/107f29bc-b1bd-4ba1-afc5-5c6b42a7205b)

### 6. Traditional vs. V2I Traffic Light Control (Same Traffic Density)
When all lanes have similar traffic volume, V2I-based adaptive signaling distributes green light time more efficiently compared to traditional phase-fixed control, reducing wait time and improving flow.

![image](https://github.com/user-attachments/assets/5f3a9109-7369-4bb2-bd4d-aba58c9f6837)
![image](https://github.com/user-attachments/assets/b7f5b389-5162-4a76-be95-014c5d870997)

### 7. Traditional vs. V2I Traffic Light Control (Unbalanced Density)
Under uneven traffic conditions, V2I significantly outperforms fixed-time lights by allocating longer green phases to congested lanes. This dynamic control helps avoid gridlocks and balances traffic distribution.

![image](https://github.com/user-attachments/assets/a8a12498-b9d7-4ee8-9ff7-fa23487dbdc3)
![image](https://github.com/user-attachments/assets/174ce446-1170-4c5d-9261-42ddd942d973)

## Future Scope
This project lays the groundwork for a scalable intelligent traffic management system, and future enhancements could include emergency vehicle prioritization through V2I signaling, integration of additional sensor data, and deployment in real-world smart city scenarios.

---

## References

- [Urban Traffic Congestion Prediction and Management Paper - IEEE Xplore](https://ieeexplore.ieee.org/document/10724090)
