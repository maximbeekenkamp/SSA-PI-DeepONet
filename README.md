# SSA-PI-DeepONet
- M. Beekenkamp, A. Bhagavathula, P. LaDuca.

## Introduction
This project combines several techniques found in Physics Informed Neural Networks (PINNs) research and implements them into a PI-DeepONet, to reduce error and computational costs. Specifically, we are using Separable Physics Informed Neural Networks (SPINNs), and Self-Adaptive Physics Informed Neural Networks (SAPINNs) to achieve these gains. <br><br>

Separable Physics Informed Neural Networks (SPINNs), originally proposed in the paper “Separable PINN: Mitigating the Curse of Dimensionality in Physics-Informed Neural Networks.” by Cho et al. are an architectural overhaul of conventional PINNs that can approximate solutions to partial differential equations (PDEs). These architectural changes allow us to leverage forward-mode autodifferentiation (AD) and operate on a per-axis basis. Compared to conventional PINNs, which use point-wise processing, SPINNs presents a notable reduction in training time whilst maintaining accuracy.<br><br>

Self-Adaptive PINNs (SA-PINNs), as proposed in the paper “Self-Adaptive Physics-Informed Neural Networks using a Soft Attention Mechanism” by McClenny, and Braga-Neto extend on the work of a simple PINN by adding a self-adaptive element which optimally regularises the components of the implemented loss function. Notably, SA-PINNs automate a process which hitherto was done by trial and error, or from information on the optimal solution known before training. The addition of the self-adaptive component further improves on the strengths of PINNs, the decreased training time, data requirements, and encoded physical laws. <br> <br>

## Motivating Literature and Sources
Wang, Sifan, et al. ["Learning the Solution Operator of Parametric Partial Differential Equations with Physics-Informed Deeponets."](https://doi.org/10.1126/sciadv.abi8605) Science Advances, vol. 7, no. 40, 2021. 

Levi D. McClenny, & Ulisses M. Braga-Neto (2020). ["Self-Adaptive Physics-Informed Neural Networks using a Soft Attention Mechanism."](https://arxiv.org/abs/2009.04544) CoRR, abs/2009.04544.

Cho, Junwoo, et al. ["Separable PINN: Mitigating the Curse of Dimensionality in Physics-Informed Neural Networks."](https://arxiv.org/abs/2211.08761) arXiv preprint arXiv:2211.08761 (2022).