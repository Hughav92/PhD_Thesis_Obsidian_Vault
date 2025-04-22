#my-work 




%% DATAVIEW_PUBLISHER: start
```dataview
TABLE title as Title, FirstAuthor as Author, year as Year, contribution as Summary
from "Literature Notes"
where contains(tags, "QOMOP")
```
%%
%% DATAVIEW_PUBLISHER: end %%