#concept #atr #automatic-terminology-recognition #domain-pertinence

Domain Pertinence is an [[Automatic Terminology Recognition|ATR]] method which can be used to "acquire term that a representative for a certain domain corpus, and not for other contrastive corpora" [[@meijerSemanticApproachExtracting2014]] (p.82). [[@meijerSemanticApproachExtracting2014]] define the method as follows:

$$DP_{D_i}(t) = \frac{freq(\frac{t}{D_i})}{max_j(freq(\frac{t}{D_j}))}$$

where $freq(\frac{t}{D_j})$ is the count of a term $t$ in domain corpus $D_i$ and $D_j$ is the contrastive corpus.

[[@astrakhantsevATR4SToolkitStateart2018]] notes that this is simplest implementation of the family of [[Automatic Terminology Recognition|ATR]] methods which are [[Automatic Terminology Recognition Methods#Methods Based on Reference Corpora|based on reference corpora]]. They provide the formalisation

$$DomainPertinence(t) = \frac{TF_{target}(t)}{TF_{reference(t)}}$$

where $TF_{target(t)}$ is the [[Term Frequency (TF)|frequency]] of term candidate $t$ in the domain specific corpus and $TF_{reference}(t)$ is the [[Term Frequency (TF)|frequency]] of term candidate $t$ in the general corpus.