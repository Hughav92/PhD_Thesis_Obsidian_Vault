
---
category:: literaturenote
tags:: 
citekey:: astrakhantsevATR4SToolkitStateart2018
status:: unread
dateread:
---

> [!Cite]
> Astrakhantsev, N. (2018). ‘ATR4S: toolkit with state-of-the-art automatic terms recognition methods in Scala’, _Language Resources and Evaluation_, 52/3: 853–72. DOI: [10.1007/s10579-017-9409-4](https://doi.org/10.1007/s10579-017-9409-4)

>[!Synth]
>**Contribution**:: 
>
>**Related**:: 
>

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


%% end annotations %%

%% Import Date: 2024-09-27T16:45:58.983+02:00 %%
