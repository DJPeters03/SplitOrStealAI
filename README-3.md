# Auto Split/Steal — Q-Learning Simulation

## Overview
This project implements a **Q-learning simulation** of the classic **Split or Steal** game, visualized on a 2×3 grid. Two independent agents repeatedly play against each other, adjusting strategies through reinforcement learning.

---

## 350-Character Description
Auto Split/Steal is a Q-learning simulation on a 2×3 board where two agents independently learn to maximize payoffs. Using ε-greedy policies, they choose between splitting or stealing, update Q-values from outcomes, and adapt over rounds to cooperative or competitive strategies.

---

## Features
- Two **independent Q-learning agents** (Agent A and Agent B).  
- Actions: **Split** or **Steal**.  
- **Payoffs:**  
  - Split + Split → +0.5 each  
  - Steal + Steal → +0 each  
  - Mismatch → Stealer gets +1, Splitter gets 0  
- Adjustable **ε (exploration)**, **α (learning rate)**, and **γ (discount factor)**.  
- Control panel: Pause, Step, Reset, and Rounds per Second.  
- Outcome counters track frequency of SS, S-Stl, Stl-S, and Stl-Stl.  
- Animated visualization of agents’ decisions on the 2×3 board.  

---

## How It Works
- Each agent maintains an independent **Q-table** mapping states to action values.  
- At each round:  
  1. Agents select actions using **ε-greedy policies**.  
  2. Rewards are assigned based on payoff outcomes.  
  3. Q-values are updated using the Q-learning rule.  
  4. Agents adapt strategies over many rounds, balancing cooperation and competition.  

---

## How to Run
1. Open `SplitOrSteal.html` in a modern web browser (Chrome, Firefox, Safari).  
2. Use sliders to adjust ε, α, and γ.  
3. Click **Start/Pause** to run the simulation or **Step** to advance manually.  
4. Watch the payoff table, Q-values, and outcomes evolve in real time.  

---

## Educational Value
This simulation illustrates:  
- **Reinforcement learning dynamics** in repeated games.  
- The **exploration vs. exploitation** trade-off.  
- Emergent behaviors in cooperative vs. competitive strategies.  

---

## File
- `SplitOrSteal.html` → Full Q-learning split/steal simulation with visualization.  
