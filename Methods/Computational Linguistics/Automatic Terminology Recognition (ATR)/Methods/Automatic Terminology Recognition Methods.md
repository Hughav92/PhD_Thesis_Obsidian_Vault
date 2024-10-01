#methods #atr #automatic-terminology-recognition 

[[@astrakhantsevATR4SToolkitStateart2018]] outlines several methods for ATR that they have included in their ATR4S toolbox. They group these into several categories:

# Methods Based on Occurrences Frequencies

These methods are fundamentally based upon the [[Term Frequency (TF)|frequency that certain terms occur within a corpus]], with the assumption that the more frequently a word or n-gram appears within a domain specific corpus, the more relevant it is to that domain.

- [[Term Frequency (TF)]]
- [[Average Term Frequency]]
- [[Inverse Document Frequency (IDF)]]
- [[Term Frequency-Inverse Document Frequency (TF-IDF)]]
- [[Residual Inverse Document Frequency (RIDF)]]
- [[Contextual Value (C-Value)]]
- [[Basic Score]]
- [[Combo Basic Score]]

# Methods Based on Occurrences Contexts

These methods are based upon the assumption that the context within which a term candidate appears can be useful to determine domain specific terms and non-terms.

- [[Normalised Contextual Value (NC-Value)]]
- [[Domain Coherence]]

# Methods Based on Reference Corpora

These methods are based upon the comparing the statistics relating to the occurrence of term candidates in a domain corpus against the statistics relating to the same terms in a reference corpus or corpora. The reference corpus is usually taken from a general domain.

- [[Domain Pertinence]]
- [[Weirdness]]
- [[Relevance]]
