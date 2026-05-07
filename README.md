# Design-a-2-stage-OpAmp-with-Miller-compensated-capacitor
Design specs: <br>
VDD = 1.8 V, <br>
Gain > 70 dB,<br>
UGB > 8 MHz,<br>
PM ~ 60 degree,<br>
Slew rate ~ 10 V/us,<br>
Load capacitor	CL = 10 pF,<br>

Iref VDD N004 45µ <br>
M1 N004 N004 0 0 NMOS l=1u w=5.07u<br>
M2 N003 N004 0 0 NMOS l=1u w=5.07u<br>
M3 N001 vin1 N003 0 NMOS l=1u w=0.9u<br>
M4 N002 vin2 N003 0 NMOS l=1u w=0.9u<br>
M5 VDD N001 N001 VDD PMOS l=1u w=4.49u<br>
M6 VDD N001 N002 VDD PMOS l=1u w=4.49u<br>
M7 Vout N004 0 0 NMOS l=1u w=18u<br>
M8 VDD N002 Vout VDD PMOS l=1u w=31u<br>
.model nmos nmos (vto=0.169V lambda=0.04 kp=296u)<br>
.model pmos pmos (vto=-0.136V lambda=0.05 kp=167u)<br>
Topology:
<img width="936" height="606" alt="image" src="https://github.com/user-attachments/assets/13800a88-50d0-4ceb-b347-8243065f1130" />
<br>
Schematic:
<img width="769" height="369" alt="image" src="https://github.com/user-attachments/assets/e12e5db3-0426-48a6-86dc-5f74f1b6aa8e" />
<br>
Simulation result: 
<img width="1015" height="446" alt="image" src="https://github.com/user-attachments/assets/f6ca8069-03b3-4cd8-a851-626f3b19b759" />
<img width="1015" height="571" alt="image" src="https://github.com/user-attachments/assets/87a9ae43-c167-46ff-930d-5b1982437e1e" />



