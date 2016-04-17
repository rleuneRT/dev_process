## usage of telegram

- telegram (and later rogerthat) is our main tool to let communication flow.
- in this doc we describe the main telegram groups & how we use them
- IMPORTANT: PEOPLE NEED TO USE 2FACTOR AUTHENTICATION !!!!

### support

- ```support_$shortcompanyname``` e.g. ```support_gig```
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

- ```support_$shortcompanyname``` 
    - e.g. ```org_gig_marketing```
    - e.g. ```org_gig_products```
    - e.g. ```org_gig_sales```
    - e.g. ```org_gig_internalit```
    - e.g. ```org_gig_development```
    - e.g. ```org_gig_research```
    - e.g. ```org_gig_proddelivery```  : e.g. hardware & shipments of projects
    - e.g. ```org_gig_qa```         : quality assurance in broad sense
    - e.g. ```org_gig_operations``` : team which keeps our systems up & running in broad sense
    - e.g. ```org_gig_admin```
    - e.g. ```org_gig_finance```
    - e.g. ```org_gig_legal```
    - e.g. ```org_gig_funding```

    - normally the name used is the same as the name of the git repo
- used for
    - communication around the topic
    - planning, info changes, ...
- who is on it
    - everyone which is working on the topic or can needs to know about it


### project

<<<<<<< HEAD
- ```project_$shortcompanyname``` 
    - e.g. ```project_gig_mauritius```
    - normally the name used is the same as the name of the git repo
=======
- `support_$shortcompanyname_$projname`
    - e.g. `project_gig_internalit`
    - e.g. `project_gig_mauritius`
    - e.g. `project_gig_funding`
    - often the name used is the same as the name of the git repo
>>>>>>> 9183cb9331b83941cca05f2d1a8d4a3d679a96ff
- used for
    - communication around such a project
    - planning, info changes, ...
- who is on it
    - everyone which is working on this project 

### milestone 

- ```milestone_$shortcompanyname_$name``` e.g. ```milestone_gig_ovc210```
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

- ```cockpit_$shortcompanyname_$name```
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


