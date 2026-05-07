# Design-a-2-stage-OpAmp-with-Miller-compensated-capacitor
Design specs:
VDD = 1.8 V,
Gain > 70 dB,
UGB > 8 MHz,
PM ~ 60 degree,
Slew rate ~ 10 V/us,
Load capacitor	CL = 10 pF,
#M1 N004 N004 0 0 NMOS l=1u w=5.07u
#M2 N003 N004 0 0 NMOS l=1u w=5.07u
#Iref VDD N004 45µ
#M3 N001 vin1 N003 0 NMOS l=1u w=0.9u
#M4 N002 vin2 N003 0 NMOS l=1u w=0.9u
#M5 VDD N001 N001 VDD PMOS l=1u w=4.49u
#M6 VDD N001 N002 VDD PMOS l=1u w=4.49u
#M7 Vout N004 0 0 NMOS l=1u w=18u
#Cc Vout N002 3p
#M8 VDD N002 Vout VDD PMOS l=1u w=31u
#Cl Vout 0 10p
#.model nmos nmos (vto=0.169V lambda=0.04 kp=296u)
#.model pmos pmos (vto=-0.136V lambda=0.05 kp=167u)
Topology:
<img width="936" height="606" alt="image" src="https://github.com/user-attachments/assets/13800a88-50d0-4ceb-b347-8243065f1130" />
Simulation result:
<img width="1015" height="446" alt="image" src="https://github.com/user-attachments/assets/f6ca8069-03b3-4cd8-a851-626f3b19b759" />
<img width="1015" height="571" alt="image" src="https://github.com/user-attachments/assets/87a9ae43-c167-46ff-930d-5b1982437e1e" />



