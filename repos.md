## Different Types of Repositories


### Repositories inside Product organizations (prodorg)

- One **home** repository
- Source **Code** repositories
- **Documntation** (GitBook) repositories
- **AtYourService (AYS) templates** repositories
- **Websites** (www) repositories


#### Home repository

- Always named ```home```
- Is the main repo of a prodorg
- It holds 
  - Documentation
  - Explains the purpose of all other repo's in the prodorg
  - Starting point for people to find their way in all other repo's in the prodorg
  - Holds specifications and product requirements document (PRD) information common to several of the repo's in the prodorg
- Milestones
  - Are releases for a product, used to group work for coding, testing, ...
- Types of issues in the ``home`` repo:
  - Only issues of type Feature Request (FR)  
- This is the ideal repo to define your roadmap covering multiple product and component repo's in the prodorg

DO NOT USE THIS REPO FOR:
- Escalating bugs
- Story cards

  
#### Code repositories

- No specific naming convention, can be any name but NOT starting with the prefixes used by for other types of repositories, as described on this page
- This is where most of the code of the products lives
- Milestones
  - Are releases for a product, used to group work for- issue types used
- Types of issues in code repo's:
  - Issues of type Bug, Feature and Question
  - DO NOT use stories, tasks or tests at this level! 
- Bug/feature management
    - All reported issues or feature requests are grouped, it acts like a funnel    
- How to easily make sure bugs and features requests become tasks
  - Put unique story card name at beginning of title e.g. story1:...
  - The Incubaid development process tools will find the story, create a task for it and put this bug/feature request (fr) in as a task (in the task there will be link to this bug/fr) 


#### Documentation (GitBook) repositories

- Always named as ```doc_$name```
- IMPORTANT
  - Often it makes more sense to leave the documentation inside the product/code repo
  - When put in a code repo, use a subdirectory ```/doc```
  - Advantage to keep it in a code repo is that documentation is linked to the code
  - The only reason to put it in a separate repo is when the documentation is not related to code or related to more than one code repo  
- Milestones
  - For grouping features and bugs related the documentation
- Types of issues in documentation repo's:
    - Issues of type Bug, Feature and Question


#### www = websites repositories

- Always named as ```www_$name```
- Contains the code for a website
- When code changes website is updated and hosted automatically
- Types of issues in website repo's:
    - Issues of type Bug, Feature and Question


#### AYS templates (AtYourService)

- Always named as ```ays_$name```
  - ```ays_$customer_$envname``` e.g. ays_gig_gentTest1
- Milestones
  - For grouping feature requests and bugs
- Types of issues in AYS template repo's:
    - Issues of type Bug, Feature and Question


### Repo's inside Project organizations (projorg)

- **Organization** repositories
- **Project** repositories
- **Cockpit** repositories


#### Organization repositories

- Always named as ```org_$name```, e.g. org_marketing...
- Suggested standard organization repo's:
    - org_development (engineering)
    - org_support (all support requests (tickets) which are not in project repo yet)
    - org_internalit (internal IT related & organization of company)
    - org_product (product management)
    - org_marketing
    - org_finance
    - org_legal
    - org_hr 
    - org_quality (all QA related issues and automation code, performance testing, portal testing and automated tests)
- Milestones
  - Defines a deadline for the project, there can be multiple, but tasks or stories can only belong to one
  - Freely chosen per project
- Types of issues in organization repo's:
  - Issues of type Story, Lead, Ticket, Monitoring, Question or Task


#### Project repositories

- Always named as ```proj_$customer``` or ```proj_$customer_$projname```
  - Projects relate to customers
  - We use this to organize our work related to 1 customer, only useful if customer project is large enough
  - Do not create specific ```proj_$customer_$projname``` unless if subproject is large enough
- Milestones
  - defines a deadline for the project, there can be multiple but tasks or stories can only belong to one
  - freely chosen per project
- Types of issues in project repo's:
  - Issues of type Stories, Leads, Ticket, Monitoring, Question or Task


#### Cockpit repositories

- Always named as ```cockpit_$customer_$name```, e.g. ```infra_gig_gentTest1```
- Used to deploy an infrastructure from out of GitHub
  - Documents a full IT enveronment
  - Has all required process information embedded in AYS service instances
  - All changes are strictly controlled by GitHub with pull requests 
- Is the cockpit environment which runs our management framework, e.g.
    - AYS robot
    - Telegram robot
    - Rogerthat robot
    - Portal
- Used to manage an environment on our G8 grid
- AYS repo's are inside
    - there can be more than 1 ays repo hosted inside a cockpit repo 
        - hosts the ays recipes and ays instances which make up the env to be managed
        - is a dir which has an empty file .ays inside 
- Milestones
  - Defines a deadline for the environment, freely to be chosen
- Types of issues can be of type
    - Issues of type Story, Task, Bug, Feature, Question, Monitor or Test