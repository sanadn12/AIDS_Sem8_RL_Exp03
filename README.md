# 🧠 Experiment 3: Value Iteration & Policy Iteration in Grid World

**Name:** Sanad Naqvi
**Roll No:** 221A023

---

## 🎯 Aim

To implement **Value Iteration** and **Policy Iteration** algorithms for solving a Grid World problem using reinforcement learning.

---

## 📌 Problem Statement

The objective is to find the **optimal policy** for an agent navigating a grid environment such that it maximizes rewards and reaches the goal efficiently.

---

## 📖 Theory

### 🔹 Markov Decision Process (MDP)

An MDP is defined by:

* States (S)
* Actions (A)
* Transition probabilities (P)
* Rewards (R)
* Discount factor (γ)

### 🔹 Value Iteration

* Computes optimal state values iteratively
* Uses Bellman optimality equation
* Updates value function until convergence

### 🔹 Policy Iteration

Consists of two steps:

1. **Policy Evaluation:** Evaluate value function for a given policy
2. **Policy Improvement:** Improve policy based on value function

This repeats until the policy becomes stable.

---

## 🛠️ Implementation

### 🔹 Libraries Used

* numpy

### 🔹 Environment Details

* Grid size: 4 × 4
* Total states: 16
* Actions: up, down, left, right
* Terminal states:

  * (0, 0) → reward = 0
  * (3, 3) → reward = 1

### 🔹 Steps

1. Defined grid world states and actions
2. Initialized reward structure and terminal states
3. Defined transition function
4. Implemented **Value Iteration algorithm**
5. Implemented **Policy Iteration algorithm**:

   * Policy evaluation
   * Policy improvement
6. Computed optimal policy and value function

---

## 📊 Results

### 🔹 Optimal Policy

```
['-', 'down', 'down', 'down']
['down', 'down', 'down', 'down']
['down', 'down', 'down', 'down']
['right', 'right', 'right', '-']
```

### 🔹 State Values

```
[0, 0.66, 0.73, 0.81]
[0.66, 0.73, 0.81, 0.9]
[0.73, 0.81, 0.9, 1.0]
[0.81, 0.9, 1.0, 0]
```

* The agent learns to move toward the goal state (3,3)
* Values increase as states get closer to the goal

---

## ✅ Conclusion

* Both Value Iteration and Policy Iteration successfully computed optimal policies.
* The agent learned the shortest path to the goal state.
* Policy Iteration converges faster in many cases due to explicit policy updates.
* This experiment demonstrates how MDP-based methods solve decision-making problems.

---

## 📚 References

* Reinforcement Learning Concepts
* MDP and Dynamic Programming Notes
* Python NumPy Documentation

---

## 📦 requirements.txt

```
numpy
```
