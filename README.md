# Adaptive Reward Correction for Mitigating Reward Hacking in Reinforcement Learning

## 🚀 Overview

This project demonstrates **reward hacking** in reinforcement learning and introduces a simple **adaptive reward correction mechanism** to improve agent behavior.

---

## 🧠 Problem

Reinforcement learning agents often exploit poorly designed reward functions instead of learning meaningful behavior.

Example:
An agent repeatedly collects the same reward by looping instead of exploring.

---

## 💡 Solution

We introduce **adaptive reward correction**, where:

* Repeated visits to the same state are tracked
* A penalty is applied for excessive repetition

---

## 🎮 Environment

* Grid World (5x5)
* Agent collects a coin (+1 reward)
* Coin remains fixed

### Baseline

* No penalty → agent exploits reward

### Adaptive

* Penalizes repeated states → better behavior

---

## ⚙️ Method

Reward = Base Reward - Penalty (if repeated state)

---

## 📊 Results

| Model    | Behavior               |
| -------- | ---------------------- |
| Baseline | Reward hacking (loops) |
| Adaptive | Improved exploration   |

---

## ▶️ Run the Project

```bash
pip install stable-baselines3 gymnasium torch matplotlib
python train.py
```

---

## 📈 Outputs

* Reward comparison graphs
* Agent path visualization
* State visit heatmaps

---

## 🎯 Goal

To reduce reward hacking and improve learning behavior in RL agents.

---

## 📜 License

MIT License
