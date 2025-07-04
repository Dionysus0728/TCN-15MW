# TCN-15MW

**Data-Driven Feature Selection for TCN-Based Mooring Tension Prediction in Floating Offshore Wind Turbines**

---

## 📘 Introduction

This repository contains the dataset and source code for the research on **mooring tension prediction** in **Floating Offshore Wind Turbines (FOWTs)** using a **Temporal Convolutional Network (TCN)** model. The approach emphasizes **data-driven feature selection** to improve prediction performance.

Simulations were conducted using [OrcaFlex](https://www.orcina.com/SoftwareProducts/OrcaFlex/), and the results were post-processed using Python-based tools.

---

## 📂 Dataset Description

Simulation data are located in the folders `EC1/` and `EC2/`, with the following contents:

- `1.xlsx`: Effective tension of **mooring line 1**
- `2.xlsx`: Effective tension of **mooring line 2**
- `3.xlsx`: Effective tension of **mooring line 3**
- `666.xlsx`: **6-DoF motion response** of the FOWT (surge, sway, heave, roll, pitch, yaw)
- `env.xlsx`: **Environmental parameters**, including wind speed, wave height, current speed, etc.

All datasets are in `.xlsx` format and aligned in time.

---

## 💻 Code Description

The code is contained in the `code/` directory. It is written in **Jupyter Notebook** format (`.ipynb`) for reproducibility.

- `code.ipynb`: Main training script implementing the TCN model
- `diff.ipynb`: Demonstrates the **differential method** for feature selection proposed in the paper

> Note: Please ensure the necessary Python packages are installed. You may use the following command to install dependencies:

```bash
pip install -r requirements.txt
