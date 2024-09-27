#atr #automatic-terminology-recognition #c-value #contextual-value

The contextual value (C-Value) is an [[Automatic Terminology Recognition|ATR]] method which promotes term candidates that appear frequently within a corpus but which do not appear as part of other term candidates within the corpus [[@astrakhantsevATR4SToolkitStateart2018]]. The method was developed by [[@frantziAutomaticRecognitionMultiword2000]], who describe it as a "measure of termhood" (p. 118), in other words as a key piece of terminology from the domain of the corpus.  [[@frantziAutomaticRecognitionMultiword2000]] define the C-Value as

$$
\text{C-value}(a) = 
\begin{cases} 
\log_2 \left|2\right| \cdot f(a) & \textit{a is not nested,} \\
\log_2 \left|2\right| \left(f(a) - \frac{1}{P(T_a)} \sum_{b\epsilon T_a} f(b)\right) & \textit{otherwise}
\end{cases}
$$

where $a$ is the candidate string, $f(\cdot)