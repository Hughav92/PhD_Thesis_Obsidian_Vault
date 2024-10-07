#concept #atr #automatic-terminology-recognition #inverse-document-frequency #idf


The Inverse Document Frequency (IDF) is an [[Automatic Terminology Recognition|ATR]] method introduced by [[@sparckjonesStatisticalInterpretationTerm1972]], which serves to evaluate how common or rare a term is within a corpus, in other words how much [[Information|information]] the term provides.

It is defined by [[@astrakhantsevATR4SToolkitStateart2018]] as

$$IDF(t) = \log \frac{D}{DTF(t)}$$

where $D$ is the total number of documents in the corpus and $DTF(t)$ is the number of documents containing term $t$.