---
title: "Large Scale Model Predictive Control with Neural Networks and Primal Active Sets"
collection: publications
permalink: /publications/NNMPC
date: 2019-10-23
venue: 'In submission'

---
[[ArXiv]](https://arxiv.org/abs/1910.10835)


## Abstract
This work presents an explicit-implicit procedure that combines an offline trained neural network with an online primal active set solver to compute a model predictive control (MPC) law with guarantees on recursive feasibility and asymptotic stability. The neural network improves the suboptimality of the controller performance and accelerates online inference speed for large systems, while the primal active set method provides corrective steps to ensure feasibility and stability. We highlight the connections between MPC and neural networks and introduce a primal-dual loss function to train a neural network to initialize the online controller. We then demonstrate online computation of the primal feasibility and suboptimality criteria to provide the desired guarantees. Next, we use these neural network and criteria measures to accelerate an online primal active set method through warm starts and early termination. Finally, we present a data set generation algorithm that is critical for successfully applying our approach to high dimensional systems. The primary motivation is developing an algorithm that scales to systems that are challenging for current approaches, involving state and input dimensions as well as planning horizons in the order of tens to hundreds. 