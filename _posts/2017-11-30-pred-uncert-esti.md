---
title: Predictive Uncertainty Estimation
Author: Adam
---

Recently, I come across a nice paper: [Simple and Scalable Predictive Uncertainty
Estimation using Deep Ensembles](https://arxiv.org/pdf/1612.01474.pdf), which is written by Balaji Lakshminarayanan, Alexander Pritzel and Charles Blundell  from Google DeepMind. I am also suprised to find that this paper is gonna be presented at NIPS 2017. So I already made up my mind to go to their talk. 

Before, I was always wondering how to estimate or quantify the predictive uncertainty under the framework of neural network. This paper actually give a good review of the work done in this direction. 

The paper points out that there has been a lot of recent interest in adapting NNs to encompass uncertainty and probabilistic
methods. The majority of this work revolves around a Bayesian formalism [4], whereby a prior
distribution is specified upon the parameters of a NN and then, given the training data, the posterior
distribution over the parameters is computed, which is used to quantify predictive uncertainty.

Recently, Gal and Ghahramani proposed using Monte Carlo dropout (MC-dropout) to estimate
predictive uncertainty by using Dropout at test time.


The contribution in this paper is two fold. First, they describe a simple and
scalable method for estimating predictive uncertainty estimates from NNs. They argue for training
probabilistic NNs (that model predictive distributions) using a proper scoring rule as the training
criteria. They additionally investigate the effect of two modifications to the training pipeline, namely
(i) ensembles and (ii) adversarial training [18] and describe how they can produce smooth predictive
estimates. Secondly, they propose a series of tasks for evaluating the quality of the predictive uncertainty
estimates, in terms of calibration and generalization to unknown classes in supervised learning
problems. They show that our method significantly outperforms (or matches) MC-dropout. 