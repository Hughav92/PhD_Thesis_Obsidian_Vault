#my-work 




%% DATAVIEW_PUBLISHER: start
```dataview
TABLE
title as Title,
FirstAuthor as Author,
year as Year,
contribution as Summary,
choice(contains(split(status, ", "), "unread"), "unread", choice(contains(split(status, ", "), "read"), "read", "")) as Status 
from "Literature Notes"
where contains(tags, "QOMOP")
SORT year DESC, year DESC
```
%%
%% DATAVIEW_PUBLISHER: end %%