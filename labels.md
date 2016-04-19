## labels

### type

- to define type of issue
- 1 needs to be used (and only 1) !!!

| name | description | used in |
| --- | --- | --- | --- |
| story |  | home, org, project |
| task |  |  home, org, project |
| ticket | type | org, project |
| bug | issue reported by anyone | code,ays,doc,www,cockpit, quality |
| feature | improvement asked for by anyone | code, project,ays,doc,www,cockpit, org, quality |
| question | anyone wants to ask something | home, code, project,ays,doc,www,cockpit, org |
| monitor | monitoring system found an issue | project,cockpit,www |
| lead | lead for sales, can convert in business | project,org |
| test | a test task | org,cockpit |
|AutomatedTest | a test which needs to run automatically on scheduled dates |quality|
|ManualTest| one time manual test | quality |
|enhancement| used for enhancement of an excisting feature|quality|

### priority

- define priority in which issue needs to resolved
- 1 needs to be used (and only 1) !!!

| name | description | used in |
| --- | --- | --- |
| critical |  | all |
| urgent |  | all |
| normal |  | all |
| minor |  | all |

### process

- define 2 optional process related labels

| name | description | used in |
| --- | --- | --- |
| duplicate |  | all |
| wontfix |  | all |

### state

- define state of issue in the kanban flow
- 1 needs to be used (and only 1) !!!
- REMARK
  - these states need to be useful over all projects e.g. over customer projects, code projects, stories, ...
  - good filters should be used in waffle to represent a kanban well

| name | description | used in |
| --- | --- | --- |
| new | new or issue in backlog | all |
| accepted | accepted in org & now tracked in kanban as to be done | all |
| question | needs input | all |
| inprogress | people are working on it | all |
| verification | testing, verification with customer | all, not on quality |
| closed | nothing to do, 100% done | all |
