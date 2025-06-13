# Model-Based Policy Optimization (MBPO) with Ensemble World Models

This repository implements a fully modular MBPO framework with:
- Ensemble-based World Models for robust dynamics prediction.
- Soft Actor-Critic (SAC) agent trained on a hybrid of real and imagined rollouts.
- Rollout scheduling, mixed-batch training, and logging utilities.

---

## 🧠 Cognitive Analogy: Dreams and Decisions

Inspired by psychological theories of the unconscious, specifically from Chapter 6 of *The Rosetta Stone of Human Mind*:

> *"Memories not recalled for long reorganize in the unconscious. The resulting product, though altered, preserves the essence of the original experience."*

We apply this concept metaphorically to MBPO:
- The **World Model** functions like the unconscious mind—accumulating interactions and forming **imagined trajectories** (dreams).
- The **SAC Agent**, like a decision-maker without direct memory, learns **solely from these dreams**—producing actions based on reorganized, indirect information.

This analogy elevates the intuition behind MBPO: agents can thrive even when they operate on representations, not reality.

---

## 📊 Logging (Key Metrics)

- **World Model Loss**: Tracks the predictive power of the ensemble model (state + reward).
- **SAC Losses**: Actor, Critic, and Alpha for stable policy/value learning.
- **Rollout Metrics**: Configurable rollout horizon and environment model usage.

---


--- SAC Performance

    Reward:37.985 | Max_reward: 91.89018965747927
    Reward:39.898 | Max_reward: 91.89018965747927
    Reward:29.361 | Max_reward: 91.89018965747927

  Acheived under 4 lakh steps on humanoid v5
## 🔧 Key Features

- Dynamic rollout scheduling
- Ensemble uncertainty handling
- Clean SAC integration
- Mixed real-model buffer sampling
- Easy-to-modify modular codebase

---

## 🧠 Future Extensions

- Incorporate model uncertainty to weight imagined samples.
- Explore KL-regularized SAC variants with ensemble disagreement.
- Apply dreaming to sparse reward settings (e.g., long-horizon navigation).

---

## 💡 Inspiration

This repository is built not just on algorithms, but on the **idea that agents, like humans, can learn and act effectively based on restructured, imagined experience.**
