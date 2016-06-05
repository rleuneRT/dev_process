## different types of repo's (IMPORTANT)
### repo's inside Product Organization (prodorg)

#### home repo for product organization repo's

- is a repo with as name ```home```
- it is the main repo of a prodorg
- it holds 
  - starting point of documentation & people to find their way in a repo
  - explains what other repo's are used & what their purpose is
  - holds specifications which are not related to 1 repo
  - holds info like product PRD, ... which are bigger than 1 repo
- milestones
  - are releases for a product, used to group work for coding/testing/...
- issue types used
  - FR 
- this is the ideal repo to define your roadmap which goes over different product/component repo's

DO NOT USE THIS REPO FOR

- escalating bugs
- story cards
  
#### code related

- no special convention today, can be any name but NOT starting with the prefixes as described in this doc
- this is where the main code of products live
- milestones
  - are releases for a product, used to group work for- issue types used
- types
  - bug, feature, question
- DO NOT
    - use stories or tasks or tests at this level !!! 
- bug/feature management
    - all issues reported or feature requests are grouped, it acts like a funnel    
- how to easily make sure bugs/fr become tasks
  - put unique story card name at beginning of title e.g. story1:...
  - the incubaid development process tools will find the story and if found create a task for it and put this bug/fr in as task (in the task there will be link to this bug/fr) 


#### documentation/gitbook

- ```doc_$name```
- IMPORTANT
  - often it makes more sense to leave the documenation inside the product/code repo
  - when put in code repo put under subdir /doc
  - advantage to keep it in a code repo is that documentation is lined to the code
  - the only reason to put it in a separate repo is when the doc is not related to code or related to more than 1 code repo  
- milestones
  - groups features & bugs
- issues can be of type
    - bug,feature,question

#### www = websites

- ```www_$name```
- the code for a website
- when code changes normally a website is updated & hosted automatically
- issues can be of type
    - bug,feature,question

#### ays templates (At Your Service)

- an AYS repo starts with ays_ ...
  - ```ays_$customer_$envname``` e.g. ays_gig_gentTest1
- milestones
  - to group feature requests & bugs
- issues can be of type
    - bug,feature,question


### repo's inside Project Organization (projorg)

#### organization related

- ```org_$name``` e.g. marketing...
- issues can be stories, leads, tickets, monitoring issues, stories, questions or tasks
- milestones
  - defines a deadline for the project, there can be multiple but tasks or stories can only belong to one
  - freely chosen per project
- suggested standard org repo's
    - org_development (engineering)
    - org_support (all support requests (tickets) which are not in project repo yet)
    - org_internalit (internal IT related & organization of company)
    - org_product (product management)
    - org_marketing 
    - org_finance
    - org_legal
    - org_hr 
    - org_quality (all QA related issues and automation code, performance testing, portal testing and automated tests)

#### project related

- ```proj_$customer``` or ```proj_$customer_$projname```
  - projects relate to customers
  - we use this to organize our work related to 1 customer, only useful if customer project is large enough
  - issues can be stories, leads, tickets, monitoring issues, stories, questions or tasks
- milestones
  - defines a deadline for the project, there can be multiple but tasks or stories can only belong to one
  - freely chosen per project
- do not create specific ```proj_$customer_$projname``` unless if subproject is large enough

#### cockpit

- ```cockpit_$customer_$name``` e.g. ```infra_gig_gentTest1```
- is used to run an infrastructure from out of GIT
  - it documents a full it env
  - it has all required process information embedded in ays
  - all changes are strictly controlled by git & pull requests 
- is the cockpit env which runs our management framework e.g.
    - ays robot
    - telegram robot
    - rogerthat robot
    - portal
- is used to manage an environment on our G8 grid
- ays repo's are inside
    - there can be more than 1 ays repo hosted inside a cockpit repo 
        - hosts the ays recipes and ays instances which make up the env to be managed
        - is a dir which has an empty file .ays inside 
- milestones
  - defines a deadline for the environment, freely to be chosen
- issues can be of type
    - story, task, bug, feature, question, monitor, test 



