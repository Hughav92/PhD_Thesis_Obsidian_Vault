#atr #automatic-terminology-recognition #weirdness #domain-pertinence 

Weirdness is an [[Automatic Terminology Recognition|ATR]] method which can be used to extract terms from a domain corpus based upon the statistical properties of term candidates in the domain corpus evaluated against their properties in a reference corpus, usually a general corpus. This method is identical to [[Domain Pertinence]] normalised for the number of words in the domain and reference corpora. [[@ahmadUniversitySurreyParticipation1999]] define Weirdness as

$$Weirdness = \frac{\frac{w_s}{t_s}}{\frac{w_g}{t_g}}$$

where $w_s$ is the [[Term Frequency (TF)|frequency]] of the term candidate in the domain corpus, $w_g$ is the [[Term Frequency (TF)|frequency]] of the term candidate in the general corpus, $t_s$ is the total count of words in the domain corpus, and $t_g$ is the total count of words in the general corpus.

[[@astrakhantsevATR4SToolkitStateart2018]] defines Weirdness in more generalised terms as

$$Weirdness(t) = \frac{NTF_{target}(t)}{NTF_{reference}(t)}$$

where $t$ is a term candidate, $NTF_{target}(t)$ is the [[Term Frequency (TF)|frequency]] of $t$ in a target corpus normalised by the number of words in the target corpus, and $NTF_{reference}(t)$ is the [[Term Frequency (TF)|frequency]] of $t$ in the reference corpus normalised by the number of words in the reference corpus.

They note that in the case of simply ranking the term candidates by their scores, [[Domain Pertinence]] and Weirdness provide identical results, as the only difference between these methods is a constant multiplier.