---
layout: page
title: some conclusions of RL
subtitle: based on Q learning 
---

### 1.DQN
[paper](https://arxiv.org/abs/1312.5602) **DQN(early)**
### 2.DQN(nature)
[paper link](https://www.nature.com/articles/nature14236) **DQN(Nature)**
![DQN_nature](/blogs/pictures/DQN_nature.png)
<center>
    <b><font face="楷体" size=5> 图1. DQN nature版本框架 </font></b>
</center>

$$Q^\ast(s, a)=\mathbb{E}_{s^{\prime}\sim\mathcal{E}}\left[r+\gamma\underset{a^{\prime}}{max}Q^{\ast}\left(s^{\prime}, a^{\prime};\bar{\theta}_{i}\right) \mid \mathrm{s}, \mathrm{a}\right]$$

$$\text{令}y_i = \mathbb{E}_{s^{'}\sim\mathcal{E}}\left[r+\gamma\underset{a^{'}}{max}Q^*(s^{'},a^{'};\bar{\theta}_{i})|s,a\right],\text{则}$$
	
$$L_i(\theta_i) = \mathbb{E}_{s,a\sim\rho(\cdot)}\left[(y_i-Q(s,a;\theta_i))^{2}\right]$$
	
$$\nabla _{\theta_i}L_{i}(\theta_i) = \mathbb{E}_{s,a\sim\rho(\dots);s^{'}\sim\mathcal{E}}\left[(r+\gamma\underset{a^{'}}{max}Q^*(s^{'},a^{'};\bar{\theta}_{i})-Q(s,a;\theta_i))\nabla _{\theta_i}Q(s,a;\theta_i)\right]$$

其中$\mathbb{E}$表示环境，$r$表示奖励信号或者回报，$\rho(\cdot)$表示动作的概率分布，$y_i$表示由目标值网络提供的真实值，$Q(s,a;\theta_i)$表示当前值网络的拟合值。
### 3.Double DQN
[paper link](https://arxiv.org/abs/1509.06461) **DQN(Double)**

### 4.Prioritized Experience Replay DQN
[paper link](https://arxiv.org/abs/1511.05952) **DQN(Prioritized)**
### 5.Dual-DQN
[paper link](https://arxiv.org/abs/1511.06581) **DQN(Dueling)**