Domain Coherence is an [[Automatic Terminology Recognition|ATR]] method which is based upon the occurrences contexts of term candidates to score terms. Defined by [[@bordeaDomainindependentTermExtraction2013]], the method is based upon the the following assumptions in order to construct a domain model from a corpus of domain texts:

> 1. **Distribution**
> 	Generic words should appear in at least one quarter of the documents in the corpus
> 2. **Length**
> 	Only single-word candidates are considered, as longer terms are more specific
> 3. **Content**
> 	Only content-bearing words are of interest (i.e. non)