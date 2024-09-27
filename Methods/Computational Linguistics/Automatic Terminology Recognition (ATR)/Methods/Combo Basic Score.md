#combo-basic #atr #automatic-terminology-recognition #basic #c-value 

In [[Automatic Terminology Recognition|ATR]], Combo Basic is a method which builds upon the [[Basic Score]]. Similarly to the [[Basic Score]], the method promotes term candidates including term candidates which are substrings of other term candidates. However, Combo Basic includes an extra parameter which enables the customisation of the level of term specificity.

Developed by [[@astrakhantsevMethodsSoftwareTerminology2015]], [[@astrakhantsevATR4SToolkitStateart2018]] defines  Combo Basic as

$$ComboBasic(t) = \left| t \right| \log f(t) + \alpha e_t + \beta e^{\prime}_t$$

where $t$ is the term candidate, $\left| t \right|$ is the length of $t$, $f(t)$ is the frequency of the term within the corpus, $\alpha$ is a smoothing parameter, $e_t$ is the number of term candidates containing $t$, $e^{\prime}_t$ is the number of term candidates included in $t$, and $\beta$ is a tuning parameter. By increasing the value of $\beta$, it is possible to extract more specific terms.