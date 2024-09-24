#automatic-terminology-recognition #atr #tf-idf #tf #idf 

In [[Automatic Terminology Recognition|ATR]], Term Frequency-Inverse Document Frequency (TF-IDF) is a linear combination of [[Term Frequency (TF)|term frequency]] and [[Inverse Document Frequency (IDF)|inverse document frequency]]. As reported by [[@astrakhantsevATR4SToolkitStateart2018]] in reference to [[@evansCLARITTRECExperiments1995]], the method can be formulated as

$$TF \cdot IDF(t) = TF(t) \cdot \log\frac{D}{DTF(t)}$$

where $D$ is the total number of documents in the corpus and $DTF(t)$ is the num