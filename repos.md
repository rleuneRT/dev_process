## different types of repo's (IMPORTANT)

#### home repo

- is a repo with as name ```home```
- it is the main repo of an organization
- it holds 
  - starting point of documentation
  - explains what other repo's are used & what their purpose is
  - holds specifications which are not related to 1 repo
  - holds info like product PRD, ... which are bigger than 1 repo
- milestones
  - not used 
- issue types used
  - not used
  
#### code related

- no special convention today, can be any name but NOT starting with the prefixes as described in this doc
- this is where the main code of products live
- milestones
  - freely to be chosen names per repo, they are used to group bugs or features
  - these milestones are then linked to a specific story !!! to get them executed
- issue types used
  - bug, feature, question
- DO NOT
    - use stories or tasks or tests at this level !!! 
- bug/feature management
    - all issues reported or feature requests are grouped, it acts like a funnel    

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

#### ays templates (At Your Service)

- an AYS repo starts with ays_ ...
  - ```ays_$customer_$envname``` e.g. ays_gig_gentTest1
- milestones
  - to group feature requests & bugs
- issues can be of type
    - bug,feature,question


