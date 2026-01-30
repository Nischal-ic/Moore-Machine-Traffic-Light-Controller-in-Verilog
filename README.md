# Moore-Machine Traffic Light Controller in Verilog
*The purpose of this project is to develop a Verilog-based traffic control system for a T-shaped road with specified timing delays.*
# Introduction
This project implements a **Moore Finite State Machine (FSM)** to control traffic signals at a **T-shaped / 2-way junction**. The controller manages **North–South (NS)** and **East–West (EW)** traffic using standard **green, yellow, and red** signal sequences with fixed timing.

---

## Design Methodology
- Modeled the controller as a **Moore FSM**, where outputs depend only on the current state  
- Defined multiple states representing **Green, Yellow, and Red** signals  
- Implemented **counter-based timing** for state transitions  
- Used synchronous reset for reliable initialization  

---

## FSM Description
- Each state corresponds to a specific traffic signal configuration  
- Fixed delays ensure safe transitions between traffic directions  
- After completing all states, the FSM loops back to the initial state

   ## Logic Diagram
  ! [Logic Diagram]<img width="1045" height="471" alt="Logic_Diagram" src="https://github.com/user-attachments/assets/58a2d3c2-b425-4ddd-aa83-0c66aa5bdcb4" />


---

## State Diagram
The FSM consists of sequential states that control traffic movement across:
- Main road
- Turn road
- Side road
  

<img width="810" height="467" alt="State_Diagram_project" src="https://github.com/user-attachments/assets/28f19c1d-6ff5-42b1-ada9-1022cac14025" />

---

## Tools & Technologies
- **Language:** Verilog HDL  
- **Design Style:** RTL Design  
- **Simulation Tool:** Xilinx Vivado / ModelSim  
- **Concepts Used:** FSM design, counters, sequential logic  

---

## Testbench & Verification
- Developed a Verilog testbench to verify FSM operation  
- Simulated clock, reset, and state transitions  
- Verified correct output behavior using waveform analysis

## Output Waveforms
<img width="625" height="250" alt="image" src="https://github.com/user-attachments/assets/804d842a-9352-4ed8-a2dd-e58ff15d1fce" />


---

## Results
The traffic light controller successfully regulates traffic flow across all directions using fixed timing control. Each signal transitions correctly between green, yellow, and red states, ensuring safe and orderly movement of vehicles.

Simulation results validate the correctness of FSM operation and timing logic. The design demonstrates a reliable approach for implementing traffic control systems using Verilog HDL.

---

## How to Run
1. Open the project in Xilinx Vivado  
2. Add RTL and testbench files  
3. Run behavioral simulation  
4. Observe state transitions and output waveforms  

---

## Future Work

- Integration of **traffic density sensors** for adaptive timing  
- Power-efficient operation using **sensor-based signal control**  
- Expansion to **multi-road (4-way or 8-way) junctions**  
- Emergency vehicle prioritization and smart city integration 

---

## Author
**Nischal Agarwal**  
Electronics and Communication Engineering  
Birla Institute of Technology, Mesra




