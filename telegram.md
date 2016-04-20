## usage of telegram

- telegram (and later rogerthat) is our main tool to let communication flow.
- in this doc we describe the main telegram groups & how we use them
- IMPORTANT: PEOPLE NEED TO USE 2FACTOR AUTHENTICATION !!!!

### support

- ```$shortcompanyname_support``` e.g. ```gig_support```
- used for
    - any customer isue which deserves attention from more than 1 person
    - for escalations
    - for information sharing
    - for planning events
- who is on it
    - everyone delivering support
    - everyone who wants to know what is going on
- IMPORTANT
    - on duty support guys
        - NEED to announce their duty ON & OFF event on this group (if less than 10 people active, for larger orgs this will not be practical). This will allow people to see how is online & active.
        - NEED to use & actively look at this group

### organization

- ```$shortcompanyname_org_$name```
- example groups
    - e.g. ```gig_org_marketing```
    - e.g. ```gig_org_products```
    - e.g. ```gig_org_sales```
    - e.g. ```gig_org_internalit```
    - e.g. ```gig_org_development```
    - e.g. ```gig_org_research```
    - e.g. ```gig_org_proddelivery```  : e.g. hardware & shipments of projects
    - e.g. ```gig_org_qa```         : quality assurance in broad sense
    - e.g. ```gig_org_operations``` : team which keeps our systems up & running in broad sense
    - e.g. ```gig_org_admin```
    - e.g. ```gig_org_finance```
    - e.g. ```gig_org_legal```
    - e.g. ```gig_org_funding```

    - normally the name used is the same as the name of the git repo
- used for
    - communication around the topic
    - planning, info changes, ...
- who is on it
    - everyone which is working on the topic or can needs to know about it


### project

    - e.g. ```gig_proj_mauritius```
    - normally the name used is the same as the name of the git repo
- used for
    - communication around such a project
    - planning, info changes, ...
- who is on it
    - everyone which is working on this project 

### milestone 

- ```$shortcompanyname_milestone_$name``` e.g. ```gig_milestone_ovc210```
- defines a milestone for the company an all main communication to do with this
- used for
    - announcing meetings e.g. stakeholder meeting, story meeting if change in time, ...
    - important events
    - inform about important information changes (e.g. stories, specs, roadmap, ...)
    - planning events e.g. story meeting is now different time per day
    - important bugs people should be aware about
- who is on it
    - everyone who has something to win or loose with this milestone internal to our company 
- THIS IS MAINLY USED FOR PRODUCE RELATED RELEASES




### cockpit

- ```$shortcompanyname_cockpit_$name```
- in line with name of cockpit git repo
- used for
    - all communication around 1 IT environment (can be for 1 customer or internal, ...)
- is also used by cockpit: ays robot
    - means we can see on this group if there are issues with the environment
    - or we can give instructions to the ays robot to do something
- e.g. is done per test environment
    - can see if someone is doing a test and what the result is
    - can see monitoring state
    - can request changes
- who can use it
    - people with right security clearance !!! can be partners & internal


### code

    - e.g. ```code_jumpscale_go-raml```
    - normally the name used is the same as the name of the git repo
- used for
    - discussion around a code repository
    - comments can also be given in pull request and such but sometimes a telegram disccusion is more usefull
- who is on it
    - everyone which is working on this repository 
