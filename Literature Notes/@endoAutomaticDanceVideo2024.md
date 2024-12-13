#literature-note 

---
category:: literaturenote
tags:: read #temporal-convolutional-network #TCN #dance #multimodal #multimodal-learning #ablation #video #audio #AIST
citekey:: endoAutomaticDanceVideo2024
status:: read
reference:: Endo, K., Tsuchida, S., Fukusato, T., & Igarashi, T. (2024). ‘Automatic Dance Video Segmentation for Understanding Choreography’. _Proceedings of the 9th International Conference on Movement and Computing_, pp. 1–9. Presented at the MOCO ’24: 9th International Conference on Movement and Computing, May 30, Utrecht Netherlands: ACM. DOI: [10.1145/3658852.3659076](https://doi.org/10.1145/3658852.3659076)
dateread:
---

> [!Cite]
> Endo, K., Tsuchida, S., Fukusato, T., & Igarashi, T. (2024). ‘Automatic Dance Video Segmentation for Understanding Choreography’. _Proceedings of the 9th International Conference on Movement and Computing_, pp. 1–9. Presented at the MOCO ’24: 9th International Conference on Movement and Computing, May 30, Utrecht Netherlands: ACM. DOI: [10.1145/3658852.3659076](https://doi.org/10.1145/3658852.3659076)

^cite

>[!Synth]
>%% begin synth %%
>**Contribution**:: The main contribution of this paper is an automated system for the segmentation of audiovisual dance recordings corresponding to individual dance moves. This is achieved through the use of a [[Temporal Convolutional Network|TCN]], which is passed a [[Multimodality|multimodal]] feature vector consisting of extracted bone vectors from the [[Digital Video Signal|video]] and [[Mel Spectrogram|mel spectrogram]] for the corresponding frame from the [[Digital Audio Signal|audio]]. The model performed with an [[F1-Score]] of 0.797, which the authors claim shows an accuracy of approximately 80%. However, the model performed a lot better on certain genres and classes of dance video than others. Through an [[Ablation Study|ablation study]], they show that the [[Multimodal Machine Learning|multimodal modal]] performs [[Statistical Significance|statistically significantly]] better than the audio or video model alone. In addition they prepare a subset of the [[AIST Dance Video Database]] [[@tsuchidaAISTDanceVideo2019]] with annotations of the segmentation points between individual dance moves, as annotated by 21 annotators including the first author. Finally, they contribute a standalone application that annotates an imported video, although at time of writing, this has not yet been made publicly available.
>
>**Related**::
>![[@tsuchidaAISTDanceVideo2019#^cite]]
>![[@baiEmpiricalEvaluationGeneric2018#^cite]]
>%% end synth %%



>[!md]
> **FirstAuthor**:: Endo, Koki  
> **Author**:: Tsuchida, Shuhei  
> **Author**:: Fukusato, Tsukasa  
> **Author**:: Igarashi, Takeo  
~    
> **Title**:: Automatic Dance Video Segmentation for Understanding Choreography  
> **Year**:: 2024   
> **Citekey**:: endoAutomaticDanceVideo2024  
> **itemType**:: conferencePaper  
> **Publisher**:: ACM  
> **Location**:: Utrecht Netherlands   
> **Pages**:: 1-9  
> **DOI**:: 10.1145/3658852.3659076  
> **ISBN**:: 9798400709944    

> [!LINK] 
>
> [[Endo et al_2024_Automatic Dance Video Segmentation for Understanding Choreography.pdf]].

> [!Abstract]
>Segmenting dance video into short movements is a popular way to easily understand dance choreography. However, it is currently done manually and requires a significant amount of effort by experts. That is, even if many dance videos are available on social media (e.g., TikTok and YouTube), it remains difficult for people, especially novices, to casually watch short video segments to practice dance choreography. In this paper, we propose a method to automatically segment a dance video into each movement. Given a dance video as input, we first extract visual and audio features: the former is computed from the keypoints of the dancer in the video, and the latter is computed from the Mel spectrogram of the music in the video. Next, these features are passed to a Temporal Convolutional Network (TCN), and segmentation points are estimated by picking peaks of the network output. To build our training dataset, we annotate segmentation points to dance videos in the AIST Dance Video Database, which is a shared database containing original street dance videos with copyright-cleared dance music. The evaluation study shows that the proposed method (i.e., combining the visual and audio features) can estimate segmentation points with high accuracy. In addition, we developed an application to help dancers practice choreography using the proposed method.
> 
# Notes

%% begin notes %%

%% end notes %%
# Annotations%% begin annotations %%


%% end annotations %%

%% Import Date: 2024-09-23T19:07:07.723+02:00 %%
