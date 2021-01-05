---
title: "Inverse Reinforcement Learning for Autonomous Navigation via Differentiable Semantic Mapping and Planning"
collection: publications
permalink: /publications/SIRL
date: 2021-1-4
venue: 'Under review'

---
[[ArXiv]](https://arxiv.org/abs/2101.00186)
[[Website]](http://tianyudwang.github.io/sirl)


## Abstract
This paper focuses on inverse reinforcement learning for autonomous navigation using distance and semantic category observations. The objective is to infer a cost function that explains demonstrated behavior while relying only on the expert's observations and state-control trajectory. We develop a map encoder, that infers semantic category probabilities from the observation sequence, and a cost encoder, defined as a deep neural network over the semantic features. Since the expert cost is not directly observable, the model parameters can only be optimized by differentiating the error between demonstrated controls and a control policy computed from the cost estimate. We propose a new model of expert behavior that enables error minimization using a closed-form subgradient computed only over a subset of promising states via a motion planning algorithm. Our approach allows generalizing the learned behavior to new environments with new spatial configurations of the semantic categories. We analyze the different components of our model in a minigrid environment. We also demonstrate that our approach learns to follow traffic rules in the autonomous driving CARLA simulator by relying on semantic observations of buildings, sidewalks, and road lanes. 