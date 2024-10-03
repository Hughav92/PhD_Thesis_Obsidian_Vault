
---
category:: literaturenote
tags:: Computer Science - Artificial Intelligence, Computer Science - Computation and Language, Computer Science - Machine Learning
citekey:: baiEmpiricalEvaluationGeneric2018
status:: unread
reference:: Bai, S., Kolter, J. Z., & Koltun, V. (2018). ‘An Empirical Evaluation of Generic Convolutional and Recurrent Networks for Sequence Modeling’. arXiv.
dateread:
---

> [!Cite]
> Bai, S., Kolter, J. Z., & Koltun, V. (2018). ‘An Empirical Evaluation of Generic Convolutional and Recurrent Networks for Sequence Modeling’. arXiv.

^d265b9

>[!Synth]
>**Contribution**:: 
>
>**Related**:: 
>

>[!md]
> **FirstAuthor**:: Bai, Shaojie  
> **Author**:: Kolter, J. Zico  
> **Author**:: Koltun, Vladlen  
~    
> **Title**:: An Empirical Evaluation of Generic Convolutional and Recurrent Networks for Sequence Modeling  
> **Year**:: 2018   
> **Citekey**:: baiEmpiricalEvaluationGeneric2018  
> **itemType**:: preprint    

> [!LINK] 
>
> [[Bai et al_2018_An Empirical Evaluation of Generic Convolutional and Recurrent Networks for.pdf]].

> [!Abstract]
>
> For most deep learning practitioners, sequence modeling is synonymous with recurrent networks. Yet recent results indicate that convolutional architectures can outperform recurrent networks on tasks such as audio synthesis and machine translation. Given a new sequence modeling task or dataset, which architecture should one use? We conduct a systematic evaluation of generic convolutional and recurrent architectures for sequence modeling. The models are evaluated across a broad range of standard tasks that are commonly used to benchmark recurrent networks. Our results indicate that a simple convolutional architecture outperforms canonical recurrent networks such as LSTMs across a diverse range of tasks and datasets, while demonstrating longer effective memory. We conclude that the common association between sequence modeling and recurrent networks should be reconsidered, and convolutional networks should be regarded as a natural starting point for sequence modeling tasks. To assist related work, we have made code available at http://github.com/locuslab/TCN .
>.
> 
# Notes
>
># Annotations  
(02/09/2024, 15:51:03)

[Go to annotation](zotero://open-pdf/library/items/DX372JDZ?page=3&annotation=BTAM78YC) “The distinguishing characteristics of TCNs are: 1) the convolutions in the architecture are causal, meaning that there is no information “leakage” from future to past; 2) the architecture can take a sequence of any length and map it to an output sequence of the same length, just as with an RNN.” ([Bai et al., 2018, p. 3](zotero://select/library/items/2UF9HWLW)) The two distinguishing features of the TCN.

[Go to annotation](zotero://open-pdf/library/items/DX372JDZ?page=3&annotation=YWB8P8GZ) “To put it simply: TCN = 1D FCN + causal convolutions.” ([Bai et al., 2018, p. 3](zotero://select/library/items/2UF9HWLW)) Nice and simple definition of a TCN.

[Go to annotation](zotero://open-pdf/library/items/DX372JDZ?page=3&annotation=BYUGMJIU) “F (s) = (x ∗d f )(s) = k−1 ∑ i=0 f (i) · xs−d·i” ([Bai et al., 2018, p. 3](zotero://select/library/items/2UF9HWLW)) Formal definition of dilation convolutions..


# Annotations%% begin annotations %%



### Imported: 2024-09-23 7:04 pm



<mark style="background-color: #000000">Quote</mark>
> The distinguishing characteristics of TCNs are: 1) the convolutions in the architecture are causal, meaning that there is no information “leakage” from future to past; 2) the architecture can take a sequence of any length and map it to an output sequence of the same length, just as with an RNN.

<mark style="background-color: #000000">Quote</mark>
> To put it simply: TCN = 1D FCN + causal convolutions.

<mark style="background-color: #000000">Quote</mark>
> F (s) = (x ∗d f )(s) = k−1 ∑ i=0 f (i) · xs−d·i


%% end annotations %%

%% Import Date: 2024-09-23T19:04:58.948+02:00 %%
