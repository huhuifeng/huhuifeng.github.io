---
layout: page
title: some conclusions of RL
subtitle: based on Q learning 
---

### DQN
[paper](https://arxiv.org/abs/1312.5602) **DQN(early)**
### DQN(nature)
[paper link](https://www.nature.com/articles/nature14236) **DQN(Nature)**
![DQN_nature](/blogs/pictures/DQN_nature.png)

$Q^\ast(s, a)=\mathbb{E}_{s^{\prime}\sim\Epsilon}\left[r+\gamma\underset{a^{\prime}}Q^{\ast}\left(s^{\prime}, a^{\prime}\right) \mid \mathrm{s}, \mathrm{a}\right]$

$\text{令}y_i = \mathbb{E}_{s^{'}\sim\mathcal{E}}\left[r+\gamma\underset{a^{'}}{max}Q^*(s^{'},a^{'})|s,a\right],\text{则}$
	
$L_i(\theta_i) = \mathbb{E}_{s,a\sim\rho(\cdot)}\left[(y_i-Q(s,a;\theta_i))^{2}\right]$
	
$\nabla_{\theta_i}L_{i}(\theta_i) = \mathbb{E}_{s,a-\rho(\dots);s^{'}-\mathcal{E}}\left[(r+\gamma\underset{a^{'}}{max}Q^*(s^{'},a^{'})-Q(s,a;\theta_i))\nabla_{\theta_i}Q(s,a;\theta_i)\right]$

### Double DQN
[paper link](https://arxiv.org/abs/1509.06461) **DQN(Double)**

### Prioritized Experience Replay DQN
[paper link](https://arxiv.org/abs/1511.05952) **DQN(Prioritized)**
### Dual-DQN
[paper link](https://arxiv.org/abs/1511.06581) **DQN(Dueling)**