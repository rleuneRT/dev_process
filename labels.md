## labels

### type

- to define type of issue
- 1 needs to be used (and only 1) !!!

| name | description | used in | 
| --- | --- | --- | --- |
| story |  | home, org, project | 
| task |  |  home, org, project |
| ticket | type | org, project |
| bug | issue reported by anyone | code,ays,doc,www,cockpit |
| feature | improvement asked for by anyone | code, project,ays,doc,www,cockpit, org |
| question | anyone wants to ask something | home, code, project,ays,doc,www,cockpit, org | 
| monitor | monitoring system found an issue | project,cockpit,www |
| lead | lead for sales, can convert in business | project,org |
| test | a test task | org,cockpit |

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
| new | new or issue in backlog (is no label, is the default)| all |
| inprogress | people are working on it | all |
| question | needs input | all |
| verification | testing, verification with customer | all |
| closed | nothing to do, 100% done | all |


{% mermaid %}
sequenceDiagram
    participant Alice
    participant Bob
    Alice->>John: Hello John, how are you?
    loop Healthcheck
        John->>John: Fight against hypochondria
    end
    Note right of John: Rational thoughts <br/>prevail...
    John-->>Alice: Great!
    John->>Bob: How about you?
    Bob-->>John: Jolly good!
{% endmermaid %}

{% mermaid %}
sequenceDiagram;
    participant Alice
    participant Bob
    Alice->>John: Hello John, how are you?
    loop Healthcheck
        John->>John: Fight against hypochondria
    end
    Note right of John: Rational thoughts <br/>prevail...
    John-->>Alice: Great!
    John->>Bob: How about you?
    Bob-->>John: Jolly good!
{% endmermaid %}
