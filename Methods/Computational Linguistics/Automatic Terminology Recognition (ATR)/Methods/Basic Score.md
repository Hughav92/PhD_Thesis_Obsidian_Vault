#atr #automatic-terminology-recognition #basic #c-value 

In [[Automatic Terminology Recognition|ATR]], Basic is a method which builds upon the [[Contextual Value (C-Value)|C-Value]] method. Similarly to the [[Contextual Value (C-Value)|C-Value]], Basic promotes term candidates that appear frequently within a corpus. However, in contrast to the [[Contextual Value (C-Value)|C-Value]], Basic promotes candidate terms that are also substrings of other candidate terms.

Basic was developed by [[@bordeaDomainindependentTermExtraction2013]], who define the Basic score as

$$b(\tau) = \left| \tau \right| \log f(\tau) + \alpha e_\tau$$

where $\tau$ is the term candidate, $\left| \tau \right|$ is the length of $\tau$, $f$ is the term candidate's frequency within the corpus (i.e. the [[Term Frequency (TF)|term frequency]]), $e_\tau$ is the number of terms that embed $\tau$, and $\alpha$ is a smoothing parameter. [[@bordeaDomainindependentTermExtraction2013]] suggest a value of $\alpha = 3.5$.

An alternative phrasing of the definition is provided by [[@astrakhantsevATR4SToolkitStateart2018]], in line with the terminology used in the other definitions drawn for other methods in this collection of description, as

$$Basic(t) = \left| t \right| \log f(t) + \alpha e_t$$