# Battery-Level-Indicator

12V Battery Voltage Level Indicator using LM3914N

## 📌 Project Overview

This project is a **12V Battery Voltage Level Indicator** designed using the **LM3914N LED display driver IC**. The circuit monitors the voltage of a 12V battery and displays the approximate voltage level using **10 LEDs**.

Different LED colors are used to make the battery level easy to understand visually. The complete schematic and PCB are designed using **KiCad**.

---

## 🎯 Objective

The main objective of this project is to design a simple and useful circuit that:

- Monitors the voltage of a 12V battery.
- Displays the battery voltage level using 10 LEDs.
- Provides a visual indication of low, medium, and high battery voltage.
- Uses the LM3914N LED display driver.
- Can be converted into a PCB using KiCad.

---

## 🧩 Components Used

| Reference | Component | Value / Description |
|-----------|-----------|---------------------|
| U1 | LM3914N | LED Display Driver |
| B1 | Battery | 12V Battery |
| J1 | 2-Pin Connector | Battery Connector |
| RV1 | Potentiometer | 10kΩ |
| R1 | Resistor | 4.7kΩ |
| R2 | Resistor | 56kΩ |
| R3 | Resistor | 18kΩ |
| R4 | Resistor | 18kΩ |
| D1 | LED | Red |
| D2 | LED | Red |
| D3 | LED | Orange |
| D4 | LED | Orange |
| D5 | LED | Yellow |
| D6 | LED | Yellow |
| D7 | LED | Green |
| D8 | LED | Green |
| D9 | LED | Blue |
| D10 | LED | Blue |

---

## ⚙️ Working Principle

The **LM3914N** is a linear LED display driver IC capable of controlling ten LED outputs according to an input voltage.

The voltage from the 12V battery is applied to the sensing circuit and then to the **SIG input** of the LM3914N. The IC compares the input voltage with its reference voltage range.

Depending on the input voltage, the LM3914N activates the corresponding LED outputs.

The circuit can operate in two display modes:

- **Dot Mode:** Only one LED is ON at a time.
- **Bar Mode:** LEDs turn ON progressively as the battery voltage increases.

This provides a simple visual indication of the battery voltage level.

---

## 🔌 Battery Connection

A 2-pin connector is used to connect the 12V battery.

```text
J1 Pin 1 → Battery Positive (+)
J1 Pin 2 → Battery Negative (-)
