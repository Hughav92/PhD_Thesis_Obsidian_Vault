#concept #atr #automatic-terminology-recognition #domain-coherence

Domain Coherence is an [[Automatic Terminology Recognition|ATR]] method which is based upon the occurrences contexts of term candidates to score terms. Defined by [[@bordeaDomainindependentTermExtraction2013]], the method is based upon the the following assumptions in order to construct a domain model from a corpus of domain texts:

> 1. **Distribution**
> 	Generic words should appear in at least one quarter of the documents in the corpus
> 2. **Length**
> 	Only single-word candidates are considered, as longer terms are more specific
> 3. **Content**
> 	Only content-bearing words are of interest (i.e. nouns, verbs, adjectives)
> 4. **Semantic Relatedness**
> 	A term is more general if it is semantically related to many specific terms (p. 4)

The first three assumptions are used as a basis for the selection of candidate terms, formalised as  using a [[Contextual Value (C-Value)|standard]] [[Basic Score|extraction]] [[Combo Basic Score|technique]] to extract multi-word term candidates from the corpus. The fourth assumption is operationalised as the [[Pointwise Mutual Information|Pointwise Mutual Information (PMI)]] in order to score the term candidates, formalised as

$$s(\theta) = \sum_{\sigma \in \Omega} PMI(\theta, \sigma) = \sum_{\sigma \in \Omega} \log (\frac{P(\theta, \sigma)}{P(\theta \cdot \sigma)})$$

where $\theta$ is the domain model candidate word, $\Omega$ is the set of top ranked multi-word terms and $P(\theta, \sigma)$ is the probability that word $\theta$ appears in the context of the term $\sigma$.

[[@astrakhantsevATR4SToolkitStateart2018]] provides a more concrete example and extension of the Domain Coherence method as:

1. Extract the 200 best term candidates from a corpus using the [[Basic Score]]
2. Filter words from the context of the 200 best term candidates through extraction of only nouns, adjective, verbs, and adverbs that occur in at least one quarter of documents in the corpus
3. Keep the candidates ranked in, for example, the top 50 by the average normalised [[Pointwise Mutual Information|PMI]], defined as:

$$s(w) = \frac{1}{\left| T \right|} \sum_{t \in T}NPMI(t, w) = \frac{1}{\left| T \right|} \sum_{t \in T} \frac{log(\frac {P(t, w)}{P(t)P(w)})}{log(P(t, w))}$$

where $w$ is a context word, $T$ is the set of best term candidates, $P(t, w)$ is the probability of the occurrence of word $w$ in the context of $t$, and $P(t)$ and $P(w)$ are the probabilities of the occurrences of term $t$ and word $w$. $P(t)$ and $P(w)$ are estimated by the [[Term Frequency (TF)|frequency]] of the $t$ and $w$ in the corpus, with the context considered as a 5 word window.