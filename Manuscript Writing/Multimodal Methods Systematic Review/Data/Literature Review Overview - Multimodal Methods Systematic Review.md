#my-work #multimodal #systematic-review #literature-review #literature-overview  


%% DATAVIEW_PUBLISHER: start
```dataview
TABLE
FirstAuthor as "First Author",
title as Title,
year as Year,   
status as Status,  
contribution as Contribution  
FROM "Literature Notes"
WHERE contains(tags, "SystematicReview")
SORT status DESC, year DESC  
```
%%

| File | First Author | Title | Year | Status | Contribution |
| ---- | ------------ | ----- | ---- | ------ | ------------ |

%% DATAVIEW_PUBLISHER: end %%