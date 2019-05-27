# Drop-Activation: Implicit Parameter Reduction and Harmonious Regularization
![GitHub](https://img.shields.io/badge/gbup-%E7%A8%B3%E4%BD%8F-blue.svg)
[![996.ICU](https://img.shields.io/badge/link-996.icu-red.svg)](https://996.icu) 

The repository is the official implementation of paper "Drop-Activation: Implicit Parameter Reduction and Harmonious Regularization" [[paper]](https://arxiv.org/abs/1811.05850).

By [Senwei Liang](https://github.com/LeungSamWai), [Yuehaw Kwoo](https://www.google.com) and [Haizhao Yang](https://haizhaoyang.github.io/).

## Introduction
Drop-Activation is a regularization method to reduce the risk of overfitting. The key idea is to drop nonlinear activation functions by setting them to be identity functions randomly during training time. During testing, we use a deterministic network with a new activation function to encode the average effect of dropping activations randomly.

## Acknowledgements
We thank to [bearpaw](https://github.com/bearpaw) for his well-organized [framework](https://github.com/bearpaw/pytorch-classification) for image classification task. 
