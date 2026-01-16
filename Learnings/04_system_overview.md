## Wireless Power Transfer – System Overview


<img width="687" height="628" alt="image" src="https://github.com/user-attachments/assets/fdd85d05-5a58-4246-8724-f0e99a7623d3" />


- Wireless power transfer in this project is based on electromagnetic induction.
- Electrical energy is converted into magnetic energy at the transmitter side and then converted back into electrical energy at the receiver side.

The system consists of:
- A **transmitter coil** connected to a high-frequency AC inverter
- A **receiver coil** mounted on the vehicle
- **Power conditioning circuits** (rectifier, filter, regulator) on the receiver side

The overall behavior of the system is similar to a **transformer without a magnetic core**, resulting in **loose coupling**, flux leakage, and reduced efficiency compared to wired charging.

“The system uses electromagnetic induction, where high-frequency AC energizes a transmitter coil to create a magnetic field. A receiver coil mounted on the vehicle induces AC voltage from this field, which is rectified and regulated for charging. The system behaves like a transformer without a magnetic core, so coupling is loose and efficiency is lower.”
