#literature-note 

---
category:: literaturenote
tags:: #read #thermography #thermal-imaging #infra-red #IR 
status:: read 
reference:: Vollmer, M. (2021). ‘Infrared Thermal Imaging’. Ikeuchi K. (ed.) _Computer Vision: A Reference Guide_, pp. 666–70. Springer International Publishing: Cham. DOI: [10.1007/978-3-030-63416-2_844](https://doi.org/10.1007/978-3-030-63416-2_844)
dateread:
---

> [!Cite]
> Vollmer, M. (2021). ‘Infrared Thermal Imaging’. Ikeuchi K. (ed.) _Computer Vision: A Reference Guide_, pp. 666–70. Springer International Publishing: Cham. DOI: [10.1007/978-3-030-63416-2_844](https://doi.org/10.1007/978-3-030-63416-2_844)
^cite

>[!Synth]
>%% begin synth %%
>
>**Contribution**:: This short chapter provides an overview of [[Infra-Red Imaging|infra-red imaging]] with a focus on its use in [[Thermography|thermography]]. First, the chapter provides a brief description of how infra-red and thermal imaging works, comparing this to [[RGB Camera|visible light sensing]] with the description of some key differences. Thereafter, the chapter describes the key parameters which relate to the amount of thermal radiation emitted by an object, namely its temperature and its emissivity. The chapter defines [[Black Body|black bodies]], namely theoretical objects with perfect absorption and perfect emission (i.e. they have a maximum possible emissivity of 1). It provides an outline of how artificial black bodies are used to calibrate thermal cameras, and the challenges that are faced in doing so. Finally, the chapter provides an description of the common specifications of current commercial thermal cameras, and outlines open problems in the field of thermal imaging.
>
>**Related**::  
>%% end synth %%

>[!md]
> **FirstAuthor**:: Vollmer, Michael  
~> **FirstEditor**:: Ikeuchi, Katsushi  
~    
> **Title**:: Infrared Thermal Imaging  
> **Year**:: 2021   
> **Citekey**:: vollmerInfraredThermalImaging2021  
> **itemType**:: bookSection  
> **Book**::   
> **Publisher**:: Springer International Publishing  
> **Location**:: Cham   
> **Pages**:: 666-670  
> **ISBN**:: 978-3-030-63416-2    

> [!LINK] 
>
> [[Vollmer_2021_Infrared Thermal Imaging.pdf]].

> [!Abstract]
>.
> 
# Notes

%% begin notes %%

# Annotations  
(10/02/2025, 17:02:55)

[Go to annotation](zotero://open-pdf/library/items/A66JSK3G?page=1&annotation=Y77753TK) “Infrared thermal imaging is a technique to generate quantitative radiometric digital images of object scenes recorded in the thermal infrared wavelength range between 0.8 and 15 μm. Besides qualitative visualization, it allows to measure surface temperatures of objects [1–3].” ([Vollmer, 2021, p. 1](zotero://select/library/items/XMABE8J8)) Definition of thermography

[Go to annotation](zotero://open-pdf/library/items/A66JSK3G?page=1&annotation=M3ERKH9A) “IR cameras operate very similar to any visible light (VIS) camera (Fig. 1) [3]. The electromagnetic radiation from objects passes a lens system and maybe additional optical components before forming an image of the object on a detector, nowadays exclusively a focal plane array (FPA). Subsequently, the information from the individual pixels is gathered by some readout integrated circuit. The camera may – though need not – be operated remotely using a computer interface.” ([Vollmer, 2021, p. 1](zotero://select/library/items/XMABE8J8)) How a thermal camera works.

[Go to annotation](zotero://open-pdf/library/items/A66JSK3G?page=1&annotation=USL8KDH6) “First, the radiation is in the infrared part of the spectrum, typically from 0.8 μm to around 25 μm wavelength (VIS: 0.4 μm to 0.8 μm).” ([Vollmer, 2021, p. 1](zotero://select/library/items/XMABE8J8)) First difference between IR cameras and RGB Cameras. Wavelength range.

[Go to annotation](zotero://open-pdf/library/items/A66JSK3G?page=2&annotation=3ETPGNV7) “Second, this radiation is mostly thermally emitted radiation [3, 5, 6], whereas visual images typically reflect scenes of scattered light.” ([Vollmer, 2021, p. 2](zotero://select/library/items/XMABE8J8)) Second difference. Senses emitted thermal energy instead of reflected, scattered visible light.

[Go to annotation](zotero://open-pdf/library/items/A66JSK3G?page=2&annotation=KJREMT2Z) “Third, the optical materials of the lenses, filters, etc. must transmit this radiation and are therefore usually not made from glass but semiconductors.” ([Vollmer, 2021, p. 2](zotero://select/library/items/XMABE8J8)) Third difference. Materials need to be conductive, so made from semiconductors instead of glass.

[Go to annotation](zotero://open-pdf/library/items/A66JSK3G?page=2&annotation=8LNAP4UC) “Fourth, the detectors are not silicon based as in VIS cameras but – depending on the used wavelength region – chosen from a wide possible range of materials and techniques including cooled photoelectron as well as uncooled thermal detectors [1–3, 5–7]. Infrared detectors are more complex than VIS detectors, and, so far, IR FPA’s have much lower pixel numbers than VIS cameras, typically below 1 Mpixel.” ([Vollmer, 2021, p. 2](zotero://select/library/items/XMABE8J8)) Fourth difference. Sensor array not made of silicone but a variety of different materials. This means a lot lower resolution.

[Go to annotation](zotero://open-pdf/library/items/A66JSK3G?page=2&annotation=BD66WXE2) “Fifth, the pixel signals are usually not spectrally filtered and therefore resemble monochrome images. Using image processing, these are then displayed either as gray scale or false color images.” ([Vollmer, 2021, p. 2](zotero://select/library/items/XMABE8J8)) Fifth difference. No spectral filtering to obtain RGB components. So only single channel.

[Go to annotation](zotero://open-pdf/library/items/A66JSK3G?page=2&annotation=S7BNHF54) “Infrared radiation from objects only depends on the temperature of the objects and a material property called emissivity.” ([Vollmer, 2021, p. 2](zotero://select/library/items/XMABE8J8)) The two parameters upon which the amount of infra-red emission from an object depend: the object's temperature and its emissivity.

[Go to annotation](zotero://open-pdf/library/items/A66JSK3G?page=2&annotation=X6JY7JEM) “Objects which emit the maximum possible radiation are black bodies. Their spectrum is defined by Planck’s law [1–3, 5, 6], and it only depends on the object temperature. The larger the temperature, the more the spectrum shifts toward shorter wavelengths (” ([Vollmer, 2021, p. 2](zotero://select/library/items/XMABE8J8)) Definition of a black body. This is an object with a maximum emissivity (epsilon) of 1. In other words it is a perfect emitter and a perfect absorber of radiation. No real object is a perfect black body, but some objects like stars are approximate black bodies.

[Go to annotation](zotero://open-pdf/library/items/A66JSK3G?page=2&annotation=PKZSDPXZ) “Mostly three ranges are commercially used, the longwave (LW: 8–14 μm), mid-wave (MW: 3–5 μm), and short-wave (SW: 0.9–1.7 μm) region” ([Vollmer, 2021, p. 2](zotero://select/library/items/XMABE8J8)) The three wavelength ranges primarily used in commercial IR cameras: long-wave (8-14 micrometer), mid-wave (3-5 micrometer), short-wave (0.9-1.7 micrometer).

[Go to annotation](zotero://open-pdf/library/items/A66JSK3G?page=2&annotation=N9RV968L) “Real objects emit less radiation than black bodies, defined by their emissivity. Any quantitative analysis requires knowledge of the correct emissivity of the objects. Analysis is usually complicated by the fact that every image represents a combination of temperature as well as emissivity contrast.” ([Vollmer, 2021, p. 2](zotero://select/library/items/XMABE8J8)) Complications of the fact that real objects are not black bodies and therefore their level of radiation is determined through their emissivity. Therefore objects of the same temperature emit different levels of radiation based upon their emissivity.

[Go to annotation](zotero://open-pdf/library/items/A66JSK3G?page=3&annotation=BN5Q8K6Q) “For camera calibration, artificial black bodies of known temperatures are analyzed. Measured objects signals are compared to them with the goal to deduce surface temperatures (assuming opaque objects). The real problem then is to understand the observed object temperature distributions, i.e., relate them, e.g., to heat transfer processes associated with the objects.” ([Vollmer, 2021, p. 3](zotero://select/library/items/XMABE8J8)) Thermal cameras are calibrated through the use of artificial black bodies of known temperatures (i.e. removing the emissivity component). However, this is only a part of the problem. If you then point the camera at a real-world object, you still then have to account for parameters such as the emissivity, the fact that the camera only reads the surface temperature, heat transfer effects, reflections of infra-red radiation, and atmospheric effects.

[Go to annotation](zotero://open-pdf/library/items/A66JSK3G?page=3&annotation=4TSULAAF) “Most cameras nowadays allow for 25 fps or 30 fps; however, those with thermal detectors often show cometary tails of moving objects due to the long time constant of the detectors. In contrast, photoelectron detector cameras also allow high-speed IR recordings; they are, however, much more expensive.” ([Vollmer, 2021, p. 3](zotero://select/library/items/XMABE8J8)) Thermal cameras can leave cometary trails with moving objects, due to the processing time taken by the sensing array.
%% end notes %%


# Annotations%% begin annotations %%

### Imported: 2025-02-10 5:03 pm


<mark style="background-color: #000000">Quote</mark>
> Infrared thermal imaging is a technique to generate quantitative radiometric digital images of object scenes recorded in the thermal infrared wavelength range between 0.8 and 15 μm. Besides qualitative visualization, it allows to measure surface temperatures of objects [1–3].

<mark style="background-color: #000000">Quote</mark>
> IR cameras operate very similar to any visible light (VIS) camera (Fig. 1) [3]. The electromagnetic radiation from objects passes a lens system and maybe additional optical components before forming an image of the object on a detector, nowadays exclusively a focal plane array (FPA). Subsequently, the information from the individual pixels is gathered by some readout integrated circuit. The camera may – though need not – be operated remotely using a computer interface.

<mark style="background-color: #000000">Quote</mark>
> First, the radiation is in the infrared part of the spectrum, typically from 0.8 μm to around 25 μm wavelength (VIS: 0.4 μm to 0.8 μm).

<mark style="background-color: #000000">Quote</mark>
> Second, this radiation is mostly thermally emitted radiation [3, 5, 6], whereas visual images typically reflect scenes of scattered light.

<mark style="background-color: #000000">Quote</mark>
> Third, the optical materials of the lenses, filters, etc. must transmit this radiation and are therefore usually not made from glass but semiconductors.

<mark style="background-color: #000000">Quote</mark>
> Fourth, the detectors are not silicon based as in VIS cameras but – depending on the used wavelength region – chosen from a wide possible range of materials and techniques including cooled photoelectron as well as uncooled thermal detectors [1–3, 5–7]. Infrared detectors are more complex than VIS detectors, and, so far, IR FPA’s have much lower pixel numbers than VIS cameras, typically below 1 Mpixel.

<mark style="background-color: #000000">Quote</mark>
> Fifth, the pixel signals are usually not spectrally filtered and therefore resemble monochrome images. Using image processing, these are then displayed either as gray scale or false color images.

<mark style="background-color: #000000">Quote</mark>
> Infrared radiation from objects only depends on the temperature of the objects and a material property called emissivity.

<mark style="background-color: #000000">Quote</mark>
> Objects which emit the maximum possible radiation are black bodies. Their spectrum is defined by Planck’s law [1–3, 5, 6], and it only depends on the object temperature. The larger the temperature, the more the spectrum shifts toward shorter wavelengths (

<mark style="background-color: #000000">Quote</mark>
> Mostly three ranges are commercially used, the longwave (LW: 8–14 μm), mid-wave (MW: 3–5 μm), and short-wave (SW: 0.9–1.7 μm) region

<mark style="background-color: #000000">Quote</mark>
> Real objects emit less radiation than black bodies, defined by their emissivity. Any quantitative analysis requires knowledge of the correct emissivity of the objects. Analysis is usually complicated by the fact that every image represents a combination of temperature as well as emissivity contrast.

<mark style="background-color: #000000">Quote</mark>
> For camera calibration, artificial black bodies of known temperatures are analyzed. Measured objects signals are compared to them with the goal to deduce surface temperatures (assuming opaque objects). The real problem then is to understand the observed object temperature distributions, i.e., relate them, e.g., to heat transfer processes associated with the objects.

<mark style="background-color: #000000">Quote</mark>
> Most cameras nowadays allow for 25 fps or 30 fps; however, those with thermal detectors often show cometary tails of moving objects due to the long time constant of the detectors. In contrast, photoelectron detector cameras also allow high-speed IR recordings; they are, however, much more expensive.


%% end annotations %%









%% Import Date: 2025-02-10T17:03:30.814+01:00 %%
