# 🚦 Autonomous Traffic Signal Control using Reinforcement Learning

## 📌 Overview

Traffic congestion at urban intersections leads to increased delays, fuel consumption, and emissions. This project explores **adaptive traffic signal control** using **Reinforcement Learning (RL)** and extends to **Multi-Agent Reinforcement Learning (MARL)** for coordinated traffic management.

The study compares three approaches:

* Tabular Q-Learning
* Deep Q-Networks (DQN)
* Hybrid Q-Learning with a Small Language Model (SLM) advisor

---

## 📄 Abstract

Urban traffic congestion at signalized intersections significantly contributes to delays, fuel consumption, and emissions. This project investigates RL-based adaptive traffic control and explores MARL for coordinated junction management.

Three controllers were evaluated using simulation data: **Q-Learning**, **DQN**, and a **hybrid Q-Learning + SLM advisor** that provides congestion insights and explainable recommendations.

Despite differences in learning behavior, all models converged to a similar average waiting time (~29.46 seconds). DQN and step-capped Q-Learning showed single-action bias, while step-capping promoted conservative decision-making. The SLM-enhanced model improved interpretability with minimal trade-offs in performance.

The findings emphasize the importance of reward design, state representation, and training strategy, while highlighting future directions in MARL coordination and sim-to-real transfer.

---

## 🎯 Objectives

* Implement RL-based traffic signal controllers
* Compare performance across different RL methods
* Analyze learning dynamics and action distributions
* Introduce explainability using an SLM-enhanced agent

---

## 🧠 Models Implemented

### 🔹 Tabular Q-Learning

* Discrete state-action learning
* Step-capping to control exploration

### 🔹 Deep Q-Network (DQN)

* Neural network approximation of Q-values
* Suitable for larger state spaces

### 🔹 Hybrid Q-Learning + SLM

* Adds explainability layer
* Generates:

  * Congestion labels
  * Action recommendations
  * Human-readable decision traces

---

## ⚙️ Environment & Tools

* **SUMO (Simulation of Urban Mobility)**
* Python
* Reinforcement Learning frameworks
* Deep Learning libraries

---

## 📊 Results Summary

* All models converged to **~29.46s average waiting time**
* DQN and Q-Learning showed **single-action dominance**
* Step-capping led to **short-term conservative behavior**
* SLM improved **interpretability** without performance gain

---

## 📈 Key Insights

* Reward design critically affects performance
* State representation impacts learning quality
* Training and evaluation must be aligned
* Explainable RL is feasible with minimal overhead

---

## 🔬 Future Work

* Advanced reward shaping techniques
* Network-wide MARL coordination
* Real-world (sim-to-real) deployment validation
* Handling dynamic and uncertain traffic demand

---

## 📁 Project Structure

```
├── data/                # Traffic simulation data
├── models/              # RL models (Q-Learning, DQN, Hybrid)
├── environment/         # SUMO configuration files
├── training/            # Training scripts
├── evaluation/          # Performance evaluation scripts
├── results/             # Output metrics and plots
└── README.md
```

---

## 🚀 How to Run

```bash
# Clone the repository
git clone https://github.com/your-username/your-repo-name.git

# Navigate to project
cd your-repo-name

# Install dependencies
pip install -r requirements.txt

# Run simulation / training
python train.py
```

---

## 👤 Author

**SURYA SAKTHIVEL**

**RAGUL SIVABAL**
MSc AI, Data Science & Digital Business
Berlin, Germany

---
