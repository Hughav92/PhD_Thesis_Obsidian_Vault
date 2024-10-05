![[Pasted image 20241001190405.png]]

---

I'm Hugh and this is the open-source site for my PhD thesis. My project is preliminarily titled "Data Fusion for the Analysis of Multimodal Musicking Datasets" and is centred on developing a [[Methods vs Methodology|methodological]] framework for the analysis of [[Music Datasets vs Musicking Datasets|musicking datasets]] consisting of multiple data modalities, with focus on the representation of spatial and temporal information in fused data. I am carrying out this project at the [RITMO Centre for Interdisciplinary Studies in Rhythm, Time and Motion](https://www.uio.no/ritmo/english/) at the [University of Oslo](https://www.uio.no/english/), Norway under the supervision of [Alexander Refsum Jensenius](https://www.uio.no/ritmo/english/people/management/alexanje/). The project began on 01.09.2024 and is intended to run until 01.09.2027.

This site encompasses everything that I am writing as part of the project, from the formal writing of the PhD thesis and article manuscripts to informal memos, notes, reflections, as well as literature overviews and databases, with the goal that this function as a knowledge base that I accumulate over the course of the project. In fact, it is a published version of the [Obsidian vault](https://obsidian.md/) that I am using as my main writing tool and is primarily a collection of Markdown pages, with the Markdown source available on [my Github](https://github.com/Hughav92/PhD_Thesis_Obsidian_Vault). As a result this site represents a continuously evolving work-in-progress, and will be updated daily over the project period.

The publishing of the process of writing a PhD thesis is intended to be part of the [Open Science](https://www.openscience.no/en/what-open-science) encouraged by the University of Oslo. Although we make our results open through the open publishing of all research results through the University of Oslo's [DUO](https://www.duo.uio.no/) repository and the release of data, analysis source code, and methodologies, the process of conducting research can still remain a bit of a black box. With this site, I hope to open the process of writing a PhD, at least to a small extent.

I aim to share as much as I can. However, some of the contents of my personal version of this vault contain copyrighted or sensitive material, which may account for several dead links in this site. Moreover, any mistakes and errors are my own and I welcome all corrections and general feedback at hughav "at" uio.no.

The contents of this site that are my own are released under a [Creative Commons BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/) license. This means that you are free to share and adapt the content here, as long as you properly attribute it, do not use it for any commercial purposes, and share any work you do to build upon it under the same license.

# What I'm Working On

These are the sub-projects that I am currently working on, with the aim that these eventually end up as a scientific paper:

- A [[Multimodal Methods Systematic Review|systematic review of analytical methods]] used in various disciplines of music research for the analysis of multimodal datasets
- An exploration of how different approaches towards the [[Time and Space in Synchronisation and Alignment|temporal synchronisation of time-series signals create a spatial perspective for further analysis methods]]
- Analysing how well [[Multimodal Learning HAR|transfer learning can be applied to leverage large, pretrained models for Human Activity Recognition]] and how multimodal learning with accelerometer and depth image data, both with and without the support of RGB camera data, compare in order to preserve user privacy - this is for the course [IN9490 – Advanced Topics in Artificial Intelligence for Intelligent Systems](https://www.uio.no/studier/emner/matnat/ifi/IN9490/)
- A study of the [[MoCap Latency Perception|perception of latency]] with respect to the visual representation of optical marker-based motion capture data and how this relates to the "human-ness" of the representation's form and the form's motion

In addition, I am working on:

- Developing a system to [[IR Light Level Compensation|compensate for varying levels of stage lighting]] in infra-red video recordings of audiences in live concert research, in order to streamline motion analysis

# Daily Note

Daily notes are where I document my goals and tasks for the day, log what I worked on and any literature that I have read, and reflect upon the ongoing status of the project.

%% DATAVIEW_PUBLISHER: start
```dataview
TABLE file.cday as "Date"
FROM "Daily Notes"
WHERE file.cday = date(today) AND file.name != "Daily Notes"
```
%%

| File | Date |
| ---- | ---- |

%% DATAVIEW_PUBLISHER: end %%

Previous daily notes can be found [[Daily Notes|here]].

# Latest Updated Pages

%% DATAVIEW_PUBLISHER: start
```dataview
TABLE file.mtime AS "Updated"
SORT file.mtime DESC
LIMIT 10
```
%%

| File                                                                                                                                                                | Updated                     |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------- |
| [[Publish Pages/Homepage.md\|Homepage]]                                                                                                                             | 6:11 PM - October 04, 2024  |
| [[Daily Notes/2024-10-04.md\|2024-10-04]]                                                                                                                           | 6:11 PM - October 04, 2024  |
| [[Manuscript Writing/Multimodal Methods Systematic Review/Methods/Method - Multimodal Methods Systematic Review.md\|Method - Multimodal Methods Systematic Review]] | 5:50 PM - October 04, 2024  |
| [[CSV.md\|CSV]]                                                                                                                                                     | 5:37 PM - October 04, 2024  |
| [[Encoding.md\|Encoding]]                                                                                                                                           | 4:24 PM - October 04, 2024  |
| [[RIS.md\|RIS]]                                                                                                                                                     | 4:23 PM - October 04, 2024  |
| [[XML.md\|XML]]                                                                                                                                                     | 4:22 PM - October 04, 2024  |
| [[Daily Notes/2024-10-02.md\|2024-10-02]]                                                                                                                           | 3:36 PM - October 04, 2024  |
| [[Literature Notes/@christodoulouMultimodalMusicDatasets2024.md\|@christodoulouMultimodalMusicDatasets2024]]                                                        | 12:18 PM - October 04, 2024 |
| [[Daily Notes/Daily Notes.md\|Daily Notes]]                                                                                                                         | 12:13 PM - October 04, 2024 |

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