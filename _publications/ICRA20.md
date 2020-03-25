---
title: "Learning Navigation Cost from Demonstrations in Partially Observable Environments"
collection: publications
permalink: /publication/ICRA20
date: 2020-3-23
venue: 'International Conference on Robotics and Automation (ICRA 2020)'

---
[[ArXiv]](https://arxiv.org/abs/2002.11637)


## Abstract
This paper focuses on inverse reinforcement learning (IRL) to enable safe and efficient autonomous navigation in unknown partially observable environments. The objective is to infer a cost function that explains expert-demonstrated navigation behavior while relying only on the observations and state-control trajectory used by the expert. We develop a cost function representation composed of two parts: a probabilistic occupancy encoder, with recurrent dependence on the observation sequence, and a cost encoder, defined over the occupancy features. The representation parameters are optimized by differentiating the error between demonstrated controls and a control policy computed from the cost encoder. Such differentiation is typically computed by dynamic programming through the value function over the whole state space. We observe that this is inefficient in large partially observable environments because most states are unexplored. Instead, we rely on a closed-form subgradient of the cost-to-go obtained only over a subset of promising states via an efficient motion-planning algorithm such as A* or RRT. Our experiments show that our model exceeds the accuracy of baseline IRL algorithms in robot navigation tasks, while substantially improving the efficiency of training and test-time inference. 