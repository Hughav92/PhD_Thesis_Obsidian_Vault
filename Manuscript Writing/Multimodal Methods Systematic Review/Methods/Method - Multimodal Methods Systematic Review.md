#my-work #reflection #methods 

# Corpora for ATR

- [[TISMIR]]
- [[ISMIR]]
- [[SysMus]]

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

**Results:**

*First Thoughts:* There are several options to export the search results. Directly from the search page you can export as an [[XML]] file. This is not very friendly for just extracting publication venues. If you instead choose to display the search results, you can export as either an Endnote bibliography or an [[RIS]] file. The RIS seems like a good option, however when Cristin export an RIS it does not use an [[Encoding]] that is compatible with extended characters. This is visible both when importing the RIS into Zotero as well as when exploring the data in Python. This means that either the data from the RIS file has to be manually corrected, or another method has to be found.

*Second Thoughts:* I couldn't access the Endnote file. I started exploring the [[XML]]. I was able to extract all of the publication venues, however this is going to be a bit of work to present it nicely keeping all of the other metadata about the publication aligned. But at the moment, at least, I have the following publication venues which IMV RITMO have published with:

>[!note]- List of IMV RITMO Journal Publication Venues (RAW)
>- [[ASSITEJ ESPANA Boletín Iberoamericano de Teatro para la Infancia y la Juventud (BITIJ)]]
>- [[Academia Letters]]
>- [[Acervo]]
>- [[Acta neuropathologica communications]]
>- [[Aftenposten (morgenutg. : trykt utg.)]]
>- [[Analytical Approaches to World Music]]
>- [[Apollon : Forskningsmagasin for Universitetet i Oslo]]
>- [[Applied Sciences]]
>- [[Atos de pesquisa em educação]]
>- [[Attention, Perception & Psychophysics]]
>- [[Ballade]]
>- [[Behavioral and Brain Sciences]]
>- [[Bioengineering]]
>- [[Brain and Cognition]]
>- [[Cahiers d'ethnomusicologie]]
>- [[Cerebral Cortex]]
>- [[Charaktery]]
>- [[Cognition]]
>- [[Cognitive Systems Research]]
>- [[Computer Music Journal]]
>- [[Convergence. The International Journal of Research into New Media Technologies]]
>- [[Corpo Grafias]]
>- [[Curator: The Museum Journal]]
>- [[Current Biology]]
>- [[Dagbladet]]
>- [[Deleuze and Guattari studies]]
>- [[Discover Education]]
>- [[EARMA Link Magazine]]
>- [[Empirical Issues in Syntax and Semantics]]
>- [[Empirical Musicology Review]]
>- [[European Journal of Higher Education IT – EJHEIT]]
>- [[European Review of Private Law]]
>- [[Filologen]]
>- [[Frontiers in Bioengineering and Biotechnology]]
>- [[Frontiers in Computer Science]]
>- [[Frontiers in Human Neuroscience]]
>- [[Frontiers in Neuroscience]]
>- [[Frontiers in Psychology]]
>- [[Frontiers in Sports and Active Living]]
>- [[Human Movement Science]]
>- [[Human Technology]]
>- [[IEEE/ACM Transactions on Audio, Speech, and Language Processing (TASLP)]]
>- [[IIC - International Review of Intellectual Property and Competition Law]]
>- [[IPKat]]
>- [[International Journal of Multimedia Information Retrieval]]
>- [[Journal of Aesthetics and Phenomenology]]
>- [[Journal of Experimental Psychology: Human Perception and Performance]]
>- [[Journal of Experimental Social Psychology]]
>- [[Journal of Jazz Studies (JJS)]]
>- [[Journal of Motor Behavior]]
>- [[Journal of Neuroscience Methods]]
>- [[Journal of New Music Research]]
>- [[Journal of Semantics]]
>- [[Journal of Sport & Exercise Psychology (JSEP)]]
>- [[Journal of The Audio Engineering Society]]
>- [[Journal of Theater Critisim and Dramaturgy]]
>- [[Journal of music theory]]
>- [[Journal of the Acoustical Society of America]]
>- [[Journal of the American Musicological Society]]
>- [[Khrono.no]]
>- [[MAGOTZI Boletín Científico de Artes del IA]]
>- [[Media, Culture and Society]]
>- [[Mind & Language]]
>- [[Morgenbladet]]
>- [[Music & Science]]
>- [[Music Perception]]
>- [[Music Theory Online]]
>- [[Music Theory Spectrum]]
>- [[Musicae Scientiae]]
>- [[Musikk & Historie]]
>- [[Musikkmagasinet Ballade]]
>- [[Mål og makt]]
>- [[Nature Communications]]
>- [[Nature Human Behaviour]]
>- [[New Media & Society]]
>- [[Nordic journal of music therapy]]
>- [[Norsk Medietidsskrift]]
>- [[Nota Bene]]
>- [[Nytt Norsk Tidsskrift]]
>- [[Organised Sound]]
>- [[PLOS ONE]]
>- [[Perspectives of New Music]]
>- [[Phenomenology and the Cognitive Sciences]]
>- [[Philosophical Transactions of the Royal Society A: Mathematical, Physical and Engineering Sciences]]
>- [[Philosophical Transactions of the Royal Society of London. Biological Sciences]]
>- [[Philosophy]]
>- [[Physics of Fluids]]
>- [[Physics of Life Reviews]]
>- [[Popular Music]]
>- [[Popular Science Turkey]]
>- [[Popular music and society]]
>- [[Proceedings of the International Conference on Live Interfaces (Proceedings of ICLI)]]
>- [[Proceedings of the International Conference on New Interfaces for Musical Expression]]
>- [[Psihologijske Teme]]
>- [[Psychological Research]]
>- [[Psychology of Aesthetics, Creativity, and the Arts]]
>- [[Psychology of Music]]
>- [[Reflections on Process in Sound]]
>- [[Resonancias]]
>- [[Reviews of Modern Physics]]
>- [[Revista de Humanidades Digitales]]
>- [[Routledge Open Research]]
>- [[Scandinavian Journal of Psychology]]
>- [[Scenekunst.no]]
>- [[Scientific Reports]]
>- [[Selected Papers of Internet Research, SPIR]]
>- [[Social Media + Society]]
>- [[Sports Coaching Review]]
>- [[Studia Musicologica Norvegica]]
>- [[Synthese]]
>- [[The Journal of Somaesthetics (JS)]]
>- [[Tidsskrift for Norsk Psykologforening]]
>- [[Transactions of the International Society for Music Information Retrieval]]
>- [[Uniforum]]
>- [[VG : Verdens gang]]
>- [[Young Acousticians Network (YAN) Newsletter]]
>- [[Z filmtidsskrift]]
>- [[arXiv]]
>- [[eLIFE]]
>- [[eLearning and Software for Education]]

The code I used to get this from the [[XML]] is as follows:

```python
import csv
import requests
import xml.etree.ElementTree as ET

# set filepath
path = "path/to/file/"
file = "cristin_search_results.xml"
p = Path(path, file)

# parse XML to element tree
tree = ET.parse(p)
root = tree.getroot()

# get each individual research result
forskningsresultater = root.findall('.//forskningsresultat')

# declare empty list for appending publication venues
navns = []

for forskningsresultat in forskningsresultater:

    # get the publication venue from the element tree, print, and append to list
    navn_elements = forskningsresultat.findall(".//kategoridata/tidsskriftsartikkel/tidsskrift/navn")

    for navn_element in navn_elements:
    
        if navn_element is not None:

            print(f"Found <navn> element: {navn_element.text}")
            navn = navn_element.text
            navns.append(navn)

# get the set of unique publication venues
navns = sorted(set(navns))

# write out to text file
with open(path + "20241004_Cristinscrape_Journals_IMVRITMO.txt", "w") as f:

    for navn in navns:

        f.write(f"{navn}\n")
```

The [[XML]] is structured so that each research result is a child element directly under the root tagged as a `<forskningsresultat>`. The publication venue is buried several elements down as `kategoridata/tidsskriftsartikkel/tidsskrift/navn`.

**Discussion:**

There are several things of note here. First, there are several venues here that aren't actually academic journals such as [[VG : Verdens gang]] and [[Dagbladet]], both of which are Norwegian newspapers. Second, there are several venues which are specifically focused on musicological research, such as [[Music & Science]] and [[Music Perception]], but actually (at first glance) a majority are either focused on more general research or concerned with other fields. I will need to implement a filtering system for these in order to only extract articles related to analytical musicological research for scraping.

**Next Steps:**

The next steps are:

1. To add to the code to nicely package all of the other metadata about each publication (authors, year, etc.) together with the publication venues in a [[CSV]] file.
2. Run this code on all other required research result [[XML|XMLs]] (IFI and PSI RITMO, as well as for conferences, monographs, and book chapters)




# Inclusion Criteria Brainstorming on Selected Papers from ATR

- Data captured from a *musicking* event, i.e. exclude data that does not attempt to capture the action of musicking such as midi+produced audio+cover art
- At least two different data modalities, with the definition of a data modality based upon the task (following Anna-Maria definition) and conceptualisation of such by author(s)
- Method of analysis used that involved synthesising data modalities with the aim of obtaining information that would not be obtainable through the analysis of a single data modality
- Peer-Reviewed