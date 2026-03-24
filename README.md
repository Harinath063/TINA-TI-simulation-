# 555 Timer Astable Multivibrator Simulation (TINA-TI)

## 📌 Project Overview

This project demonstrates the design and simulation of an **Astable Multivibrator** using the **555 Timer IC** in **TINA-TI (Texas Instruments Analog Simulator)**.

An astable multivibrator is a free-running oscillator that continuously generates a square wave without any external triggering. This project helps in understanding timing circuits, waveform generation, and frequency control.

---

## 🎯 Objectives

* To design an astable multivibrator using 555 Timer IC
* To simulate the circuit in TINA-TI
* To observe output waveform and timing characteristics
* To analyze frequency and duty cycle

---

## 🛠️ Software Used

* **TINA-TI** by Texas Instruments

---

## 🔧 Components Used

* 555 Timer IC
* Resistors (R1, R2)
* Capacitor (C)
* Power Supply (Vcc)
* Oscilloscope (for waveform observation)

---

## ⚙️ Circuit Description

The 555 Timer is configured in **Astable Mode**, where it continuously switches between HIGH and LOW states.

### Connections:

* Pin 1 → Ground
* Pin 2 → Trigger (connected to Pin 6)
* Pin 3 → Output
* Pin 4 → Reset (connected to Vcc)
* Pin 5 → Control Voltage (optional capacitor to ground)
* Pin 6 → Threshold (connected to Pin 2)
* Pin 7 → Discharge (connected between R1 and R2)
* Pin 8 → Vcc

---

## 📐 Working Principle

* Capacitor charges through R1 and R2
* Capacitor discharges through R2
* Output switches HIGH during charging
* Output switches LOW during discharging

This continuous charging and discharging produces a square wave output.

---

## 📊 Mathematical Analysis

Time HIGH:
t_high = 0.693 × (R1 + R2) × C

Time LOW:
t_low = 0.693 × R2 × C

Total Time Period:
T = 0.693 × (R1 + 2R2) × C

Frequency:
f = 1 / T

Duty Cycle:
D = [(R1 + R2) / (R1 + 2R2)] × 100

---

## 📈 Simulation Results

* Output waveform observed is a **square wave**
* Capacitor voltage shows **charging and discharging curve**
* Frequency depends on R1, R2, and C values

---

## 🔍 Observations

* Increasing capacitor value decreases frequency
* Increasing resistance increases time period
* Duty cycle is always greater than 50% in basic astable mode

---

## 🚀 Applications

* LED blinking circuits
* Pulse generation
* Clock signals
* Tone/sound generation
* PWM applications

---

## ⚠️ Limitations

* Duty cycle cannot be exactly 50% without modification
* Frequency stability depends on component tolerances

---

## 📁 How to Run the Simulation

1. Open TINA-TI software
2. Create a new circuit
3. Place 555 Timer IC from components
4. Connect resistors and capacitor as per astable configuration
5. Add oscilloscope
6. Run transient analysis
7. Observe waveform

---

## 📌 Future Improvements

* Modify circuit for 50% duty cycle
* Add variable resistor for frequency control
* Interface with microcontroller for advanced applications

---

## 👨‍💻 Author

V.Venkata Harinath
ECE Diploma 2nd year 
SVGP TIRUPATI.

---

## 📜 License

This project is for educational purposes.
