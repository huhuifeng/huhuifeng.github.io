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
<center>
    <b><font face="楷体" size=5> 图1 DQN nature版本框架 </font></b>
</center>

$$Q^\ast(s, a)=\mathbb{E}_{s^{\prime}\sim\mathcal{E}}\left[r+\gamma\underset{a^{\prime}}{max}Q^{\ast}\left(s^{\prime}, a^{\prime}\right) \mid \mathrm{s}, \mathrm{a}\right]$$

$$\text{令}y_i = \mathbb{E}_{s^{'}\sim\mathcal{E}}\left[r+\gamma\underset{a^{'}}{max}Q^*(s^{'},a^{'})|s,a\right],\text{则}$$
	
$$L_i(\theta_i) = \mathbb{E}_{s,a\sim\rho(\cdot)}\left[(y_i-Q(s,a;\theta_i))^{2}\right]$$
	
$$\nabla _{\theta_i}L_{i}(\theta_i) = \mathbb{E}_{s,a\sim\rho(\dots);s^{'}\sim\mathcal{E}}\left[(r+\gamma\underset{a^{'}}{max}Q^*(s^{'},a^{'})-Q(s,a;\theta_i))\nabla _{\theta_i}Q(s,a;\theta_i)\right]$$

### Double DQN
[paper link](https://arxiv.org/abs/1509.06461) **DQN(Double)**

### Prioritized Experience Replay DQN
[paper link](https://arxiv.org/abs/1511.05952) **DQN(Prioritized)**
### Dual-DQN
[paper link](https://arxiv.org/abs/1511.06581) **DQN(Dueling)**