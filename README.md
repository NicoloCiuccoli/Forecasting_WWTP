# Forecasting and Early Warning System for Wastewater Treatment Plant Sensors

This repository contains the dataset and Python code associated with the article:  
**"Forecasting and Early Warning System for Wastewater Treatment Plant Sensors Using Multitask and LSTM Neural Networks: A Simulated and Real-World Case Study"**  

Authors: Nicolò Ciuccoli, Francesco Fatone, Massimiliano Sgroi, Anna Laura Eusebi, Riccardo Rosati, Laura Screpanti, Adriano Mancini, David Scaradozzi  
Affiliations: Università Politecnica delle Marche, SIMAU and DII Departments  
Contact: Nicolò Ciuccoli ([n.ciuccoli@univpm.it](mailto:n.ciuccoli@univpm.it))  

---

## Abstract
This study develops an Early Warning System (EWS) for wastewater treatment plants, focusing on the Peschiera Borromeo WWTP in Milan, Italy. Predictive models, including Multitask Learning (MTL) and Long Short-Term Memory (LSTM) networks, estimate key water quality parameters such as Chemical Oxygen Demand (COD) and Total Suspended Solids (TSS). Using simulated and real-world datasets, the system predicts effluent quality up to 6 hours in advance, helping to ensure safe water reuse in agriculture.

---

## Repository Contents
- **`dataset/`**: Contains simulated and real-world datasets used for training and testing the predictive models.
- **`code/`**: Jupyter Notebooks for implementing and evaluating the predictive models:
  - **`MLT_simulated_dataset_and_Fault.ipynb`**: Code for the Multitask Learning (MTL) neural network, including training and results on the simulated dataset.
  - **`LSTM_Simulated_Dataset.ipynb`**: Code for the Long Short-Term Memory (LSTM) network, including training and results on the simulated dataset.
  - **`MLT_Real_Dataset.ipynb`**: Code for the MTL neural network, including training and results on the real-world dataset.
  - **`LSTM_Real_Dataset.ipynb`**: Code for the LSTM network, including training and results on the real-world dataset.

---
---

## Dataset Description
### **Simulated Dataset**
- **Training Set**: 1 year of hourly data (8,640 samples) generated under normal WWTP operating conditions.
- **Fault Scenario Set**: 1,324 samples simulating critical malfunctions.

### **Real Dataset**
- Data collected from December 2021 to March 2022 at Peschiera Borromeo WWTP (2,340 hourly samples).  

### **Key Variables**
| Parameter           | Type     | Unit  | Description                              |
|---------------------|----------|-------|------------------------------------------|
| Influent pH         | Input    | -     | Acidity/alkalinity of incoming water     |
| Flow Rate           | Input    | m³/h  | Volume of water entering the plant       |
| Biofor Dissolved Oxygen | Input | mg/L  | Oxygen concentration in biological reactors |
| Biofor Temperature  | Input    | °C    | Water temperature in biological reactors |
| Effluent COD        | Output   | mg/L  | Organic matter concentration in effluent |
| Effluent TSS        | Output   | mg/L  | Suspended solids concentration in effluent |

---

## Code Overview
### **Scripts**
- `MLT_simulated_dataset_and_Fault.ipynb`: Preprocessing, training, and evaluation of the MTL neural network on the simulated dataset, including fault scenarios.
- `LSTM_Simulated_Dataset.ipynb`: Preprocessing, training, and evaluation of the LSTM network for 6-hour forecasting on the simulated dataset.
- `MLT_Real_Dataset.ipynb`: Preprocessing, training, and evaluation of the MTL neural network on the real-world dataset.
- `LSTM_Real_Dataset.ipynb`: Preprocessing, training, and evaluation of the LSTM network for 6-hour forecasting on the real-world dataset.





### Dependencies
The following libraries are required to run the code:

#### **Standard Libraries**
- `os`
- `sys`
- `random`
- `csv`
- `math`
- `pickle`
- `pathlib`

#### **Third-party Libraries**
- `numpy` (1.19.5 or later)
- `pandas` (1.1.5 or later)
- `tensorflow` (2.6.0 or later)
- `scikit-learn` (0.24.2 or later)
- `scipy` (1.7.1 or later)
- `matplotlib` (3.4.3 or later)

#### **Keras Utilities**
- `keras.utils.vis_utils` (for visualizing model architectures)


Copyright (C) 2025 Nicolò Ciuccoli, Francesco Fatone, Massimiliano Sgroi, Anna Laura Eusebi, Riccardo Rosati, Laura Screpanti, Adriano Mancini, David Scaradozzi.  
This program is free software: you can redistribute it and/or modify it under the terms of the GNU Affero General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.