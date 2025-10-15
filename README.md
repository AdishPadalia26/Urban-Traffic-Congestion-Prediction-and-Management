# Traffic-Congestion-Prediction-and-Management
This project proposes an AI-powered framework for predicting and managing traffic congestion in urban environments. By integrating Gated Recurrent Unit models, Vehicle-to-Infrastructure communication via DSRC, and SUMO-based traffic simulations, the system delivers accurate congestion forecasts and real-time signal optimization. Achieving over 85% prediction accuracy and 91% traffic management efficiency, the solution promotes sustainable mobility, reduced travel times, and smart city infrastructure readiness.

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
This diagram illustrates the internal workings of the Gated Recurrent Unit (GRU) used for traffic prediction. It shows how the update gate and reset gate manage the flow of sequential information, allowing the model to learn long-term dependencies in traffic patterns efficiently.

![image](https://github.com/user-attachments/assets/155a4559-fad9-487e-ba7f-3590392bc0bb)


### 2. V2I Communication Flow
A representation of Vehicle-to-Infrastructure (V2I) communication, where vehicles exchange real-time data with roadside units (RSUs). This enables adaptive signal control based on current traffic conditions, improving traffic flow and safety.

![image](https://github.com/user-attachments/assets/eaec2993-d367-411b-a7b8-c14d37113fa3)


### 3. DSRC Communication
This figure shows how Dedicated Short Range Communication (DSRC) facilitates both V2V (vehicle-to-vehicle) and V2I interactions. DSRC helps in collision avoidance, traffic signal optimization, and cruise control synchronization.

![image](https://github.com/user-attachments/assets/825121a7-cdbc-4d1b-b223-469b8239273a)


### 4. SUMO Traffic Simulation Flow
A flowchart describing the steps in SUMO simulation—from importing GIS data, defining traffic demand, integrating the GRU prediction model, to real-time signal adjustments via V2I. It validates how simulated traffic responds to intelligent management strategies.

![image](https://github.com/user-attachments/assets/d46c7408-cc4c-4eef-876e-3819fb318e65)


### 5. GRU Prediction vs. Actual Traffic Data (Junction-wise)
These graphs compare predicted traffic volumes from the GRU model with actual recorded values for different junctions. The close alignment between the two lines indicates high predictive accuracy, validating the model’s effectiveness.

![image](https://github.com/user-attachments/assets/018a2e91-6174-407f-b570-1921c1a1ced5)

![image](https://github.com/user-attachments/assets/107f29bc-b1bd-4ba1-afc5-5c6b42a7205b)


### 6. Traditional vs. V2I Traffic Light Control (Same Traffic Density)
When all lanes have similar traffic volume, V2I-based adaptive signaling distributes green light time more efficiently compared to traditional phase-fixed control, reducing wait time and improving throughput.

![image](https://github.com/user-attachments/assets/5f3a9109-7369-4bb2-bd4d-aba58c9f6837)

![image](https://github.com/user-attachments/assets/b7f5b389-5162-4a76-be95-014c5d870997)


### 7. Traditional vs. V2I Traffic Light Control (Unbalanced Density)
Under uneven traffic conditions, V2I significantly outperforms fixed-time lights by allocating longer green phases to congested lanes. This dynamic control helps avoid gridlocks and balances traffic distribution more effectively.

![image](https://github.com/user-attachments/assets/a8a12498-b9d7-4ee8-9ff7-fa23487dbdc3)

![image](https://github.com/user-attachments/assets/174ce446-1170-4c5d-9261-42ddd942d973)

## Future Scope
This project lays the groundwork for a scalable intelligent traffic management system, and future enhancements could include emergency vehicle prioritization through V2I signaling, integration of IoT sensors for real-time monitoring, and robust cybersecurity measures to ensure secure data exchange. Additionally, deploying the system in live urban environments will help evaluate its real-world effectiveness and scalability. Further research could explore advanced deep learning models like Transformers, dynamic route suggestion systems for drivers, and the use of smart infrastructure to enhance urban mobility and sustainability.






