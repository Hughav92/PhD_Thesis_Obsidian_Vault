![[Pasted image 20241001190405.png]]

---

I'm Hugh and this is the open-source site for my PhD thesis. My project is preliminarily titled "Data Fusion for the Analysis of Multimodal Musicking Datasets" and is centred on developing a [[Methods vs Methodology|methodological]] framework for the analysis of [[Music Datasets vs Musicking Datasets|musicking datasets]] consisting of multiple data modalities, with focus on the representation of spatial and temporal information in fused data. I am carrying out this project at the [RITMO Centre for Interdisciplinary Studies in Rhythm, Time and Motion](https://www.uio.no/ritmo/english/) at the [University of Oslo](https://www.uio.no/english/), Norway under the supervision of [Alexander Refsum Jensenius](https://www.uio.no/ritmo/english/people/management/alexanje/). The project began on 01.09.2024 and is intended to run until 01.09.2027.

This site encompasses everything that I am writing as part of the project, from the formal writing of the PhD thesis and article manuscripts to informal memos, notes, reflections, as well as literature overviews and databases, with the goal that this function as a knowledge base that I accumulate over the course of the project. In fact, it is a published version of the [Obsidian vault](https://obsidian.md/) that I am using as my main writing tool and is primarily a collection of Markdown pages, with the Markdown source available on [my Github](https://github.com/Hughav92/PhD_Thesis_Obsidian_Vault). As a result this site represents a continuously evolving work-in-progress, and will be updated daily over the project period.

The publishing of the process of writing a PhD thesis is intended to be part of the [Open Science](https://www.openscience.no/en/what-open-science) encouraged by the University of Oslo. Although we make our methods and results open through the open publishing of all research results through the University of Oslo's [DUO](https://www.duo.uio.no/) repository and the release of data, analysis source code, and methodologies through various channels, the process of conducting research can still remain a bit of a black box. With this site, I hope to open the process of writing a PhD, at least to a small extent.

I aim to share as much as I can. However, some of the contents of my personal version of this vault contain copyrighted or sensitive material, which may account for several dead links in this site. Moreover, any mistakes and errors are my own and I welcome all corrections and general feedback at hughav "at" uio.no.

The contents of this site that are my own are released under a [Creative Commons BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/) license. This means that you are free to share and adapt the content here in any way you like, as long as you properly attribute it, do not use it for any commercial purposes, and share any work you do to build upon it under the same license.

# What I'm Working On

These are the sub-projects that I am currently working on, with the aim that these eventually end up as a scientific paper:

- A [[Multimodal Methods Systematic Review|systematic review of analytical methods]] used in various disciplines of music research for the analysis of multimodal datasets
- An exploration of how different approaches towards the [[Time and Space in Synchronisation and Alignment|temporal synchronisation of time-series signals create a spatial perspective for further analysis methods]]
- Analysing how well [[Multimodal Learning HAR|transfer learning can be applied to leverage large, pretrained models for Human Activity Recognition]] and how multimodal learning with accelerometer and depth image data, both with and without the support of RGB camera data, compare in order to preserve user privacy - this is for the course [IN9490 – Advanced Topics in Artificial Intelligence for Intelligent Systems](https://www.uio.no/studier/emner/matnat/ifi/IN9490/)
- A study of the [[MoCap Latency Perception|perception of latency]] with respect to the visual representation of optical marker-based motion capture data and how this relates to the "human-ness" of the representation's form and the form's motion
- Developing a method for the processing and analysis of audience motion in live concert research from [[IR Low Light Level Motion Analysis|infra-red videos recorded a low light levels]]
- A [[Aarhus Lighting Interactive System|system]] to map [[Electrocardiogram|ElectroCardioGram (ECG)]] signals to a lighting system in real-time to visualise aspects of the cardiac dynamics of performers and audiences in symphonic orchestra performance.
- An [[SiFiBand in Interactive Music|evaluation]] of the [[SiFiBand]] in interactive music contexts.
- A [[Comparative Analysis of Thermography and IR Signals|comparative analysis]] of how [[Thermography|thermographic]] and [[Infra-Red Imaging|Infra-Red (IR)]] imaging can be used for motion analysis.

# Where to Start

As this site represents a work in progress, consisting of many different types of writing (and eventually a non-linear presentation of my final thesis), there is no clear starting point for reading this site. In addition, there are and will be quite a number of pages without any writing at any given point, as my method for working in this way is to create an empty page for any concept, idea, or personal reflection that I will return to. Pages are also sorted into categories (the folders in the sidebar on the right) when I feel that the way that I am writing about the topic aligns with a category, so this is also a continually updating process. Therefore I would suggest the following ways of exploring this site:

- Starting with the [[Homepage#What I'm Working On|What I'm Working On]] section to follow the progress on current sub-projects and papers.
- Reading the [[Daily Notes]] to see what I am working on on any given day.
- Looking at the [[Homepage#Latest Updated Pages|Latest Updated Pages]] to see which pages I have been writing recently.
- Searching for the following tags:
	- #concept - These pages and sections consist of the presentation of a concept from the literature without any reflection, synthesis or opinion. Think of these as "Wikipedia" style pages.
	- #procedural - These pages are related to the process of carrying out the project. These include the daily notes, reflections on conferences and workshops, and reflections on the structure of the thesis, for example.
	- #reflection - These pages are where I engage with the literature. I reflect on ideas and attempt to synthesise and contrast them, and give my thoughts on them.
	- #my-work - These pages consist of the presentation of my work. This includes work in progress writing, brainstorming sessions, paper drafts, code snippets, and preliminary results, among others.
	- #finished-work - These pages are the final submitted forms of my work. This includes, for example, published papers or thesis chapters.
	- #literature-note - These pages contain metadata on and summaries of literature that I have read, as well as tabular summaries of relevant literature.
- Picking a page that looks interesting from the sidebar to the left.
- Exploring the graph view in the sidebar to the right, which shows the links between individual pages. For each page there is a small graph view showing all the pages which are linked to the current page. However, if you click on the icon "Global Graph", this will show the links between all pages on this site. I'm currently working on colour-coding these nodes according to category.

# Daily Note

Daily notes are where I document my goals and tasks for the day, log what I worked on and any literature that I have read, and reflect upon the ongoing status of the project.

%% DATAVIEW_PUBLISHER: start
```dataview
TABLE date(file.name) as "Date"
FROM "Daily Notes"
WHERE date(file.name) = date(today) AND file.name != "Daily Notes"
```
%%

| File                                      | Date           |
| ----------------------------------------- | -------------- |
| [[Daily Notes/2025-04-01.md\|2025-04-01]] | April 01, 2025 |

%% DATAVIEW_PUBLISHER: end %%

Previous daily notes can be found [[Daily Notes|here]].

# Latest Updated Pages

%% DATAVIEW_PUBLISHER: start
```dataview
TABLE file.mtime AS "Updated"
FROM -"Meetings" AND -"Literature" AND -"Obsidian Templates"
SORT file.mtime DESC
LIMIT 10
```
%%

| File                                                                                       | Updated                  |
| ------------------------------------------------------------------------------------------ | ------------------------ |
| [[Non-Manuscript Work/DCASE Checking/DCASE Checking - Papers.md\|DCASE Checking - Papers]] | 6:07 PM - April 01, 2025 |
| [[Literature Notes/@wangNercslipSystemSound2022.md\|@wangNercslipSystemSound2022]]         | 6:04 PM - April 01, 2025 |
| [[Publish Pages/Homepage.md\|Homepage]]                                                    | 6:03 PM - April 01, 2025 |
| [[Daily Notes/2025-03-31.md\|2025-03-31]]                                                  | 6:03 PM - April 01, 2025 |
| [[Daily Notes/2025-04-01.md\|2025-04-01]]                                                  | 6:03 PM - April 01, 2025 |
| [[Daily Notes/2025-02-10.md\|2025-02-10]]                                                  | 6:03 PM - April 01, 2025 |
| [[Daily Notes/2025-01-14.md\|2025-01-14]]                                                  | 6:03 PM - April 01, 2025 |
| [[Daily Notes/2025-01-17.md\|2025-01-17]]                                                  | 6:03 PM - April 01, 2025 |
| [[Daily Notes/2024-12-16.md\|2024-12-16]]                                                  | 6:03 PM - April 01, 2025 |
| [[Daily Notes/2024-12-12.md\|2024-12-12]]                                                  | 6:03 PM - April 01, 2025 |

%% DATAVIEW_PUBLISHER: end %%

# Links

I can be found at the following places:

- [University of Oslo employee page](https://www.uio.no/ritmo/english/people/phd-fellows/hughav/index.html)
- [Google Scholar](https://scholar.google.com/citations?user=1H848AwAAAAJ&hl=en)
- [Github](https://github.com/Hughav92)

# Works Cited

The works cited in this site can be found on [[Works Cited|this page]].

# Attributions

The literature notes and overviews that I use as part of this vault are a lightly modified version of the template provided by [Alexandra Phelan](https://medium.com/@alexandraphelan/an-updated-academic-workflow-zotero-obsidian-cffef080addd).

Images in header image from:

- [Video Data Shape](https://www.tensorflow.org/images/tutorials/video/video_data_shape.png)
- [MoCap](https://www.researchgate.net/profile/Michal-Balazia/publication/308457587/figure/fig3/AS:641838260162560@1530037574587/Motion-capture-data-Skeleton-is-represented-by-a-stick-figure-of-17-joints-left-Seven.png)
- [3D Tensor](https://tensorflow.rstudio.com/guides/tensorflow/images/tensor/3-axis_block.png)
- [4D Tensor](https://www.tensorflow.org/static/guide/images/tensor/4-axis_block.png)
- [3D Tensor with Values](https://www.tensorflow.org/static/guide/images/tensor/3-axis_front.png)

All images taken from the literature are attributed in the corresponding note.