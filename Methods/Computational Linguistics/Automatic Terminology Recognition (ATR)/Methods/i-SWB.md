#atr #automatic-terminology-recognition #topic-modelling #i-SWB

i-SWB is a [[Topic Modelling|topic model]] and [[Automatic Terminology Recognition|ATR]] method based upon [[Topic Modelling|topic modelling]] introduced by [[@liNovelTopicModel2013]]. 

# i-SWB Model

The i-SWB model is shown in the figure below, from [[@liNovelTopicModel2013]] (p. 886)

![[Pasted image 20241002170428.png]]

i-SWB is based upon the construction of three kinds of topics from the documents of a domain specific corpus

1. A background topics - $\phi^B$
2. A number of general topics - $\phi^t, 1 \leq t \leq T$
3. A document specific topic - $\phi^D$

Each of these have a symmetric [[Dirichlet Distribution|Dirichlet prior]] of $\beta_1$, $\beta_0$, and $\beta_2$ respectively, with each topic characterised by a distribution of the $V$ words contained in the corpus of $D$ documents.

$\alpha$ is a fixed parameter of the symmetric [[Dirichlet Distribution|Dirichlet prior]] for the $D$ document multinomials represented by a $D \cdot T$ matrix $\theta$.

$w_{d,n}$ is the observed variable representing the $n^{th}$ word in document $d$, $u_{d,n}$ is the hidden variable representing the kind of topic to which $w_{d,n}$ is assigned, and $z_{d,n}$ is the hidden variable representing the general topic to which $w_{d,n}$ is assigned.

$\pi_{d,n}$ is a 3D vector used to control topic generation and its value determined through an experience function

$$p(DF_{w_{d,n}},\Phi_{w_{d,n}})$$

where $DF_{w_{d,n}}$ is the document frequency of $w_{d,n}$ and $\Phi_{w_{d,n}}$ is the probability vector that $w_{d,n}$ distributes over all general topics.

The model is sampled using a [[Gibbs Sampler|Gibbs sampler]].

# ATR Method

i-SWB is a topic model developed by [[@liNovelTopicModel2013]], used as part of a method to extract terms from a domain corpus defined as

1. Parts of speech are tagged. [[@liNovelTopicModel2013]] report that they used a [[Entropy|maximum-entropy]] [parts-of-speech tagger implemented by the Stanford NLP group](https://www-nlp.stanford.edu/software/tagger.shtml).
2. Filtering based upon linguistic properties. [[@liNovelTopicModel2013]] report that they filter for noun phrases, formulated as $(FW | Verb | Adjective | Noun)^* Noun$ where $FW$ indicates unknown words.
3. Calculation of the [[Term Frequency (TF)|frequency]] of each term candidate within the corpus and exclude those term candidates which appear only once.
4. Calculate the term score for a candidate as a combination of term frequency and i-SWB model results as

$$Termhood(c_i) = log(tf_i) \cdot \sum_{1 \leq j \leq L_i, w_j \in \cup \{V_t\}_{t \in T \cup \{B,D\}}} \phi_{w_j}^{mt_{w_j}}$$

for $mt_{w_j} = \underset{t \in T \cup \{B,D\}}{argmax}(\phi_{w_j}^{t})$, where $c_i$ is a term candidate, $tf_i$ is the [[Term Frequency (TF)|frequency]] of $c_i$ within the corpus, $L_i$ is the set of words $\{w_{i1}, w_{i2}, \dots, w_{iL_i}\}$ contained in $c_i$, $V_t$, $V_B$, and $V_D$ 