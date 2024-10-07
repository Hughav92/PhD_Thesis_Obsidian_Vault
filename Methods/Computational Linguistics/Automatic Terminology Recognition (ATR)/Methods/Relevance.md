#concept #atr #automatic-terminology-recognition #relevance #weirdness #domain-pertinence 

Relevance is an [[Automatic Terminology Recognition|ATR]] method which can be used to extract terms from a domain corpus based upon the statistical properties of term candidates in the domain corpus evaluated against their properties in a reference corpus, usually a general corpus. This method serves as an extension of [[Domain Pertinence]] and [[Weirdness]], which takes into account the number of documents in which the term candidate appears in addition to the size of the corpus.

[[@penasCorpusbasedTerminologyExtraction2001]] define Relevance as

$$Relevance(t, sc, gc) = 1 - \frac{1}{\log_2 (2 + \frac{F_{t,sc} \cdot D_{t,sc}}{F_{t,gc}})}$$

where $F_{t,sc}$ is the normalised [[Term Frequency (TF)|frequency]] of term candidate $t$ in the domain corpus $sc$, $F_{t,gc}$ is the normalised [[Term Frequency (TF)|frequency]] of term candidate $t$ in the reference corpus, and $D_{t,sc}$ is the number of documents in the domain corpus in which term candidate $t$ appears.

[[@astrakhantsevATR4SToolkitStateart2018]] offers the following definition, in line with the definitions of [[Domain Pertinence]] and [[Weirdness]] offered in other notes, as

$$Relevance(t) = 1 - (log_2 (2 + \frac{NTF_{target}(t) \cdot DF_{target}(t)}{NTF_{reference}(t)}))$$