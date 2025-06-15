# Reinforcement-Learning-for-Smart-Crop-Irrigation

This project presents a reinforcement learning-based irrigation system trained using PPO, A2C, and DQN algorithms. The system simulates crop growth and soil conditions to optimize water usage while ensuring healthy crop development. Built using Stable-Baselines3 and a custom Gymnasium environment.

---

## 🧠 Project Overview

- **Objective**: Maximize crop yield by intelligently managing irrigation under varying climate and soil conditions.
- **Techniques**: DQN, A2C, PPO (Stable-Baselines3)
- **Observations Used**:
  - Soil moisture
  - Crop coefficient
  - Leaf Area Index (LAI)
  - Growth stage
  - Irrigation history

---

## 📁 Repository Structure

```
RL-Crop-Irrigation/
├── models/            # Trained RL agent checkpoints
├── media/             # Plots, growth stage images, videos
├── logs/              # Training monitor logs
├── notebook/          # Final Jupyter notebook
├── docs/              # Final project report (PDF)
├── requirements.txt   # Python dependencies
├── .gitignore
└── README.md
```

---

## 📊 Results & Visuals

### 🔹 PPO Agent
- Trained for 1,000,000 timesteps
- ![PPO](media/ppo_sb3_1000000_rewards.png)

### 🔹 DQN Agent
- ![Training](media/training_rewards.png)
- ![Epsilon Decay](media/epsilon_decay.png)
- ![Eval Avg](media/eval_average_reward.png)
- ![Eval Bars](media/eval_rewards_per_episode.png)

### 🔹 A2C Agent
- ![Training](media/a2c_logs_1000000_rewards.png)
- ![Eval Avg](media/a2c_average_reward.png)
- ![Eval Bars](media/a2c_rewards_per_episode.png)

---

## 🌱 Crop Growth Stages

| Stage      | Image                        |
|------------|------------------------------|
| Seedling   | ![](media/seedling.png)      |
| Vegetative | ![](media/vegetative.png)    |
| Stressed   | ![](media/stressed.png)      |
| Mature     | ![](media/mature.png)        |

---

## 🎥 Simulation Videos

- [Healthy Growth](media/Crop_with_perfect_growth.mp4)
- [Stressed Growth](media/Crop_with_stressed_stage.mp4)

---

## 🛠 Setup Instructions

```bash
git clone https://github.com/your-username/RL-Crop-Irrigation.git
cd RL-Crop-Irrigation

# Optional: Create virtual environment
python -m venv venv
source venv/bin/activate  # Windows: venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt
```

---

## 📘 References

- [Stable-Baselines3](https://github.com/DLR-RM/stable-baselines3)
- [Gymnasium](https://github.com/Farama-Foundation/Gymnasium)
- [APSIM Weather Simulation](https://www.apsim.info)
- [Crop-Gym Environment](https://github.com/WUR-AI/crop-gym)

---

## 👨‍💻 Contributors

- **Aravind Aripaka** – Lead developer, RL integration, visualization
- **Team** – Environment modeling and testing

---

## 📄 License

This repository is provided for academic and educational use only.
