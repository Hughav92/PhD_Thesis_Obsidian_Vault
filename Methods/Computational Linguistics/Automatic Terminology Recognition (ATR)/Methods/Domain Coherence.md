Domain Coherence is an [[Automatic Terminology Recognition|ATR]] method which is based upon the occurrences contexts of term candidates to score terms. Defined by [[@bordeaDomainindependentTermExtraction2013]], the method is based upon the the following assumptions in order to construct a domain model from a corpus of domain texts:

> 1. **Distribution**
> 	Generic words should appear in at least one quarter of the documents in the corpus
> 2. **Length**
> 	Only single-word candidates are considered, as longer terms are more specific
> 3. **Content**
> 	Only content-bearing words are of interest (i.e. nouns, verbs, adjectives)
> 4. **Semantic Relatedness**
> 	A term is more general if it is semantically related to many specific terms (p. 4)

The first three steps are used to select candidate terms. [[@astrakhantsevATR4SToolkitStateart2018]] provides the concrete parameters of extracting 

1. Multi-word terms are extracted using a [[Contextual Value (C-Value)|a standard term extraction technique]].
2. 