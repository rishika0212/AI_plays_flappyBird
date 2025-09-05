# 🎮 Flappy Bird NEAT AI

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.8%2B-3776AB?logo=python&logoColor=white" alt="Python" />
  <img src="https://img.shields.io/badge/Pygame-2.x-0C9A4A?logo=pygame&logoColor=white" alt="Pygame" />
  <img src="https://img.shields.io/badge/NEAT--Python-evolutionary-8E44AD" alt="NEAT-Python" />
</p>

Welcome to a colorful Flappy Bird clone where an AI learns to fly using NEAT (NeuroEvolution of Augmenting Topologies) — watch neural networks evolve to master the game!

---

## ✨ Features
- 🧠 **AI-powered gameplay** using NEAT to evolve bird behavior
- 🌈 **Smooth animations** and polished visuals
- 📈 **Score tracking** and fitness evaluation
- 🧩 **Modular design**: Bird, Pipe, Base, and Game loop

---

## 🚀 Getting Started

### 1) Requirements
- **Python** 3.8+
- **Dependencies**:
  - `pygame`
  - `neat-python`

### 2) Install
```bash
pip install pygame neat-python
```

### 3) Run
```bash
python flappy.py
```
- The NEAT config is loaded from `config-feedforward.txt` (already included).
- A window will open and the AI will start learning over generations.

---

## 🕹️ How It Works (Quick Overview)
- Each bird is controlled by a small neural network.
- Inputs include the bird's `y` position and distances to the next pipe openings.
- Networks are evolved with NEAT over generations to maximize survival and score.

---

## 📸 Screenshots

<p align="center">
  <img src="screenshots/image.png" alt="Gameplay Screenshot 1" width="45%" style="margin: 8px; border-radius: 8px;" />
  <img src="screenshots/image2.png" alt="Gameplay Screenshot 2" width="45%" style="margin: 8px; border-radius: 8px;" />
</p>

---

## 📁 Project Structure
```
.
├── flappy.py                 # Main game + NEAT training loop
├── config-feedforward.txt    # NEAT configuration
├── imgs/                     # Game assets (bird, pipes, background)
└── screenshots/              # Project screenshots
```

---

## 🧪 Tuning Tips
- Adjust **pipe gap** in `Pipe.GAP` for difficulty.
- Modify **bird physics** in `Bird.move()` for different behavior.
- Evolve more generations by changing `p.run(main, 50)` in `flappy.py`.

---

## 🙌 Acknowledgments
- Built with ❤️ using **Pygame** and **NEAT-Python**.

---

## 📄 License
This project is for learning and experimentation. Add a license if you plan to share/distribute.