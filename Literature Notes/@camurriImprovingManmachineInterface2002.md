#literature-note 

---
category:: literaturenote
tags:: #User-interfaces #Humans #read #Concrete #Algorithm-design-and-analysis #Computational-modeling #Facial-animation #Information-processing #Interactive-systems #Robot-sensing-systems #Software-libraries #QOMOP 
status:: read 
dateread:: 2025-04-23
reference:: Camurri, A., Coletta, P., Mazzarino, B., Trocca, R., & Volpe, G. (2002). ‘Improving the man-machine interface through the analysis of expressiveness in human movement’. _Proceedings. 11th IEEE international workshop on robot and human interactive communication_, pp. 417–22. DOI: [10.1109/ROMAN.2002.1045658](https://doi.org/10.1109/ROMAN.2002.1045658)

---

> [!Cite]
> Camurri, A., Coletta, P., Mazzarino, B., Trocca, R., & Volpe, G. (2002). ‘Improving the man-machine interface through the analysis of expressiveness in human movement’. _Proceedings. 11th IEEE international workshop on robot and human interactive communication_, pp. 417–22. DOI: [10.1109/ROMAN.2002.1045658](https://doi.org/10.1109/ROMAN.2002.1045658)
^cite

>[!Synth]
>%% begin synth %%
>
>**Contribution**:: This paper aims to demonstrate the application of computation techniques for the analysis of expressive qualities of human motion. This is framed in terms of the author's previous multi-layer model for the analysis of expressive gesture. The author's walk through the process of deriving the [[Quantity of Motion]] and [[Contraction Index]] from [[Silhouette Motion Image|Silhouette Motion Images]] derived from video recordings of a dancer, which they then correlate with expressive qualities of the dance as evaluated by human participants. This paper seems to provide the first formal definition of [[Quantity of Motion]] as a feature in the analysis of human motion.
>
>**Related**::  
>![[@camurriMultilayeredConceptualFramework2001a#^cite]]
>![[@camurriInteractiveSystemsDesign2002#^cite]]
>![[@camurriRecognizingEmotionDance2003#^cite]]
>![[@camurriApplicationMultimediaTechniques2003#^cite]]
>![[@camurriMultimodalAnalysisExpressive2004#^cite]]
>
>%% end synth %%

>[!md]
> **FirstAuthor**:: Camurri, Antonio  
> **Author**:: Coletta, Paolo  
> **Author**:: Mazzarino, Barbara  
> **Author**:: Trocca, Riccardo  
> **Author**:: Volpe, Gualtiero  
~    
> **Title**:: Improving the man-machine interface through the analysis of expressiveness in human movement  
> **Year**:: 2002   
> **Citekey**:: camurriImprovingManmachineInterface2002  
> **itemType**:: conferencePaper   
> **Pages**:: 417-422  
> **DOI**:: 10.1109/ROMAN.2002.1045658    

> [!LINK] 
>
> [[Literature/Library/BN7Y8K9L/Camurri et al._2002_Improving the man-machine interface through the analysis of expressiveness in human movement.pdf|Camurri et al._2002_Improving the man-machine interface through the analysis of expressiveness in human movement]].

> [!Abstract]
>In this paper our recent development in the research of computational models and algorithms f o r the real-time analysis of full-hody human movement are presented. Our aim is to find methods and techniques to extract cues relevant to KANSEI and emotional content in human expressive gesture in real time. Analysis of expressiveness in human gestures can contribute to new paradigms for the design of improved human-robot interfaces. As a main concrete result of our research work, a software platform named EyesWeb has been developed and is distributed for free (www.eyesweb.org). EyesWeb supports research in multimodal interaction, and provides a concrete tool f o r developing real-time interactive applications. Human movement analysis is provided by means of a library of algorithms f o r sensors and video processing, features extraction, gesture segmentation, etc. A visual environment is provided to compose such basic algorithms in order to develop more sophisticated analysis techniques.


%% begin QOM %%

> [!Quantity of Motion]
>**Modality**:: Video
>
>**Operationalisation**:: Calculated as the area of the [[Silhouette Motion Image]]. Specifically framed first as an approximation of momentum $mass \times velocity$ and then as an approximation of a velocity curve.
>
>**Use**:: Used as one out of several features to explore the extraction of gestural expressivity. Shown to correlate with subjective evaluations of dancers' motion by observers.
>
>**Other**:: Important paper, first formal definition of [[Quantity of Motion]]. Originally defined as an approximation of momentum, which was its original meaning in the Cartesian use of the term (with the caveat that Descartes made several mistakes). It's then treated as approximating a velocity curve (without momentum), so this paper raises several really interesting questions (in the notes below).

%% end QOM %%


# Notes

%% begin notes %%

# Annotations  
(23/04/2025, 18:06:07)

[Go to annotation](zotero://open-pdf/library/items/BN7Y8K9L?page=419&annotation=3ZNC783N) “Extraction of low level features and parameters (Layer 2): in particular, the quantity of motion and the contraction index are here presented as examples of cues at this level.” ([Camurri et al., 2002, p. 419](zotero://select/library/items/8RSJZX3F)) Quantity of motion as a feature extracted on layer 2 of Camurri's model.

[Go to annotation](zotero://open-pdf/library/items/BN7Y8K9L?page=419&annotation=ZXPRAFN9) “A Silhouette Motion Image is an image camying information about variations of the silhouette shape and position in the last few frames. SMIs can be seen as a special case of Motion Templates (see [14]j and are inspired to ME1 and MHI ([12]j, where information about time is implicit in the image and not explicitly recorded. We use an extension of SMIs which also takes account of the internal motion in silhouettes (see Figure 2b).” ([Camurri et al., 2002, p. 419](zotero://select/library/items/8RSJZX3F)) Definition of silhouette motion image (SMI).

[Go to annotation](zotero://open-pdf/library/items/BN7Y8K9L?page=419&annotation=IJ2ZCNH2) “information about variations of the silhouette shape and position in the last few frames. SMIs can be seen as a special case of Motion Templates (see [14]j and are inspired to ME1 and MHI ([12]j, where information about time is implicit in the image and not explicitly recorded. We use an extension of SMIs which also takes account of the internal motion in silhouettes (see Figure 2b).” ([Camurri et al., 2002, p. 419](zotero://select/library/items/8RSJZX3F)) Definition of silhouette motion image (SMI).

[Go to annotation](zotero://open-pdf/library/items/BN7Y8K9L?page=419&annotation=TS8R4ZSP) “The simplest use of a SMI is calculating its area. The result can he thought as a rough approximation of the quantity of motion, i.e. q = m * v , where m is the mass and v stands for velocity. The shape of the graph is close to the shape of the graphs of velocity of a marker put on a limb.” ([Camurri et al., 2002, p. 419](zotero://select/library/items/8RSJZX3F)) Formal definition of quantity of motion. The area of the silhouette motion image. Taken as a simple approximation of mass x velocity. This is super interesting because this means that it is meant to approximate momentum. And it is meant in the terms of its definition by Descartes. Why QOM and not momentum?

[Go to annotation](zotero://open-pdf/library/items/BN7Y8K9L?page=420&annotation=GSF3C3DE) “The SMI has interesting properties: the evolution in time of its (normalized) area (what we called quantity of motion) resembles the evolution of velocity of biological motion, which can be roughly described as a sequence of bell-shaped curves (motion hells). In order to segment motion by identifying the component gestures, it is interesting to extract a list of these motion bells and their features, e.g., peak value and duration. This can be also useful to obtain a first simple symbolical description of motion. One of the problems with the SMI approach, even dividing it in two vertical halves, is that several different movements may result super-imposed to each other, resulting in several motion bells to be overlapped. It is necessary to separate those motion hells in order to have a better description of motion. A first attempt consists in recognizing phases during which the dancer is moving (motion phases) and phases during which the dancer does not (i.e., movement is not perceived by a spectator) to move (pause phases). Actually, even if the dancer seems not to be moving, very m a l l movements occur and they %e detected by the motion image (together with some nhise). An empirical threshold has been defined: the dancer is considered to be moving if the area of the motion image is greater than 2.5% of the total area of the silhouette. Figure 4 shows motion bells after segmentation: a motion bell characterizes each motion phase” ([Camurri et al., 2002, p. 420](zotero://select/library/items/8RSJZX3F)) This is even more interesting. Here the justification is that the QOM curve resembles a velocity curve. There is no mention of mass. So there are some questions. First does a QOM curve resemble a velocity curve? Second, does this then hold for other modalities for which QOM is calculated (i.e. accelerometers/optical MoCap)? And if this is a modality from which we can calculated velocity, why calculated QOM? What does QOM tell us that velocity can't? Third, what happened to the mass? Does QOM represent a momentum curve?

# Date Read

2025-04-23

# Figures

![[Pasted image 20250423183654.png]]
Examples of a [[Silhouette Motion Image]]
%% end notes %%


# Annotations%% begin annotations %%



### Imported: 2025-04-23 6:08 pm


<mark style="background-color: #f0ff00">Quote</mark>
> Extraction of low level features and parameters (Layer 2): in particular, the quantity of motion and the contraction index are here presented as examples of cues at this level.

<mark style="background-color: #000000">Quote</mark>
> A Silhouette Motion Image is an image camying information about variations of the silhouette shape and position in the last few frames. SMIs can be seen as a special case of Motion Templates (see [14]j and are inspired to ME1 and MHI ([12]j, where information about time is implicit in the image and not explicitly recorded. We use an extension of SMIs which also takes account of the internal motion in silhouettes (see Figure 2b).

<mark style="background-color: #000000">Quote</mark>
> information about variations of the silhouette shape and position in the last few frames. SMIs can be seen as a special case of Motion Templates (see [14]j and are inspired to ME1 and MHI ([12]j, where information about time is implicit in the image and not explicitly recorded. We use an extension of SMIs which also takes account of the internal motion in silhouettes (see Figure 2b).

<mark style="background-color: #f0ff00">Quote</mark>
> The simplest use of a SMI is calculating its area. The result can he thought as a rough approximation of the  quantity of motion, i.e. q = m * v , where m is the mass and v stands for velocity. The shape of the graph is close to the shape of the graphs of velocity of a marker put on a limb.

<mark style="background-color: #f0ff00">Quote</mark>
> The SMI has interesting properties: the evolution in time of its (normalized) area (what we called quantity of motion) resembles the evolution of velocity of biological motion, which can be roughly described as a sequence of bell-shaped curves (motion hells). In order to segment motion by identifying the component gestures, it is interesting to extract a list of these motion bells and their features, e.g., peak value and duration. This can be also useful to obtain a first simple symbolical description of motion. One of the problems with the SMI approach, even dividing it in two vertical halves, is that several different movements may result super-imposed to each other, resulting in several motion bells to be overlapped. It is necessary to separate those motion hells in order to have a better description of motion. A first attempt consists in recognizing phases during which the dancer is moving (motion phases) and phases during which the dancer does not (i.e., movement is not perceived by a spectator) to move (pause phases). Actually, even if the dancer seems not to be moving, very m a l l movements occur and they %e detected by the motion image (together with some nhise). An empirical threshold has been defined: the dancer is considered to be moving if the area of the motion image is greater than 2.5% of the total area of the silhouette. Figure 4 shows motion bells after segmentation: a motion bell characterizes each motion phase

<mark style="background-color: #f0ff00">Quote</mark>
> Extraction of low level features and parameters (Layer 2): in particular, the quantity of motion and the contraction index are here presented as examples of cues at this level.

<mark style="background-color: #000000">Quote</mark>
> A Silhouette Motion Image is an image camying information about variations of the silhouette shape and position in the last few frames. SMIs can be seen as a special case of Motion Templates (see [14]j and are inspired to ME1 and MHI ([12]j, where information about time is implicit in the image and not explicitly recorded. We use an extension of SMIs which also takes account of the internal motion in silhouettes (see Figure 2b).

<mark style="background-color: #000000">Quote</mark>
> information about variations of the silhouette shape and position in the last few frames. SMIs can be seen as a special case of Motion Templates (see [14]j and are inspired to ME1 and MHI ([12]j, where information about time is implicit in the image and not explicitly recorded. We use an extension of SMIs which also takes account of the internal motion in silhouettes (see Figure 2b).

<mark style="background-color: #f0ff00">Quote</mark>
> The simplest use of a SMI is calculating its area. The result can he thought as a rough approximation of the * quantity of motion, i.e. q=m * v, where m is the mass and v stands for velocity. The shape of the graph is close to the shape of the graphs of velocity of a marker put on a limb.

<mark style="background-color: #f0ff00">Quote</mark>
> The SMI has interesting properties: the evolution in time of its (normalized) area (what we called quantity of motion) resembles the evolution of velocity of biological motion, which can be roughly described as a sequence of bell-shaped curves (motion hells). In order to segment motion by identifying the component gestures, it is interesting to extract a list of these motion bells and their features, e.g., peak value and duration. This can be also useful to obtain a first simple symbolical description of motion. One of the problems with the SMI approach, even dividing it in two vertical halves, is that several different movements may result super-imposed to each other, resulting in several motion bells to be overlapped. It is necessary to separate those motion hells in order to have a better description of motion. A first attempt consists in recognizing phases during which the dancer is moving (motion phases) and phases during which the dancer does not (i.e., movement is not perceived by a spectator) to move (pause phases). Actually, even if the dancer seems not to be moving, very mall movements occur and they %e detected by the motion image (together with some nhise). An empirical threshold has been defined: the dancer is considered to be moving if the area of the motion image is greater than 2.5% of the total area of the silhouette. Figure 4 shows motion bells after segmentation: a motion bell characterizes each motion phase


%% end annotations %%









%% Import Date: 2025-04-23T18:08:38.177+02:00 %%
