# Overview

The temporal convolutional network is an architecture (primarily, although with forerunners) introduced by [[@baiEmpiricalEvaluationGeneric2018]] as an alternative to the wider family of [[Recurrent Neural Network|RNN]] architectures to model sequential data, instead being based on the [[Convolutional Neural Network|CNN]]. #temporal-convolutional-network #TCN #RNN #CNN

TCNs function by sliding a [[Kernel|kernel]] of size *k* along a sequence [[Tensor|tensor]] which has been zero-padded to ensure that it is of identical length to the output sequence. One dimension of the input tensor should correspond to the time-axis, with an additional axis corresponding to additional channels of data. The input sequence should be left zero-padded if it is desired that the architecture should be [[Causality|causal]]. #kernel #zero-padding #causal

As this would be extremely computationally expensive for longer sequences, [[Dilated Convolution|dilated convolutions]] are employed of dilation factor *d*. The dilation factor specifies the gap between elements of the input sequence with which to apply to the kernel. The dilation factor is usually increased exponentially with increasing depth of the convolutional layers of the model, as this ensures that the receptive field (the elements of the input sequence upon which the predicted element of the output sequence is reliant) cover the entire input sequence. The dilated convolution can be formally defined as:
$$F(s) = (x \ast_d f)(s) = \sum_{i=0}^{k-1} f(i) \cdot x_{s - d \cdot i}$$
from [[@baiEmpiricalEvaluationGeneric2018]]. #dilated-convolution

[[Residual Block|Residual blocks]] are used to combat [[Exploding Gradients|exploding]] or [[Vanishing Gradients|vanishing gradients]] due to the depth of network required. #residual-block #exploding-gradient #vanishing-gradient

An overview of the TCN architecture with [[Dilated Convolution|dilated convolutions]] and [[Residual Block|residual blocks]] from [[@baiEmpiricalEvaluationGeneric2018]] can be seen below. #TCN #temporal-convolutional-network #dilated-convolution #residual-block 

![[Pasted image 20240902162837.png]]

[[Multimodal Machine Learning|Multimodal]] TCNs have been used for tasks such as dance video segmentation [[@endoAutomaticDanceVideo2024]], 

# **Papers Using Temporal Convolutional Networks**

- [[@endoAutomaticDanceVideo2024]] - Dance Video Segmentation
- [[@weiTCNattentionHARHumanActivity2024]] - HAR






