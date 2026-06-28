# CS 370 Project Two: Pirate Intelligent Agent

## Overview

This project focused on developing a pirate intelligent agent capable of solving a maze using **Deep Q-Learning (DQN)**. The objective was to train a non-player character (NPC) to navigate obstacles and find a treasure by learning through reinforcement learning instead of following a hard-coded path.

---

# Project Reflection

## Briefly explain the work that you did on this project.

The project included starter code that provided the game environment (`TreasureMaze.py`), the experience replay system (`GameExperience.py`), and the notebook structure. My responsibility was to complete the Deep Q-Learning implementation without modifying the provided Python files.

I designed and implemented the training loop, epsilon-greedy exploration, replay memory training, target network updates, performance tracking, and data visualizations. During development, I discovered that the provided environment created a sparse-reward problem, making it difficult for a standard DQN to learn consistently through random exploration alone.

To solve this, I implemented a **Breadth-First Search (BFS) warm-start** that generated successful example paths and seeded the replay memory before reinforcement learning began. The DQN then continued training on those experiences, eventually learning an effective navigation policy while still satisfying the project requirement of using Deep Q-Learning.

I also added inline comments, completion checks, training statistics, and graphs to improve readability and demonstrate my understanding of reinforcement learning.

---

# Connecting My Learning to Computer Science

## What do computer scientists do and why does it matter?

Computer scientists solve complex problems by designing algorithms, building software systems, and creating intelligent solutions that improve efficiency and decision-making. Their work affects nearly every industry, from healthcare and finance to cybersecurity, transportation, and entertainment.

Artificial intelligence is one example of this impact. Rather than programming every possible action, computer scientists can build systems that learn from experience and improve over time, allowing software to solve increasingly complex real-world problems.

---

## How do I approach a problem as a computer scientist?

This project reinforced the importance of breaking large problems into smaller, manageable pieces. I first studied the provided code to understand how each component interacted before making changes.

When the original Deep Q-Learning implementation struggled to learn because of sparse rewards, I researched reinforcement learning best practices, tested several approaches, analyzed the results, and implemented a BFS warm-start to provide successful experiences before allowing the DQN to continue learning independently.

This iterative process of researching, testing, debugging, and refining solutions reflects how I approach software development and problem solving.

---

## What are my ethical responsibilities to the end user and the organization?

Computer scientists have a responsibility to develop software that is reliable, secure, and trustworthy. AI systems should be thoroughly tested, well documented, and designed to minimize unintended behavior.

Developers must also write maintainable code, communicate design decisions clearly, and protect user data whenever applicable. This project emphasized that creating intelligent software is not only about producing correct results but also about building systems that are understandable, maintainable, and dependable.

---

# Skills Demonstrated

- Deep Q-Learning (DQN)
- Reinforcement Learning
- Neural Networks
- Experience Replay
- Target Networks
- Epsilon-Greedy Exploration
- Breadth-First Search (BFS)
- Python
- TensorFlow / Keras
- Algorithm Design
- Debugging and Performance Analysis
- Data Visualization

---

# Repository Contents

- `TreasureHuntGame.ipynb` — Completed Deep Q-Learning implementation
- `README.md` — Project overview and reflection
- `ProjectTwo.html` — Exported notebook for submission
