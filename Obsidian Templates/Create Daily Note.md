
# Goals

- [ ] 

# Tasks

- [ ] 

# What I Worked On

- 

# Reflections

- 

# Literature Read

- 

# Notes Created


%% DATAVIEW_PUBLISHER: start
```dataview
TABLE file.cday AS "Created"
WHERE file.cday = this.file.day
```
%%

| File | Created |
| ---- | ------- |

%% DATAVIEW_PUBLISHER: end %%

# Yesterday's Daily Note

%% DATAVIEW_PUBLISHER: start
```dataview
TABLE file.cday AS "Date"
WHERE date(file.name) = date(this.file.name)+dur(-1 day)
SORT file.cday DESC
```
%%

| File | Date |
| ---- | ---- |

%% DATAVIEW_PUBLISHER: end %%
# Tomorrow's Daily Note

%% DATAVIEW_PUBLISHER: start
```dataview
TABLE file.cday AS "Date"
WHERE date(file.name) = date(this.file.name)+dur(1 day)
SORT file.cday DESC
```
%%

%% DATAVIEW_PUBLISHER: end %%


