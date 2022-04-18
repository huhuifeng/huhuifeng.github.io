---
layout: page
title: Base on Q learning
subtitle:  some algorithms based on Q learning
---
## Model-free RL
1. **playing atari with deep reinforcement learning** NIPS Deep Learning Workshop 2013. [paper](https://arxiv.org/abs/1312.5602) **DQN(early)**

    *Volodymyr Mnih, Koray Kavukcuoglu, David Silver, Alex Graves, Ioannis Antonoglou, Daan Wierstra, Martin Riedmiller*

   <details>
   <summary> Abstract </summary>
   We present the first deep learning model to successfully learn control policies directly from high-dimensional sensory input using reinforcement learning. The model is a      convolutional neural network, trained with a variant of Q-learning, whose input is raw pixels and whose output is a value function estimating future rewards. We apply our          method to seven Atari 2600 games from the Arcade Learning Environment, with no adjustment of the architecture or learning algorithm. We find that it outperforms all             previous       approaches on six of the games and surpasses a human expert on three of them.
   </details>

2. **Human-level control through deep reinforcement learning** Nature 2015. [paper](https://www.nature.com/articles/nature14236) **DQN(nature)**

    *Volodymyr Mnih, Koray Kavukcuoglu, David Silver, Andrei A. Rusu, Joel Veness, Marc G. Bellemare, Alex Graves, Martin Riedmiller, Andreas K. Fidjeland, Georg Ostrovski, Stig Petersen, Charles Beattie, Amir Sadik, Ioannis Antonoglou, Helen King, Dharshan Kumaran, Daan Wierstra, Shane Legg & Demis Hassabis*
    
   <details>
   <summary> Abstract </summary>
      The theory of reinforcement learning provides a normative account, deeply rooted in psychological and neuroscientific3 perspectives on animal behaviour, of how agents may optimize their control of an environment. To use reinforcement learning successfully in situations approaching real-world complexity, however, agents are confronted with a difficult task: they must derive efficient representations of the environment from high-dimensional sensory inputs, and use these to generalize past experience to new situations. Remarkably, humans and other animals seem to solve this problem through a harmonious combination of reinforcement learning and hierarchical sensory processing systems the former evidenced by a wealth of neural data revealing notable parallels between the phasic signals emitted by dopaminergic neurons and temporal difference reinforcement learning algorithms. While reinforcement learning agents have achieved some successes in a variety of domains, their applicability has previously been limited to domains in which useful features can be handcrafted, or to domains with fully observed, low-dimensional state spaces. Here we use recent advances in training deep neural networks to develop a novel artificial agent, termed a deep Q-network, that can learn successful policies directly from high-dimensional sensory inputs using end-to-end reinforcement learning. We tested this agent on the challenging domain of classic Atari 2600 games. We demonstrate that the deep Q-network agent, receiving only the pixels and the game score as inputs, was able to surpass the performance of all previous algorithms and achieve a level comparable to that of a professional human games tester across a set of 49 games, using the same algorithm, network architecture and hyperparameters. This work bridges the divide between high-dimensional sensory inputs and actions, resulting in the first artificial agent that is capable of learning to excel at a diverse array of challenging tasks.
   </details>
   
3. **Deep Reinforcement Learning with Double Q-learning** AAAI 16. [paper](https://arxiv.org/abs/1509.06461) **DQN(Double)**

    *Hado van Hasselt, Arthur Guez, David Silver*
    
   <details>
   <summary> Abstract </summary>
   The popular Q-learning algorithm is known to overestimate action values under certain conditions. It was not previously known whether, in practice, such overestimations are common, whether they harm performance, and whether they can generally be prevented. In this paper, we answer all these questions affirmatively. In particular, we first show that the recent DQN algorithm, which combines Q-learning with a deep neural network, suffers from substantial overestimations in some games in the Atari 2600 domain. We then show that the idea behind the Double Q-learning algorithm, which was introduced in a tabular setting, can be generalized to work with large-scale function approximation. We propose a specific adaptation to the DQN algorithm and show that the resulting algorithm not only reduces the observed overestimations, as hypothesized, but that this also leads to much better performance on several games.
   </details>
   
4. **Dueling Network Architectures for Deep Reinforcement Learning** ICML16. [paper](https://arxiv.org/abs/1511.06581) **DQN(Dueling)**

    *Ziyu Wang, Tom Schaul, Matteo Hessel, Hado van Hasselt, Marc Lanctot, Nando de Freitas*
    
   <details>
   <summary> Abstract </summary>
   In recent years there have been many successes of using deep representations in reinforcement learning. Still, many of these applications use conventional architectures, such as convolutional networks, LSTMs, or auto-encoders. In this paper, we present a new neural network architecture for model-free reinforcement learning. Our dueling network represents two separate estimators: one for the state value function and one for the state-dependent action advantage function. The main benefit of this factoring is to generalize learning across actions without imposing any change to the underlying reinforcement learning algorithm. Our results show that this architecture leads to better policy evaluation in the presence of many similar-valued actions. Moreover, the dueling architecture enables our RL agent to outperform the state-of-the-art on the Atari 2600 domain.
   </details>

5. **Deep Recurrent Q-Learning for Partially Observable MDPs** AAA15. [paper](https://arxiv.org/abs/1507.06527)

    *Matthew Hausknecht, Peter Stone*
    
   <details>
   <summary> Abstract </summary>
   Deep Reinforcement Learning has yielded proficient controllers for complex tasks. However, these controllers have limited memory and rely on being able to perceive the complete game screen at each decision point. To address these shortcomings, this article investigates the effects of adding recurrency to a Deep Q-Network (DQN) by replacing the first post-convolutional fully-connected layer with a recurrent LSTM. The resulting \textit{Deep Recurrent Q-Network} (DRQN), although capable of seeing only a single frame at each timestep, successfully integrates information through time and replicates DQN's performance on standard Atari games and partially observed equivalents featuring flickering game screens. Additionally, when trained with partial observations and evaluated with incrementally more complete observations, DRQN's performance scales as a function of observability. Conversely, when trained with full observations and evaluated with partial observations, DRQN's performance degrades less than DQN's. Thus, given the same length of history, recurrency is a viable alternative to stacking a history of frames in the DQN's input layer and while recurrency confers no systematic advantage when learning to play the game, the recurrent net can better adapt at evaluation time if the quality of observations changes.
   </details>
    
6. **Prioritized Experience Replay** ICLR 2016. [paper](https://arxiv.org/abs/1511.05952) **DQN(Prioritized)**

    *Tom Schaul, John Quan, Ioannis Antonoglou, David Silver*

   <details>
   <summary> Abstract </summary>
   Experience replay lets online reinforcement learning agents remember and reuse experiences from the past. In prior work, experience transitions were uniformly sampled from a replay memory. However, this approach simply replays transitions at the same frequency that they were originally experienced, regardless of their significance. In this paper we develop a framework for prioritizing experience, so as to replay important transitions more frequently, and therefore learn more efficiently. We use prioritized experience replay in Deep Q-Networks (DQN), a reinforcement learning algorithm that achieved human-level performance across many Atari games. DQN with prioritized experience replay achieves a new state-of-the-art, outperforming DQN with uniform replay on 41 out of 49 games.
   </details>
 
7. **Asynchronous Methods for Deep Reinforcement Learning** ICML2016. [paper](https://arxiv.org/abs/1602.01783)

    *Volodymyr Mnih, Adrià Puigdomènech Badia, Mehdi Mirza, Alex Graves, Timothy P. Lillicrap, Tim Harley, David Silver, Koray Kavukcuoglu*
    
   <details>
   <summary> Abstract </summary>
   We propose a conceptually simple and lightweight framework for deep reinforcement learning that uses asynchronous gradient descent for optimization of deep neural network controllers. We present asynchronous variants of four standard reinforcement learning algorithms and show that parallel actor-learners have a stabilizing effect on training allowing all four methods to successfully train neural network controllers. The best performing method, an asynchronous variant of actor-critic, surpasses the current state-of-the-art on the Atari domain while training for half the time on a single multi-core CPU instead of a GPU. Furthermore, we show that asynchronous actor-critic succeeds on a wide variety of continuous motor control problems as well as on a new task of navigating random 3D mazes using a visual input.
   </details>
    
8. **A Distributional Perspective on Reinforcement Learning** ICML2017. [paper](https://arxiv.org/abs/1707.06887)
    
    *Marc G. Bellemare, Will Dabney, Rémi Munos*
    
   <details>
   <summary> Abstract </summary>
   In this paper we argue for the fundamental importance of the value distribution: the distribution of the random return received by a reinforcement learning agent. This is in contrast to the common approach to reinforcement learning which models the expectation of this return, or value. Although there is an established body of literature studying the value distribution, thus far it has always been used for a specific purpose such as implementing risk-aware behaviour. We begin with theoretical results in both the policy evaluation and control settings, exposing a significant distributional instability in the latter. We then use the distributional perspective to design a new algorithm which applies Bellman's equation to the learning of approximate value distributions. We evaluate our algorithm using the suite of games from the Arcade Learning Environment. We obtain both state-of-the-art results and anecdotal evidence demonstrating the importance of the value distribution in approximate reinforcement learning. Finally, we combine theoretical and empirical evidence to highlight the ways in which the value distribution impacts learning in the approximate setting.
   </details>

9. **Noisy Networks for Exploration** ICLR2018. [paper](https://arxiv.org/abs/1706.10295)

    *Meire Fortunato, Mohammad Gheshlaghi Azar, Bilal Piot, Jacob Menick, Ian Osband, Alex Graves, Vlad Mnih, Remi Munos, Demis Hassabis, Olivier Pietquin, Charles Blundell, Shane Legg*

   <details>
   <summary> Abstract </summary>
   We introduce NoisyNet, a deep reinforcement learning agent with parametric noise added to its weights, and show that the induced stochasticity of the agent's policy can be used to aid efficient exploration. The parameters of the noise are learned with gradient descent along with the remaining network weights. NoisyNet is straightforward to implement and adds little computational overhead. We find that replacing the conventional exploration heuristics for A3C, DQN and dueling agents (entropy reward and ϵ-greedy respectively) with NoisyNet yields substantially higher scores for a wide range of Atari games, in some cases advancing the agent from sub to super-human performance.
   </details>
   
10. **Rainbow: Combining Improvements in Deep Reinforcement Learning** AAAI2018. [paper](https://arxiv.org/abs/1710.02298) **(contrast DQNs)**

    *Matteo Hessel, Joseph Modayil, Hado van Hasselt, Tom Schaul, Georg Ostrovski, Will Dabney, Dan Horgan, Bilal Piot, Mohammad Azar, David Silver*
   
   
      <details>
      <summary> Abstract </summary>
       The deep reinforcement learning community has made several independent improvements to the DQN algorithm. However, it is unclear which of these extensions are complementary and can be fruitfully combined. This paper examines six extensions to the DQN algorithm and empirically studies their combination. Our experiments show that the combination provides state-of-the-art performance on the Atari 2600 benchmark, both in terms of data efficiency and final performance. We also provide results from a detailed ablation study that shows the contribution of each component to overall performance.
      </details>
   
## Model-based RL

1. **Sample-Efficient Reinforcement Learning with Stochastic Ensemble Value Expansion** NIPS2018. [paper](https://arxiv.org/abs/1807.01675)

    *Jacob Buckman, Danijar Hafner, George Tucker, Eugene Brevdo, Honglak Lee*

      <details>
      <summary> Abstract </summary>
       The deep reinforcement learning community has made several independent improvements to the DQN algorithm. However, it is unclear which of these extensions are complementary and can be fruitfully combined. This paper examines six extensions to the DQN algorithm and empirically studies their combination. Our experiments show that the combination provides state-of-the-art performance on the Atari 2600 benchmark, both in terms of data efficiency and final performance. We also provide results from a detailed ablation study that shows the contribution of each component to overall performance.
      </details>

2. **Model-Based Value Estimation for Efficient Model-Free Reinforcement Learning**  ICML2018.[paper](https://arxiv.org/abs/1803.00101)

    *Vladimir Feinberg, Alvin Wan, Ion Stoica, Michael I. Jordan, Joseph E. Gonzalez, Sergey Levine* 
    
3. **Value Prediction Network** NIPS2017. [paper](https://arxiv.org/abs/1707.03497)

    *Vladimir Feinberg, Alvin Wan, Ion Stoica, Michael I. Jordan, Joseph E. Gonzalez, Sergey Levine*
    
4. **Imagination-Augmented Agents for Deep Reinforcement Learning** NIPS2017. [paper](https://arxiv.org/abs/1707.06203)

    *Théophane Weber, Sébastien Racanière, David P. Reichert, Lars Buesing, Arthur Guez, Danilo Jimenez Rezende, Adria Puigdomènech Badia, Oriol Vinyals, Nicolas Heess, Yujia Li, Razvan Pascanu, Peter Battaglia, Demis Hassabis, David Silver, Daan Wierstra*
    
5. **Continuous Deep Q-Learning with Model-based Acceleration** ICML2016. [paper](https://arxiv.org/abs/1603.00748)
    
    *Shixiang Gu, Timothy Lillicrap, Ilya Sutskever, Sergey Levine*

6. **Uncertainty-driven Imagination for Continuous Deep Reinforcement Learning** CoRL2017. [paper](http://proceedings.mlr.press/v78/kalweit17a/kalweit17a.pdf)
    
    *Gabriel Kalweit, Joschka Boedecker*
    
7. **Model-Ensemble Trust-Region Policy Optimization** ICLR2018. [paper](https://arxiv.org/abs/1802.10592)
    
    *Thanard Kurutach, Ignasi Clavera, Yan Duan, Aviv Tamar, Pieter Abbeel*

8. **Deep Reinforcement Learning in a Handful of Trials using Probabilistic Dynamics Models** NIPS2018. [paper](https://arxiv.org/abs/1805.12114)
    
    *Kurtland Chua, Roberto Calandra, Rowan McAllister, Sergey Levine*
    
9. **Dyna, an integrated architecture for learning, planning, and reacting** ACM1991. [paper](https://dl.acm.org/citation.cfm?id=122377)
    
    *Sutton, Richard S*
    
10. **Learning Continuous Control Policies by Stochastic Value Gradients** NIPS 2015. [paper](https://arxiv.org/abs/1510.09142)
    
    *Nicolas Heess, Greg Wayne, David Silver, Timothy Lillicrap, Yuval Tassa, Tom Erez*
    
11. **Imagination-Augmented Agents for Deep Reinforcement Learning** NIPS 2017. [paper](https://arxiv.org/abs/1707.06203)

    *Théophane Weber, Sébastien Racanière, David P. Reichert, Lars Buesing, Arthur Guez, Danilo Jimenez Rezende, Adria Puigdomènech Badia, Oriol Vinyals, Nicolas Heess, Yujia Li, Razvan Pascanu, Peter Battaglia, Demis Hassabis, David Silver, Daan Wierstra*
    
12. **Learning and Policy Search in Stochastic Dynamical Systems with Bayesian Neural Networks** ICLR 2017. [paper](https://arxiv.org/abs/1605.07127)
    
    *Stefan Depeweg, José Miguel Hernández-Lobato, Finale Doshi-Velez, Steffen Udluft*
    
