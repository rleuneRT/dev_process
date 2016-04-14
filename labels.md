## labels

### type

- to define type of issue
- 1 needs to be used (and only 1) !!!

| name | description | used in | 
| --- | --- | --- | --- |
| story |  | home, milestone, project, infra | 
| task |  |  home, milestone, project, infra |
| ticket | type | project |
| bug | issue reported by anyone | code,ays,doc,www,infra,cockpit |
| feature | improvement asked for by anyone | code, project,ays,doc,www,infra,cockpit |
| question | anyone wants to ask something | home, code, project,ays,doc,www,infra,cockpit | 
| monitor | monitoring system found an issue | project,cockpit,www,infra |
| lead | lead for sales, can convert in business | project |
| test | a test task | milestone,infra,cockpit |

### priority

- define priority in which issue needs to resolved
- 1 needs to be used (and only 1) !!!

| name | description | used in | color |
| --- | --- | --- | --- |
| critical |  | home, project,ays,doc | todo |
| urgent |  | home, code, project,ays,doc | todo |
| normal |  | home, code, project,ays,doc | todo |
| minor |  | home, code, project,ays,doc | todo |

### process 

- define 2 optional process related labels

| name | description | used in | color |
| --- | --- | --- | --- |
| duplicate |  | home, project,ays,doc | todo |
| wontfix |  | home, project,ays,doc | todo |

### state

- define state of issue in the kanban flow
- 1 needs to be used (and only 1) !!!
- REMARK
  - these states need to be useful over all projects e.g. over customer projects, code projects, stories, ...
  - good filters should be used in waffle to represent a kanban well 

| name | description | used in | color |
| --- | --- | --- | --- |
| new | new or issue in backlog | home, project,ays,doc | todo |
| accepted | accepted in milestone & now tracked in kanban as to be done | home, project,ays,doc | todo |
| question | needs input | home, project,ays,doc | todo |
| inprogress | people are working on it | home, project,ays,doc | todo |
| verification | testing, verification with customer | home, project,ays,doc | todo |
| closed | nothing to do, 100% done | home, project,ays,doc | todo |
