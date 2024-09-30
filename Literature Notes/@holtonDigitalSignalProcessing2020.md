
---
category:: literaturenote
tags:: Digital techniques, Signal processing
citekey:: holtonDigitalSignalProcessing2020
status:: unread
dateread:
---

> [!Cite]
> Holton, T. (2020). _Digital signal processing: principles and applications_. Cambridge, United Kingdom ; New York, NY, USA: Cambridge University Press.

>[!Synth]
>**Contribution**:: 
>
>**Related**:: 
>

>[!md]
> **FirstAuthor**:: Holton, Thomas  
~    
> **Title**:: Digital signal processing: principles and applications  
> **Year**:: 2020   
> **Citekey**:: holtonDigitalSignalProcessing2020  
> **itemType**:: book  
> **Publisher**:: Cambridge University Press  
> **Location**:: Cambridge, United Kingdom ; New York, NY, USA  
> **ISBN**:: 978-1-108-41844-7    

> [!LINK] 
>
> [[Holton_2020_Digital signal processing.pdf]].

> [!Abstract]
>
> "Combining clear explanations of elementary principles, advanced topics, and applications, with step-by-step mathematical derivations, this textbook provides a comprehensive yet accessible introduction to digital signal processing. All the key topics are covered, including discrete-time Fourier transform, z-transform, discrete Fourier transform, and A/D conversion, as well as more advanced topics such as FIR and IIR filtering algorithms, multi-rate systems, the discrete cosine transform, and spectral signal processing. Over 600 full-color illustrations, 200 fully worked examples, hundreds of end-of-chapter homework problems, and detailed computational examples of DSP algorithms implemented in Matlab and C aid understanding and help put knowledge into practice. A wealth of supplementary material accompanies the book online, including interactive programs for instructors, a full set of solutions, and Matlab laboratory exercises, making this the ideal text for senior undergraduate and graduate courses on digital signal processing"--
>.
> 
# Notes
>.


# Annotations%% begin annotations %%



### Imported: 2024-09-30 4:43 pm



<mark style="background-color: #ffaa00">Quote</mark>
> Consider a continuous-time signal cos Ω0t. Since the argument of the cosine must be in radians, Ω0t must have units of radians, and therefore the continuous-time frequency Ω0 has units of radians/sec; that is, it is an angular frequency. Now consider a discrete-time sequence cos ω0n. Again, the argument of the cosine must be radians, so ω0n must be in radians. Thus, the discrete-time frequency ω0 must have units of radians/sample, which is equal to radians, since “sample” is a number and therefore dimensionless. That is, discrete-time frequency is actually equivalent to phase. In this book, we will always use capital omega Ω to denote continuous-time frequency and small omega ω to denote discrete-time frequency.

<mark style="background-color: #ffaa00">Quote</mark>
> In the continuous-time world, sinusoids of different frequencies are unique. That is, given two frequencies Ω1 and Ω2,ifΩ1 / = Ω2,then cos Ω1t / = cos Ω2t for all t. In the discrete-time world, sinusoidal sequences of different frequencies are not necessarily distinct. Consider two “different” discrete-time sinusoidal sequences x1[n] = cos ω1n and x2[n] = cos ω2n, where ω1 / = ω2. We might expect x1[n]/ = x2[n] over all n, but that is not always true. Specifically, let ω2 = ω1 +2πk, where k is an integer. As long as k / = 0, then ω1 / = ω2, but x2[n] = cos ω2n = cos(ω1 +2πk) = cos ω1n = x1[n]. Thus, x1[n]=x2[n]foralln. This says that discrete-time sinusoidal sequences whose frequencies ω1 and ω2 differ by an integer multiple of 2π are indistinguishable. Of course, that makes sense when you remember that discrete-time frequency is actually phase. Figure 1.21 shows the equivalence of three discrete-time sinusoidal sequences whose frequencies differ by multiples of 2π.


%% end annotations %%

%% Import Date: 2024-09-30T16:43:51.110+02:00 %%
