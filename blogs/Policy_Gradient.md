---
layout: page
title: Policy Gradient
subtitle:  some policy Gradient algorithm
---

# PPO
# TRPO
1. **Trust region policy optimization** 	16 pages, ICML 2015 [paper](https://arxiv.org/abs/1502.05477) **TRPO**

    *J. Schulman, S. Levine, P. Moritz, M. I. Jordan, and P. Abbeel. *

   <details>
   <summary> Abstract </summary>
   We describe an iterative procedure for optimizing policies, with guaranteed monotonic improvement. By making several approximations to the theoretically-justified procedure, we develop a practical algorithm, called Trust Region Policy Optimization (TRPO). This algorithm is similar to natural policy gradient methods and is effective for optimizing large nonlinear policies such as neural networks. Our experiments demonstrate its robust performance on a wide variety of tasks: learning simulated robotic swimming, hopping, and walking gaits; and playing Atari games using images of the screen as input. Despite its approximations that deviate from the theory, TRPO tends to give monotonic improvement, with little tuning of hyperparameters.
   </details>

# DDPG
