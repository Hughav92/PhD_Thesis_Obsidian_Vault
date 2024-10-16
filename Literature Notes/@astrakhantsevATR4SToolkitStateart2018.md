#literature-note 

---
category:: literaturenote
tags:: read #automatic-terminology-recognition #atr #corpus #methods #toolbox #computational-linguistics
citekey:: astrakhantsevATR4SToolkitStateart2018
status:: read
reference:: Astrakhantsev, N. (2018). ‘ATR4S: toolkit with state-of-the-art automatic terms recognition methods in Scala’, _Language Resources and Evaluation_, 52/3: 853–72. DOI: [10.1007/s10579-017-9409-4](https://doi.org/10.1007/s10579-017-9409-4)
dateread:
---

> [!Cite]
> Astrakhantsev, N. (2018). ‘ATR4S: toolkit with state-of-the-art automatic terms recognition methods in Scala’, _Language Resources and Evaluation_, 52/3: 853–72. DOI: [10.1007/s10579-017-9409-4](https://doi.org/10.1007/s10579-017-9409-4)

^58f2b5

>[!Synth]
>**Contribution**:: This paper presents a review of multiple methods for both [[Automatic Terminology Recognition|automatic terminology recognition]] and the [[Automatic Terminology Recognition Methods#Methods for Term Candidate Ranking|ranking of term candidates]]. In addition, this paper contributes a [Scala toolbox](https://github.com/ispras/atr4s) which implements 15 of these methods. Finally the authors evaluate theses methods in their implementation, and find that [[PU-ATR]] performs best for small datasets and corpora in cases where time complexity is not an issue, [[Basic Score]] or [[Combo Basic Score]] perform best for large datasets, and [[Key Concept Relatedness]] performs best for tasks requiring the recognition of few terms for domains well covered by Wikipedia.
>
>**Related**:: 
>![[@ahmadUniversitySurreyParticipation1999#^a6ecc9]]
>![[@astrakhantsevMethodsSoftwareTerminology2015#^7148a9]]
>![[@bordeaDomainindependentTermExtraction2013#^005332]]
>![[@churchInverseDocumentFrequency1999#^0906bd]]
>![[@evansCLARITTRECExperiments1995#^1a4cc3]]
>![[@frantziAutomaticRecognitionMultiword2000#^f79158]]
>![[@justesonTechnicalTerminologyLinguistic1995#^8f8387]]
>![[@liNovelTopicModel2013#^a3b1e8]]
>![[@lossio-venturaCombiningCvalueKeyword2013#^5e30eb]]
>![[@meijerSemanticApproachExtracting2014#^5676be]]
>![[@omara-evesTechniquesIdentifyingCrossdisciplinary2013#^510779]]
>![[@parkAutomaticGlossaryExtraction2002#^3da2ba]]
>![[@penasCorpusbasedTerminologyExtraction2001#^d0d6d0]]
>![[@sparckjonesStatisticalInterpretationTerm1972#^ddbe22]]
>![[@zhangComparativeEvaluationTerm2008#^f864dd]]
>![[@zhangJATE20Java2016#^29f77d]]]


>[!md]
> **FirstAuthor**:: Astrakhantsev, Nikita  
~    
> **Title**:: ATR4S: toolkit with state-of-the-art automatic terms recognition methods in Scala  
> **Year**:: 2018   
> **Citekey**:: astrakhantsevATR4SToolkitStateart2018  
> **itemType**:: journalArticle  
> **Journal**:: *Language Resources and Evaluation*  
> **Volume**:: 52  
> **Issue**:: 3   
> **Pages**:: 853-872  
> **DOI**:: 10.1007/s10579-017-9409-4    

> [!LINK] 
>
> [[Astrakhantsev_2018_ATR4S toolkit with state-of-the-art automatic terms recognition methods in Scala.pdf]].

> [!Abstract]
>
> Automatically recognized terminology is widely used for various domain-specific texts processing tasks, such as machine translation, information retrieval or ontology construction. However, there is still no agreement on which methods are best suited for particular settings and, moreover, there is no reliable comparison of already developed methods. We believe that one of the main reasons is the lack of state-of-the-art method implementations, which are usually non-trivial to recreate—mostly, in terms of software engineering efforts. In order to address these issues, we present ATR4S, an open-source software written in Scala that comprises 13 state-of-the-art methods for automatic terminology recognition (ATR) and implements the whole pipeline from text document preprocessing, to term candidates collection, term candidate scoring, and finally, term candidate ranking. It is highly scalable, modular and configurable tool with support of automatic caching. We also compare 13 state-of-the-art methods on 7 open datasets by average precision and processing time. Experimental comparison reveals that no single method demonstrates best average precision for all datasets and that other available tools for ATR do not contain the best methods.
>.
> 
# Notes
>
># Annotations  
(24/09/2024, 10:23:56)

[Go to annotation](zotero://open-pdf/library/items/UPF8HZH6?page=854&annotation=679B4ZJQ) “Automatic terminology recognition (ATR) aims at extraction of terms—words and collocations designating domain-specific concepts—from a collection of text documents belonging to that domain.” ([Astrakhantsev, 2018, p. 854](zotero://select/library/items/YPFDJJKB)) Definition of Automatic Terminology Recognition (ATR).

[Go to annotation](zotero://open-pdf/library/items/UPF8HZH6?page=855&annotation=6YNVB2YI) “Finally, the most recent survey by Astrakhantsev et al. (2015) identified the general pipeline of ATR methods: preprocessing, term candidates collection, term candidate scoring, and term candidate ranking.” ([Astrakhantsev, 2018, p. 855](zotero://select/library/items/YPFDJJKB)) Description of general pipeline of ATR methods..


# Annotations%% begin annotations %%


### Imported: 2024-09-24 10:20 am



<mark style="background-color: #000000">Quote</mark>
> Automatic terminology recognition (ATR) aims at extraction of terms—words and collocations designating domain-specific concepts—from a collection of text documents belonging to that domain.

<mark style="background-color: #000000">Quote</mark>
> Finally, the most recent survey by Astrakhantsev et al. (2015) identified the general pipeline of ATR methods: preprocessing, term candidates collection, term candidate scoring, and term candidate ranking.


### Imported: 2024-09-27 4:45 pm



<mark style="background-color: #000000">Quote</mark>
> TF-IDF is a classical information retrieval measure showing high values for term candidates that occur frequently in few documents:  TF  IDFðtÞ 1⁄4 TFðtÞ  log D  DTFðtÞ

<mark style="background-color: #000000">Quote</mark>
> RIDF was originally proposed for keywords extraction (Church and Gale 1999) and than re-used for term recognition (Zhang et al. 2016). It is based on the assumption that the deviation of observed IDF from the IDF modeled by Poisson distribution is higher for keywords than for ordinary words.  RIDFðtÞ 1⁄4 TFðtÞ  log D  DTFðtÞ þ logð1  eATFðtÞÞ;


### Imported: 2024-09-27 4:56 pm



<mark style="background-color: #000000">Quote</mark>
> Automatic terminology recognition (ATR) aims at extraction of terms—words and collocations designating domain-specific concepts—from a collection of text documents belonging to that domain.

<mark style="background-color: #000000">Quote</mark>
> Finally, the most recent survey by Astrakhantsev et al. (2015) identified the general pipeline of ATR methods: preprocessing, term candidates collection, term candidate scoring, and term candidate ranking.

<mark style="background-color: #000000">Quote</mark>
> TF-IDF is a classical information retrieval measure showing high values for term candidates that occur frequently in few documents:  TF  IDFðtÞ 1⁄4 TFðtÞ  log D  DTFðtÞ

<mark style="background-color: #000000">Quote</mark>
> RIDF was originally proposed for keywords extraction (Church and Gale 1999) and than re-used for term recognition (Zhang et al. 2016). It is based on the assumption that the deviation of observed IDF from the IDF modeled by Poisson distribution is higher for keywords than for ordinary words.  RIDFðtÞ 1⁄4 TFðtÞ  log D  DTFðtÞ þ logð1  eATFðtÞÞ;

<mark style="background-color: #000000">Quote</mark>
> C-Value, one of the most popular methods, promotes term candidates that occur frequently, but not as parts of other term candidates. This method was supposed to work with multi-word term candidates only; ATR4S includes modification proposed by Ventura et al. (2013) that supports one-word term candidates as well:  C-ValueðtÞ 1⁄4  log2ðjtj þ aÞ  TFðtÞ; if fs : t  sg 1⁄4 ;;  log2ðjtj þ aÞ  TFðtÞ   P  s TFðsÞ jfs : t  sgj    ;


%% end annotations %%

%% Import Date: 2024-10-03T12:40:19.683+02:00 %%
