# AC–DC Converter

An AC–DC converter designed and simulated using LTspice.

## Project Overview

The project focuses on converting a sinusoidal AC input into a regulated DC output of approximately 5 V. The circuit was evaluated through transient simulations under different load resistances and operating temperatures.

## Design Specifications

- **Simulation tool:** LTspice
- **Input signal:** 3.5 V amplitude, 1 kHz sinusoid
- **Target DC output:** 5–5.2 V
- **Analysis:** Transient response, load variation, and temperature sweep

## Simulation Results

### Load Variation

| Load Resistance | Average Output Voltage | Peak-to-Peak Ripple | Ripple Percentage |
|---|---:|---:|---:|
| 1 kΩ | 5.0211 V | 27.6 mV | 0.55% |
| 2.5 kΩ | 5.0846 V | 1.7 mV | 0.03% |
| 5 kΩ | 5.0877 V | 1.2 mV | 0.02% |

For all three simulated load conditions, the average output voltage remained within the specified range, and the output ripple was below 1%.

### Temperature Analysis

With a 5 kΩ load, the simulated average output voltage varied as follows:

| Temperature | Average Output Voltage |
|---|---:|
| 20°C | 5.0040 V |
| 50°C | 5.0749 V |
| 80°C | 5.1311 V |

The results show how temperature variation affects the output voltage of the circuit.

## Repository Contents

- `circuit/`: LTspice schematic
- `report/`: Original project report in Persian

## How to Run

1. Install LTspice.
2. Open `circuit/AC-DC-Converter.asc`.
3. Run the transient simulation.
4. Adjust the load resistance to reproduce the load-variation cases.
5. Configure the temperature sweep to reproduce the temperature analysis.

**Note:** All reported results are from LTspice simulations; no physical hardware measurements are claimed.