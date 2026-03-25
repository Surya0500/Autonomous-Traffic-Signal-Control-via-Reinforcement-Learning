🚦 Autonomous Traffic Signal Control using Reinforcement Learning
📌 Overview

Urban traffic congestion at signalized intersections leads to increased delays, fuel consumption, and emissions. Traditional fixed-time and actuated traffic systems often fail to adapt to dynamic traffic patterns.

This project explores adaptive traffic signal control using Reinforcement Learning (RL) and evaluates multiple learning approaches, including a hybrid model enhanced with a Small Language Model (SLM) for explainability.

📂 Dataset

The dataset used in this project is publicly available on Kaggle:

🔗 https://www.kaggle.com/datasets/olaidegabriel/traffic-dataset

This dataset was used for:

Traffic flow analysis
Congestion pattern identification
Training and evaluation of RL models
🎯 Objectives
Develop intelligent traffic signal control using RL
Compare different RL models and their performance
Analyze learning behavior and decision-making patterns
Introduce explainability into RL using language models
Identify limitations and future research directions
🧠 Models Implemented
🔹 Tabular Q-Learning
Discrete state-action learning
Step-capping to control exploration
Encourages conservative, short-horizon decisions
🔹 Deep Q-Network (DQN)
Neural network approximation of Q-values
Handles larger and more complex state spaces
Exhibits action selection instability in some scenarios
🔹 Hybrid Q-Learning + Small Language Model (SLM)
Integrates a language model for explainability

Capabilities:

Generates congestion labels
Provides action recommendations
Produces human-readable decision traces
⚙️ Methodology
Used secondary traffic simulation data
Applied consistent training and evaluation conditions across models

Evaluation Metrics:

Mean waiting time
Learning dynamics
Action distribution patterns
Reward convergence behavior
📊 Results
⏱️ All models converged to a similar average waiting time (~29.46 seconds)
⚠️ DQN and step-capped Q-Learning showed single-action dominance issues
🧭 Step-capped Q-Learning favored short-term conservative strategies
💡 SLM-enhanced model improved interpretability with minimal trade-offs
🔍 Key Insights
RL performance is highly sensitive to:
Reward design
State representation
Training vs evaluation setup
Explainability improves transparency but not necessarily performance
🚀 Future Work
Develop discriminative reward functions
Scale to Multi-Agent Reinforcement Learning (MARL)
Improve sim-to-real transfer
Reduce action-selection bias in deep RL models
🛠️ Tech Stack
Python
Reinforcement Learning (Q-Learning, DQN)
Machine Learning / AI
Data Analysis
📁 Project Structure
├── data/
├── models/
├── training/
├── evaluation/
├── results/
├── README.md

👥 Authors
👤 Surya Sakthivel
GitHub: https://github.com/Surya0500
LinkedIn: https://www.linkedin.com/in/surya-sakthivel-de/
👤 Ragul Sivabal
GitHub: https://github.com/ragul16g-oss
LinkedIn: https://linkedin.com/in/ragul-sivabal
📖 Citation

If you use this work, please cite:

@misc{traffic_rl_project,
  author = {Surya Sakthivel and Ragul Sivabal},
  title = {Autonomous Traffic Signal Control using Reinforcement Learning},
  year = {2026},
  publisher = {GitHub},
  url = {https://github.com/Surya0500}
}

🤝 Contributing

Contributions and suggestions are welcome!

📜 License

This project is for academic and research purposes.
