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
   We present the first deep learning model to successfully learn control policies directly from high-dimensional sensory input using reinforcement learning. The model is a      convolutional neural network, trained with a variant of Q-learning, whose input is raw pixels and whose output is a value function estimating future rewards. We apply our          method to seven Atari 2600 games from the Arcade Learning Environment, with no adjustment of the architecture or learning algorithm. We find that it outperforms all             previous       approaches on six of the games and surpasses a human expert on three of them.
   </details>
   
4. **Dueling Network Architectures for Deep Reinforcement Learning** ICML16. [paper](https://arxiv.org/abs/1511.06581) **DQN(Dueling)**

    *Ziyu Wang, Tom Schaul, Matteo Hessel, Hado van Hasselt, Marc Lanctot, Nando de Freitas*
    
   <details>
   <summary> Abstract </summary>
   We present the first deep learning model to successfully learn control policies directly from high-dimensional sensory input using reinforcement learning. The model is a      convolutional neural network, trained with a variant of Q-learning, whose input is raw pixels and whose output is a value function estimating future rewards. We apply our          method to seven Atari 2600 games from the Arcade Learning Environment, with no adjustment of the architecture or learning algorithm. We find that it outperforms all             previous       approaches on six of the games and surpasses a human expert on three of them.
   </details>

5. **Deep Recurrent Q-Learning for Partially Observable MDPs** AAA15. [paper](https://arxiv.org/abs/1507.06527)

    *Matthew Hausknecht, Peter Stone*
    
   <details>
   <summary> Abstract </summary>
   We present the first deep learning model to successfully learn control policies directly from high-dimensional sensory input using reinforcement learning. The model is a      convolutional neural network, trained with a variant of Q-learning, whose input is raw pixels and whose output is a value function estimating future rewards. We apply our          method to seven Atari 2600 games from the Arcade Learning Environment, with no adjustment of the architecture or learning algorithm. We find that it outperforms all             previous       approaches on six of the games and surpasses a human expert on three of them.
   </details>
    
6. **Prioritized Experience Replay** ICLR 2016. [paper](https://arxiv.org/abs/1511.05952) **DQN(Prioritized)**

    *Tom Schaul, John Quan, Ioannis Antonoglou, David Silver*

   <details>
   <summary> Abstract </summary>
   We present the first deep learning model to successfully learn control policies directly from high-dimensional sensory input using reinforcement learning. The model is a      convolutional neural network, trained with a variant of Q-learning, whose input is raw pixels and whose output is a value function estimating future rewards. We apply our          method to seven Atari 2600 games from the Arcade Learning Environment, with no adjustment of the architecture or learning algorithm. We find that it outperforms all             previous       approaches on six of the games and surpasses a human expert on three of them.
   </details>
 
7. **Asynchronous Methods for Deep Reinforcement Learning** ICML2016. [paper](https://arxiv.org/abs/1602.01783)

    *Volodymyr Mnih, Adrià Puigdomènech Badia, Mehdi Mirza, Alex Graves, Timothy P. Lillicrap, Tim Harley, David Silver, Koray Kavukcuoglu*\
    
   <details>
   <summary> Abstract </summary>
   We present the first deep learning model to successfully learn control policies directly from high-dimensional sensory input using reinforcement learning. The model is a      convolutional neural network, trained with a variant of Q-learning, whose input is raw pixels and whose output is a value function estimating future rewards. We apply our          method to seven Atari 2600 games from the Arcade Learning Environment, with no adjustment of the architecture or learning algorithm. We find that it outperforms all             previous       approaches on six of the games and surpasses a human expert on three of them.
   </details>
    
8. **A Distributional Perspective on Reinforcement Learning** ICML2017. [paper](https://arxiv.org/abs/1707.06887)
    
    *Marc G. Bellemare, Will Dabney, Rémi Munos*
    
   <details>
   <summary> Abstract </summary>
   We present the first deep learning model to successfully learn control policies directly from high-dimensional sensory input using reinforcement learning. The model is a      convolutional neural network, trained with a variant of Q-learning, whose input is raw pixels and whose output is a value function estimating future rewards. We apply our          method to seven Atari 2600 games from the Arcade Learning Environment, with no adjustment of the architecture or learning algorithm. We find that it outperforms all             previous       approaches on six of the games and surpasses a human expert on three of them.
   </details>

9. **Noisy Networks for Exploration** ICLR2018. [paper](https://arxiv.org/abs/1706.10295)

    *Meire Fortunato, Mohammad Gheshlaghi Azar, Bilal Piot, Jacob Menick, Ian Osband, Alex Graves, Vlad Mnih, Remi Munos, Demis Hassabis, Olivier Pietquin, Charles Blundell, Shane Legg*

   <details>
   <summary> Abstract </summary>
   We present the first deep learning model to successfully learn control policies directly from high-dimensional sensory input using reinforcement learning. The model is a      convolutional neural network, trained with a variant of Q-learning, whose input is raw pixels and whose output is a value function estimating future rewards. We apply our          method to seven Atari 2600 games from the Arcade Learning Environment, with no adjustment of the architecture or learning algorithm. We find that it outperforms all             previous       approaches on six of the games and surpasses a human expert on three of them.
   </details>
   
10. **Rainbow: Combining Improvements in Deep Reinforcement Learning** AAAI2018. [paper](https://arxiv.org/abs/1710.02298) **(contrast DQNs)**

    *Matteo Hessel, Joseph Modayil, Hado van Hasselt, Tom Schaul, Georg Ostrovski, Will Dabney, Dan Horgan, Bilal Piot, Mohammad Azar, David Silver*
   
   <details>
   <summary> Abstract </summary>
   We present the first deep learning model to successfully learn control policies directly from high-dimensional sensory input using reinforcement learning. The model is a      convolutional neural network, trained with a variant of Q-learning, whose input is raw pixels and whose output is a value function estimating future rewards. We apply our          method to seven Atari 2600 games from the Arcade Learning Environment, with no adjustment of the architecture or learning algorithm. We find that it outperforms all             previous       approaches on six of the games and surpasses a human expert on three of them.
   </details>
   
   
## Model-based RL
