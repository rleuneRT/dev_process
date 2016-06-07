## Project Organizations (projorg) Repositories

In a **project** organization (prodorg) following repositories can exist:

- **Organization** repositories
- **Project** repositories
- **Cockpit** repositories

Below each of the "projorg" repositories is discussed.

### Organization repositories

- Always named as ```org_$name```
- Examples:
  - org_marketing (https://github.com/gig-projects/org_marketing)
  - org_development (https://github.com/gig-projects/org_development)
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
  - Defines a deadline (date) for the project, there can be multiple, but tasks or stories can only belong to one
  - Freely chosen per project
- Types of issues in organization repo's:
  - Issues of type Story, Lead, Ticket, Monitoring, Question or Task


### Project repositories

- Always named as ```proj_$customer``` or ```proj_$customer_$projname```
  - Projects relate to customers
  - We use this to organize our work related to 1 customer, only useful if customer project is large enough
  - Do not create specific ```proj_$customer_$projname``` unless if subproject is large enough
- Milestones
  - defines a deadline for the project, there can be multiple but tasks or stories can only belong to one
  - freely chosen per project
- Types of issues in project repo's:
  - Issues of type Stories, Leads, Ticket, Monitoring, Question or Task


### Cockpit repositories

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