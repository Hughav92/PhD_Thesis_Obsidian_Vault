#methods 

# Corpora for ATR

- [[TISMIR]]
- [[ISMIR]]

# ATR Method

Currently [[PU-ATR]], as this was shown to work well by [[@astrakhantsevATR4SToolkitStateart2018]].

# Preliminary Work

## Scraping Bibliographic Information from Cristin

### 2024.10.04 - First Test

**Aim:** To obtain a preliminary set of publication venues from which to scrape corpora

**What I did:** As a preliminary test, I scraped journals that RITMO has published in. This was achieved through the following steps.

1. On Cristin I selected *Research results/NVI*
2. I selected *Search in results*
3. I selected *Advanced search*
4. Under *Unit* I selected:
	1. *University of Oslo*
	2. *Det humanistiske fakultet (140000)*
	3. *Institutt for musikvitenskap (143600)*
	4. *RITMO (IMV) Senter for tverrfaglig forskning på rytme, tid og bevegelse (143695)*
5. Under *Category* I selected *Journal article*

This just presents the result from IMV. I need to repeat this for IFI and PSI.

**Results:** There are several options to export the search results. Directly from the search page you can export as an [[XML]] file. This is not very friendly for just extracting publication venues. If you instead choose to display the search results, you can export as either an Endnote bibliography or an [[RIS]] file. The RIS seems like a good option, however when Cristin export an RIS it does not use an [[Encoding]] that is compatible with extended characters. This is visible both when importing the RIS into Zotero as well as when exploring the data in Python. This means that either the data from the RIS file has to be manually corrected, or another method has to be found.


# Inclusion Criteria Brainstorming on Selected Papers from ATR

- Data captured from a *musicking* event, i.e. exclude data that does not attempt to capture the action of musicking such as midi+produced audio+cover art
- At least two different data modalities, with the definition of a data modality based upon the task (following Anna-Maria definition) and conceptualisation of such by author(s)
- Method of analysis used that involved synthesising data modalities with the aim of obtaining information that would not be obtainable through the analysis of a single data modality
- Peer-Reviewed