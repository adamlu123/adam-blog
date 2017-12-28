---
title: Bayesian Methods in Neural Network	 
Author: Adam
background: '/img/bg-post0.jpg'
---

This post tries to summarize main research ideas of applying baysian methods into neural network as well as some possible (though kind of vague) directions that I might want to delve into as my research problem. 

Typically, a discussion of bayesian methods in deep learning community would start with some draw backs of deep neural network, such as:  data hungry, poor at representing uncertainty and finicky to optimise (choice of architecture). On top of that, we talk about the the benefit of involving baysian thinking. I would like to summarize it in one sentence, that is: instead of considering a single answer to a question (a local/global minimum of some loss function), bayesian methods enable us to consider an entire distribution of answers. 

Within the framework of deep neural network, there are several questions we can explore:
<!-- $$\text{S}_1(N) = \sum_{p=1}^N \text{E}(p)$$ -->

