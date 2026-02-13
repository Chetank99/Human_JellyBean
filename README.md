# Human_JellyBean: Adaptive Decision Making in Non-Stationary Environments


## Scope:
This repo is part of the [**BSE662 - Decision Making and The Brain**](https://sites.google.com/view/decisionlabiitk/teaching?authuser=0#h.fyk15nbxqb4j) course project. 

## Meet the team!!

Course Instructor: [Dr. Arjun Ramakrishnan](https://sites.google.com/view/decisionlabiitk/people/arjun?authuser=0)

Mentor for this project: [Chetan Kandpal](https://github.com/Chetank99)

Students (_names in alphabetical order_)

### Team: **Brain Dead**: 
Their fork [link](https://github.com/KushalAgrawal123/Human_JellyBean/tree/Brain-Dead-BSE662)
- **Akash Guru** ([@Akash-22-stack](https://github.com/Akash-22-stack))
- **Akash Rathi** ([@clammyface](https://github.com/clammyface))
- **Gulshan Kumar** ([@kumargulshann](https://github.com/kumargulshann))
- **Ishani** ([@Ishaniiitk23](https://github.com/Ishaniiitk23))
- **Kushal Agrawal** ([@KushalAgrawal123](https://github.com/KushalAgrawal123))
- **Vivek Kumar Gupta** ([@Vivek280404](https://github.com/Vivek280404))
- **Yash Kumar** ([@kyash23](https://github.com/kyash23))

### Team: **The Decision Matrix**:
Their fork [link](https://github.com/krrishkh/Human_JellyBean/tree/The-Decision-Matrix) 
- **Ankit** ([@akankitt](https://github.com/akankitt))
- **Asif** ([@AsiF-7488](https://github.com/AsiF-7488))
- **Krrish Khandelwal** ([@krrishkh](https://github.com/krrishkh))

---

## Project Overview

**Goal:** Design a playable version of the Jelly Bean World task, collect human decision-making data, and develop models to explain human performance in a changing environment.

Humans excel in non-static, never-ending environments where rules evolve without warning. In contrast, most Reinforcement Learning (RL) algorithms assume stability and resettable episodes. This mismatch often leads to "catastrophic forgetting" or slow adaptation in RL agents.

    We aim to identify the missing components in current computational models of adaptive decision-making.

---

## The Task: Human-Playable Jelly Bean World

We are adapting the [**Jelly Bean World (JBW)**](https://arxiv.org/pdf/2002.06306) environment—originally designed for continual learning agents—into a task suitable for human experiments.

**Key Features:**
*   **Continuous Gameplay:** No "episodes" or resets. The world is a never-ending stream of experience.
*   **Non-Stationary Rewards:** The value of items (e.g., colored beans) changes over time without explicit instruction.
*   **Implicit Rules:** Participants must infer changes solely through interaction and feedback.

**Objectives:**
1.  **Navigate** a grid world to collect items.
2.  **Adapt** strategies as item values shift.
3.  **Maximize** total reward over an extended period.

*(Specific task mechanics and modification details are currently being finalized by the project groups).*

---

## Goals!!

We are collecting human behavioral data to serve as a benchmark for adaptive intelligence.

**Data Metrics:**
*   **Choices & Trajectories:** How do humans explore and exploit?
*   **Reaction Times:** Usage of cognitive effort during stable vs. volatile phases.
*   **Adaptation Speed:** How quickly is a new rule learned after a change point?

### Hypothesis
We hypothesize that humans will demonstrate superior **meta-learning** capabilities, detecting changes quickly and updating strategies without overwriting prior knowledge, compared to standard RL baselines. We aim to quantify this "adaptation gap."

---

## Computational Models

We will compare human performance against two primary computational baselines:

### 1. Baseline: Temporal Difference (TD) Learning
*   **Algorithm:** Standard Q-Learning / SARSA.
*   **Assumption:** The environment is stationary.
*   **Expected Failure:** Slow adaptation and catastrophic forgetting when reward functions change.

### 2. Extended Model: Elastic Weight Consolidation (EWC)
*   **Algorithm:** RL agents augmented with EWC.
*   **Mechanism:** Protects parameters important for previous tasks to reduce forgetting.
*   **Expected Outcome:** Better retention of old rules than TD, but likely less flexible than continuous human adaptation.

---

## Reading List & Resources

### Essential Blogs (Start Here)
1.  [The Explore-Exploit Dilemma](https://neuwritesd.org/2019/11/07/knowing-when-to-hold-or-fold-em-the-explore-exploit-dilemma/) - NeuWriteSD
2.  [A Long Peek into Reinforcement Learning](https://lilianweng.github.io/posts/2018-02-19-rl-overview/) - Lilian Weng
3.  [Enabling Continual Learning in Neural Networks](https://deepmind.google/discover/blog/enabling-continual-learning-in-neural-networks/) - Google DeepMind

### Key Papers
*   **Restless Bandits:** Whittle (1988) - [JSTOR Link](https://www.jstor.org/stable/3214163)
*   **Exploratory Decisions in Humans:** Daw et al. (2006) - [Nature](https://www.nature.com/articles/nature04766)
*   **Tracking in Stationary Environments:** Sutton et al. (2007) - [ACM DL](https://dl.acm.org/doi/10.1145/1273496.1273606)

### Project Foundations
*   **Paper:** [Rethinking the Foundations for Continual Reinforcement Learning](https://arxiv.org/abs/2310.16912) (Also see [Video Explanation](https://www.youtube.com/watch?v=StXlhNtLJVI))
*   **Jelly Bean World:** [Paper](https://arxiv.org/pdf/2002.06306) | [Original Code](https://github.com/eaplatanios/jelly-bean-world)

---
