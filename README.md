# AUTOMATED_AMPLIFIER_CIRCUIT_DESIGN_GENERATION
A GenAI-based project using a Variational Autoencoder (VAE) for automated design of analog amplifier circuits by predicting optimal resistor values (RC, RE, RG) based on user-defined specifications.


# ⚙️ Automated Amplifier Circuit Design Generation using GenAI

This project explores the use of **Variational Autoencoders (VAE)** to automatically generate analog amplifier circuit resistor values based on input specifications. It aims to simplify and accelerate the early-stage analog design process using deep generative models.

---

## 👥 Team Members

- Vaishnavi Sanjay Kadolkar (02FE22BEC115)  
- Santoshi Uppin (02FE22BEC085)  
- Swaroop Patil (02FE23BEC401)  
- Swayam Mane (02FE22BEC113)  

**Guide:** Dr. Swati Mavinkattimath  
**Institution:** KLE Technological University  
**Semester:** VI, 2024–2025  
**Department:** Electronics and Communication Engineering

---

## 🎯 Objectives

- Predict RC, RE, RG values for amplifier circuits using a trained generative model.
- Use a **VAE** to map input parameters (e.g., configuration, gain, Vcc, Vout) to resistor values.
- Accelerate amplifier design through intelligent automation.
- Evaluate model using regression metrics like MSE, MAE, RMSE, and R².

---

## 💡 Problem Statement

Manual selection of resistor values in analog circuits is time-consuming and error-prone.  
This project proposes a **data-driven, GenAI approach** to automate the resistor value generation process using machine learning.

---

## 📊 Dataset Overview

- **Inputs:**
  - Amplifier configuration (CE, CC, CG)
  - Voltage gain
  - Vcc (supply voltage)
  - Vout (output voltage)

- **Outputs:**
  - RC (collector resistance)
  - RE (emitter resistance)
  - RG (gate resistance)

- Format: CSV, tabular, preprocessed with one-hot encoding and MinMax normalization.

---

## 🧠 Model Architecture

### 🔹 Variational Autoencoder (VAE)

- **Encoder:** Compresses input to latent space.
- **Latent space:** Represents distributions (mean & variance).
- **Decoder:** Reconstructs RC, RE, RG from latent representation.

### 🔍 Loss Function

- **Reconstruction Loss:** Mean Squared Error (MSE)  
- **Regularization:** Kullback–Leibler Divergence (KLD)  
- **Total Loss:** MSE + β·KLD

---


## 📷 Visuals

### 📌 Block Diagram  
<img src="workflow.png" alt="Block Diagram" width="500"/>

### 📉 Loss over Epochs  
<img src="loss.png" alt="Training Loss" width="500" height="350"/>

### 🧩 Generated Amplifier Circuit  
<img src="output.png" alt="Generated Circuit" width="500" height="350"/>

---

## 📈 Performance Metrics

<img src="performance_matrics.png" alt="Generated Circuit" width="500" height="350"/>

---

## 🚀 Applications

- Analog circuit design automation  
- Education tools for learning design-space relationships  
- EDA tools integration for intelligent suggestions  
- Rapid prototyping of single-stage amplifiers  

---

## 🔮 Future Scope

- Integration of performance metrics into training loss function  
- Expansion to multi-stage amplifier design generation  
- SPICE netlist generation for simulation and testing  
- Incorporation with layout tools such as **LayoutCopilot**  
- Use of **Graph Neural Networks (GNNs)** for full topology prediction  

---

## ✅ Conclusion

- VAE-based models can predict resistor values with reasonable accuracy.  
- Enables faster, AI-assisted circuit prototyping.  
- Demonstrates the potential of GenAI in analog hardware design automation.


