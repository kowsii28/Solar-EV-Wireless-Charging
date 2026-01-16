# Solar-EV-Wireless-Charging
DIploma project key takeaways

### Repository Structure
```      
│
├── Learnings
│   ├── 01_solar_panel.md
│   ├── 02_battery.md
│   ├── 03_inverter.md
│   ├── 04_system_overview.md
│   ├── 05_transmitter_coil.md
│   ├── 06_receiver_coil.md
│
├── Report
│ └── EV_PROJECT_REPORT.pdf  
│
└── README.md  
```



# Solar-Assisted Wireless EV Charging System

## Project Overview
This project demonstrates a prototype of a **static wireless charging system for electric vehicles** using **electromagnetic induction** and **solar-assisted power input**.

The goal of the project is to understand how renewable energy, power electronics, and wireless power transfer can be integrated for EV charging without physical connectors.

---



## Problem Statement
Conventional EV charging requires physical cables, which:
- Cause wear and tear
- Are inconvenient in outdoor environments
- Human assistance needed

Wireless charging provides a safer and more convenient alternative methods which provides new way for charging the EV's.

---



## System Flow 
1. Sunlight is converted into electrical energy using a solar panel
2. Generated DC power is stored in a battery
3. Battery DC is converted into high-frequency AC using an inverter
4. AC energizes a transmitter coil to create a magnetic field
5. A receiver coil on the vehicle induces AC voltage
6. Induced power is rectified, regulated, and used to charge the battery
7. Arduino monitors and displays charging status

---


## Key Features
- Contactless power transfer
- Solar-assisted energy source
- Embedded control using Arduino
- Safe charging with regulation
- LCD-based status display

---



## Important Note
This is a **static wireless charging prototype**.  
Charging is performed **only when the vehicle is stationary**.  
Dynamic charging while the vehicle is in motion is considered **future scope** and was not implemented.

---



## Components used
- Solar Panel
- Rechargeable Battery
- Inverter (DC–AC)
- Inductive Coils
- Rectifier & Voltage Regulator
- Arduino UNO
- IR Sensor
- LCD Display

---



## Learning Outcome
This project helped me gain practical understanding of:
- Photovoltaic energy conversion
- Battery charging mechanisms
- Inverter operation
- Wireless power transfer principles
- Embedded system control
- System-level engineering design

---



## Future Scope
- Dynamic wireless charging using road-embedded coils
- Higher power transfer efficiency
- Automatic coil alignment
- Smart EV charging integration

