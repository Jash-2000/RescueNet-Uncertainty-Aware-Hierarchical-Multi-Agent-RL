## Problem Statement
Imagine you have a team of robots dropped into an unknown building after an earthquake. They need to find survivors. Nobody knows where the survivors are. The robots can only see a small area around themselves. They need to coordinate without a central controller telling each one what to do every second. This is a Search and Rescue (SAR) problem. The paper proposes a specific mathematical framework for solving it with multiple learning agents. This defines a set of problems:
  - Partial Observablity: each robot sees only a local part of the environment.
  - Hierarchical Problem Statement: they must spread out, share information indirectly, and later converge when a victim is likely found.
  - Decentralized Control: the number of robots can become large, so coordination must scale well.
  - Long Horizon Task: they do not know exactly where the victim is and the reward is delayed.

This work this tries to solve this problem for a Multi-Agent formulation by introduceing structure at three levels:
  - Hierarchy: a high-level policy chooses a mode/option such as explore, navigate, or form.
  - Graph reasoning: agents reason through an interaction graph instead of as isolated individuals.
  - Uncertainty reduction: the mission objective is tied to reducing uncertainty about victim location.

---

![Implementation Video](https://github.com/Jash-2000/RescueNet-Uncertainty-Aware-Hierarchical-Multi-Agent-RL/blob/main/Figures/sar_animation_v2_fixed.gif)
