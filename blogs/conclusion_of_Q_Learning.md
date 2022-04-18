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
#### 经验池技术
![Experience Replay](/blogs/pictures/experience_Replay.png)
<center>
    <b><font face="楷体" size=5> 图2. 经验池技术示意图</font></b>
</center>
DQN中一个比较重要的<font face="黑体" color=orange>trick</font>就是经验池技术(<font face="黑体" color=red>Experience Replay</font>)[^1]。经验池技术也不是DQN论文首次提出,只是首次运用到深度强化学习当中，该技术是1993年就提出了。它的主要作用是解决<font face="黑体" color=red>数据的相关性和非静态分布问题</font>。即将每个时间步Agent与环境交互得到的状态转移样本$(s_t,a_t,r_t,s_{t+1})$，存储到一个记忆单元（多维元组；有一个存储上限，即容量$D$）中，在要训练的时候<font face = "黑体" color = red>随机抽取一些</font>用于神经网络的训练，注意此处是一些，Q learning每次训练的是采用一个样本进行训练。
<b><font color=blue>经验池技术的好处</font></b>：
- 经验池的每个状态转移样本都可能在许多权重更新中使用，这可以<b><font face="黑体" color=red>提高数据利用率</font></b>.


[^1]:Long-Ji Lin. Reinforcement learning for robots using neural networks. Technical report, DTIC Document, 1993.

### 3.Double DQN
[paper link](https://arxiv.org/abs/1509.06461) **DQN(Double)**

### 4.Prioritized Experience Replay DQN
[paper link](https://arxiv.org/abs/1511.05952) **DQN(Prioritized)**
### 5.Dual-DQN
[paper link](https://arxiv.org/abs/1511.06581) **DQN(Dueling)**