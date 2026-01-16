## Inverter – DC to AC Conversion

Wireless power transfer requires a changing magnetic field, which cannot be produced by DC. Therefore, an inverter is used.

The inverter converts DC power from the battery into high-frequency AC using MOSFET-based switching.


<img width="1372" height="1044" alt="image" src="https://github.com/user-attachments/assets/90931fb1-4271-4ff6-871f-7c51fa9de0d4" />

### IC555 Timer
- NE555 is used in astable mode
- It generates a square-wave pulse
- This pulse is used to turn MOSFETs ON and OFF
- “The NE555 timer generates a continuous square-wave signal that controls the MOSFET switching in the inverter.”

**NE555 is NOT a power device. It is only a signal generator (oscillator).**

### Frequency Generation 

Frequency is decided by:
- Two resistors
- One capacitor

Formula:

```

f ≈ 1.44 / ((R1 + 2R2) × C)

```
Why frequency matters

- Low frequency (50 Hz) → used for mains inverter
- Higher frequency (kHz) → better for:
           Smaller coils
           Better magnetic coupling
           Wireless power transfer

📌 For my project
DON’T care about 50 Hz accuracy
care about high-frequency switching

### MOSFETs as Power Switches (CORE IDEA)

What MOSFETs do in the circuit

- NE555 output → MOSFET Gate
- MOSFET switches battery power ON/OFF
- Handles high current, unlike NE555
- “MOSFETs are used as high-speed electronic switches to handle the power required by the inverter.”

  
📌 Key takeaway
- NE555 controls → MOSFET switches → power flows

### Why Two MOSFETs Are Used (Push–Pull Action)


In the circuit -> Two MOSFETs switch alternately

Current flows:
- First in one direction
- Then in opposite direction
- This creates AC output from DC input.
- Alternating switching = alternating current

### Transformer / Load Connection

In wireless charging project

- Replace transformer primary with transmitter coil
- Do not need step-up voltage
- Need alternating current through the coil
- In this project, the transmitter coil acts as the inverter load instead of a step-up transformer.

### Square Wave Output Is ACCEPTABLE

- Output is square wave. So there is no pure sine wave

Wireless power transfer needs:
- Changing magnetic field
- Not waveform purity
- “Square-wave AC is sufficient for inductive wireless power transfer in prototype systems.”

### Working Principle

- DC from the battery is applied to MOSFET switches which changes its position very rapidly
- MOSFETs turn ON and OFF rapidly & produces high-frequency AC (square wave)
- Switching action chops DC into alternating pulses
- The output waveform is a high-frequency square wave
- Square wave AC is sufficient to create a changing magnetic field
- High frequency improves magnetic coupling between coils

### Output
- Type: AC
- Frequency: Few kHz to tens of kHz


### Key Point
The inverter does not generate energy.  
It only changes the **form** of electrical energy from DC to AC.
