# v2g-ai-forecasting-simulation
AI-Driven Vehicle-to-Grid (V2G) Forecasting and Simulation Framework combining LSTM/Seq2Seq load–PV–EV forecasting with a MATLAB/Simulink physical energy system model. Includes forecasting scripts, Simulink architecture (PV, load, EV chargers, battery, grid), and optimization algorithms for smart charging and energy scheduling.

Vehicle-to-Grid (V2G) AI Forecasting & Simulation Framework

This repository contains forecasting models, MATLAB system simulations, and optimization algorithms developed for an AI-driven V2G management framework.
It demonstrates:

✔ Load forecasting (LSTM)
✔ PV generation forecasting (Seq2Seq)
✔ EV availability forecasting (Seq2Seq)
✔ MATLAB/Simulink V2G system model
✔ Optimization layer (Genetic Algorithm & RL)

📌 Repository Structure

Folder	Description
/forecasting	LSTM and Seq2Seq models for load, PV, EV availability
/simulation/matlab	MATLAB/Simulink physical system models
/optimization	GA and RL-based scheduling algorithms
/docs	Diagrams, figures, and draft documentation
🧠 Machine Learning Forecasting Models

All forecasting modules use 24-hour input → 24-hour output (96 timesteps).

> Load model: Single-feature LSTM

> PV model: Seq2Seq multistep LSTM

> EV model: Seq2Seq binary availability model

Outputs include:

- RMSE, MAE, MAPE
- Prediction curves
- Saved trained models (*.h5)

⚡ MATLAB/Simulink V2G System

The Simulink model includes:

- PV subsystem
- Load subsystem
- Bidirectional EV chargers
- Battery model
- Grid interconnection
- AI control input

Outputs exported to /simulation/matlab/exports/:

- Power balance
- Grid import/export
- Fleet SOC
- Stability indicators

🎯 Optimization Layer

> GA Scheduler: Minimizes energy cost & peak load
> RL Agent (optional): Learns charging/discharging policy

📈 Results

All generated plots (forecasting and scheduling) appear under /forecasting/.../results/ or /optimization/results/.

👨‍🏫 Supervisor Notes

This repository is structured to clearly show:

> Weekly progress

> Code improvements

> Simulation results

> Versioned forecasting models

> Clear commit history

> Visualizations of every step
