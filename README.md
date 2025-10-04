

# Discrete Signal Analysis and Processing 

[![Jupyter Notebook](https://img.shields.io/badge/Notebook-Jupyter-orange.svg)](https://jupyter.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

## Overview

This project is a comprehensive notebook for studying and implementing concepts from Discrete-Time Signal Processing (DTSP). It contains Python code (Jupyter Notebook) for:

- **Z-Transform calculation and visualization**
- **System causality (causal, non-causal) analysis**
- **System property checks (linearity, time-invariance, homogeneity, BIBO stability)**
- **Signal analysis (even/odd, energy/power, periodicity, etc.)**
- **Type of signal (periodic, aperiodic, energy, power)**

The notebook is intended as a course project and reference for students learning DTSP.

---

## Features

### 1. Z-Transform Plot
- Computes the Z-transform of a discrete signal.
- Plots the Z-transform in the complex plane for visualization.

### 2. System Analysis
- Checks whether an impulse response is causal or non-causal.
- Calculates system response for a given input and impulse response.
- Determines if the system is linear, time-invariant, homogeneous, and BIBO stable.

### 3. Signal Analysis
- Analyzes discrete signals for:
  - Even/Odd nature
  - Energy or Power classification
  - Periodicity (periodic/aperiodic)
- Visualizes signals using matplotlib.

### 4. Type of Signal
- Finds the period of discrete signals.
- Classifies signals as energy or power signals.

---

## Getting Started

### Prerequisites

- Python 3.x
- Jupyter Notebook or Google Colab
- Required Python packages: `numpy`, `matplotlib`

Install dependencies with:

```bash
pip install numpy matplotlib
```

### Running the Notebook

1. Clone this repository:
   ```bash
   git clone https://github.com/sarveshvengurlekar/Discrete_Signal_Analysis_and_Processing.git
   ```
2. Open `Copy_of_DTSP_CP (1).ipynb` in Jupyter Notebook or upload to Google Colab.
3. Run the notebook cells sequentially to see code, outputs, and visualizations.

---

## Folder Structure

```
.
├── Discrete_signal_processing_Code.ipynb   # Main notebook with all code and explanations
└── README.md                   # Project documentation (this file)
```

---

## Example Usage

### Z-Transform

```python
discrete_signal = np.array([1, 2, 3, 4, 5])
z_transform_signal = z_transform(discrete_signal)
plot_z_transform(z_transform_signal)
```

### System Causality

```python
x = [1, 2, 3]
h = [4, 5, 6]
y = calculate_response(x, h)
print("System Response Y(n):", y)
print("Causal:", check_causal(h))
print("Non-Causal:", check_noncausal(h))
```

### Signal Analysis

```python
t = np.linspace(0, 5, 100)
x = np.sin(2*np.pi*t)
analysis = analyze_signal(x, t)
print("Signal Analysis:", analysis)
plot_signal(x, t)
```

---

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

