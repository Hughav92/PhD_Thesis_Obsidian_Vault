#concept #residual-inverse-document-frequency #ridf #atr #automatic-terminology-recognition 

In [[Automatic Terminology Recognition|ATR]], Residual Inverse Document Frequency is a method proposed by [[@churchInverseDocumentFrequency1999]], as reported by [[@astrakhantsevATR4SToolkitStateart2018]]. Similarly to [[Term Frequency-Inverse Document Frequency (TF-IDF)|TF-IDF]], it is a combination of [[Term Frequency (TF)|term frequency]] and [[Inverse Document Frequency (IDF)|inverse document frequency]]. According to [[@astrakhantsevATR4SToolkitStateart2018]](p. 858), it is builds upon the assumption that the deviation of the corpus [[Inverse Document Frequency (IDF)|IDF]] from the [[Inverse Document Frequency (IDF)|IDF]] modelled by a [[Poisson Distribution|Poisson distribution]] is higher for keywords than for ordinary words.

RIDF can be defined as

$$RIDF = TF(t) \cdot \log \frac{D}{DTF(t)} + \log (1-e^{-ATF(t)})$$

[[@astrakhantsevATR4SToolkitStateart2018]] notes that its use by [[@churchInverseDocumentFrequency1999]] was first in the context of [[Keyword Extraction|keyword extraction]], however it is [[@zhangJATE20Java2016]] who proposed its use for [[Automatic Terminology Recognition|ATR]].