## Giri R (212223060068)
# Attenuation Measurement 2.5 GB & 10 GB
# Attenuation-Limited Fiber Length

## Aim
- Calculate the attenuation-limited fiber length based on the power budget equation.  
- Simulate the resulting system and verify that it meets performance objectives.

---

## Theory
The **power budget equation** states that the power budget in a transmission system must equal the sum of all power losses plus the power margin.  

The power budget is the difference between the transmitter output power and the receiver sensitivity in dBm:

<img width="994" height="468" alt="image" src="https://github.com/user-attachments/assets/28074fe1-e571-4356-bf4c-29cf212c8173" />

In this exercise, all parameters are given except the fiber length, which must be determined.  

The **receiver sensitivity** is defined as the minimum power required to achieve a BER of <img width="54" height="38" alt="image" src="https://github.com/user-attachments/assets/56f53e67-161a-4d53-ba6e-e31a3725ea43" />, corresponding to a Q factor of 6.  
- Receiver sensitivity depends on the bit rate.  
- Fiber attenuation depends on the operating wavelength.  

---

## Pre-lab Calculations
Using the power budget equation and the parameters below, determine the attenuation-limited fiber length:

- **Transmitter output power:** 0 dBm  
- **Operating wavelength:** 1550 nm  
- **Bit rate:** 2.5 Gb/s  
- **Receiver sensitivity:** -30 dBm  
- **Fiber attenuation:** 0.19 dB/km  
- **Number of connectors:** 2  
- **Loss per connector:** 0.5 dB  
- **Additional known losses:** 0 dB  
- **Power margin:** 6 dB  

---

## Layout
- The system has been created using **OptiSystem** and exported as an **OptiPerformer** file.  
- Two versions exist: one for **2.5 Gb/s** and one for **10 Gb/s**.  
- Work with the **2.5 Gb/s** version first.  
- An optical attenuator represents connector loss and system margin.  
- Adjust parameters according to the table above.  
- Dispersion and nonlinear effects in the fiber are disabled.  
- To set the receiver sensitivity to -30 dBm for 2.5 Gb/s, set the **thermal noise parameter** in the receiver to **8.97e-24 W/Hz**.  
- Visualizer components are included to obtain necessary simulation data.  

---

## Simulation
1. Run the simulation and record:
   - **Optical power levels (dBm):**
     - Both ends of fiber  
     - Receiver input  
   - **BER analysis:**
     - BER  
     - Q factor  
     - Eye diagram  

2. Set the fiber length to **125% of the calculated pre-lab value** and repeat the simulation and data recording.  

---

## Analysis and Report
Compare simulation results with pre-lab calculations and record observations.  

Your report should contain:
- **Cover Page**
  - Title of the lab  
  - Course name and number  
  - Your name  



## Graph of 10GB
- **Low Noise:**
  <img width="1920" height="962" alt="image" src="https://github.com/user-attachments/assets/2585a294-1c30-454e-9c22-53f741e0bd26" />
- **High Noise:**
  <img width="1920" height="944" alt="image" src="https://github.com/user-attachments/assets/d275ec34-e2ba-46a8-981d-d0ef1687879e" />
## Graph of 2.5 GB
- **Low Noise:**
  <img width="1920" height="942" alt="image" src="https://github.com/user-attachments/assets/56eb997f-9542-43e9-98cc-7b2e15ac026a" />
- **High Noise:**
  <img width="1920" height="949" alt="image" src="https://github.com/user-attachments/assets/2228ebce-4693-45cd-8b84-e9e4b5e21a0e" />

  


## Tabulation: 
<img width="978" height="1577" alt="image" src="https://github.com/user-attachments/assets/683cefb3-38a8-49ce-a185-4fc749188887" />


## Result:
thus the experiment was succesfully completed and output is verified
