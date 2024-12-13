#literature-note 

---
category:: literaturenote
tags:: read
citekey:: astrakhantsevATR4SToolkitStateart2018
status:: read
reference:: Astrakhantsev, N. (2018). ‘ATR4S: toolkit with state-of-the-art automatic terms recognition methods in Scala’, _Language Resources and Evaluation_, 52/3: 853–72. DOI: [10.1007/s10579-017-9409-4](https://doi.org/10.1007/s10579-017-9409-4)
dateread:
---

> [!Cite]
> Astrakhantsev, N. (2018). ‘ATR4S: toolkit with state-of-the-art automatic terms recognition methods in Scala’, _Language Resources and Evaluation_, 52/3: 853–72. DOI: [10.1007/s10579-017-9409-4](https://doi.org/10.1007/s10579-017-9409-4)
^cite

>[!Synth]
>%% begin synth %%
>
>**Contribution**:: This paper presents a review of multiple methods for both [[Automatic Terminology Recognition|automatic terminology recognition]] and the [[Automatic Terminology Recognition Methods#Methods for Term Candidate Ranking|ranking of term candidates]]. In addition, this paper contributes a [Scala toolbox](https://github.com/ispras/atr4s) which implements 15 of these methods. Finally the authors evaluate theses methods in their implementation, and find that [[PU-ATR]] performs best for small datasets and corpora in cases where time complexity is not an issue, [[Basic Score]] or [[Combo Basic Score]] perform best for large datasets, and [[Key Concept Relatedness]] performs best for tasks requiring the recognition of few terms for domains well covered by Wikipedia.
>
>**Related**:: 
>![[@ahmadUniversitySurreyParticipation1999#^cite]]
>![[@astrakhantsevMethodsSoftwareTerminology2015#^cite]]
>![[@bordeaDomainindependentTermExtraction2013#^cite]]
>![[@churchInverseDocumentFrequency1999#^cite]]
>![[@evansCLARITTRECExperiments1995#^cite]]
>![[@frantziAutomaticRecognitionMultiword2000#^cite]]
>![[@justesonTechnicalTerminologyLinguistic1995#^cite]]
>![[@liNovelTopicModel2013#^cite]]
>![[@lossio-venturaCombiningCvalueKeyword2013#^cite]]
>![[@meijerSemanticApproachExtracting2014#^cite]]
>![[@omara-evesTechniquesIdentifyingCrossdisciplinary2013#^cite]]
>![[@parkAutomaticGlossaryExtraction2002#^cite]]
>![[@penasCorpusbasedTerminologyExtraction2001#^cite]]
>![[@sparckjonesStatisticalInterpretationTerm1972#^cite]]
>![[@zhangComparativeEvaluationTerm2008#^cite]]
>![[@zhangJATE20Java2016#^cite]]
>>%% end synth %%

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

%% begin notes %%
># Annotations  
(24/09/2024, 10:23:56)

[Go to annotation](zotero://open-pdf/library/items/UPF8HZH6?page=854&annotation=679B4ZJQ) “Automatic terminology recognition (ATR) aims at extraction of terms—words and collocations designating domain-specific concepts—from a collection of text documents belonging to that domain.” ([Astrakhantsev, 2018, p. 854](zotero://select/library/items/YPFDJJKB)) Definition of Automatic Terminology Recognition (ATR).

[Go to annotation](zotero://open-pdf/library/items/UPF8HZH6?page=855&annotation=6YNVB2YI) “Finally, the most recent survey by Astrakhantsev et al. (2015) identified the general pipeline of ATR methods: preprocessing, term candidates collection, term candidate scoring, and term candidate ranking.” ([Astrakhantsev, 2018, p. 855](zotero://select/library/items/YPFDJJKB)) Description of general pipeline of ATR methods..
# Annotations  
(24/09/2024, 10:23:56)

[Go to annotation](zotero://open-pdf/library/items/UPF8HZH6?page=854&annotation=679B4ZJQ) “Automatic terminology recognition (ATR) aims at extraction of terms—words and collocations designating domain-specific concepts—from a collection of text documents belonging to that domain.” ([Astrakhantsev, 2018, p. 854](zotero://select/library/items/YPFDJJKB)) Definition of Automatic Terminology Recognition (ATR).

[Go to annotation](zotero://open-pdf/library/items/UPF8HZH6?page=855&annotation=6YNVB2YI) “Finally, the most recent survey by Astrakhantsev et al. (2015) identified the general pipeline of ATR methods: preprocessing, term candidates collection, term candidate scoring, and term candidate ranking.” ([Astrakhantsev, 2018, p. 855](zotero://select/library/items/YPFDJJKB)) Description of general pipeline of ATR methods.
%% end notes %%


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


### Imported: 2024-12-12 6:42 pm



<mark style="background-color: #000000">Quote</mark>
> Automatic terminology recognition (ATR) aims at extraction of terms—words and collocations designating domain-specific concepts—from a collection of text documents belonging to that domain.

<mark style="background-color: #000000">Quote</mark>
> Finally, the most recent survey by Astrakhantsev et al. (2015) identified the general pipeline of ATR methods: preprocessing, term candidates collection, term candidate scoring, and term candidate ranking.

<mark style="background-color: #000000">Quote</mark>
> TF-IDF is a classical information retrieval measure showing high values for term candidates that occur frequently in few documents: TF � IDFðtÞ ¼ TFðtÞ � log D DTFðtÞ ; ð1Þ

<mark style="background-color: #000000">Quote</mark>
> RIDF was originally proposed for keywords extraction (Church and Gale 1999) and than re-used for term recognition (Zhang et al. 2016). It is based on the assumption that the deviation of observed IDF from the IDF modeled by Poisson distribution is higher for keywords than for ordinary words. RIDFðtÞ ¼ TFðtÞ � log D DTFðtÞ þ logð1 � e�ATFðtÞÞ; ð2Þ

<mark style="background-color: #000000">Quote</mark>
> C-Value, one of the most popular methods, promotes term candidates that occur frequently, but not as parts of other term candidates. This method was supposed to work with multi-word term candidates only; ATR4S includes modification proposed by Ventura et al. (2013) that supports one-word term candidates as well: C-ValueðtÞ ¼ log2ðjtj þ aÞ � TFðtÞ; � if fs : t � sg ¼ ;; log2ðjtj þ aÞ � TFðtÞ � � P s TFðsÞ P ðÞ jfs : t � sgj � � ; else: 8 < < :

<mark style="background-color: #000000">Quote</mark>
> BasicðtÞ ¼ jtj log f ðtÞ þ aet ;

<mark style="background-color: #000000">Quote</mark>
> ComboBasic modifies Basic further, so that the level of term specificity can be customized by changing parameters of the method: ComboBasicðtÞ ¼ jtj log fðtÞ þ aet þ be0 t; ð5Þ where e0 t is a number of term candidates that are contained in t. Therefore, by increasing b, one can extract more specific terms and vice versa.

<mark style="background-color: #000000">Quote</mark>
> DomainCoherence works in 3 steps. First, it extracts the 200 best term candidates by using Basic method. Then, words from contexts of previously extracted 200 terms are filtered: it keeps only nouns, adjectives, verbs and adverbs that occur in at least one quarter of all documents and are similar to these 200 term candidates, i.e. ranked in the top 50 by averaged Normalized PMI: sðwÞ ¼ 1 jTj X NPMIðt; wÞ ¼ 1 jTj X log Pðt;wÞ PðtÞPðwÞ � � � � logðPðt; wÞÞ ; ð6Þ where w is a context word; T is a set of the 200 best term candidates extracted by Basic; P(t, w) is a probability of occurrence of word w in the context of t; P(t) and P(w) are probabilities of occurrences of term t and word w, correspondingly. These probabilities are estimated on the basis of occurrence frequencies in the input collection; context is considered to be a 5 words window. Finally, as a weight of a term candidate, DomainCohrerence takes the average of the same NPMI measures computed with each of 50 context words extracted at the previous step.

<mark style="background-color: #000000">Quote</mark>
> DomainPertinence (Meijer et al. 2014) is the simplest implementation of this idea: DomainPertinenceðtÞ ¼ TFtargetðtÞ ðÞ TFreferenceðtÞ ; ð7Þ where TFtargetðtÞ is a frequency of term candidate t in target (domain-specific) ðÞ collection; TFreference is a frequency in reference (general) collection.

<mark style="background-color: #000000">Quote</mark>
> Weirdness (Ahmad et al. 1999) normalizes it by sizes (in number of words) of document collections: WeirdnessðtÞ ¼ NTFtargetðtÞ ðÞ NTFreferenceðtÞ ; ð8Þ where NTFtargetðtÞ and NTFreference are frequencies of t normalized by sizes of target ðÞ and reference collections, respectively.13

<mark style="background-color: #f0ff00">Quote</mark>
> document collections: WeirdnessðtÞ ¼ NTFtargetðtÞ ðÞ NTFreferenceðtÞ ; ð8Þ where NTFtargetðtÞ and NTFreference are frequencies of t normalized by sizes of target ðÞ and reference collections, respectively.13 Relevance (Pen˜

<mark style="background-color: #000000">Quote</mark>
> Relevance (Pen˜as et al. 2001) further updates it by taking into account fraction of documents, where term candidate occur: RelevanceðtÞ ¼ 1 � log2 2 þ NTFtargetðtÞ � DFtargetðtÞ � � ðÞ � NTFreferenceðtÞ � � � � �� ð9Þ


%% end annotations %%

%% Import Date: 2024-12-12T18:42:25.199+01:00 %%
