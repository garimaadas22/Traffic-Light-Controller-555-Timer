# 🚦 Traffic Light Controller — 555 Timer IC (No Arduino, No Code)

## 📌 Overview

A fully hardware-based **Traffic Light Controller** designed and simulated in **Tinkercad**, using **555 Timer ICs** to automate the sequential switching of **Red, Yellow, and Green LEDs** — no microcontroller, no programming required.

This project demonstrates core electronics concepts like **astable multivibrator operation**, **pulse generation**, and **timing control** using only passive and discrete components.

---

## ⚙️ How It Works

Two **555 Timer ICs** are configured in **astable mode** to generate continuous clock pulses. These pulses drive the LEDs in a timed sequence that mimics a real-world traffic signal:

| Phase  | LED    | Meaning          |
|--------|--------|------------------|
| 🔴 Stop  | Red    | Vehicles stop    |
| 🟡 Ready | Yellow | Prepare to move  |
| 🟢 Go    | Green  | Vehicles proceed |

The timing intervals (on/off durations) are set by **RC networks** (resistors + capacitors) connected to each 555 timer, giving full control over how long each LED stays on — no firmware needed.

---

## 🧰 Components Used

| Component         | Quantity | Purpose                          |
|-------------------|----------|----------------------------------|
| 555 Timer IC      | 2        | Pulse generation & timing        |
| Red LED           | 1        | Stop signal                      |
| Yellow LED        | 1        | Caution/ready signal             |
| Green LED         | 1        | Go signal                        |
| Resistors         | Multiple | Current limiting & RC timing     |
| Capacitors        | 2        | RC timing network per 555 timer  |
| Breadboard        | 1        | Prototyping                      |
| Power Supply (9V) | 1        | Circuit power                    |
| Connecting Wires  | —        | Connections                      |

---

## 🔌 Circuit Design Highlights

- **Astable Mode** — Both 555 timers run continuously, producing a square wave output without any external trigger.
- **Sequential LED control** — Timer outputs are cascaded/combined so only one LED is active at a time, replicating real traffic light phasing.
- **No microcontroller** — Pure analog/digital logic via ICs and passive components.


## 🖥️ Simulation

Designed and simulated using **[Tinkercad]**

> You can fork and run the simulation directly in Tinkercad to observe the LED sequencing in real time.


##  Circuit Diagram

The breadboard layout includes:
- Power rails (red/blue) feeding both 555 ICs
- RC networks on each timer for independent timing
- LED outputs with current-limiting resistors
- Cross-connections between timer stages for phase sequencing

---

## 💡 Concepts Demonstrated

- 555 Timer IC in astable configuration
- RC time constant and frequency calculations
- Pulse width modulation basics
- Sequential logic without a processor
- Practical traffic signal automation

---

### Simulate Online
1. Open [Tinkercad](https://www.tinkercad.com/)
2. Import or recreate the circuit from the schematic
3. Click **Start Simulation** to watch the LEDs cycle


### Build on Hardware
1. Gather all components listed above
2. Assemble on a breadboard following the circuit diagram
3. Power with a 9V battery or DC supply
4. Adjust R/C values to change timing durations


## Author

**Garimaa Das**
- Built using Tinkercad
- No Arduino. No code. Pure hardware logic.


> *"The best code is no code at all."* — This project takes that literally.
