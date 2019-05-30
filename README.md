# Drop-Activation: Implicit Parameter Reduction and Harmonious Regularization
![GitHub](https://img.shields.io/github/license/gbup-group/DIANet.svg)
[![996.ICU](https://img.shields.io/badge/link-996.icu-red.svg)](https://996.icu) 

The repository is the official implementation of paper "Drop-Activation: Implicit Parameter Reduction and Harmonious Regularization" [[paper]](https://arxiv.org/abs/1811.05850).

By [Senwei Liang](https://github.com/LeungSamWai), [Yuehaw Kwoo](https://www.google.com) and [Haizhao Yang](https://haizhaoyang.github.io/).

## Introduction
Drop-Activation is a regularization method to reduce the risk of overfitting. The key idea is to drop nonlinear activation functions by setting them to be identity functions randomly during training time. During testing, we use a deterministic network with a new activation function to encode the average effect of dropping activations randomly.

![image-w20](https://github.com/LeungSamWai/Drop-Activation/blob/master/images/fig-dropact.jpg)

## Requirement
* [Pytorch](https://pytorch.org/) 1.0.0

## Usage
* Clone the repository of Drop-Activation
```
git clone https://github.com/LeungSamWai/Drop-Activation.git
```
* Train the WideResNet28-10 using Drop Activation on CIFAR100
```
python cifar.py -a da_wrn --dataset cifar100 --depth 28 --depth 28 --widen-factor 10 --drop 0.3 --epochs 200 --schedule 60 120 160 --wd 5e-4 --gamma 0.2 --checkpoint checkpoints/cifar100/WRN-28-10-drop-DropActivation
```


## Citing
* If you find it useful in your research, please cite 
```
@article{Liang2018Drop,
         title={Drop-Activation: Implicit Parameter Reduction and Harmonic Regularization},
         author={Liang, Senwei and Kwoo, Yuehaw and Yang, Haizhao},
         year={2018},}
```

## Acknowledgements
We thank [bearpaw](https://github.com/bearpaw) for his well-organized pytorch [framework](https://github.com/bearpaw/pytorch-classification) for image classification task. 
